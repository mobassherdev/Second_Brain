# REST API Interview Questions (150 Total)

---

# REST Fundamentals

1. What is a REST API?
2. What does REST stand for?
3. Who introduced REST?
4. What are the REST architectural constraints?
5. What are the advantages of REST APIs?
6. What are the disadvantages of REST APIs?
7. What is the difference between REST and SOAP?
8. What is the difference between REST and GraphQL?
9. What makes an API RESTful?
10. When should you use REST instead of GraphQL?

---

# HTTP Methods

11. What is the HTTP protocol?
12. What is the purpose of the GET method?
13. What is the purpose of the POST method?
14. What is the purpose of the PUT method?
15. What is the purpose of the PATCH method?
16. What is the purpose of the DELETE method?
17. What is the purpose of the OPTIONS method?
18. What is the purpose of the HEAD method?
19. What is the difference between PUT and PATCH?
20. Which HTTP methods are idempotent?

---

# HTTP Status Codes

21. What are HTTP status codes?
22. What does 200 OK mean?
23. What does 201 Created mean?
24. What does 202 Accepted mean?
25. What does 204 No Content mean?
26. What does 400 Bad Request mean?
27. What does 401 Unauthorized mean?
28. What does 403 Forbidden mean?
29. What does 404 Not Found mean?
30. What does 500 Internal Server Error mean?

---

# Request & Response

31. What are HTTP headers?
32. What is the request body?
33. What is the response body?
34. What are query parameters?
35. What are path parameters?
36. What is the difference between path parameters and query parameters?
37. What is the `Content-Type` header?
38. What is the `Accept` header?
39. What is the `Authorization` header?
40. What is the `User-Agent` header?

---

# REST Principles

41. What does stateless mean in REST?
42. Why should REST APIs be stateless?
43. What is resource-based URL design?
44. What is URI naming convention?
45. What are REST naming best practices?
46. What is HATEOAS?
47. Why is HATEOAS rarely implemented?
48. What is content negotiation?
49. How do clients and servers communicate in REST?
50. What REST API best practices do you follow?

---

# Authentication & Authorization

51. What is authentication?
52. What is authorization?
53. What is the difference between authentication and authorization?
54. What authentication methods are commonly used in REST APIs?
55. What is Basic Authentication?
56. What is Bearer Token Authentication?
57. What is JWT authentication?
58. What is OAuth 2.0?
59. When should you use API Keys?
60. What authentication best practices do you follow?

---

# JWT & Security

61. How does JWT work?
62. What are the three parts of a JWT?
63. What is the difference between access tokens and refresh tokens?
64. Where should JWT tokens be stored?
65. How do you invalidate JWT tokens?
66. How do you implement logout with JWT?
67. How do you prevent token theft?
68. What are common JWT security mistakes?
69. How do you secure REST APIs?
70. What API security best practices do you follow?

---

# API Design

71. How do you design RESTful endpoints?
72. What naming conventions do you use for endpoints?
73. Should endpoints use nouns or verbs?
74. How do you design nested resources?
75. When should you use nested routes?
76. How do you implement pagination?
77. How do you implement filtering?
78. How do you implement sorting?
79. How do you implement searching?
80. What API design mistakes should you avoid?

---

# Validation & Error Handling

81. Why is request validation important?
82. How do you validate request bodies?
83. How do you validate query parameters?
84. How do you validate route parameters?
85. What validation libraries have you used?
86. How do you return validation errors?
87. How do you design consistent error responses?
88. What HTTP status codes should validation errors use?
89. How do you handle unexpected server errors?
90. What error-handling best practices do you follow?

---

# Versioning & Documentation

91. Why should APIs be versioned?
92. What API versioning strategies are available?
93. What is URI versioning?
94. What is header versioning?
95. What is media type versioning?
96. How do you document REST APIs?
97. What is OpenAPI (Swagger)?
98. How do you generate API documentation?
99. How do you test REST APIs?
100. What REST API documentation best practices do you follow?

---

# Performance & Caching

101. How do you optimize REST API performance?
102. What is HTTP caching?
103. What is the `Cache-Control` header?
104. What is an ETag?
105. What are conditional requests?
106. What is the `If-None-Match` header?
107. What is the `If-Modified-Since` header?
108. When should you cache API responses?
109. What data should not be cached?
110. What caching best practices do you follow?

---

# Idempotency & Reliability

111. What is idempotency?
112. Which HTTP methods are idempotent?
113. Why is idempotency important?
114. How do you make POST requests idempotent?
115. What is an idempotency key?
116. How do you prevent duplicate requests?
117. How do you handle retries safely?
118. What are distributed transactions?
119. How do you ensure data consistency across services?
120. What reliability best practices do you follow?

---

# Scalability & Architecture

121. How do you scale REST APIs?
122. What is an API Gateway?
123. Why use an API Gateway?
124. What is a reverse proxy?
125. What is load balancing?
126. What is horizontal scaling?
127. What is vertical scaling?
128. How do REST APIs work in a microservices architecture?
129. How do microservices communicate?
130. What architecture best practices do you follow?

---

# Monitoring & Production

131. How do you monitor REST APIs?
132. What API metrics do you track?
133. How do you log API requests?
134. How do you trace requests across services?
135. How do you debug production API issues?
136. How do you implement rate limiting?
137. How do you handle API throttling?
138. How do you secure APIs in production?
139. What production deployment best practices do you follow?
140. How do you test REST APIs in production?

---

# Senior Real-World Interview Questions

141. Describe the largest REST API you've built.
142. What was the most challenging API design problem you've solved?
143. How do you review REST API pull requests?
144. How do you design APIs for backward compatibility?
145. How would you migrate a monolithic API to microservices?
146. How would you design a REST API for an e-commerce platform?
147. How would you design a REST API for a school management system?
148. What REST API features do you use most frequently in production?
149. If you were starting a new production backend today, how would you design your API layer?
150. In your opinion, what separates a junior, mid-level, and senior backend API developer?

---

# ANSWERS


---

## Part 1 (1â€“10): REST Fundamentals

---

## Question 1: What is a REST API?

## Answer:
A REST API (Representational State Transfer Application Programming Interface) is an architectural style for designing networked applications. It uses HTTP methods to perform operations on resources identified by URLs.

```
GET /api/users        â†’ Get all users
POST /api/users       â†’ Create a user
GET /api/users/1      â†’ Get user 1
PUT /api/users/1      â†’ Update user 1
DELETE /api/users/1   â†’ Delete user 1
```

## Key Points:
- Architectural style for APIs.
- Uses HTTP methods (GET, POST, PUT, DELETE).
- Resources identified by URLs.
- Stateless communication.
- JSON for data exchange.

## Interview Tip:
"REST is an architectural style â€” it uses HTTP methods to operate on resources identified by URLs."

---

## Question 2: What does REST stand for?

## Answer:
REST stands for **Representational State Transfer**. It was introduced by Roy Fielding in his 2000 doctoral dissertation.

## Key Points:
- Representational State Transfer.
- Introduced by Roy Fielding in 2000.
- Architectural style, not a protocol.
- Based on HTTP principles.

## Interview Tip:
"REST = Representational State Transfer â€” it's an architectural style, not a protocol."

---

## Question 3: Who introduced REST?

## Answer:
Roy Fielding introduced REST in his 2000 doctoral dissertation "Architectural Styles and the Design of Network-based Software Architectures." He was one of the principal authors of the HTTP specification.

## Key Points:
- Roy Fielding, 2000.
- Doctoral dissertation.
- One of HTTP specification authors.
- Defined six architectural constraints.

## Interview Tip:
"Roy Fielding defined REST in his 2000 dissertation â€” he was also an author of the HTTP spec."

---

## Question 4: What are the REST architectural constraints?

## Answer:
1. **Client-Server**: Separation of concerns.
2. **Stateless**: No session state on server.
3. **Cacheable**: Responses can be cached.
4. **Uniform Interface**: Standard way to interact.
5. **Layered System**: Intermediaries (load balancers, proxies).
6. **Code on Demand** (optional): Server can send executable code.

## Key Points:
- Client-Server separation.
- Stateless communication.
- Cacheable responses.
- Uniform interface.
- Layered system.
- Code on Demand (optional).

## Interview Tip:
"The six constraints define REST â€” stateless, cacheable, uniform interface are the most important."

---

## Question 5: What are the advantages of REST APIs?

## Answer:
- **Simple**: Uses standard HTTP methods.
- **Scalable**: Stateless design enables horizontal scaling.
- **Flexible**: Works with any data format (JSON, XML).
- **Cacheable**: HTTP caching improves performance.
- **Wide support**: Every language/platform supports HTTP.
- **Decoupled**: Client and server evolve independently.

## Key Points:
- Simple and standard.
- Scalable (stateless).
- Flexible data formats.
- Cacheable.
- Universal support.

## Interview Tip:
"REST's biggest advantage is simplicity â€” it uses HTTP, which everyone understands."

---

## Question 6: What are the disadvantages of REST APIs?

## Answer:
- **Over-fetching**: Getting more data than needed.
- **Under-fetching**: Need multiple requests for related data.
- **No real-time**: HTTP request-response only.
- **Versioning complexity**: Managing API versions.
- **No type safety**: No built-in schema validation.

## Key Points:
- Over-fetching and under-fetching.
- No real-time support.
- Versioning complexity.
- No built-in schema.

## Interview Tip:
"REST's main disadvantage is over-fetching â€” GraphQL solves this with flexible queries."

---

## Question 7: What is the difference between REST and SOAP?

## Answer:
| Feature | REST | SOAP |
|---------|------|------|
| Style | Architectural style | Protocol |
| Data format | JSON, XML | XML only |
| Transport | HTTP | HTTP, SMTP, etc. |
| Complexity | Simple | Complex |
| Performance | Faster (less overhead) | Slower (XML parsing) |

## Key Points:
- REST: architectural style, JSON, simple.
- SOAP: protocol, XML only, complex.
- REST is more popular for modern APIs.
- SOAP for enterprise/legacy systems.

## Interview Tip:
"REST is simpler and faster; SOAP is more rigid but has built-in security (WS-Security)."

---

## Question 8: What is the difference between REST and GraphQL?

## Answer:
| Feature | REST | GraphQL |
|---------|------|---------|
| Endpoints | Multiple | Single |
| Data | Fixed structure | Flexible queries |
| Over-fetching | Common | None |
| Under-fetching | Common | None |
| Learning curve | Low | Higher |

## Key Points:
- REST: multiple endpoints, fixed structure.
- GraphQL: single endpoint, flexible queries.
- GraphQL solves over/under-fetching.
- REST is simpler to start with.

## Interview Tip:
"REST for simple CRUD; GraphQL when you need flexible data fetching."

---

## Question 9: What makes an API RESTful?

## Answer:
An API is RESTful if it follows REST constraints:
1. **Client-Server**: Separation of concerns.
2. **Stateless**: No server-side session.
3. **Cacheable**: Responses can be cached.
4. **Uniform Interface**: Resource-based URLs, HTTP methods.
5. **Resource identification**: URLs identify resources.

## Key Points:
- Follows REST constraints.
- Resource-based URLs.
- HTTP methods for operations.
- Stateless communication.
- Cacheable responses.

## Interview Tip:
"A RESTful API follows REST constraints â€” resource-based URLs, HTTP methods, stateless."

---

## Question 10: When should you use REST instead of GraphQL?

## Answer:
- **Simple CRUD**: Standard create/read/update/delete.
- **Public APIs**: Widely understood.
- **Caching**: HTTP caching is simpler.
- **File uploads**: Native HTTP support.
- **Microservices**: Service-to-service communication.

## Key Points:
- Simple CRUD operations.
- Public APIs.
- HTTP caching.
- File uploads.
- Microservices.

## Interview Tip:
"REST for simple, public APIs; GraphQL for complex, flexible data needs."

---

## Part 2 (11â€“20): HTTP Methods

---

## Question 11: What is the HTTP protocol?

## Answer:
HTTP (Hypertext Transfer Protocol) is the foundation of data communication on the web. It defines how clients and servers communicate using requests and responses.

## Key Points:
- Foundation of web communication.
- Request-response model.
- Stateless protocol.
- Uses TCP/IP.
- Methods: GET, POST, PUT, DELETE, etc.

## Interview Tip:
"HTTP is the language of the web â€” clients send requests, servers send responses."

---

## Question 12: What is the purpose of the GET method?

## Answer:
GET retrieves a resource without modifying it. It's safe and idempotent.

```
GET /api/users        â†’ Get all users
GET /api/users/1      â†’ Get user 1
```

## Key Points:
- Retrieve resources.
- Safe (no side effects).
- Idempotent (same result every time).
- Can be cached.
- No request body.

## Interview Tip:
"GET retrieves data â€” it should never modify anything."

---

## Question 13: What is the purpose of the POST method?

## Answer:
POST creates a new resource. It's not idempotent â€” multiple calls create multiple resources.

```
POST /api/users
Body: { "name": "Alice", "email": "alice@example.com" }
â†’ Creates a new user
```

## Key Points:
- Create new resources.
- Not idempotent.
- Has request body.
- Returns 201 Created.
- Used for non-idempotent operations.

## Interview Tip:
"POST creates resources â€” calling it twice creates two resources."

---

## Question 14: What is the purpose of the PUT method?

## Answer:
PUT replaces an entire resource. It's idempotent â€” multiple calls produce the same result.

```
PUT /api/users/1
Body: { "name": "Alice", "email": "alice@example.com", "role": "admin" }
â†’ Replaces user 1 entirely
```

## Key Points:
- Replace entire resource.
- Idempotent.
- All fields required.
- Creates if not exists (sometimes).
- Full replacement.

## Interview Tip:
"PUT replaces the entire resource â€” all fields are required."

---

## Question 15: What is the purpose of the PATCH method?

## Answer:
PATCH updates specific fields of a resource. It's not necessarily idempotent.

```
PATCH /api/users/1
Body: { "name": "Alice Updated" }
â†’ Updates only the name field
```

## Key Points:
- Partial update.
- Only changed fields required.
- Not necessarily idempotent.
- More flexible than PUT.
- Smaller payloads.

## Interview Tip:
"PATCH for partial updates; PUT for full replacements."

---

## Question 16: What is the purpose of the DELETE method?

## Answer:
DELETE removes a resource. It's idempotent â€” deleting the same resource multiple times has the same effect.

```
DELETE /api/users/1
â†’ Deletes user 1
```

## Key Points:
- Remove resources.
- Idempotent.
- Returns 204 No Content.
- Can return 200 with deleted resource.
- Idempotent: deleting twice = same result.

## Interview Tip:
"DELETE removes resources â€” it's idempotent because deleting twice is the same as once."

---

## Question 17: What is the purpose of the OPTIONS method?

## Answer:
OPTIONS returns the allowed HTTP methods for a resource. It's used for CORS preflight requests.

```
OPTIONS /api/users
â†’ Returns: Allow: GET, POST, PUT, DELETE
```

## Key Points:
- Returns allowed methods.
- Used for CORS preflight.
- Browser sends automatically.
- No request body.
- Safe and idempotent.

## Interview Tip:
"OPTIONS is used for CORS preflight â€” the browser sends it before cross-origin requests."

---

## Question 18: What is the purpose of the HEAD method?

## Answer:
HEAD is identical to GET but returns only headers, no body. It's used to check if a resource exists or to get metadata.

```
HEAD /api/users/1
â†’ Returns headers only, no body
```

## Key Points:
- Same as GET but no body.
- Check resource existence.
- Get metadata (Content-Length, Last-Modified).
- Safe and idempotent.
- Faster than GET.

## Interview Tip:
"HEAD is GET without the body â€” useful for checking if a resource exists."

---

## Question 19: What is the difference between PUT and PATCH?

## Answer:
| Feature | PUT | PATCH |
|---------|-----|-------|
| Purpose | Replace entire resource | Update specific fields |
| Body | All fields required | Only changed fields |
| Idempotent | Yes | Not necessarily |
| Use case | Full replacement | Partial update |

## Key Points:
- PUT: full replacement, all fields required.
- PATCH: partial update, only changed fields.
- PUT is idempotent; PATCH may not be.
- PUT for full updates; PATCH for partial.

## Interview Tip:
"PUT replaces everything; PATCH updates only what you send."

---

## Question 20: Which HTTP methods are idempotent?

## Answer:
- **GET**: Yes (safe, no changes).
- **PUT**: Yes (full replacement).
- **PATCH**: Not necessarily.
- **DELETE**: Yes (deleting twice = same result).
- **POST**: No (creates new resources).
- **HEAD**: Yes (same as GET, no body).
- **OPTIONS**: Yes (returns allowed methods).

## Key Points:
- GET, PUT, DELETE, HEAD, OPTIONS: idempotent.
- POST: not idempotent.
- PATCH: not necessarily idempotent.
- Idempotent = same result on multiple calls.

## Interview Tip:
"GET, PUT, DELETE are idempotent. POST is not. PATCH may or may not be."

---

## Part 3 (21â€“30): HTTP Status Codes

---

## Question 21: What are HTTP status codes?

## Answer:
HTTP status codes are three-digit numbers that indicate the result of an HTTP request. They're grouped by category:
- **2xx**: Success
- **3xx**: Redirection
- **4xx**: Client error
- **5xx**: Server error

## Key Points:
- Three-digit numbers.
- Indicate request result.
- 2xx: success, 4xx: client error, 5xx: server error.
- Standard across all HTTP APIs.

## Interview Tip:
"Status codes tell the client what happened â€” 2xx success, 4xx client error, 5xx server error."

---

## Question 22: What does 200 OK mean?

## Answer:
The request was successful. The response body contains the requested data.

```
GET /api/users/1 â†’ 200 OK (with user data)
```

## Key Points:
- Request successful.
- Response contains data.
- Most common success code.
- Used for GET, PUT, PATCH.

## Interview Tip:
"200 OK â€” the standard success response."

---

## Question 23: What does 201 Created mean?

## Answer:
A new resource was successfully created. The response should include the created resource or a Location header.

```
POST /api/users â†’ 201 Created (with new user data)
```

## Key Points:
- Resource created successfully.
- Response contains created resource.
- Location header with resource URL.
- Used for POST requests.

## Interview Tip:
"201 Created for successful POST requests that create resources."

---

## Question 24: What does 202 Accepted mean?

## Answer:
The request has been accepted for processing but hasn't completed yet. Used for async operations.

```
POST /api/reports/generate â†’ 202 Accepted (processing started)
```

## Key Points:
- Request accepted, not completed.
- For async operations.
- Client can poll for completion.
- Returns location of processing status.

## Interview Tip:
"202 Accepted for async operations â€” the request is being processed."

---

## Question 25: What does 204 No Content mean?

## Answer:
The request was successful but there's no content to return. Used for DELETE operations or updates that don't return data.

```
DELETE /api/users/1 â†’ 204 No Content
```

## Key Points:
- Success, no content.
- No response body.
- Common for DELETE.
- Also for PUT/PATCH without response.

## Interview Tip:
"204 No Content for successful operations that don't return data."

---

## Question 26: What does 400 Bad Request mean?

## Answer:
The server cannot process the request due to client error â€” invalid syntax, missing fields, or validation failure.

```
POST /api/users â†’ 400 Bad Request (missing required fields)
```

## Key Points:
- Client error.
- Invalid request data.
- Validation failures.
- Missing required fields.

## Interview Tip:
"400 Bad Request for validation errors â€” the client sent invalid data."

---

## Question 27: What does 401 Unauthorized mean?

## Answer:
The client is not authenticated. The request lacks valid credentials.

```
GET /api/users â†’ 401 Unauthorized (no token provided)
```

## Key Points:
- Not authenticated.
- Missing or invalid credentials.
- Client should authenticate.
- Different from 403 (not authorized).

## Interview Tip:
"401 = not authenticated (who are you?). 403 = not authorized (what can you do?)."

---

## Question 28: What does 403 Forbidden mean?

## Answer:
The client is authenticated but not authorized to access the resource.

```
DELETE /api/users/1 â†’ 403 Forbidden (not an admin)
```

## Key Points:
- Authenticated but not authorized.
- Client doesn't have permission.
- Different from 401 (not authenticated).
- Don't reveal why access is denied.

## Interview Tip:
"403 Forbidden = you're logged in but don't have permission."

---

## Question 29: What does 404 Not Found mean?

## Answer:
The requested resource doesn't exist.

```
GET /api/users/999 â†’ 404 Not Found
```

## Key Points:
- Resource doesn't exist.
- Most common error code.
- Don't reveal internal structure.
- Return consistent error format.

## Interview Tip:
"404 Not Found â€” the resource doesn't exist."

---

## Question 30: What does 500 Internal Server Error mean?

## Answer:
The server encountered an unexpected condition that prevented it from fulfilling the request.

```
GET /api/users â†’ 500 Internal Server Error (database connection failed)
```

## Key Points:
- Server-side error.
- Unexpected condition.
- Don't expose internal details.
- Log the error for debugging.

## Interview Tip:
"500 is a server error â€” log it but don't expose internal details to the client."

---

## Part 4 (31â€“40): Request & Response

---

## Question 31: What are HTTP headers?

## Answer:
Headers are key-value pairs sent with HTTP requests and responses. They provide metadata about the request or response.

```
Content-Type: application/json
Authorization: Bearer eyJhbGciOi...
Accept: application/json
```

## Key Points:
- Key-value pairs.
- Metadata about request/response.
- Standard headers: Content-Type, Authorization.
- Custom headers for application-specific data.

## Interview Tip:
"Headers provide metadata â€” Content-Type, Authorization, Accept are the most common."

---

## Question 32: What is the request body?

## Answer:
The request body contains data sent by the client to the server. Used with POST, PUT, PATCH methods.

```json
POST /api/users
Body: { "name": "Alice", "email": "alice@example.com" }
```

## Key Points:
- Data sent to server.
- Used with POST, PUT, PATCH.
- JSON format typically.
- Not used with GET, DELETE.

## Interview Tip:
"The request body carries data to the server â€” JSON is the standard format."

---

## Question 33: What is the response body?

## Answer:
The response body contains data returned by the server to the client.

```json
GET /api/users/1
Response: { "id": 1, "name": "Alice", "email": "alice@example.com" }
```

## Key Points:
- Data returned to client.
- JSON format typically.
- Contains requested resource or error details.
- May be empty (204 No Content).

## Interview Tip:
"The response body carries data back to the client â€” always use consistent format."

---

## Question 34: What are query parameters?

## Answer:
Query parameters are key-value pairs appended to the URL after `?`.

```
GET /api/users?page=1&limit=10&sort=name
```

## Key Points:
- Appended to URL after `?`.
- Key=value pairs, separated by `&`.
- For filtering, sorting, pagination.
- Optional parameters.
- Visible in URL.

## Interview Tip:
"Query parameters for filtering, sorting, and pagination."

---

## Question 35: What are path parameters?

## Answer:
Path parameters are dynamic segments in the URL path.

```
GET /api/users/1      â†’ { id: 1 }
GET /api/users/1/posts â†’ { userId: 1 }
```

## Key Points:
- Dynamic URL segments.
- Identify specific resources.
- Required for the endpoint.
- Part of the URL path.

## Interview Tip:
"Path parameters identify specific resources â€” `/users/1` gets user 1."

---

## Question 36: What is the difference between path parameters and query parameters?

## Answer:
| Feature | Path Parameters | Query Parameters |
|---------|----------------|------------------|
| Purpose | Identify resource | Filter, sort, paginate |
| Required | Yes | Optional |
| Syntax | `/users/1` | `?page=1` |
| Use case | Specific resource | Options, filters |

## Key Points:
- Path: identify resources (required).
- Query: options, filters (optional).
- Path for specific resources.
- Query for modifiers.

## Interview Tip:
"Path parameters for resources; query parameters for options."

---

## Question 37: What is the `Content-Type` header?

## Answer:
`Content-Type` specifies the media type of the request or response body.

```
Content-Type: application/json
Content-Type: application/xml
Content-Type: multipart/form-data
```

## Key Points:
- Specifies body format.
- `application/json` for JSON.
- `multipart/form-data` for file uploads.
- Required for POST, PUT, PATCH.

## Interview Tip:
"Content-Type tells the server/client what format the body is in."

---

## Question 38: What is the `Accept` header?

## Answer:
`Accept` tells the server what content types the client can handle.

```
Accept: application/json
Accept: text/html
```

## Key Points:
- Client's preferred content types.
- Server returns matching format.
- Content negotiation.
- Multiple types with quality values.

## Interview Tip:
"Accept tells the server what format the client wants."

---

## Question 39: What is the `Authorization` header?

## Answer:
`Authorization` contains credentials for authenticating the client.

```
Authorization: Bearer eyJhbGciOi...
Authorization: Basic dXNlcjpwYXNz
```

## Key Points:
- Authentication credentials.
- Bearer token for JWT.
- Basic for username/password.
- Sent with every authenticated request.

## Interview Tip:
"Authorization header carries the token â€” Bearer for JWT, Basic for username/password."

---

## Question 40: What is the `User-Agent` header?

## Answer:
`User-Agent` identifies the client software (browser, app, library).

```
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64)
```

## Key Points:
- Identifies client software.
- Browser, app, or library.
- Used for analytics.
- Can be spoofed.

## Interview Tip:
"User-Agent identifies the client â€” useful for analytics and debugging."

---

## Part 5 (41â€“50): REST Principles

---

## Question 41: What does stateless mean in REST?

## Answer:
Stateless means each request contains all information needed to process it. The server doesn't store client state between requests.

## Key Points:
- Each request is independent.
- No server-side session.
- All data in the request.
- Enables horizontal scaling.
- Authentication via tokens.

## Interview Tip:
"Stateless = each request contains everything needed. No server-side sessions."

---

## Question 42: Why should REST APIs be stateless?

## Answer:
- **Scalability**: Any server can handle any request.
- **Reliability**: No session loss on server failure.
- **Simplicity**: No session management.
- **Caching**: Easier to cache responses.

## Key Points:
- Horizontal scaling.
- No session management.
- Any server handles any request.
- Easier caching.

## Interview Tip:
"Stateless enables horizontal scaling â€” any server can handle any request."

---

## Question 43: What is resource-based URL design?

## Answer:
URLs represent resources (nouns), not actions (verbs).

```
Good: /api/users, /api/users/1
Bad: /api/getUsers, /api/createUser
```

## Key Points:
- URLs are nouns (resources).
- HTTP methods are verbs (actions).
- `/users` not `/getUsers`.
- `/users/1` not `/getUser?id=1`.

## Interview Tip:
"URLs are nouns; HTTP methods are verbs. `/users` not `/getUsers`."

---

## Question 44: What is URI naming convention?

## Answer:
- **Plural nouns**: `/users`, not `/user`.
- **Lowercase**: `/users`, not `/Users`.
- **Hyphens**: `/user-profiles`, not `/user_profiles`.
- **No verbs**: `/users`, not `/getUsers`.
- **Hierarchical**: `/users/1/posts`.

## Key Points:
- Plural nouns.
- Lowercase.
- Hyphens for multi-word.
- No verbs.
- Hierarchical structure.

## Interview Tip:
"Plural, lowercase, hyphens, no verbs â€” the URI naming conventions."

---

## Question 45: What are REST naming best practices?

## Answer:
1. **Use nouns**: `/users`, not `/getUsers`.
2. **Use plural**: `/users`, not `/user`.
3. **Use lowercase**: `/users`, not `/Users`.
4. **Use hyphens**: `/user-profiles`.
5. **Nest for relationships**: `/users/1/posts`.

## Key Points:
- Nouns, not verbs.
- Plural naming.
- Lowercase with hyphens.
- Hierarchical for relationships.

## Interview Tip:
"Plural nouns, lowercase, hyphens â€” the REST naming best practices."

---

## Question 46: What is HATEOAS?

## Answer:
HATEOAS (Hypermedia As The Engine Of Application State) means the API response includes links to related actions.

```json
{
  "id": 1,
  "name": "Alice",
  "links": [
    { "rel": "self", "href": "/api/users/1" },
    { "rel": "posts", "href": "/api/users/1/posts" }
  ]
}
```

## Key Points:
- Responses include links.
- Clients discover actions.
- Part of REST maturity model.
- Rarely fully implemented.

## Interview Tip:
"HATEOAS includes links in responses â€” clients discover actions dynamically."

---

## Question 47: Why is HATEOAS rarely implemented?

## Answer:
- **Complexity**: Adds overhead to responses.
- **Client support**: Most clients don't use links.
- **Documentation**: Swagger/OpenAPI is sufficient.
- **Performance**: Extra data in responses.

## Key Points:
- Adds complexity.
- Clients don't use links.
- Swagger is sufficient.
- Performance overhead.

## Interview Tip:
"HATEOAS is theoretically ideal but rarely practical â€” Swagger documentation is sufficient."

---

## Question 48: What is content negotiation?

## Answer:
Content negotiation is the process of selecting the best representation for a response based on client preferences.

```
Client: Accept: application/json
Server: Content-Type: application/json
```

## Key Points:
- Client specifies preferred format.
- Server returns matching format.
- Via Accept header.
- Multiple formats supported.

## Interview Tip:
"Content negotiation lets clients request their preferred format via the Accept header."

---

## Question 49: How do clients and servers communicate in REST?

## Answer:
1. **Client sends request**: HTTP method, URL, headers, body.
2. **Server processes**: Validates, executes logic.
3. **Server sends response**: Status code, headers, body.

## Key Points:
- Request-response model.
- HTTP methods for actions.
- Status codes for results.
- Headers for metadata.
- Body for data.

## Interview Tip:
"Client sends request â†’ Server processes â†’ Server sends response."

---

## Question 50: What REST API best practices do you follow?

## Answer:
1. **Resource-based URLs**: Nouns, not verbs.
2. **Proper HTTP methods**: GET, POST, PUT, DELETE.
3. **Appropriate status codes**: 200, 201, 400, 404, 500.
4. **Consistent responses**: Same format everywhere.
5. **Versioning**: `/api/v1/`.
6. **Pagination**: For list endpoints.
7. **Validation**: Validate all input.

## Key Points:
- Resource-based URLs.
- Proper HTTP methods.
- Appropriate status codes.
- Consistent responses.
- Versioning and pagination.

## Interview Tip:
"Resource-based URLs, proper methods, consistent responses â€” the REST best practices."

---

## Part 6 (51â€“60): Authentication & Authorization

---

## Question 51: What is authentication?

## Answer:
Authentication verifies the identity of a client â€” "who are you?"

```
POST /api/login
Body: { "email": "alice@example.com", "password": "secret" }
â†’ Returns token if valid
```

## Key Points:
- Verify identity.
- "Who are you?"
- Credentials check.
- Returns token or session.

## Interview Tip:
"Authentication proves who you are â€” it's the login process."

---

## Question 52: What is authorization?

## Answer:
Authorization determines what an authenticated client can access â€” "what can you do?"

```
GET /api/admin/users â†’ 403 Forbidden (not an admin)
```

## Key Points:
- Determine permissions.
- "What can you do?"
- Role-based access control.
- Checked after authentication.

## Interview Tip:
"Authorization determines what you can do â€” it's checked after authentication."

---

## Question 53: What is the difference between authentication and authorization?

## Answer:
- **Authentication**: "Who are you?" (identity verification).
- **Authorization**: "What can you do?" (permission check).

## Key Points:
- Authentication: identity.
- Authorization: permissions.
- Authentication first, then authorization.
- 401 for auth failure, 403 for permission failure.

## Interview Tip:
"401 = not authenticated. 403 = not authorized."

---

## Question 54: What authentication methods are commonly used in REST APIs?

## Answer:
1. **Basic Auth**: Username/password in headers.
2. **Bearer Token**: JWT or opaque token.
3. **API Keys**: Key in header or query param.
4. **OAuth 2.0**: Delegated authentication.

## Key Points:
- Basic Auth: simple, not secure alone.
- Bearer Token: JWT, stateless.
- API Keys: for service-to-service.
- OAuth 2.0: third-party authentication.

## Interview Tip:
"JWT for user authentication; API Keys for service-to-service; OAuth for third-party."

---

## Question 55: What is Basic Authentication?

## Answer:
Basic Auth sends username and password as Base64-encoded string in the Authorization header.

```
Authorization: Basic dXNlcjpwYXNz
```

## Key Points:
- Username:password encoded in Base64.
- Sent in Authorization header.
- Not secure without HTTPS.
- Simple but limited.

## Interview Tip:
"Basic Auth is simple but requires HTTPS â€” credentials are Base64-encoded, not encrypted."

---

## Question 56: What is Bearer Token Authentication?

## Answer:
Bearer Token sends a token in the Authorization header. The server validates the token to authenticate the request.

```
Authorization: Bearer eyJhbGciOi...
```

## Key Points:
- Token in Authorization header.
- "Bearer" prefix.
- Stateless authentication.
- JWT or opaque token.

## Interview Tip:
"Bearer Token is the standard for REST APIs â€” stateless and scalable."

---

## Question 57: What is JWT authentication?

## Answer:
JWT (JSON Web Token) is a compact, self-contained token containing user claims. It's signed and can be verified without a database lookup.

```
Header.Payload.Signature
eyJhbGciOiJIUzI1NiJ9.eyJ1c2VySWQiOjF9.signature
```

## Key Points:
- Compact, self-contained token.
- Contains user claims.
- Signed (not encrypted).
- Stateless verification.
- Three parts: header, payload, signature.

## Interview Tip:
"JWT is self-contained â€” the server can verify it without a database lookup."

---

## Question 58: What is OAuth 2.0?

## Answer:
OAuth 2.0 is an authorization framework that allows third-party applications to access resources on behalf of a user.

## Key Points:
- Authorization framework.
- Third-party access.
- Delegated authentication.
- Access tokens and refresh tokens.
- Multiple grant types.

## Interview Tip:
"OAuth 2.0 for third-party authentication â€” 'Login with Google' uses OAuth."

---

## Question 59: When should you use API Keys?

## Answer:
- **Service-to-service**: Internal communication.
- **Public APIs**: Rate limiting per key.
- **Simple authentication**: No user context needed.
- **Webhooks**: Verify sender identity.

## Key Points:
- Service-to-service communication.
- Rate limiting.
- Simple authentication.
- Webhook verification.

## Interview Tip:
"API Keys for service-to-service; JWT for user authentication."

---

## Question 60: What authentication best practices do you follow?

## Answer:
1. **HTTPS always**: Encrypt in transit.
2. **JWT for users**: Stateless, scalable.
3. **HTTP-only cookies**: Secure token storage.
4. **Token expiration**: Short-lived access tokens.
5. **Refresh tokens**: For token renewal.
6. **Rate limiting**: Prevent brute force.

## Key Points:
- HTTPS for security.
- JWT for stateless auth.
- HTTP-only cookies.
- Token expiration.
- Rate limiting.

## Interview Tip:
"HTTPS + JWT + HTTP-only cookies + token expiration â€” the authentication best practices."

---

## Part 7 (61â€“70): JWT & Security

---

## Question 61: How does JWT work?

## Answer:
1. **User logs in**: Server validates credentials.
2. **Server creates JWT**: Signs with secret.
3. **Client stores token**: Cookie or localStorage.
4. **Client sends token**: In Authorization header.
5. **Server verifies token**: Checks signature and expiration.

## Key Points:
- Login creates token.
- Client stores and sends token.
- Server verifies on each request.
- Stateless (no server storage).
- Signed with secret.

## Interview Tip:
"JWT flow: login â†’ get token â†’ send with requests â†’ verify in middleware."

---

## Question 62: What are the three parts of a JWT?

## Answer:
1. **Header**: Algorithm and token type.
2. **Payload**: Claims (user data, expiration).
3. **Signature**: Verification signature.

```
eyJhbGciOiJIUzI1NiJ9.eyJ1c2VySWQiOjF9.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c
```

## Key Points:
- Header: algorithm, type.
- Payload: claims, data.
- Signature: verification.
- Base64-encoded.
- Not encrypted (readable).

## Interview Tip:
"JWT has three parts: header, payload, signature â€” all Base64-encoded."

---

## Question 63: What is the difference between access tokens and refresh tokens?

## Answer:
| Feature | Access Token | Refresh Token |
|---------|-------------|---------------|
| Lifetime | Short (15 min) | Long (7 days) |
| Purpose | API access | Get new access tokens |
| Storage | Memory/cookie | Secure cookie |
| Usage | Every request | Only when expired |

## Key Points:
- Access token: short-lived, for API calls.
- Refresh token: long-lived, for renewal.
- Access token expires quickly.
- Refresh token gets new access tokens.

## Interview Tip:
"Access tokens are short-lived for security; refresh tokens are long-lived for UX."

---

## Question 64: Where should JWT tokens be stored?

## Answer:
- **HTTP-only cookies**: Most secure (XSS-resistant).
- **Memory**: Most secure but lost on refresh.
- **localStorage**: Convenient but vulnerable to XSS.

## Key Points:
- HTTP-only cookies: most secure.
- Memory: secure but not persistent.
- localStorage: convenient but risky.
- Always use HTTPS.

## Interview Tip:
"HTTP-only cookies are the most secure â€” they're invisible to JavaScript."

---

## Question 65: How do you invalidate JWT tokens?

## Answer:
1. **Token blacklist**: Store invalidated tokens in Redis.
2. **Short expiration**: Expire tokens quickly.
3. **Refresh token rotation**: Invalidate old refresh tokens.
4. **Version check**: Token version in database.

## Key Points:
- Token blacklist in Redis.
- Short expiration.
- Refresh token rotation.
- Version checking.

## Interview Tip:
"JWT can't be invalidated directly â€” use a blacklist or short expiration."

---

## Question 66: How do you implement logout with JWT?

## Answer:
1. **Clear client storage**: Remove token from cookie/storage.
2. **Blacklist token**: Add to Redis blacklist.
3. **Clear refresh token**: Delete from database.

```javascript
// Server-side logout
await redis.set(`blacklist:${token}`, "true", "EX", tokenExpiration);
res.clearCookie("token");
```

## Key Points:
- Clear client token.
- Blacklist server-side.
- Clear refresh token.
- Token expires naturally.

## Interview Tip:
"Logout = clear client token + blacklist server-side."

---

## Question 67: How do you prevent token theft?

## Answer:
1. **HTTP-only cookies**: Prevent JavaScript access.
2. **Short expiration**: Limit damage window.
3. **HTTPS only**: Prevent interception.
4. **Refresh token rotation**: Detect reuse.
5. **IP binding**: Detect unusual locations.

## Key Points:
- HTTP-only cookies.
- Short expiration.
- HTTPS.
- Refresh token rotation.
- IP binding.

## Interview Tip:
"HTTP-only cookies + short expiration + HTTPS â€” the token security trifecta."

---

## Question 68: What are common JWT security mistakes?

## Answer:
1. **Storing in localStorage**: Vulnerable to XSS.
2. **Long expiration**: Extended damage window.
3. **No HTTPS**: Token interception.
4. **Weak secrets**: Easy to forge.
5. **Storing sensitive data**: JWT is readable.

## Key Points:
- localStorage is risky.
- Long expiration is dangerous.
- Always use HTTPS.
- Strong secrets.
- Don't store secrets in JWT.

## Interview Tip:
"Never store JWT in localStorage â€” use HTTP-only cookies."

---

## Question 69: How do you secure REST APIs?

## Answer:
1. **HTTPS**: Encrypt all traffic.
2. **Authentication**: Verify identity.
3. **Authorization**: Check permissions.
4. **Input validation**: Prevent injection.
5. **Rate limiting**: Prevent abuse.
6. **CORS**: Restrict origins.
7. **Security headers**: Helmet.js.

## Key Points:
- HTTPS for encryption.
- Authentication and authorization.
- Input validation.
- Rate limiting.
- CORS and security headers.

## Interview Tip:
"HTTPS + authentication + authorization + validation + rate limiting â€” the API security essentials."

---

## Question 70: What API security best practices do you follow?

## Answer:
1. **HTTPS everywhere**: No exceptions.
2. **JWT with HTTP-only cookies**: Secure token storage.
3. **Input validation**: Zod or Joi.
4. **Rate limiting**: Prevent brute force.
5. **CORS configuration**: Restrict origins.
6. **Security headers**: Helmet.js.
7. **Dependency scanning**: Check for vulnerabilities.

## Key Points:
- HTTPS everywhere.
- HTTP-only cookies for tokens.
- Input validation.
- Rate limiting.
- Security headers.

## Interview Tip:
"HTTPS, validation, rate limiting, security headers â€” the security best practices."

---

## Part 8 (71â€“80): API Design

---

## Question 71: How do you design RESTful endpoints?

## Answer:
1. **Resource-based**: `/users`, `/posts`.
2. **HTTP methods**: GET, POST, PUT, DELETE.
3. **Plural nouns**: `/users`, not `/user`.
4. **Nested for relationships**: `/users/1/posts`.
5. **Versioning**: `/api/v1/users`.

## Key Points:
- Resource-based URLs.
- HTTP methods for operations.
- Plural nouns.
- Nested for relationships.
- Versioning.

## Interview Tip:
"Resource-based URLs with HTTP methods â€” that's RESTful design."

---

## Question 72: What naming conventions do you use for endpoints?

## Answer:
- **Plural nouns**: `/users`, `/posts`.
- **Lowercase**: `/users`, not `/Users`.
- **Hyphens**: `/user-profiles`.
- **No verbs**: `/users`, not `/getUsers`.
- **Hierarchical**: `/users/1/posts`.

## Key Points:
- Plural, lowercase, hyphens.
- No verbs in URLs.
- Hierarchical for relationships.

## Interview Tip:
"Plural, lowercase, hyphens, no verbs â€” the endpoint naming conventions."

---

## Question 73: Should endpoints use nouns or verbs?

## Answer:
Nouns. HTTP methods are the verbs.

```
Good: GET /api/users
Bad: GET /api/getUsers
```

## Key Points:
- URLs are nouns (resources).
- HTTP methods are verbs (actions).
- `/users` not `/getUsers`.
- REST convention.

## Interview Tip:
"URLs are nouns; HTTP methods are verbs â€” never use verbs in URLs."

---

## Question 74: How do you design nested resources?

## Answer:
```
GET /api/users/1/posts        â†’ Posts by user 1
GET /api/users/1/posts/5      â†’ Post 5 by user 1
POST /api/users/1/posts       â†’ Create post for user 1
```

## Key Points:
- Hierarchical URLs.
- Parent-child relationships.
- `/users/1/posts` for user's posts.
- Limit nesting depth (2-3 levels).

## Interview Tip:
"Nested resources for parent-child relationships â€” but keep nesting shallow."

---

## Question 75: When should you use nested routes?

## Answer:
- **Strong ownership**: Posts belong to users.
- **Context needed**: Always in context of parent.
- **Logical hierarchy**: Natural parent-child.

Avoid when:
- **Independent resources**: Tags, categories.
- **Deep nesting**: More than 2-3 levels.

## Key Points:
- Strong ownership relationships.
- Context-dependent resources.
- Limit to 2-3 levels.
- Use top-level for independent resources.

## Interview Tip:
"Nested routes for strong ownership; top-level for independent resources."

---

## Question 76: How do you implement pagination?

## Answer:
```
GET /api/users?page=1&limit=10

Response:
{
  "data": [...],
  "meta": { "page": 1, "limit": 10, "total": 100, "pages": 10 }
}
```

## Key Points:
- `page` and `limit` query params.
- Include pagination metadata.
- Total count for page indicators.
- Cursor-based for large datasets.

## Interview Tip:
"Always include pagination metadata â€” total count, current page, total pages."

---

## Question 77: How do you implement filtering?

## Answer:
```
GET /api/users?role=admin&status=active
GET /api/products?minPrice=10&maxPrice=50
```

## Key Points:
- Query parameters for filters.
- Validate filter values.
- Index filtered columns.
- Document available filters.

## Interview Tip:
"Use query parameters for filtering â€” validate all values."

---

## Question 78: How do you implement sorting?

## Answer:
```
GET /api/users?sort=name        â†’ Ascending
GET /api/users?sort=-name       â†’ Descending
GET /api/users?sort=name,-createdAt â†’ Multiple fields
```

## Key Points:
- `sort` query parameter.
- `-` prefix for descending.
- Multiple fields with commas.
- Index sorted columns.

## Interview Tip:
"Use `-` prefix for descending: `sort=-createdAt`."

---

## Question 79: How do you implement searching?

## Answer:
```
GET /api/users?search=alice
GET /api/products?search=phone&category=electronics
```

## Key Points:
- `search` query parameter.
- Full-text search for text fields.
- Combine with filters.
- Index search columns.

## Interview Tip:
"Use `search` query parameter for text search â€” combine with filters."

---

## Question 80: What API design mistakes should you avoid?

## Answer:
1. **Verbs in URLs**: `/getUsers` instead of `/users`.
2. **Wrong HTTP methods**: Using GET for mutations.
3. **Inconsistent responses**: Different formats per endpoint.
4. **No pagination**: Returning all records.
5. **No versioning**: Breaking changes without versioning.
6. **Exposing internals**: Database IDs in URLs.

## Key Points:
- No verbs in URLs.
- Correct HTTP methods.
- Consistent responses.
- Always paginate.
- Version your API.

## Interview Tip:
"The biggest mistake is using verbs in URLs â€” use nouns and HTTP methods."

---

## Part 9 (81â€“90): Validation & Error Handling

---

## Question 81: Why is request validation important?

## Answer:
- **Security**: Prevent injection attacks.
- **Data integrity**: Ensure valid data.
- **Error prevention**: Catch issues early.
- **User experience**: Clear error messages.

## Key Points:
- Security (injection prevention).
- Data integrity.
- Early error detection.
- Clear error messages.

## Interview Tip:
"Validation prevents bad data and security vulnerabilities â€” always validate."

---

## Question 82: How do you validate request bodies?

## Answer:
```javascript
const { z } = require("zod");

const UserSchema = z.object({
  name: z.string().min(1),
  email: z.string().email(),
  age: z.number().int().min(0)
});

const result = UserSchema.safeParse(req.body);
if (!result.success) {
  return res.status(400).json({ errors: result.error.flatten() });
}
```

## Key Points:
- Validate before processing.
- Use Zod or Joi.
- Return 400 for validation errors.
- Include error details.

## Interview Tip:
"Zod for validation â€” it gives you runtime safety and TypeScript types."

---

## Question 83: How do you validate query parameters?

## Answer:
```javascript
const QuerySchema = z.object({
  page: z.coerce.number().int().min(1).default(1),
  limit: z.coerce.number().int().min(1).max(100).default(10),
  sort: z.string().optional()
});

const result = QuerySchema.safeParse(req.query);
```

## Key Points:
- Validate query params.
- Coerce strings to numbers.
- Default values.
- Type conversion.

## Interview Tip:
"Query params are always strings â€” coerce to numbers with `z.coerce.number()`."

---

## Question 84: How do you validate route parameters?

## Answer:
```javascript
const ParamsSchema = z.object({
  id: z.coerce.number().int().positive()
});

const result = ParamsSchema.safeParse(req.params);
```

## Key Points:
- Validate route params.
- Coerce to correct type.
- Validate format (UUID, integer).
- Return 400 for invalid params.

## Interview Tip:
"Route params are strings â€” coerce and validate them."

---

## Question 85: What validation libraries have you used?

## Answer:
- **Zod**: TypeScript-first, runtime validation.
- **Joi**: Popular, schema-based.
- **Yup**: Similar to Joi.
- **express-validator**: Express-specific.

## Key Points:
- Zod: TypeScript-first, recommended.
- Joi: most popular.
- Yup: browser-friendly.
- express-validator: Express-specific.

## Interview Tip:
"Zod is my go-to â€” TypeScript-first with runtime validation."

---

## Question 86: How do you return validation errors?

## Answer:
```json
{
  "error": {
    "code": "VALIDATION_ERROR",
    "message": "Invalid input",
    "details": [
      { "field": "email", "message": "Invalid email format" },
      { "field": "age", "message": "Must be positive" }
    ]
  }
}
```

Status: 400 Bad Request.

## Key Points:
- Consistent error format.
- Field-level error details.
- 400 status code.
- Clear error messages.

## Interview Tip:
"Return field-level validation errors â€” it helps the client fix the issue."

---

## Question 87: How do you design consistent error responses?

## Answer:
```json
{
  "error": {
    "code": "NOT_FOUND",
    "message": "User not found",
    "status": 404
  }
}
```

All errors follow the same structure.

## Key Points:
- Consistent format across all errors.
- Include code, message, status.
- Field-level details for validation.
- Don't expose internal details.

## Interview Tip:
"A consistent error format makes your API predictable and easy to consume."

---

## Question 88: What HTTP status codes should validation errors use?

## Answer:
- **400 Bad Request**: Invalid input data.
- **422 Unprocessable Entity**: Valid syntax, invalid data.
- **409 Conflict**: Duplicate data.

## Key Points:
- 400: general validation errors.
- 422: valid syntax, invalid data.
- 409: conflicts (duplicates).
- Be consistent.

## Interview Tip:
"400 for validation errors; 422 for semantic errors; 409 for conflicts."

---

## Question 89: How do you handle unexpected server errors?

## Answer:
```javascript
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).json({
    error: {
      code: "INTERNAL_ERROR",
      message: "An unexpected error occurred"
    }
  });
});
```

## Key Points:
- Catch all errors.
- Log for debugging.
- Don't expose internal details.
- Return generic message.

## Interview Tip:
"Log the error, return a generic message â€” never expose stack traces to clients."

---

## Question 90: What error-handling best practices do you follow?

## Answer:
1. **Consistent format**: Same error structure everywhere.
2. **Appropriate status codes**: 400, 401, 403, 404, 500.
3. **Field-level details**: For validation errors.
4. **Don't expose internals**: No stack traces in production.
5. **Log errors**: For debugging.

## Key Points:
- Consistent format.
- Appropriate status codes.
- Field-level details.
- Hide internal details.
- Log for debugging.

## Interview Tip:
"Consistent format + appropriate status codes + field-level details â€” the error handling best practices."

---

## Part 10 (91â€“100): Versioning & Documentation

---

## Question 91: Why should APIs be versioned?

## Answer:
- **Backward compatibility**: Don't break existing clients.
- **Independent evolution**: New features without breaking old.
- **Client migration**: Clients can upgrade at their pace.
- **Breaking changes**: Manage breaking changes safely.

## Key Points:
- Backward compatibility.
- Independent evolution.
- Client migration.
- Breaking change management.

## Interview Tip:
"Versioning prevents breaking existing clients â€” it's essential for production APIs."

---

## Question 92: What API versioning strategies are available?

## Answer:
1. **URI versioning**: `/api/v1/users`.
2. **Header versioning**: `Accept-Version: 1`.
3. **Media type versioning**: `Accept: application/vnd.api.v1+json`.
4. **Query parameter**: `/api/users?version=1`.

## Key Points:
- URI: most common, visible.
- Header: cleaner URLs.
- Media type: content negotiation.
- Query parameter: simple.

## Interview Tip:
"URI versioning is the most practical â€” visible and easy to test."

---

## Question 93: What is URI versioning?

## Answer:
Version in the URL path.

```
/api/v1/users
/api/v2/users
```

## Key Points:
- Version in URL path.
- Most visible approach.
- Easy to route.
- Easy to test.

## Interview Tip:
"URI versioning is the most common â€” `/api/v1/users`."

---

## Question 94: What is header versioning?

## Answer:
Version in the request header.

```
GET /api/users
Accept-Version: 1
```

## Key Points:
- Version in header.
- Cleaner URLs.
- Less visible.
- Harder to test.

## Interview Tip:
"Header versioning keeps URLs clean but is harder to test."

---

## Question 95: What is media type versioning?

## Answer:
Version in the Accept header.

```
GET /api/users
Accept: application/vnd.api.v1+json
```

## Key Points:
- Version in Accept header.
- Content negotiation.
- Complex but flexible.
- Rarely used.

## Interview Tip:
"Media type versioning is complex â€” URI versioning is simpler."

---

## Question 96: How do you document REST APIs?

## Answer:
1. **OpenAPI/Swagger**: Industry standard.
2. **Postman Collections**: Shareable API docs.
3. **README**: Quick start guide.
4. **Code annotations**: Generate docs from code.

## Key Points:
- OpenAPI/Swagger for standard docs.
- Postman for testing.
- README for quick start.
- Auto-generation from code.

## Interview Tip:
"Swagger/OpenAPI is the standard â€” generate docs from code annotations."

---

## Question 97: What is OpenAPI (Swagger)?

## Answer:
OpenAPI (formerly Swagger) is a specification for describing REST APIs. It defines endpoints, parameters, responses, and authentication.

## Key Points:
- API specification standard.
- Describes endpoints, parameters, responses.
- Machine-readable (YAML/JSON).
- Generates interactive docs.
- Industry standard.

## Interview Tip:
"OpenAPI is the standard for API documentation â€” Swagger UI makes it interactive."

---

## Question 98: How do you generate API documentation?

## Answer:
```javascript
// swagger-jsdoc
const swaggerJsdoc = require("swagger-jsdoc");
const options = {
  definition: { openapi: "3.0.0", info: { title: "API", version: "1.0.0" } },
  apis: ["./routes/*.js"]
};
const specs = swaggerJsdoc(options);
```

## Key Points:
- Generate from code annotations.
- swagger-jsdoc for Express.
- Swagger UI for interactive docs.
- Keep docs in sync with code.

## Interview Tip:
"Generate docs from code annotations â€” it keeps them in sync."

---

## Question 99: How do you test REST APIs?

## Answer:
- **Postman**: Manual testing and collections.
- **Supertest**: Automated integration tests.
- **curl**: Command-line testing.
- **Jest**: Unit tests for business logic.

## Key Points:
- Postman for manual testing.
- Supertest for automated tests.
- curl for quick tests.
- Jest for unit tests.

## Interview Tip:
"Supertest for automated API tests; Postman for manual testing."

---

## Question 100: What REST API documentation best practices do you follow?

## Answer:
1. **OpenAPI spec**: Industry standard.
2. **Examples**: Request/response examples.
3. **Error documentation**: All error codes.
4. **Authentication**: How to authenticate.
5. **Versioning**: Document versions.

## Key Points:
- OpenAPI specification.
- Request/response examples.
- Error documentation.
- Authentication guide.
- Version documentation.

## Interview Tip:
"Examples are the most important part of API documentation â€” show request and response."

---

## Part 11 (101â€“110): Performance & Caching

---

## Question 101: How do you optimize REST API performance?

## Answer:
1. **Caching**: HTTP caching, Redis.
2. **Pagination**: Limit response size.
3. **Compression**: gzip responses.
4. **Database optimization**: Indexes, query optimization.
5. **CDN**: Static assets.
6. **Connection pooling**: Database connections.

## Key Points:
- Caching for frequent data.
- Pagination for large datasets.
- Compression for smaller responses.
- Database optimization.
- CDN for static assets.

## Interview Tip:
"Caching and pagination are the biggest performance wins."

---

## Question 102: What is HTTP caching?

## Answer:
HTTP caching stores responses to avoid re-fetching. The server sets cache headers, and clients/intermediaries cache responses.

## Key Points:
- Store responses for reuse.
- Cache-Control header.
- ETag for validation.
- Reduces server load.

## Interview Tip:
"HTTP caching reduces server load â€” use Cache-Control and ETag headers."

---

## Question 103: What is the `Cache-Control` header?

## Answer:
`Cache-Control` specifies caching behavior.

```
Cache-Control: public, max-age=3600      # Cache for 1 hour
Cache-Control: private, no-cache          # Don't cache
Cache-Control: no-store                   # Don't store at all
```

## Key Points:
- `public`: CDN can cache.
- `private`: only browser can cache.
- `max-age`: cache duration in seconds.
- `no-cache`: revalidate before use.
- `no-store`: don't cache.

## Interview Tip:
"`max-age=3600` caches for 1 hour. Use `private` for user-specific data."

---

## Question 104: What is an ETag?

## Answer:
An ETag is a unique identifier for a specific version of a resource. The server sends it, and the client can use it to check if the resource has changed.

```
ETag: "abc123"
```

## Key Points:
- Unique identifier for resource version.
- Server sends in response.
- Client sends in conditional requests.
- Prevents unnecessary data transfer.

## Interview Tip:
"ETags prevent unnecessary data transfer â€” the client checks if the resource changed."

---

## Question 105: What are conditional requests?

## Answer:
Conditional requests include headers that specify conditions. The server only returns data if conditions are met.

```
If-None-Match: "abc123"    # Only if ETag doesn't match
If-Modified-Since: Tue, 01 Jan 2024  # Only if modified since
```

## Key Points:
- Include conditions in headers.
- Server checks conditions.
- Returns 304 Not Modified if unchanged.
- Saves bandwidth.

## Interview Tip:
"Conditional requests save bandwidth â€” return 304 if nothing changed."

---

## Question 106: What is the `If-None-Match` header?

## Answer:
`If-None-Match` sends the ETag. The server returns 304 if the resource hasn't changed.

```
If-None-Match: "abc123"
â†’ 304 Not Modified (if unchanged)
â†’ 200 OK with new data (if changed)
```

## Key Points:
- Sends ETag for validation.
- 304 if unchanged.
- 200 with new data if changed.
- Saves bandwidth.

## Interview Tip:
"`If-None-Match` with ETag â€” return 304 if nothing changed."

---

## Question 107: What is the `If-Modified-Since` header?

## Answer:
`If-Modified-Since` sends a date. The server returns 304 if the resource hasn't been modified since that date.

```
If-Modified-Since: Tue, 01 Jan 2024 00:00:00 GMT
â†’ 304 Not Modified (if unchanged)
â†’ 200 OK with new data (if changed)
```

## Key Points:
- Sends date for validation.
- 304 if not modified since.
- 200 with new data if modified.
- Time-based validation.

## Interview Tip:
"`If-Modified-Since` for time-based cache validation."

---

## Question 108: When should you cache API responses?

## Answer:
- **Public data**: Same for all users.
- **Rarely changing**: Static or semi-static data.
- **Expensive operations**: Complex queries.
- **High traffic**: Frequently accessed endpoints.

## Key Points:
- Public, shared data.
- Rarely changing data.
- Expensive operations.
- High-traffic endpoints.

## Interview Tip:
"Cache public, rarely-changing data â€” don't cache user-specific or real-time data."

---

## Question 109: What data should not be cached?

## Answer:
- **User-specific data**: Personal information.
- **Real-time data**: Stock prices, live scores.
- **Sensitive data**: Financial information.
- **Frequently changing**: Data that changes every request.

## Key Points:
- User-specific data.
- Real-time data.
- Sensitive data.
- Frequently changing data.

## Interview Tip:
"Don't cache user-specific or real-time data â€” use `Cache-Control: no-store`."

---

## Question 110: What caching best practices do you follow?

## Answer:
1. **Cache public data**: Same for all users.
2. **Set appropriate TTL**: Balance freshness and performance.
3. **Use ETags**: For conditional requests.
4. **CDN caching**: For global distribution.
5. **Redis caching**: For expensive operations.

## Key Points:
- Cache public data.
- Appropriate TTL.
- ETags for validation.
- CDN for global caching.
- Redis for expensive operations.

## Interview Tip:
"Cache-Control for browser caching; Redis for server-side caching; CDN for global caching."

---

## Part 12 (111â€“120): Idempotency & Reliability

---

## Question 111: What is idempotency?

## Answer:
Idempotency means making the same request multiple times produces the same result as making it once.

## Key Points:
- Same result on multiple calls.
- Safe to retry.
- GET, PUT, DELETE are idempotent.
- POST is not idempotent.

## Interview Tip:
"Idempotent = calling twice is the same as calling once."

---

## Question 112: Which HTTP methods are idempotent?

## Answer:
- **GET**: Yes (read-only).
- **PUT**: Yes (full replacement).
- **DELETE**: Yes (deleting twice = same result).
- **PATCH**: Not necessarily.
- **POST**: No (creates new resources).

## Key Points:
- GET, PUT, DELETE: idempotent.
- POST: not idempotent.
- PATCH: not necessarily.

## Interview Tip:
"GET, PUT, DELETE are idempotent. POST is not."

---

## Question 113: Why is idempotency important?

## Answer:
- **Safe retries**: Network failures can be retried.
- **Consistency**: No duplicate side effects.
- **Reliability**: Operations can be repeated safely.

## Key Points:
- Safe to retry.
- No duplicate effects.
- Network reliability.
- Consistent behavior.

## Interview Tip:
"Idempotency makes retries safe â€” essential for reliable APIs."

---

## Question 114: How do you make POST requests idempotent?

## Answer:
Use an idempotency key â€” a unique identifier the client sends with each request.

```
POST /api/payments
Idempotency-Key: abc123
Body: { "amount": 100 }
```

## Key Points:
- Unique idempotency key.
- Server checks if key was used.
- Returns cached result if duplicate.
- Prevents duplicate operations.

## Interview Tip:
"Idempotency keys make POST requests idempotent â€” essential for payments."

---

## Question 115: What is an idempotency key?

## Answer:
An idempotency key is a unique identifier sent with a request. The server stores it and returns the cached response for duplicate keys.

## Key Points:
- Unique identifier per request.
- Server stores and checks.
- Returns cached response for duplicates.
- Prevents duplicate operations.

## Interview Tip:
"Idempotency keys prevent duplicate operations â€” essential for financial transactions."

---

## Question 116: How do you prevent duplicate requests?

## Answer:
1. **Idempotency keys**: Unique per request.
2. **Database constraints**: Unique constraints.
3. **Redis locks**: Distributed locks.
4. **Token-based dedup**: Track processed requests.

## Key Points:
- Idempotency keys.
- Database unique constraints.
- Redis distributed locks.
- Token deduplication.

## Interview Tip:
"Idempotency keys + database constraints = duplicate prevention."

---

## Question 117: How do you handle retries safely?

## Answer:
1. **Idempotent operations**: Safe to retry.
2. **Exponential backoff**: Wait before retrying.
3. **Max retries**: Limit retry attempts.
4. **Idempotency keys**: For non-idempotent operations.

## Key Points:
- Idempotent operations for safety.
- Exponential backoff.
- Max retry limits.
- Idempotency keys for POST.

## Interview Tip:
"Exponential backoff + idempotency keys = safe retries."

---

## Question 118: What are distributed transactions?

## Answer:
Distributed transactions span multiple services or databases. They're complex because all services must succeed or all must roll back.

## Key Points:
- Span multiple services.
- All-or-nothing semantics.
- Complex to implement.
- Saga pattern for compensation.

## Interview Tip:
"Distributed transactions are complex â€” use the Saga pattern for compensation."

---

## Question 119: How do you ensure data consistency across services?

## Answer:
1. **Saga pattern**: Compensating transactions.
2. **Event sourcing**: Store events, replay for consistency.
3. **Two-phase commit**: Lock then commit.
4. **Eventual consistency**: Accept temporary inconsistency.

## Key Points:
- Saga pattern for compensation.
- Event sourcing for replay.
- Two-phase commit for strong consistency.
- Eventual consistency for performance.

## Interview Tip:
"Saga pattern is the most practical for microservices â€” compensate on failure."

---

## Question 120: What reliability best practices do you follow?

## Answer:
1. **Idempotent operations**: Safe retries.
2. **Circuit breakers**: Prevent cascading failures.
3. **Timeouts**: Don't wait forever.
4. **Retries with backoff**: Handle transient failures.
5. **Health checks**: Monitor service health.

## Key Points:
- Idempotent operations.
- Circuit breakers.
- Timeouts.
- Retries with backoff.
- Health checks.

## Interview Tip:
"Idempotent operations + circuit breakers + timeouts = reliable APIs."

---

## Part 13 (121â€“130): Scalability & Architecture

---

## Question 121: How do you scale REST APIs?

## Answer:
1. **Horizontal scaling**: More servers.
2. **Load balancing**: Distribute traffic.
3. **Caching**: Redis, CDN.
4. **Database optimization**: Read replicas, connection pooling.
5. **Async processing**: Background jobs.

## Key Points:
- Horizontal scaling.
- Load balancing.
- Caching.
- Database optimization.
- Async processing.

## Interview Tip:
"Horizontal scaling + caching + database optimization = scalable APIs."

---

## Question 122: What is an API Gateway?

## Answer:
An API Gateway is a single entry point for all API requests. It handles routing, authentication, rate limiting, and other cross-cutting concerns.

## Key Points:
- Single entry point.
- Routing to services.
- Authentication.
- Rate limiting.
- Cross-cutting concerns.

## Interview Tip:
"API Gateway = single entry point for all API requests."

---

## Question 123: Why use an API Gateway?

## Answer:
- **Single entry point**: Simplifies client integration.
- **Cross-cutting concerns**: Auth, rate limiting, logging.
- **Routing**: Route to appropriate services.
- **Load balancing**: Distribute traffic.
- **Security**: Centralized security.

## Key Points:
- Single entry point.
- Cross-cutting concerns.
- Routing and load balancing.
- Centralized security.

## Interview Tip:
"API Gateway handles auth, rate limiting, and routing â€” one place for all cross-cutting concerns."

---

## Question 124: What is a reverse proxy?

## Answer:
A reverse proxy sits between clients and servers, forwarding requests to backend servers. It provides load balancing, caching, and security.

## Key Points:
- Sits between clients and servers.
- Forwards requests.
- Load balancing.
- Caching and security.
- Nginx, HAProxy.

## Interview Tip:
"Reverse proxy = load balancer + cache + security layer."

---

## Question 125: What is load balancing?

## Answer:
Load balancing distributes incoming requests across multiple servers to prevent any single server from being overwhelmed.

## Key Points:
- Distributes requests.
- Multiple servers.
- Prevents overload.
- Round-robin, least connections.
- Nginx, AWS ALB.

## Interview Tip:
"Load balancing distributes traffic â€” essential for scalability."

---

## Question 126: What is horizontal scaling?

## Answer:
Horizontal scaling (scaling out) adds more servers to handle increased load.

## Key Points:
- Add more servers.
- Each handles portion of load.
- Load balancer distributes.
- More resilient.

## Interview Tip:
"Horizontal scaling = more servers. Vertical scaling = bigger server."

---

## Question 127: What is vertical scaling?

## Answer:
Vertical scaling (scaling up) adds more resources (CPU, RAM) to a single server.

## Key Points:
- Add resources to one server.
- Simpler but limited.
- Hardware maximums.
- Single point of failure.

## Interview Tip:
"Vertical scaling has limits â€” horizontal scaling is more resilient."

---

## Question 128: How do REST APIs work in a microservices architecture?

## Answer:
Each microservice exposes its own REST API. An API Gateway routes requests to appropriate services.

```
Client â†’ API Gateway â†’ User Service (REST API)
                     â†’ Order Service (REST API)
                     â†’ Payment Service (REST API)
```

## Key Points:
- Each service has its own API.
- API Gateway routes requests.
- Services communicate via REST or messaging.
- Independent deployment.

## Interview Tip:
"Each microservice has its own REST API â€” the gateway routes requests."

---

## Question 129: How do microservices communicate?

## Answer:
1. **REST APIs**: Synchronous, HTTP-based.
2. **Message queues**: Asynchronous (RabbitMQ, Kafka).
3. **gRPC**: High-performance RPC.
4. **WebSockets**: Real-time communication.

## Key Points:
- REST for synchronous.
- Message queues for asynchronous.
- gRPC for performance.
- WebSockets for real-time.

## Interview Tip:
"REST for synchronous; message queues for asynchronous; gRPC for performance."

---

## Question 130: What architecture best practices do you follow?

## Answer:
1. **API Gateway**: Single entry point.
2. **Service isolation**: Independent services.
3. **Async communication**: Message queues for non-blocking.
4. **Caching**: Redis for frequent data.
5. **Monitoring**: Track all services.

## Key Points:
- API Gateway for routing.
- Service isolation.
- Async communication.
- Caching for performance.
- Monitoring for observability.

## Interview Tip:
"API Gateway + service isolation + async communication + caching + monitoring."

---

## Part 14 (131â€“140): Monitoring & Production

---

## Question 131: How do you monitor REST APIs?

## Answer:
1. **Response times**: Track latency.
2. **Error rates**: Monitor 4xx, 5xx errors.
3. **Request volume**: Traffic patterns.
4. **Uptime**: Health checks.
5. **Logs**: Structured logging.

## Key Points:
- Response times.
- Error rates.
- Request volume.
- Uptime monitoring.
- Structured logging.

## Interview Tip:
"Monitor response times, error rates, and uptime â€” the API monitoring essentials."

---

## Question 132: What API metrics do you track?

## Answer:
- **Latency**: Response time (p50, p95, p99).
- **Error rate**: Percentage of failed requests.
- **Throughput**: Requests per second.
- **Availability**: Uptime percentage.
- **Saturation**: Resource usage.

## Key Points:
- Latency percentiles.
- Error rate percentage.
- Throughput (RPS).
- Availability (uptime).
- Saturation (resources).

## Interview Tip:
"Latency, error rate, throughput, availability â€” the four golden signals."

---

## Question 133: How do you log API requests?

## Answer:
```javascript
app.use(morgan("combined"));
// Or structured logging
app.use((req, res, next) => {
  logger.info({
    method: req.method,
    path: req.path,
    status: res.statusCode,
    duration: Date.now() - start
  });
  next();
});
```

## Key Points:
- Morgan for HTTP logging.
- Structured logging (JSON).
- Log method, path, status, duration.
- Include request ID for tracing.

## Interview Tip:
"Structured JSON logging is essential â€” it enables searching and analysis."

---

## Question 134: How do you trace requests across services?

## Answer:
1. **Request ID**: Unique ID per request.
2. **Correlation ID**: Propagate across services.
3. **Distributed tracing**: Jaeger, Zipkin.
4. **Logging**: Include request ID in all logs.

## Key Points:
- Unique request ID.
- Propagate across services.
- Distributed tracing tools.
- Include in all logs.

## Interview Tip:
"Request ID + correlation ID + distributed tracing = request tracing."

---

## Question 135: How do you debug production API issues?

## Answer:
1. **Check logs**: Structured logs with request ID.
2. **Check metrics**: Latency, error rates.
3. **Reproduce**: Try in staging.
4. **Check dependencies**: Database, external APIs.
5. **Profile**: CPU, memory usage.

## Key Points:
- Logs for context.
- Metrics for patterns.
- Reproduce in staging.
- Check dependencies.
- Profile resources.

## Interview Tip:
"Start with logs and metrics â€” they show what went wrong."

---

## Question 136: How do you implement rate limiting?

## Answer:
```javascript
const rateLimit = require("express-rate-limit");

const limiter = rateLimit({
  windowMs: 15 * 60 * 1000, // 15 minutes
  max: 100, // 100 requests per window
  message: { error: "Too many requests" }
});

app.use("/api/", limiter);
```

## Key Points:
- Limit requests per time window.
- Different limits per endpoint.
- Return 429 on limit.
- Use Redis for distributed limiting.

## Interview Tip:
"Rate limiting prevents abuse â€” use Redis for distributed rate limiting."

---

## Question 137: How do you handle API throttling?

## Answer:
Throttling delays or rejects requests when limits are exceeded.

```javascript
// Return 429 with Retry-After header
res.status(429).json({
  error: "Too many requests",
  retryAfter: 60
});
res.setHeader("Retry-After", 60);
```

## Key Points:
- Delay or reject excessive requests.
- 429 status code.
- Retry-After header.
- Different limits per user/tier.

## Interview Tip:
"Return 429 with Retry-After header â€” clients know when to retry."

---

## Question 138: How do you secure APIs in production?

## Answer:
1. **HTTPS**: Encrypt all traffic.
2. **Authentication**: JWT or API keys.
3. **Authorization**: Role-based access.
4. **Rate limiting**: Prevent abuse.
5. **Input validation**: Prevent injection.
6. **CORS**: Restrict origins.
7. **Security headers**: Helmet.js.

## Key Points:
- HTTPS everywhere.
- Authentication and authorization.
- Rate limiting.
- Input validation.
- CORS and security headers.

## Interview Tip:
"HTTPS + auth + rate limiting + validation + CORS = production security."

---

## Question 139: What production deployment best practices do you follow?

## Answer:
1. **Health checks**: `/health` endpoint.
2. **Graceful shutdown**: Handle SIGTERM.
3. **Environment variables**: Secure configuration.
4. **Logging**: Structured logging.
5. **Monitoring**: Track metrics.
6. **Rollback plan**: Quick rollback on issues.

## Key Points:
- Health checks.
- Graceful shutdown.
- Environment variables.
- Logging and monitoring.
- Rollback plan.

## Interview Tip:
"Health checks + graceful shutdown + monitoring = production-ready deployment."

---

## Question 140: How do you test REST APIs in production?

## Answer:
1. **Smoke tests**: Basic functionality after deploy.
2. **Synthetic monitoring**: Simulated user requests.
3. **Canary testing**: Test with small traffic percentage.
4. **A/B testing**: Compare versions.

## Key Points:
- Smoke tests after deploy.
- Synthetic monitoring.
- Canary testing.
- A/B testing.

## Interview Tip:
"Smoke tests after every deploy â€” verify basic functionality."

---

## Part 15 (141â€“150): Senior Real-World Interview Questions

---

## Question 141: Describe the largest REST API you've built.

## Answer:
Pick a real project and describe:
- **Scale**: Endpoints, users, requests per second.
- **Architecture**: Microservices, databases.
- **Challenges**: What was hard and how you solved it.
- **Your role**: What you specifically contributed.
- **Results**: Performance improvements.

## Key Points:
- Quantify the scale.
- Describe the architecture.
- Highlight challenges.
- Explain your contributions.
- Show impact.

## Interview Tip:
"Tell a story with a beginning (problem), middle (solution), and end (result)."

---

## Question 142: What was the most challenging API design problem you've solved?

## Answer:
Describe:
1. **Symptoms**: What was happening.
2. **Investigation**: How you diagnosed it.
3. **Root cause**: What was wrong.
4. **Fix**: How you resolved it.
5. **Lesson**: What you learned.

## Key Points:
- Symptoms, investigation, root cause, fix, lesson.
- Debugging process.
- Tools used.
- What you learned.

## Interview Tip:
"Interviewers want to see your design thinking process."

---

## Question 143: How do you review REST API pull requests?

## Answer:
Check for:
1. **Naming conventions**: Resource-based URLs.
2. **HTTP methods**: Correct methods.
3. **Status codes**: Appropriate codes.
4. **Validation**: Input validation.
5. **Error handling**: Consistent errors.
6. **Security**: Auth, input sanitization.

## Key Points:
- Naming conventions.
- HTTP methods and status codes.
- Validation and error handling.
- Security checks.

## Interview Tip:
"Check naming, methods, status codes, validation, and security."

---

## Question 144: How do you design APIs for backward compatibility?

## Answer:
1. **Versioning**: `/api/v1/`, `/api/v2/`.
2. **Additive changes**: Add fields, don't remove.
3. **Optional fields**: New fields are optional.
4. **Deprecation notices**: Warn before removing.
5. **Documentation**: Document changes.

## Key Points:
- Versioning for breaking changes.
- Additive changes preferred.
- Optional new fields.
- Deprecation notices.
- Document everything.

## Interview Tip:
"Add fields, don't remove them. Version for breaking changes."

---

## Question 145: How would you migrate a monolithic API to microservices?

## Answer:
1. **Identify boundaries**: Find service boundaries.
2. **Strangler fig**: Extract one service at a time.
3. **API Gateway**: Route to appropriate service.
4. **Shared database â†’ separate databases**: Gradually separate.
5. **Test thoroughly**: Verify each migration.

## Key Points:
- Identify service boundaries.
- Strangler fig pattern.
- API Gateway for routing.
- Gradual database separation.
- Test each migration.

## Interview Tip:
"Strangler fig pattern â€” extract one service at a time, don't rewrite everything."

---

## Question 146: How would you design a REST API for an e-commerce platform?

## Answer:
```
/api/v1/products         â†’ Product catalog
/api/v1/users            â†’ User management
/api/v1/orders           â†’ Order management
/api/v1/cart             â†’ Shopping cart
/api/v1/payments         â†’ Payment processing
/api/v1/reviews          â†’ Product reviews
```

## Key Points:
- Resource-based endpoints.
- Nested for relationships.
- Versioning from day one.
- Pagination for all lists.
- Comprehensive error handling.

## Interview Tip:
"Resource-based design with versioning â€” products, users, orders, cart, payments."

---

## Question 147: How would you design a REST API for a school management system?

## Answer:
```
/api/v1/students         â†’ Student management
/api/v1/teachers         â†’ Teacher management
/api/v1/courses          â†’ Course management
/api/v1/enrollments      â†’ Student-course relationships
/api/v1/grades           â†’ Grade management
/api/v1/attendance       â†’ Attendance tracking
```

## Key Points:
- Resource-based endpoints.
- Many-to-many relationships (enrollments).
- Nested resources for context.
- Versioning and pagination.

## Interview Tip:
"Many-to-many relationships (enrollments) are the key design challenge."

---

## Question 148: What REST API features do you use most frequently in production?

## Answer:
- **CRUD endpoints**: Standard create/read/update/delete.
- **Pagination**: For all list endpoints.
- **Validation**: Zod for input validation.
- **Error handling**: Consistent error format.
- **Authentication**: JWT with HTTP-only cookies.
- **Rate limiting**: Prevent abuse.

## Key Points:
- CRUD endpoints.
- Pagination and filtering.
- Input validation.
- Error handling.
- Authentication and rate limiting.

## Interview Tip:
"CRUD, pagination, validation, error handling, auth â€” the production essentials."

---

## Question 149: If you were starting a new production backend today, how would you design your API layer?

## Answer:
- **Express.js or Fastify**: Web framework.
- **TypeScript**: Type safety.
- **Zod**: Input validation.
- **JWT**: Authentication.
- **OpenAPI**: Documentation.
- **Rate limiting**: Prevent abuse.
- **Structured logging**: Pino.

## Key Points:
- Express/Fastify for framework.
- TypeScript for type safety.
- Zod for validation.
- JWT for auth.
- OpenAPI for docs.

## Interview Tip:
"Express + TypeScript + Zod + JWT + OpenAPI â€” the modern API stack."

---

## Question 150: In your opinion, what separates a junior, mid-level, and senior backend API developer?

## Answer:
- **Junior**: Knows basic CRUD. Can build simple endpoints.
- **Mid-level**: Understands REST principles, validation, error handling. Can design APIs independently.
- **Senior**: Designs scalable architecture, handles production issues, mentors others. Understands security, performance, and trade-offs.

The biggest differentiator: a senior thinks about failure scenarios and designs for resilience.

## Key Points:
- Junior: basic CRUD.
- Mid-level: REST principles, validation.
- Senior: architecture, security, performance.
- Senior designs for failure.
- Senior mentors others.

## Interview Tip:
"The best answer shows self-awareness. Pick your level and explain what you're doing to grow."

---

# End of REST API Interview Questions & Answers
