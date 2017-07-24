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
- [ ] minimize JS/CSS
- [ ] concat JS/CSS (less HTTP requests)
- [ ] Gzip necessary to all assets
- [ ] make use of CDN (be closer to the user)
- [ ] keep `<meta charset="">` just below `<title>`
- [ ] use Cache (`Expires` and `ETag` headers) at a certain Level
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
- [ ] use lazy-load methods when possible
- [ ] inline critical CSS
- [ ] use `Keep-Alive` header (less TCP connections)
- [ ] minimize or stop redirects
- [ ] calculate only once
- [ ] aggregate and reduce amount of XHR calls 
- [ ] set `AllowOverride None` in _httpd.conf_ (Apache)
- [ ] use `GOTO` for code isolating
- [ ] prefer DEFER Over ASYNC
- [ ] use WebM instead of (animated) GIF


##External Resources:

- [Apache HTTP server boilerplate configs](https://github.com/h5bp/server-configs-apache)
- [Understanding critical CSS](https://www.smashingmagazine.com/2015/08/understanding-critical-css/)
- [Prefer DEFER Over ASYNC](http://calendar.perfplanet.com/2016/prefer-defer-over-async/)
- [Making touch scrolling fast by default](https://developers.google.com/web/updates/2017/01/scrolling-intervention)
- [WebPagetest](http://www.webpagetest.org)
