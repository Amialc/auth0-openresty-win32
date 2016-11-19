# Auth0 + Openresty (Nginx) API Seed
This seed project gives an example of how to set up Auth0 with a Nginx API.

# Running the example
In order to run the example, you need to set two enviroment variables: `JWT_SECRET` which is should be equal to your client secret and `JWT_SECRET_IS_BASE64_ENCODED` which should be equal `true` if your client secret is encoded with base64.

After that you can start nginx server by using `start nginx` command. This server has configured endpoint [http://localhost/protected](http://localhost/protected) that validates JWT that send in header `Authorization: Bearer <YOUR_JWT_TOKEN>`