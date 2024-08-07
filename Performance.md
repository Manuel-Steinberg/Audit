# Performance:

- [ ] add an index for where clauses columns
- [ ] use views
- [ ] create Classes only when its required
- [ ] Check configuration of ...
  - file uploads
  - `upload_max_filesize`
  - `post_max_size`
  - `max_execution_time`
  - `shell_exec`
  - `max_input_time`
  - `memory_limit`
- [ ] use nginx instead of Apache
- [ ] minimize JS/CSS/SVG/JPEG/PNG/AVIF/WEBP/GIF etc.
- [ ] concat JS/CSS (less HTTP requests)
- [ ] Compress (Gzip) necessary to all assets
- [ ] make use of CDN (be closer to the user)
- [ ] keep `<meta charset="">` just below `<title>`
- [ ] use Cache (`Expires` and `ETag` headers) at a certain Level
- [ ] use cache busting techniques (`?v=...`) wisely, e.g., `<link rel="icon" href="/favicon.ico?v=2" />`
- [ ] use "===" instead of "=="
- [ ] str_replace is faster than preg_replace, but strtr is faster than str_replace by a factor of 4
- [ ] Pass reference to the function if it does not affect your logic
- [ ] keep JavaScript after the content
- [ ] use memcache for the reducing database load and APC for opcode caching and intermediate code optimization
- [ ] close database connections
- [ ] reduce Number of hits to DB
- [ ] don´t forget to disable debugging functions!
- [ ] use native functions
- [ ] put most frequently used switch/if-else case on the top
- [ ] use JSON instead of XML
- [ ] use `isset()` where ever possible instead of using `count()`, `strlen()`, `sizeof()`
- [ ] use `''` (single quotes) instead of `""`(double quootes)
- [ ] concat strings with points
- [ ] make use of Call-By-Reference/Pointer
- [ ] use `<svg>`-icons/graphics and so on
- [ ] use the `<picture>`-HTML element (`<img>`as a fallback)
- [ ] use prefetch methods like lazy-load when possible, e.g., `loading='lazy'` in `<img ... >`
- [ ] use `<link rel="preconnect">` and `<link rel="dns-prefetch">` to the CDN domain(s).
- [ ] inline critical CSS
- [ ] use `Keep-Alive` header (less TCP connections)
- [ ] minimize or stop redirects
- [ ] calculate only once
- [ ] aggregate and reduce amount of XHR calls 
- [ ] set `AllowOverride None` in _httpd.conf_ (Apache)
- [ ] use `GOTO` for code isolating
- [ ] prefer DEFER Over ASYNC
- [ ] use WebM instead of (animated) GIF
- [ ] use WebP image format
- [ ] use Accelerated Mobile Pages (AMP) & Instant Articlss
- [ ] use CSS `rel="preload"` option
- [ ] use httpd.conf instead of `.htaccess` (if possible)
- [ ] use unary plus (+) to convert string to number (applicable for JS) 
- [ ] use one Framework maximum
- [ ] use `content-visibility: auto` in your CSS for text-containers.
- [ ] reduce number of images
- [ ] optimize images/videos
- [ ] minimize Code
- [ ] avoid CSS frameworks
- [ ] use PurgeCSS
- [ ] use static pages if possible
- [ ] do not use analytics
- [ ] avoid ads
- [ ] avoid nesting elements in CSS
- [ ] send emails in text rather `html` format
- [ ] use guard clauses to exit early
- [ ] use dedicated performance benchmark methods, e.g. `performance.now()` in JS
- [ ] use `.map()` method for array manipulations
- [ ] use `console.table()` in JS to print debug information
- [ ] use `<use>` to eliminate duplicates within svg
- [ ] use `<img>` over CSS `background-image`  
- [ ] Functions are faster than static methods are faster than object methods
- [ ] Call by Value is slightly faster than Call by Reference
- [ ] use native functions, e.g., `navigator.clipboard.writeText()`
- [ ] do not use async-snippets in JS
- [ ] use `display:none` for hiding/showing over creating new elements
- [ ] use `navigator.share` rather than third party libraries
- [ ] use `textContent` over `innerText` for reading the content of an element
- [ ] use `insertAdjacentHTML` or `appendChild` over `innerHTML`
- [ ] use the once param for one and done events



## Snippets 

[Asnyc JS snippets are an anti-pattern](https://csswizardry.com/2022/10/speeding-up-async-snippets/)

```javasacript
<script>
  var script = document.createElement('script');
  script.src = 'file.js';
  document.head.appendChild(script);
</script>
```

```javascript
el.addEventListener('click', handleClick, {
  once: true
});
```

## External Resources:

- [Apache HTTP server boilerplate configs](https://github.com/h5bp/server-configs-apache)
- [PHP Benchmarks](https://phpbench.com/)
- [Understanding critical CSS](https://www.smashingmagazine.com/2015/08/understanding-critical-css/)
- [Prefer DEFER Over ASYNC](http://calendar.perfplanet.com/2016/prefer-defer-over-async/)
- [Making touch scrolling fast by default](https://developers.google.com/web/updates/2017/01/scrolling-intervention)
- [WebPagetest](http://www.webpagetest.org)
- [Customizing the Apache Configuration (Serverpilot)](https://serverpilot.io/docs/customize-apache-settings)
- [Create instant pages](https://instant.page/)
- [Preload, prefetch and other <link> tags](https://3perf.com/blog/link-rels/)
- [The cost of JS framworks](https://timkadlec.com/remembers/2020-04-21-the-cost-of-javascript-frameworks/)
- [content-visibility: the new CSS property that boosts your rendering performance](https://web.dev/content-visibility/)
- [Optimizing CSS for faster page loads](https://pustelto.com/blog/optimizing-css-for-faster-page-loads/)
- [How to Load Fonts in a Way That Fights FOUT and Makes Lighthouse Happy](https://css-tricks.com/how-to-load-fonts-in-a-way-that-fights-fout-and-makes-lighthouse-happy/)
- [Maximally optimizing image loading for the web in 2021](https://www.industrialempathy.com/posts/image-optimizations/)
- [Using Performant Next-Gen Images in CSS with image-set](https://css-tricks.com/using-performant-next-gen-images-in-css-with-image-set/)
- [Optimising Largest Contentful Paint](https://csswizardry.com/2022/03/optimising-largest-contentful-paint)
