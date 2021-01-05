# Review, Research, and Discussion
In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

## What are the advantages of storing tokens in “Cookies” vs “Local Storage”

[local storage vs cookies](https://dev.to/cotter/localstorage-vs-cookies-all-you-need-to-know-about-storing-jwt-tokens-securely-in-the-front-end-15id)

### Local Storage

**Pros: It's convenient.**

It's pure JavaScript and it's convenient. If you don't have a back-end and you're relying on a third-party API, you can't always ask them to set a specific cookie for your site.
Works with APIs that require you to put your access token in the header like this: Authorization Bearer ${access_token}.


**Cons: It's vulnerable to XSS attacks.**

An XSS attack happens when an attacker can run JavaScript on your website. This means that the attacker can just take the access token that you stored in your localStorage.

An XSS attack can happen from a third-party JavaScript code included in your website, like React, Vue, jQuery, Google Analytics, etc. It's almost impossible not to include any third-party libraries in your site.

### Cookies

**Pros: The cookie is not accessible via JavaScript; hence, it is not as vulnerable to XSS attacks as localStorage.**

If you're using httpOnly and secure cookies, that means your cookies cannot be accessed using JavaScript. This means, even if an attacker can run JS on your site, they can't read your access token from the cookie.
It's automatically sent in every HTTP request to your server.


**Cons: Depending on the use case, you might not be able to store your tokens in the cookies.**

Cookies have a size limit of 4KB. Therefore, if you're using a big JWT Token, storing in the cookie is not an option.
There are scenarios where you can't share cookies with your API server or the API requires you to put the access token in the Authorization header. In this case, you won't be able to use cookies to store your tokens.

## Explain 3rd party cookies.

[all you need to know about 3rd party cookies](https://cookie-script.com/all-you-need-to-know-about-third-party-cookies.html)

Third party cookies are cookies set by a party other than the site you are currently on.  It allows other sites to track your browsing across the web and is commonly used to target custom advertising.

## How do pixel tags work?

[what is a tracking pixel?](https://whatagraph.com/blog/articles/tracking-pixel)

Tracking pixels are similar to 'ad codes' used in old print advertisements.  They allow tracking of metrics and details about where and how digital ads are viewed so advertisers can spend more efficiently.

# Vocabulary Terms
- **cookies** - An HTTP cookie (also called web cookie, Internet cookie, browser cookie, or simply cookie) is a small piece of data stored on the user's computer by the web browser while browsing a website. Cookies were designed to be a reliable mechanism for websites to remember stateful information (such as items added in the shopping cart in an online store) or to record the user's browsing activity (including clicking particular buttons, logging in, or recording which pages were visited in the past). They can also be used to remember pieces of information that the user previously entered into form fields, such as names, addresses, passwords, and payment card numbers.

Cookies perform essential functions in the modern web. Perhaps most importantly, authentication cookies are the most common method used by web servers to know whether the user is logged in or not, and which account they are logged in with. Without such a mechanism, the site would not know whether to send a page containing sensitive information, or require the user to authenticate themselves by logging in. The security of an authentication cookie generally depends on the security of the issuing website and the user's web browser, and on whether the cookie data is encrypted. Security vulnerabilities may allow a cookie's data to be read by a hacker, used to gain access to user data, or used to gain access (with the user's credentials) to the website to which the cookie belongs (see cross-site scripting and cross-site request forgery for examples).[1]

Tracking cookies, and especially third-party tracking cookies, are commonly used as ways to compile long-term records of individuals' browsing histories — a potential privacy concern that prompted European[2] and U.S. lawmakers to take action in 2011.[3][4] European law requires that all websites targeting European Union member states gain "informed consent" from users before storing non-essential cookies on their device.
- **Access control** - limiting the level of authorization of authenticated users, commonly done with roles.
- **authorization** - the level of access granted to an authenticated user (ex: admin vs guest)
- **conditional rendering** - elements in react that are rendered based on conditional if/else logic



# Preparation Materials



How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.


