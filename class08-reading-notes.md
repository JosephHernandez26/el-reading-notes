# El Reading Notes of the 401 Variety

## Class 08 reading notes

### El Questions

### Review, Research, and Discussion

#### When is Basic Authorization used vs. Bearer Authorization?

* The Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret (see RFC7616 and RFC7617).

* The Bearer authentication scheme is dedicated to the authentication using a token and is described by the RFC6750. Even if this scheme comes from an OAuth2 specification, you can still use it in any other context where tokens are exchange between a client and a server.

* Concerning the JWT authentication and as it is a token, the best choice is the Bearer authentication scheme. Nevertheless, nothing prevent you from using a custom scheme that could fit on your requirements.

[Source](https://stackoverflow.com/questions/34013299/web-api-authentication-basic-vs-bearer)

#### What does the JSON Web Token package do?

* JWT (JSON Web Token) is an open standard (published in the RFC 7519) which defines a compact and self-contained method to encapsulate and share assertions (claims) about an entity (subject) between peers in a secure manner by using JSON objects.

[Source](https://www.bbva.com/en/json-web-tokens-jwt-how-to-use-them-safely/)

#### What considerations should we make when creating and storing a SECRET?

**There are four main phases a password or other secret can go through**

**1. Creation**

* Secrets can either be created manually by a user

**2. Storage**

* Secrets can be stored centrally or separately, using designated solutions.

**3. Rotation**

* Secrets can be changed or reset on a schedule, thus improving the overall protection of an organization’s infrastructure.

**4. Revocation**

* Secrets can be revoked in the case of a cybersecurity incident.

* At each of these phases, secrets should be protected from unauthorized access, intervention, and manipulation.

**Secrets Management Best Practices**

**1. Build a secrets management policy**

* Using the list of bad practices from the previous section, determine your secrets management strategy and build a basic secrets management policy for your organization.

**2. Automate secrets management processes**

* When things aren’t automated, there’s always room for human errors. That’s why you need to deploy dedicated secrets management software for managing secrets in a secure and centralized manner.

**3. Manage privileges**

* Users and applications with elevated privileges have access to the most critical data, services, and resources.

[Source](https://www.ekransystem.com/en/blog/secrets-management)

#### Document the following Vocabulary Terms

**encryption**

> Encryption is the process of scrambling or enciphering data so it can be read only by someone with the means to return it to its original state. It is a crucial feature of a safe and trustworthy Internet. It helps provide data security for sensitive information.

[Source](https://www.internetsociety.org/issues/encryption/what-is/)

**token**

> Tokens are the smallest individual words, phrases, or characters that JavaScript can understand.

[Source](https://www.java-samples.com/showtutorial.php?tutorialid=171)

**bearer**

> The bearer token is a cryptic string with no meaning or uses but becomes important within a proper tokenization system.

[Source](https://stackoverflow.com/questions/51506579/sending-authorization-token-bearer-through-javascript)

**secret**

> Programming often involves keeping a bunch of secrets around. You’ve got account passwords, OAuth tokens, SSL and SSH private keys. The best way to keep a secret is, well, to keep it secret.

[Source](https://github.blog/2013-01-25-secrets-in-the-code/)

**JSON Web Token**

> JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

[Source](https://jwt.io/introduction)

 <a href="#top">Take Me To The Repo!!</a>