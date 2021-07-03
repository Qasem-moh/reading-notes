# authorization

- What is OAuth?

        OAuth is an open-standard authorization protocol or framework
        that describes how unrelated servers and services can safely
        allow authenticated access to their assets without actually
        sharing the initial, related, single logon credential.

- Give an example of what using OAuth would look like.

        The simplest example of OAuth is when you go to log onto a
        website and it offers one or more opportunities to log on
        using another website’s/service’s logon. You then click on
        the button linked to the other website, the other website
        authenticates you, and the website you were originally
        connecting to logs you on itself afterward using permission
        gained from the second website.


        Another common example OAuth scenario could be a user sending
        cloud-stored files to another user via email, when the cloud
        storage and email systems are otherwise unrelated other
        than supporting the OAuth framework (e.g., Google Gmail and
        Microsoft OneDrive). When the end-user attaches the files
        to their email and browses to select the files to attach,
        OAuth could be used behind the scenes to allow the email
        system to seamlessly authenticate and browse to the
        protected files without requiring a second logon to the
        file storage system. Another example, one given in the
        OAuth 2.0 RFC, is an end-user using a third-party printing
        service to print picture files stored on an unrelated web
        server.


        In all cases, two or more services are being used for one
        transaction by the end-user, and every end-user would
        appreciate not being asked to log in a second time for what
        they feel is a single transaction. For OAuth to work, the
        end-user’s client software (e.g., a browser), the services
        involved and authentication provider must support the right
        version of OAuth (1.0 versus 2.0).

- How does OAuth work? What are the steps that it takes to
  authenticate the user?

          Let’s assume a user has already signed into one website or
          service (OAuth only works using HTTPS). The user then
          initiates a feature/transaction that needs to access another
          unrelated site or service. The following happens (greatly
          simplified):

          1- The first website connects to the second website on behalf
             of the user, using OAuth, providing the user’s verified
             identity.

          2- The second site generates a one-time token and a one-time
             secret unique to the transaction and parties involved.

          3- The first site gives this token and secret to the
              initiating user’s client software.

          4- The client’s software presents the request token and
              secret to their authorization provider (which may or may
              not be the second site).

          5- If not already authenticated to the authorization
              provider, the client may be asked to authenticate. After
              authentication, the client is asked to approve the
              authorization transaction to the second website.

          6- The user approves (or their software silently approves) a
              particular transaction type at the first website.

          7- The user is given an approved access token (notice it’s no
              longer a request token).

          8- The user gives the approved access token to the first
              website.

          9- The first website gives the access token to the second
               website as proof of authentication on behalf of the user.

          10- The second website lets the first website access their
              site on behalf of the user.

          11- The user sees a successfully completed transaction
              occurring.

          12- OAuth is not the first authentication/authorization
              system to work this way on behalf of the end-user. In
              fact,many authentication systems, notably Kerberos, work
              similarly. What is special about OAuth is its ability to
              work across the web and its wide adoption. It succeeded
              with adoption rates where previous attempts failed (for
              various reasons).

- What is OpenID?

        OpenID is for humans logging into machines

****


# Authentication and Authorization Flows


1- What is the difference between authorization and authentication?

2- What is Authorization Code Flow?

3- What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

4- What is Implicit Flow with Form Post?

5- What is Client Credentials Flow?

6- What is Device Authorization Flow?

7- What is Resource Owner Password Flow?

