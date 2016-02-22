# Security:

- [ ] use `htmlentities()`
- [ ] set `display_errors = 0`
- [ ] check `$_SERVER['HTTP_REFERER']` for XSS-test
- [ ] use `htmlentities()` instead of `htmlspecialchars`
- [ ] check `strlen(htmlentities())` before and after manipulation
- [ ] set a proper cookie lifetime with `session_set_cookie_params`e.g. 1200
- [ ] set `session.use_only_cookies = 1`
- [ ] set `session.cookie_httponly = 1`
- [ ] set `session.cookie_secure = 1`
- [ ] only allow https on your server
- [ ] do not use the default name in `session.name`
- [ ] set `session.use_trans_sid = 1`
- [ ] use `session_regenerate_id()`
- [ ] disable file uplaods, when they´re not necessary
- [ ] never run the server as root. Run as an ordinary unprivileged user!
- [ ] the MySQL data directory should be only accessible from the server account.
- [ ] protect PHP option files
- [ ] periodically check the MySQL accounts


#### External resources:
- http://chxo.com/scripts/safe_html/index.html
