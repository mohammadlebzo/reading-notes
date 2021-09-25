# Reading 10

## What is OAuth

1. *What is OAuth*? [source](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

It is an ***open-standard authorization protocol or framework*** that *describes* how can **unrelated servers and services** *allow access* to their **assets without actually sharing any of their information**.

2. *Give an example of what using OAuth would look like*.

**ex**: when you want to **sign-up** there are many websites that allow you to **sign-up using Google**, **Facebook**, **GitHub**, **twitter**, **etc...**.

3. *How does OAuth work*? *What are the steps that it takes to authenticate the user*? [source](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

    1. The **first website** *connects* to the **second website** on *behalf* of the *user*, **using OAuth**, providing the **user’s verified identity**.
    2. The **second site** *generates* a **one-time token** and a **one-time secret unique** to the transaction and parties involved.
    3. The **first site** gives this *token* and *secret* to the **initiating user’s client software**.
    4. The **client’s software** presents the request *token* and *secret* to their **authorization provider** (which may or may not be the second site).
    5. If not already *authenticated* to the **authorization provider**, the *client* may be asked to *authenticate*. After *authentication*, the client is asked to approve the **authorization transaction** to the **second website**.
    6. The *user* approves (or their software silently approves) a particular transaction type at the **first website**.
    7. The *user* is given an approved **access token** (notice it’s no longer a request token).
    8. The *user* gives the *approved* **access token** to the **first website**.
    9. The **first website** gives the **access token** to the **second website** as *proof* of *authentication* on **behalf of the user**.
    10. The **second website** lets the **first website** *access* their site on **behalf of the user**.
    11. The *user* sees a **successfully completed transaction occurring**.

4. *What is OpenID*? [A source that helped](https://openid.net/what-is-openid/)

It is an **standard and decentralized authentication protocol**, that allows you to *use an account* to *sign-in* to **multiple websites**, without **creating new passwords**, and you can also *control* the **amount of shared information** with the *website*.

## Authorization and Authentication flows

1. *What is the difference between authorization and authentication*? 

**Authorization** is the *process* of **verifying what can the user access**, *but* **Authentication** is the *process* of **verifying the identity of the user**.

2. *What is Authorization Code Flow*? 

**Authorization Code Flow** is a *process* used to *obtain* an **access token to authorize API requests**.

3. *What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)*?

**Authorization Code Flow with Proof Key for Code Exchange** (**PKCE**) is a *process* used to **authenticate native or mobile application users**.

4. *What is Implicit Flow with Form Post*?

**Implicit Flow with Form Post** is a *process* used to **implement web sign-in**.

5. *What is Client Credentials Flow*? [source](https://curity.io/resources/learn/oauth-client-credentials-flow/#:~:text=The%20Client%20Credentials%20flow%20is,authentication%20involved%20in%20the%20process.&text=This%20flow%20is%20useful%20for,involve%20contacting%20OAuth%20protected%20APIs.)

**Client Credentials Flow** is a **server to server flow** that is *used* for *systems* that need to *perform* **API operations when there is no users**. 

6. *What is Device Authorization Flow*? [source](https://oauth.net/2/device-flow/#:~:text=The%20OAuth%202.0%20Device%20Authorization,video%20to%20a%20YouTube%20channel.)

**Device Authorization Flow** is an **OAuth 2.0 extension** that *enables* devices with **no browser or limited input capability to obtain an access token**.

7. *What is Resource Owner Password Flow*? [source](https://www.oreilly.com/library/view/getting-started-with/9781449317843/ch04.html#:~:text=The%20Resource%20Owner%20Password%20Credentials,%2C%20optionally%2C%20a%20refresh%20token.&text=The%20primary%20difference%20is%20that,is%20accessible%20to%20the%20application.)

**Resource Owner Password Flow** is a *process* that **allows the exchange of usernames and passwords for tokens**.

## Things I want to know more about

None.
