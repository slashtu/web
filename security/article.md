## Dominik Kundel: XSS, CSRF, CSP, JWT, WTF? IDK ¯\_(ツ)_/¯ | JSConf Iceland 2018

> https://youtu.be/c6mqdsfWdmE

  #### 1. JWT 
  #### 2. windows.opener
  #### 3. csrf
  #### 4. xss - 2005 myspace samy worm
  * inject javascript by CSS (background:url) and eval() function
  #### 5. JSONP and serviceworker
  #### 6. CSP
  * CSP is not your security strategy, CSP is a safty net
  #### 6. IFRAME and Clickjacking
  * X-Frame-Options: DENY
  ### Summary
  * use httpOnly
  * be sceptical of JWT
  * rel = "noopener noreferrer"
  * use CSRF token
  * blocking XSS
  * be aware of encoding
  * be careful with JSONP
  * use CSP as a safty net
  * stay up-to-date

## Practical
  #### Https
  ```
   never use Http
  ```

  #### Cookie
  ```
  Set-Cookie: key=value; SameSite=Strict
  Set-Cookie: key=value; HttpOnly
  Set-Cookie: <cookie-name>=<cookie-value>; Domain=<domain-value>
  
  // Multiple directives are also possible, for example:
  Set-Cookie: <cookie-name>=<cookie-value>; Domain=<domain-value>; Secure; HttpOnly
  ```
  
  #### Content Security Policy
  
  
## Express
https://expressjs.com/en/advanced/best-practice-security.html
