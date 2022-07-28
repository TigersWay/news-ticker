<svelte:options tag="news-ticker" />

<script>
  import { onMount  } from 'svelte';

  export let id, duration = 6;
  let container, items = [], current = 0;

  onMount(() => {
    const nodes = id ? document.getElementById(id).children : document.getElementsByTagName('news-ticker').item(0).children;
    items = [...nodes].map(el => el.innerHTML);
    console.log(items);
    current = 0;

    const interval = setInterval(() => {
      current = (current + 1) % items.length;
    }, duration * 1000);

    return () => {
      clearInterval(interval);
    };
  });
</script>

<div class="ticker" bind:this={container}>
  <p>{@html items[current]}</p>
</div>

<style>
  .ticker {
    width: 100%;
    height: 2.2rem;
    display: flex;
    align-items: center;
    margin: 0 4px;
    overflow: hidden;
  }
  .ticker > p {margin: 0;}
</style>
