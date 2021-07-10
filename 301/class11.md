# What is OAuth

1. What is OAuth?
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

2. Give an example of what using OAuth would look like.
The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

3. How does OAuth work? What are the steps that it takes to authenticate the user?

- The User Shows Intent.
- The Consumer Gets Permission.
- The User Is Redirected to the Service Provider.
- The User Gives Permission.
- The Consumer Obtains an Access Token.

4. What is OpenID?

OpenID is about authentication: as a commenter on StackOverflow pithily put it: "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."

# Authorization and Authentication flows

1. What is the difference between authorization and authentication?
In authentication process, the identity of users are checked for providing the access to the system. While in authorization process, person’s or user’s authorities are checked for accessing the resources. Authentication is done before the authorization process, whereas authorization process is done after the authentication process.

2. What is Authorization Code Flow?
Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow, which exchanges an Authorization Code for a token.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE).

4. What is Implicit Flow with Form Post?
Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls.

5. What is Client Credentials Flow?
In fact there is no user at all, the resulting access tokens will not contain a user, but will instead contain the Client ID as subject (if not configured otherwise). This flow is useful for systems that need to perform API operations when no user is present

6. What is Device Authorization Flow?
The authorization flow defined by this specification, sometimes referred to as the "device flow", instructs the user to review the authorization request on a secondary device, such as a smartphone, which does have the requisite input and browser capabilities to complete the user interaction.

What is Resource Owner Password Flow?
Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form. The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.

