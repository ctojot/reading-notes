# API Integration

## Review API Server Build

### Explain the different between a query string parameter and a path parameter.

Query string parameters are typically used to send data to the server as key-value pairs appended to the end of a URL and path parameters are used to include dynamic values within the URL path itself.

### What would our API URL with a path id parameter be given the following information:

```text
Domain: http://our-site.com
v3
model name: stuff
id: things
```

http://our-site.com/v3/stuff/things

### We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.

A dynamic API with an interface is basically something that can do all sorts of tasks. You don't need to know how it works on the inside, all you need to know the controls.

## Review Auth Server Build

### Describe how you would use middleware to implement basic and bearer auth.

Basic auth is a simple method where the user's credentials are included in the request headers. The server checks these credentials to determine if the user is allowed to access the resource. The middlesware would check the auth header for the username and password and decodes it. It then compares it to predetermined credentials. If the credentials match, authorization is given.

Bearer auth involves sending a token in the request header. The server validates the token to determine if the request is authorized.

### Describe the handshake necessary to implement OAuth.

The handshake involves a series of steps and interactions between the user, the app, and the OAuth server. The OAuth handshake ensures that the client application obtains access to a user's resources without the user sharing their credentials directly with the client

### Describe how Role Based Access Control works to a non-technical friend.

RBAC is a way to manage who has access to what within an organization's computer systems or software applications.
