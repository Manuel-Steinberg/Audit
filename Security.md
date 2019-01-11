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
- [ ] set `session.cookie_domain = YOURDOMAIN.TLD` (inclusive the respective subdomain)
- [ ] set `session.cookie_path = /PATH/`
- [ ] only allow https on your server
- [ ] do not use the default name in `session.name`
- [ ] set `session.use_trans_sid = 1`
- [ ] use `session_regenerate_id()`
- [ ] disable file uplaods, when they´re not necessary
- [ ] never run the server as root. Run as an ordinary unprivileged user!
- [ ] the MySQL data directory should be only accessible from the server account.
- [ ] use `mysql_real_escape_string()`
- [ ] protect PHP option files
- [ ] periodically check the MySQL accounts
- [ ] use Two-Factor-Authentification
- [ ] santisize any values being passed to your system
- [ ] make us of `$_ENV[]`
- [ ] provide CSRF/XSRF protected forms
- [ ] hide vulnerable HTTP response header, e.g. *X-Powered-By*
- [ ] only allow requests on URLs which exist, e.g. */wp-config* when you do not use WordPress
- [ ] validate GET-Parameters
- [ ] disable global variables
- [ ] add a DMARC policy
- [ ] set `X-Content-Type-Options: nosniff`
- [ ] set `X-Frame-Options: DENY`
- [ ] set `Content-Security-Policy: 'self'` (e.g. block JavaScript execution)
- [ ] set `X-XSS-Protection: 1; mode=block`
- [ ] set `Strict-Transport-Security: max-age=...`
- [ ] set `Referrer-Policy: 'no-referrer-when-downgrade'`
- [ ] set a DNS SPF entry
- [ ] validate user input
- [ ] block *.git*-folder access via URL
- [ ] disable server signatures
- [ ] use strong encryption algorithms
- [ ] use hash-function for salting
- [ ] use delays for sensitive pages, e.g. login
- [ ] set up notification center to get notified on possible attacks
- [ ] no passwords, tokens etc. in public repositories
- [ ] use POST instead of GET-requests (Exception: Search)
- [ ] use 2FA 
- [ ] be scant with third party integrations
- [ ] keep everything up-to-date
- [ ] hack yourself before someone else will
- [ ] use only reliable PSPs
- [ ] force user to choose a strong password
- [ ] use HSTS-Header when possible
- [ ] set `rel="noopener noreferrer"` in `<a target="_blank" ... />` 
- [ ] redirect http to https
- [ ] check your sitemap urls
- [ ] use as few as possible platforms, tools, engines etc.
- [ ] do not run multiple services like mail, webserver etc. on the same machine/instance
- [ ] provide a security whitepaper
- [ ] Scan Third-Party Libraries/Plugins (CMS)
- [ ] Keep Third-Party Libraries/Plugins (CMS) up-to-date
- [ ] Make use of HTML5 validation, e.g. required, min, pattern, type etc.
- [ ] use speaking URLs (trustability)


##### User Input
###### Common threats:

- input of specials chars, e.g. metacharacters
- input of any kind of commands
- input more signs than neccessary
- input wrong type
- manipulate hidden input fields

#### Snippets:
```php
// set up array with expected data and types
$form_data = array( 'city' => 'string'
                   ,'zip'  => 'int');
```
```php
// simple XSS-Prevention
if ($_SERVER['HTTP_REFERRER'] != $_SERVER['HTTP_HOST']) {
  exit('... Man-In-The-Middle ...');
}
```
```js
var newWnd = window.open();
// reset the "opener" property
newWnd.opener = null;
```

#### External resources:
- http://chxo.com/scripts/safe_html/index.html
- http://www.phpgangsta.de/2-faktor-authentifizierung-mit-dem-google-authenticator
- https://detectify.com/
- https://github.com/h5bp/server-configs
- http://cto-security-checklist.sqreen.io/
- https://www.crypteron.com/blog/the-real-problem-with-encryption/
- https://blog.appcanary.com/2017/http-security-headers.html
- https://observatory.mozilla.org/
