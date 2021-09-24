#  What are the advantages of storing tokens in “Cookies” vs “Local Storage”

### Local Storage

![](https://images.indepth.dev/images/2020/10/LocalStorage--1--1.png)

**It’s pure JavaScript and it’s convenient. If you don’t have a back-end and you’re relying on a third-party API, you can’t always ask the third-party API to set a specific cookie for your site.**

**Works with APIs that require you to put your access token in the header, like this: Authorization Bearer ${access_token}.**

### httpOnly Cookies

![](https://images.indepth.dev/images/2020/10/Cookie.png)
**If you’re using httpOnly and secure cookies this means that your cookies cannot be accessed using JavaScript so even if an attacker can run JS on your site, they can't read your access token from the cookie.**
**It’s automatically sent in every HTTP request to your server.**

- Local storage is vulnerable because it’s easily accessible using JavaScript and an attacker can retrieve your access token and use it later. However, while httpOnly cookies are not accessible using JavaScript, this doesn't mean that by using cookies you are safe from XSS attacks involving your access token.

- If an attacker can run JavaScript in your application then they can just send an HTTP request to your server which will automatically include your cookies; It’s just less convenient for the attacker because they can’t read the content of the token although they rarely have to. It might also be more advantageous for the attacker to attack using the victim’s browser (by just sending that HTTP request) rather than using the attacker’s machine.

**Both localStorage and cookies are vulnerable to XSS attacks, but it's harder for the attacker to do the attack when you're using httpOnly cookies.**

# Explain 3rd party cookies.

![](https://clearcode.cc/wp-content/uploads/2018/11/cookie-text.png?ver=1541148268)

# How do pixel tags work?
![](https://www.seobility.net/en/wiki/images/f/fc/Tracking-pixel.png)

**A tracking pixel, also known as a marketing pixel, is a 1×1 pixel graphic used to track user behavior, site conversions, web traffic, and other metrics similar to a cookie. The tiny pixel-sided image is usually hidden and embedded in everything from banner ads to emails**

| Term       |       Definition             |
| -----------|------------------------------|
|cookies|The data contained in a cookie is automatically transmitted between the web browser and the web server, so CGI scripts on the server can read and write cookie values that are stored on the client. JavaScript can also manipulate cookies using the cookie property of the Document object.|
|authorization|The JavaScript client library simplifies numerous aspects of the authorization process: It creates the redirect URL for Google's authorization server and provides a method to direct the user to that URL. It handles the redirect from that server back to your application|
|access control|Access control is a fundamental component of data security that dictates who's allowed to access and use company information and resources. Through authentication and authorization, access control policies make sure users are who they say they are and that they have appropriate access to company data.|
|conditional rendering|Conditional rendering is a term to describe the ability to render different user interface (UI) markup if a condition is true or false. In React, it allows us to render different elements or components based on a condition. This concept is applied often in the following scenarios: Rendering external data from an API|