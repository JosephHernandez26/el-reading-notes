# **El Reading Notes of the 401 Variety**

## **Class 36 reading notes**

### **El Questions**

1. **What are the advantages of storing tokens in “Cookies” vs “Local Storage”**
   - Cookies and local storage serve different purposes:
     - Cookies are mainly for reading server-side.
     - Local storage can only be read by the client-side.
   - Apart from saving data, a big technical difference is the size of data you can store, and Local Storage gives you more to work with.
   - Ultimately, the developer needs to determine where the data should be stored and who needs to access it.
   - [The Source](https://medium.datadriveninvestor.com/cookies-vs-local-storage-2f3732c7d977)
2. **Explain 3rd party cookies.**
   - Third-party Cookies are cookies that are set by a website other than the one the user is currently on.
   - **For example**: A social media *website* has a "Like" button,
     - This button stores a cookie (data) on the user's computer.
     - That same Cookie can later be accessed by the website itself to identify visitors and determine which websites the user likes to visit - that is a a 3rd Party Cookie.
   - [The Source](https://cookie-script.com/all-you-need-to-know-about-third-party-cookies.html)
3. **How do pixel tags work?**
   - Pixel Tags, (*'web beacons'*) attach to a browser and collect information about an anonymous user's movements on the Internet.
   - They allow sites to provide users with ads for services and products that are relevant to them.
   - [The Source](https://en.ryte.com/wiki/Tracking_Pixel#How_does_a_tracking_pixel_work)

### **Document the following Vocabulary Terms**

1. **Cookies**
   - An HTTP Cookie (*Web Cookie, Browser Cookie*) is a small piece of data that a server sends to a user's web browser.
   - The browser may store the Cookie and send it back to the same server with later requests.
   - Typically, an HTTP Cookie is used to tell if two requests come from the same browser—keeping a user logged in, for example.
   - It remembers stateful information for the stateless HTTP protocol.
 - *Cookies are mainly used for three purposes*:
   1. **Session management**
      - Logins, shopping carts, game scores, or anything else the server should remember.
   2. **Personalization**
      - User preferences,
      - Themes, and other settings.
   3. **Tracking**
      - Recording and analyzing user behavior.
      - [The Source](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies)
2. **Authorization**
   - The HTTP Authorization request header can be used to provide credentials that authenticate a user agent with a server, allowing access to a protected resource.
   - The Authorization header is usually, but not always, sent after the user agent first attempts to request a protected resource without credentials.
      - [The Source](https://en.wikipedia.org/wiki/Authorization)
3. **Access Control**
   - Role-Based Access Control (**RBAC**), aka, Role-Based Security (**RBS**), is a mechanism that restricts system access to users using their roles and privileges and permissions.
   - Within an application, roles are created for various user types.
      - [The Source](https://blog.logrocket.com/using-accesscontrol-for-rbac-and-abac-in-node-js/#:~:text=Role%2Dbased%20access%20control%2C%20also,e.g.%2C%20writer%20or%20reader)
4. **Conditional Rendering**
   - This is the ability to render different User Interfaces(UI) based on a boolean condition.

 <a href="#top">Take Me To The Repo!!</a>
