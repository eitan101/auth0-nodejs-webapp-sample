# Apps Demo

## With Userinfo Endpoint

create ``.env`` file with the following properties:

```env
OAUTH2_CLIENT_ID=cVst-hietkse9uNr3fdvMnVFh-IOxmC2
OAUTH2_CLIENT_SECRET=************
OAUTH2_CALLBACK_URL=http://localhost:3000/callback
OAUTH2_AUTHORIZATION_URL=https://login-poc.auth0.com/authorize
OAUTH2_TOKEN_URL=https://login-poc.auth0.com/oauth/token
OIDC_USERINFO_URL=https://login-poc.auth0.com/userinfo%
```

run:

```sh
docker run --env-file .env -p 3000:3000 -it eitnaya/oauth2-app
```

## Without Userinfo Endpoint

Same as above, just omit the ``OIDC_USERINFO_URL``.