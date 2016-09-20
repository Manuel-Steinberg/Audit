# Performance:

- [ ] add an index for where clauses columns
- [ ] use views
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
- [ ] put most frequently used switch/if-else cases on the top
- [ ] use JSON instead of XML
- [ ] use `isset()` where ever possible instead of using `count()`, `strlen()`, `sizeof()`
- [ ] concat strings with points
- [ ] use `<svg>`-icons/graphics and so on
- [ ] use the `<picture>`-HTML element (`<img>`as a fallback)
- [ ] use lazy-load methods when possible
- [ ] inline critical CSS
- [ ] use `Keep-Alive` header (less TCP connections)
- [ ] minimize or stop redirects


##External Resources:

- https://github.com/h5bp/server-configs-apache
- https://www.smashingmagazine.com/2015/08/understanding-critical-css/
