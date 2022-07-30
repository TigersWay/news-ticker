# news-ticker  ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/tigersway/news-ticker?style=flat-square) ![GitHub last commit](https://img.shields.io/github/last-commit/tigersway/news-ticker?style=flat-square) ![GitHub issues](https://img.shields.io/github/issues/tigersway/news-ticker?style=flat-square)

### Usage  [![jsDelivr hits (GitHub)](https://img.shields.io/jsdelivr/gh/hm/tigersway/news-ticker?logo=jselivr&style=flat-square)](https://www.jsdelivr.com/package/gh/tigersway/news-ticker)

```html
<!doctype html>
<html class="no-js" lang="en">
<head>
...
<body>
...
  <div class="news-wrapper">
    <news-ticker id="one" duration=3>
      <p>First news</p>
      <p>Second news with a <a href="https://google.com">link</a></p>
      <p>And of course some "<strong>colors</strong>" like <span style="color:red;">red</span> or <span style="color:lime">lime</span>!</p>
    </news-ticker>
  </div>
...
  <script src='https://cdn.jsdelivr.net/gh/tigersway/news-ticker@1/dist/news-ticker.esm.min.js' type="module"></script>
</body>
</html>
```

Options:

- id: CSS id selector, needed if you have more than 1 news-ticker on the same page,
- duration: (default 6) Number of seconds between flips.

### CHANGELOG

**v1.0.0**

- Everything should be working!

**v0.1.0**

- First public release
