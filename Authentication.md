# Authentication

### What is OAuth?

* is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.

### Give an example of what using OAuth would look like.

*  when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

### How does OAuth work? What are the steps that it takes to authenticate the user?

1- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.

2- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.

3- The first site gives this token and secret to the initiating user’s client software.

4- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).

5- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.

6- The user approves (or their software silently approves) a particular transaction type at the first website.

7- The user is given an approved access token (notice it’s no longer a request token).

8- The user gives the approved access token to the first website.

9- The first website gives the access token to the second website as proof of authentication on behalf of the user.

10- The second website lets the first website access their site on behalf of the user.

### What is OpenID?

* OpenID is about authentication: as a commenter on StackOverflow pithily put it: "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."


### What is the difference between authorization and authentication?

**Authentication** : is the process of verifying who a user is, while 

**Authorization** : is the process of verifying what they have access to.

### What is Authorization Code Flow?

* Exchanges an Authorization code for a token.

### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

* A version of the Authorization Code Flow, to mitigate the single-page apps’ special challenges and for additional security when using mobile and native applications.

### What is Implicit Flow with Form Post?

* provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets.

### What is Client Credentials Flow?

* The system authenticates and authorizes the app rather than a user.

### What is Device Authorization Flow?

* The device asks the user to go to a link on their computer or smartphone and authorize the device.

### What is Resource Owner Password Flow?

* The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.