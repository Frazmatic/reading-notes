# Class 15

## Significance

## Things I want to know more about

## Questions:

[What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

1. What is OAuth?

    A framework for shared authorization credentials.

2. Give an example of what using OAuth would look like.

When you can log in on one site with another site's login (e.g. using Google's login on another site)

3. How does OAuth work? What are the steps that it takes to authenticate the user?

    1. Using OAuth, first (authenticating) sie provides credentials to 2nd site using OAuth.
    2. Second site generates a one-time request token &  secret unique to transaction.
    3. First site gives token & secret to client.
    4. Client presents token & secret to authorization provider.
    5.  Auth provider may request client authentication, client approves authorization transaction to first site.
    6. User (or client software) approves transaction.
    7. Client given approved access token.
    8. Client gives approved access token to first site.
    9. First site gives approved access token to second site.
    10. Second site site lets first site access on behalf of client.
    11. user sees successfully completed transactoin.
 
4. What is OpenId?

An authentication protocol, used to identify people, that is sometimes used with OAuth.

[Authorization and Authentication flows](https://auth0.com/docs/flows)

1. What is the difference between authorization and authentication?

authorization: provide authorization to access resources
authentication: verify ID

2. What is Authorization Code Flow?

Server side authorization rocess. Server receives login request, redirects to authorization server, gets login from user and receives an authorization code, uses this code with client ID and client secret to get an ID token and access token from auth server. Access token can be used to control authorization with API.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

With apps that can't store clienty secret securely (i.e. all their code is browser based and exposed), the app createse a 'code verifier' and 'code challenge', auth server sues code challenge to create an authorization code, client sends auth code and code verifier back to authorization server, auth server provides an id token and access token.

4. What is Implicit Flow with Form Post?

Something intended for 'public clients' which be used when an "application needs only an ID token".

5. What is Client Credentials Flow?

Used for 'machine to machine' interactions where the app itself needs to be authenticated and authorized.

6. What is Device Authorization Flow?

Goes to an external device (such as a smartphone) for authorization. 

7. What is Resource Owner Password Flow?

user enters credentials directly in the app.