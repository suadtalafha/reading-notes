# API 

## API Design Best Practices (Links to an external site.)
1- What does REST stand for?

Representational state transfer .

2- REST APIs are designed around a resources__. 
HTTP

 3- What is an identifer of a resource? Give an example.

A resource has an identifier, which is a URI that uniquely identifies that resource. ` https://adventure-works.com/orders/1 `.

4- What are the most common HTTP verbs?

GET, POST, PUT, PATCH AND DELETE

5- What should the URIs be based on?

When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

6- Give an example of a good URI.

`https://adventure-works.com/orders `

7- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

Web APIs that expose a large number of small resources. no it’s bad thing.

8- What status code does a successful GET request return?

A successful GET method typically returns HTTP status code 200 (OK)

9- What status code does an unsuccessful GET request return?

A successful GET method typically returns HTTP status code 200 (OK)

10- What status code does a successful POST request return?

it returns HTTP status code 201 (Created). The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource.

11- What status code does a successful DELETE request return?

It’s respond with HTTP status code 204.

![image](https://cloud.google.com/endpoints/docs/images/api_keys_overview.png)