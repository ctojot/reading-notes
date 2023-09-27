# Bearer Authentication

## Intro to JWT

### What is a JSON Web Token (JWT)?

JSON Web Token is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object

### When should we use JSON Web Tokens?

We should use JWT because they are small in size so they're great for HTML and HTTP enviornments.

### Claims are expected in which structural component of a JWT?

The payload

## Are JWTs Secure?

### If I get a JWT and I can decode the payload, how can we call that secure?

JWT is secure because for the two parties, the signature involves a secret and if you do not know the secret, you wouldn't be able to full decode the whole JWT.

### If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature

Both parties need to know the secret.

### Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter

Let use the sentence, "I am here" as an example. Take away the spaces you get "Iamhere". Now the sentence is concatenated. We took the 3 words and smooshed them together to make one thing. Now with what we got, I want to send this to someone, but i don't want anyone else to able to know what I'm saying if they get a hold of it. So what we're gonna do is we're going to make a secret. We'll replace the e's with !'s and I'm also going to tell the person that I'm sending this to what I'm doing. Then we're left with "Iamh!r!". Now if anyone looks at this messge, they won't know what it says, but the person I'm sending this to will because I told them the secret to my message for them to decode it.

## JWTs Explained

### Why use JWT?

JWT is digitally signed meaning the information is verified and trusted.

### JWT is Compact and self-contained. Describe how this is useful to a non-technical friend

JWT being compact and self-contained is useful because:

- It's not a big file so it can be sent via URL and transmitted very fast
- The token contains info abou the user
- User doesn't have to repetitvely login, when they revist the sight, their token will be sent to the system

### What are the three components (the structure) of a JWT signature?

- Header
- Payload
- Signature

## Reflection

### What are your learning goals after reading and reviewing the class README?

