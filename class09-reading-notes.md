# El Reading Notes of the 401 Variety

## Class 09 reading notes

### El Questions

#### 1. What header(s) are used in authentication and authorization?

- Basic `HTTP` authentication uses a Authorization header filled with `Basic <credentials>`.

## 2. What is safe to put into a JWT?

- Actually, pretty much any data will (or should be) safe in-so-far-as the server can decode the data using `secret` (*should be known only to the server*).

## 3. How are JWTs validated?

- `JWT`s (JSON Web Tokens) are validated by decryption via `secret` again, this is known only by the server. Then it is decoded by `base_64` decoding to reveal the JavaScript `Object` data.

### Document the following Vocabulary Terms:

**RBAC**

> Role Based Access Control. Basically allows a specific user to have constricted access throughout a server based on saved data on said person.

**User Roles**

> These are the roles, or capabilities allowed to a specific user based on data on the server provided about said user.

**JWT Token**

> JSON Web Token is a compact URL-safe means of representing claims to be transferred between two parties (from https://jwt.io/). This means that JWT provides data for proving credentials of a user to a server.

 <a href="#top">Take Me To The Repo!!</a>
 