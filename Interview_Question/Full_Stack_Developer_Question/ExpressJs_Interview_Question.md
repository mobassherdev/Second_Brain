

# Express.js Interview Questions (150 Total)

---

## Introduction

1. What is Express.js?
2. Why was Express.js created?
3. What problems does Express.js solve?
4. What are the advantages of Express.js?
5. What are the disadvantages of Express.js?
6. How does Express.js differ from Node.js?
7. When would you use Express.js instead of the native `http` module?
8. What is the Express application object?
9. How do you create an Express application?
10. What is the request-response lifecycle in Express?

---

## Routing

11. What is routing in Express.js?
12. How do you define a GET route?
13. How do you define a POST route?
14. What are PUT and PATCH requests?
15. What is the difference between PUT and PATCH?
16. How do you define a DELETE route?
17. How do route parameters work?
18. What is `req.params`?
19. What is `req.query`?
20. What is `req.body`?

---

## Request & Response Objects

21. What is the `req` object?
22. What is the `res` object?
23. How do you send a JSON response?
24. How do you send a status code?
25. How do you redirect a request?
26. What is `res.send()`?
27. What is `res.json()`?
28. What is `res.end()`?
29. What is `res.status()`?
30. What is the difference between `send()` and `json()`?

---

## Route Organization

31. What is `express.Router()`?
32. Why should you use Express Routers?
33. How do you create modular routes?
34. How do you organize routes in a large application?
35. What is route chaining?
36. What are route parameters?
37. How do optional route parameters work?
38. How do wildcard routes work?
39. How do nested routes work?
40. What are common routing mistakes?

---

## Basic Express Features

41. How do you serve static files in Express?
42. What is the `express.static()` middleware?
43. How do you parse JSON request bodies?
44. What is `express.json()`?
45. What is `express.urlencoded()`?
46. How do you enable CORS?
47. What is the `cors` package?
48. How do you configure environment variables?
49. How do you start and stop an Express server?
50. What best practices do you follow when starting a new Express project?

---

# Middleware

51. What is middleware in Express.js?
52. How does middleware work?
53. What is the middleware execution flow?
54. What is the purpose of the `next()` function?
55. What happens if `next()` is not called?
56. What is application-level middleware?
57. What is router-level middleware?
58. What is built-in middleware?
59. What is third-party middleware?
60. How do you create custom middleware?

---

# Request Processing

61. In what order is middleware executed?
62. How do you apply middleware globally?
63. How do you apply middleware to specific routes?
64. How do you chain multiple middleware functions?
65. What is the difference between middleware and route handlers?
66. How do you skip middleware?
67. How do you pass data between middleware?
68. What are common middleware use cases?
69. What are common mistakes when writing middleware?
70. How do you debug middleware execution?

---

# Error Handling

71. How does Express.js handle errors?
72. What is error-handling middleware?
73. Why does error middleware have four parameters?
74. How do you create a global error handler?
75. How do you handle asynchronous errors?
76. What happens when an error is thrown inside an async route?
77. How do you return consistent error responses?
78. How do you log application errors?
79. What HTTP status codes should be used for common API errors?
80. What are Express.js error-handling best practices?

---

# Authentication & Authorization

81. How do you implement authentication in Express.js?
82. What is JWT authentication?
83. How does JWT work?
84. How do you verify a JWT?
85. Where should JWT tokens be stored?
86. What is refresh token authentication?
87. What is the difference between authentication and authorization?
88. How do you implement role-based access control (RBAC)?
89. How do you protect private routes?
90. What are common authentication mistakes?

---

# Validation & Security

91. How do you validate incoming request data?
92. What validation libraries have you used?
93. How do you sanitize user input?
94. How do you prevent SQL Injection?
95. How do you prevent NoSQL Injection?
96. How do you prevent Cross-Site Scripting (XSS)?
97. How do you prevent Cross-Site Request Forgery (CSRF)?
98. How do you implement rate limiting in Express.js?
99. What security middleware do you commonly use (e.g., Helmet, CORS, Morgan)?
100. What security best practices do you follow when building Express APIs?

---

# Project Architecture

101. How do you structure a large Express.js application?
102. What folder structure do you recommend for enterprise Express.js projects?
103. What is the MVC architecture pattern?
104. What are the responsibilities of Controllers?
105. What should be placed in the Service Layer?
106. What is the Repository Pattern?
107. Why should business logic not be written in controllers?
108. How do you organize routes, controllers, services, and models?
109. How do you manage configuration for different environments?
110. What Express.js architecture patterns have you used in production?

---

# API Design

111. How do you design a RESTful API?
112. How do you version APIs?
113. How do you structure consistent API responses?
114. How do you implement pagination?
115. How do you implement filtering, sorting, and searching?
116. How do you handle file uploads in Express.js?
117. How do you implement API documentation?
118. What tools have you used for API documentation (Swagger/OpenAPI)?
119. How do you implement request logging?
120. How do you monitor API usage?

---

# Performance & Scalability

121. How do you improve the performance of an Express.js application?
122. What causes slow Express.js APIs?
123. How do you optimize database queries?
124. How do you implement caching in Express.js?
125. When would you use Redis?
126. How do you compress HTTP responses?
127. How do you handle high traffic?
128. How do you implement load balancing?
129. How do you scale an Express.js application horizontally?
130. What production performance best practices do you follow?

---

# Testing & Deployment

131. How do you test Express.js APIs?
132. What testing frameworks have you used?
133. How do you write unit tests for controllers and services?
134. How do you write integration tests for Express APIs?
135. How do you mock database calls during testing?
136. How do you deploy an Express.js application?
137. How do you containerize an Express.js application using Docker?
138. How do you manage environment variables in production?
139. How do you implement CI/CD for Express.js applications?
140. How do you monitor production applications?

---

# Senior Real-World Interview Questions

141. Describe the largest Express.js application you've worked on.
142. What was the most difficult Express.js bug you've fixed?
143. How do you debug production issues in Express.js?
144. How do you review Express.js pull requests?
145. What coding standards do you enforce in your team?
146. How do you mentor junior backend developers?
147. How would you migrate a legacy Express.js application to a cleaner architecture?
148. If you were building a production REST API today, what architecture and tooling would you choose?
149. What best practices do you always follow in production Express.js applications?
150. In your opinion, what separates a junior, mid-level, and senior Express.js developer?

---

# ANSWERS


---

## Part 1 (1â€“10): Introduction

---

## Question 1: What is Express.js?

## Answer:
Express.js is a minimal, flexible Node.js web framework that provides a robust set of features for building web applications and APIs. It's the most popular Node.js framework and sits on top of Node's built-in `http` module.

```javascript
const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.send("Hello, World!");
});

app.listen(3000);
```

## Key Points:
- Minimal, unopinionated web framework for Node.js.
- Built on top of the `http` module.
- Routing, middleware, and request/response handling.
- Most popular Node.js framework.
- Lightweight and flexible.

## Interview Tip:
"Express is the de facto standard for Node.js APIs â€” it's minimal, flexible, and has the largest ecosystem."

---

## Question 2: Why was Express.js created?

## Answer:
Express was created to simplify building web applications with Node.js. The native `http` module is low-level â€” you have to manually parse URLs, handle routing, and manage request/response objects. Express adds:
- Simple routing.
- Middleware support.
- Request/response helpers.
- Static file serving.

Created by TJ Holowaychuk in 2010.

## Key Points:
- Simplifies Node.js web development.
- Adds routing and middleware.
- Request/response helpers.
- Created in 2010.
- Inspired by Ruby's Sinatra.

## Interview Tip:
"Express was created because the native `http` module is too low-level for practical web development."

---

## Question 3: What problems does Express.js solve?

## Answer:
1. **Routing**: Manual URL parsing is tedious.
2. **Middleware**: No built-in request processing pipeline.
3. **Request parsing**: Manual body parsing is error-prone.
4. **Static files**: No built-in static file serving.
5. **Error handling**: No standardized error handling.
6. **Code organization**: No conventions for structuring apps.

## Key Points:
- Routing simplified.
- Middleware pipeline.
- Request body parsing.
- Static file serving.
- Error handling conventions.
- Code organization patterns.

## Interview Tip:
"Express solves the 'plumbing' problem â€” routing, parsing, and middleware that every web app needs."

---

## Question 4: What are the advantages of Express.js?

## Answer:
- **Minimal**: Small footprint, no bloat.
- **Flexible**: Unopinionated â€” use any pattern.
- **Middleware**: Extensible via middleware.
- **Ecosystem**: Largest Node.js ecosystem.
- **Community**: Huge community and resources.
- **Performance**: Lightweight and fast.
- **Full-stack**: Works for APIs and server-rendered apps.

## Key Points:
- Minimal and flexible.
- Middleware-based architecture.
- Largest ecosystem.
- Huge community.
- Fast and lightweight.

## Interview Tip:
"Express is minimal and flexible â€” you can build anything from a simple API to a complex enterprise app."

---

## Question 5: What are the disadvantages of Express.js?

## Answer:
- **Unopinionated**: No built-in patterns â€” you must choose your own.
- **Middleware complexity**: Too many middleware can be confusing.
- **No TypeScript built-in**: Requires manual setup.
- **Callback-heavy**: Historically callback-based (though async/await works).
- **Security**: No built-in security features â€” must add manually.
- **No validation**: Must use external libraries.

## Key Points:
- Unopinionated (pro and con).
- No built-in security.
- No built-in validation.
- Callback-heavy historically.
- Manual TypeScript setup.

## Interview Tip:
"Express is unopinionated â€” that's its strength and weakness. You have freedom but must make more decisions."

---

## Question 6: How does Express.js differ from Node.js?

## Answer:
| Feature | Node.js | Express.js |
|---------|---------|------------|
| Type | Runtime environment | Web framework |
| Purpose | Run JavaScript on server | Build web apps/APIs |
| Features | File system, network, etc. | Routing, middleware |
| Routing | Manual | Built-in |
| Middleware | None | Extensive |

Express is built ON Node.js â€” it extends Node's capabilities.

## Key Points:
- Node.js: runtime environment.
- Express: web framework built on Node.
- Node for low-level operations.
- Express for web development.
- Express uses Node's `http` module.

## Interview Tip:
"Node.js is the engine; Express is the framework. You can have Node without Express, but not the other way around."

---

## Question 7: When would you use Express.js instead of the native `http` module?

## Answer:
Use Express for:
- **Routing**: Multiple endpoints.
- **Middleware**: Request processing pipeline.
- **APIs**: RESTful APIs with multiple routes.
- **Production apps**: Anything beyond a simple server.

Use native `http` for:
- **Minimal servers**: Health checks, proxies.
- **Learning**: Understanding how HTTP works.
- **Performance-critical**: When every millisecond counts.

## Key Points:
- Express for routing and middleware.
- Native `http` for minimal servers.
- Express for production APIs.
- Native `http` for learning.
- Most projects should use Express.

## Interview Tip:
"Use Express for anything beyond a simple server â€” it handles routing, middleware, and more."

---

## Question 8: What is the Express application object?

## Answer:
The app object is created by `express()` and provides methods for routing, middleware, and server configuration.

```javascript
const app = express();

app.get("/", handler);      // Routing
app.use(middleware);        // Middleware
app.listen(3000);           // Start server
app.set("view engine", "ejs"); // Configuration
```

## Key Points:
- Created by `express()`.
- Routing methods (get, post, put, delete).
- Middleware methods (use).
- Configuration (set, get).
- Server startup (listen).

## Interview Tip:
"The app object is the center of Express â€” it handles routing, middleware, and configuration."

---

## Question 9: How do you create an Express application?

## Answer:
```javascript
const express = require("express");
const app = express();

// Middleware
app.use(express.json());

// Routes
app.get("/", (req, res) => {
  res.send("Hello, World!");
});

// Start server
app.listen(3000, () => {
  console.log("Server running on port 3000");
});
```

## Key Points:
- `express()` creates the app.
- `app.use()` for middleware.
- `app.get()` for routes.
- `app.listen()` to start.
- Modular structure for large apps.

## Interview Tip:
"The basic Express setup is 5 lines â€” create app, add middleware, define routes, start listening."

---

## Question 10: What is the request-response lifecycle in Express?

## Answer:
1. **Client sends request**: HTTP request arrives.
2. **Middleware pipeline**: Request passes through middleware in order.
3. **Route matching**: Express finds matching route.
4. **Route handler**: Handler processes the request.
5. **Response sent**: `res.send()`, `res.json()`, etc.
6. **Client receives response**: HTTP response sent back.

```
Client â†’ Middleware â†’ Route Handler â†’ Response â†’ Client
```

## Key Points:
- Request arrives from client.
- Passes through middleware chain.
- Route handler processes it.
- Response sent back.
- Order matters (middleware before routes).

## Interview Tip:
"The lifecycle is: request â†’ middleware â†’ route â†’ response. Middleware runs before route handlers."

---

## Part 2 (11â€“20): Routing

---

## Question 11: What is routing in Express.js?

## Answer:
Routing determines how an application responds to client requests at specific URLs (endpoints) and HTTP methods.

```javascript
app.get("/users", (req, res) => { /* GET /users */ });
app.post("/users", (req, res) => { /* POST /users */ });
app.put("/users/:id", (req, res) => { /* PUT /users/123 */ });
app.delete("/users/:id", (req, res) => { /* DELETE /users/123 */ });
```

## Key Points:
- Maps URLs to handlers.
- Supports all HTTP methods.
- Route parameters for dynamic URLs.
- Middleware per route.
- Router for modular organization.

## Interview Tip:
"Routing maps URLs to handlers â€” it's how Express knows what code to run for each request."

---

## Question 12: How do you define a GET route?

## Answer:
```javascript
app.get("/users", (req, res) => {
  res.json([{ id: 1, name: "Alice" }]);
});

// With route parameter
app.get("/users/:id", (req, res) => {
  res.json({ id: req.params.id });
});
```

## Key Points:
- `app.get(path, handler)`.
- Handler receives `req` and `res`.
- Route parameters with `:param`.
- Return data with `res.json()`.

## Interview Tip:
"GET routes are for retrieving data â€” use `res.json()` for API responses."

---

## Question 13: How do you define a POST route?

## Answer:
```javascript
app.post("/users", (req, res) => {
  const { name, email } = req.body;
  // Create user
  res.status(201).json({ id: 1, name, email });
});
```

## Key Points:
- `app.post(path, handler)`.
- Access body with `req.body`.
- Requires body parsing middleware.
- Return 201 for creation.
- Validate input before processing.

## Interview Tip:
"POST routes create resources â€” always validate input and return 201 on success."

---

## Question 14: What are PUT and PATCH requests?

## Answer:
- **PUT**: Replace an entire resource.
- **PATCH**: Update specific fields of a resource.

```javascript
// PUT - replace entire user
app.put("/users/:id", (req, res) => {
  const { name, email, role } = req.body;
  // Replace all fields
});

// PATCH - update specific fields
app.patch("/users/:id", (req, res) => {
  const { name } = req.body;
  // Update only name
});
```

## Key Points:
- PUT: replace entire resource.
- PATCH: partial update.
- Both use `req.body` for data.
- PUT requires all fields.
- PATCH requires only changed fields.

## Interview Tip:
"PUT replaces; PATCH updates. Use PATCH for partial updates."

---

## Question 15: What is the difference between PUT and PATCH?

## Answer:
| Feature | PUT | PATCH |
|---------|-----|-------|
| Purpose | Replace resource | Update fields |
| Body | All fields required | Only changed fields |
| Idempotent | Yes | No (usually) |
| Use case | Full replacement | Partial update |

## Key Points:
- PUT replaces the entire resource.
- PATCH updates specific fields.
- PUT is idempotent.
- PATCH is for partial updates.
- Choose based on use case.

## Interview Tip:
"PUT for full replacement, PATCH for partial updates â€” know the difference."

---

## Question 16: How do you define a DELETE route?

## Answer:
```javascript
app.delete("/users/:id", (req, res) => {
  // Delete user
  res.status(204).send();
});
```

## Key Points:
- `app.delete(path, handler)`.
- Access ID from `req.params`.
- Return 204 (no content) on success.
- 404 if not found.

## Interview Tip:
"DELETE routes remove resources â€” return 204 on success, 404 if not found."

---

## Question 17: How do route parameters work?

## Answer:
Route parameters are dynamic URL segments prefixed with `:`.

```javascript
app.get("/users/:id", (req, res) => {
  console.log(req.params.id); // "123"
});

// Multiple parameters
app.get("/users/:userId/posts/:postId", (req, res) => {
  console.log(req.params.userId);  // "123"
  console.log(req.params.postId);  // "456"
});
```

## Key Points:
- `:param` syntax in route path.
- Accessed via `req.params.param`.
- Multiple parameters supported.
- Always strings (parse if needed).
- Match any value in that position.

## Interview Tip:
"Route parameters are always strings â€” parse them to numbers if needed."

---

## Question 18: What is `req.params`?

## Answer:
`req.params` is an object containing route parameter values.

```javascript
// Route: /users/:id
// URL: /users/123
req.params.id // "123"
```

## Key Points:
- Object with route parameter values.
- Always strings.
- Matches `:param` in route path.
- Used for resource IDs.
- Multiple params supported.

## Interview Tip:
"`req.params` gives you route parameters â€” always strings, always from the URL path."

---

## Question 19: What is `req.query`?

## Answer:
`req.query` is an object containing URL query string parameters.

```javascript
// URL: /users?page=1&limit=10&sort=name
req.query.page  // "1"
req.query.limit // "10"
req.query.sort  // "name"
```

## Key Points:
- Object with query string values.
- Always strings.
- Parsed from `?key=value&key2=value2`.
- Used for filtering, sorting, pagination.
- Optional parameters.

## Interview Tip:
"`req.query` is for query string parameters â€” filtering, sorting, pagination."

---

## Question 20: What is `req.body`?

## Answer:
`req.body` contains the parsed request body (JSON, form data, etc.).

```javascript
app.post("/users", (req, res) => {
  const { name, email } = req.body;
  // Process data
});
```

Requires body parsing middleware:
```javascript
app.use(express.json());
app.use(express.urlencoded({ extended: true }));
```

## Key Points:
- Contains parsed request body.
- Requires middleware (`express.json()`).
- JSON and form data supported.
- Always validate before using.
- Undefined without middleware.

## Interview Tip:
"`req.body` is undefined without body parsing middleware â€” always add `express.json()`."

---

## Part 3 (21â€“30): Request & Response Objects

---

## Question 21: What is the `req` object?

## Answer:
The `req` object represents the HTTP request. It contains:
- `req.params`: Route parameters.
- `req.query`: Query string.
- `req.body`: Request body.
- `req.headers`: Request headers.
- `req.method`: HTTP method.
- `req.path`: URL path.
- `req.ip`: Client IP.

## Key Points:
- Represents the HTTP request.
- Contains params, query, body, headers.
- Passed to route handlers and middleware.
- Read-only (mostly).
- Extended by middleware.

## Interview Tip:
"`req` is the incoming request â€” it contains everything the client sent."

---

## Question 22: What is the `res` object?

## Answer:
The `res` object represents the HTTP response. It provides methods to send data back to the client.

- `res.send()`: Send a response.
- `res.json()`: Send JSON.
- `res.status()`: Set status code.
- `res.redirect()`: Redirect.
- `res.sendFile()`: Send a file.

## Key Points:
- Represents the HTTP response.
- Methods to send data.
- Chainable (e.g., `res.status(201).json()`).
- End the request cycle.
- One response per request.

## Interview Tip:
"`res` is the outgoing response â€” use it to send data back to the client."

---

## Question 23: How do you send a JSON response?

## Answer:
```javascript
res.json({ id: 1, name: "Alice" });

// With status code
res.status(201).json({ id: 1, name: "Alice" });

// Chainable
res.status(200).json({ success: true, data: users });
```

## Key Points:
- `res.json(data)` sends JSON response.
- Sets `Content-Type: application/json`.
- Can chain with `res.status()`.
- Automatically serializes objects.
- Preferred for APIs.

## Interview Tip:
"`res.json()` is the standard for API responses â€” it sets the correct Content-Type automatically."

---

## Question 24: How do you send a status code?

## Answer:
```javascript
res.status(201).json({ id: 1 });           // Created
res.status(404).json({ error: "Not found" }); // Not found
res.status(500).json({ error: "Server error" }); // Server error
```

## Key Points:
- `res.status(code)` sets status code.
- Chainable with other methods.
- Common codes: 200, 201, 400, 401, 403, 404, 500.
- Always send appropriate status codes.

## Interview Tip:
"Always use appropriate status codes â€” 200 for success, 201 for creation, 404 for not found."

---

## Question 25: How do you redirect a request?

## Answer:
```javascript
res.redirect("/new-page");
res.redirect(301, "/new-page"); // Permanent redirect
res.redirect(302, "/temp");     // Temporary redirect
```

## Key Points:
- `res.redirect(url)` redirects client.
- Default: 302 (temporary).
- 301 for permanent redirects.
- Can specify status code.
- Ends the request cycle.

## Interview Tip:
"`res.redirect()` sends a redirect response â€” use 301 for permanent, 302 for temporary."

---

## Question 26: What is `res.send()`?

## Answer:
`res.send()` sends a response of various types (string, Buffer, object, array).

```javascript
res.send("Hello");           // String
res.send({ message: "ok" }); // Object (becomes JSON)
res.send(Buffer.from("hi")); // Buffer
```

## Key Points:
- Sends various types.
- Strings: text/html.
- Objects: application/json.
- Buffer: application/octet-stream.
- Sets Content-Type automatically.

## Interview Tip:
"`res.send()` is versatile but `res.json()` is clearer for JSON responses."

---

## Question 27: What is `res.json()`?

## Answer:
`res.json()` sends a JSON response. It's specifically for JSON data.

```javascript
res.json({ id: 1, name: "Alice" });
```

Sets `Content-Type: application/json` automatically.

## Key Points:
- Sends JSON response.
- Sets Content-Type automatically.
- Serializes objects.
- Preferred for APIs.
- Clearer than `res.send()` for JSON.

## Interview Tip:
"`res.json()` is the standard for API responses â€” always use it for JSON data."

---

## Question 28: What is `res.end()`?

## Answer:
`res.end()` ends the response process without sending any data.

```javascript
res.status(204).end(); // No content
```

## Key Points:
- Ends response without data.
- Use for 204 No Content.
- Doesn't send body.
- Faster than `res.send()`.
- Rarely used directly.

## Interview Tip:
"`res.end()` is for responses with no body â€” like 204 No Content."

---

## Question 29: What is `res.status()`?

## Answer:
`res.status()` sets the HTTP status code. It's chainable.

```javascript
res.status(201).json({ id: 1 });
res.status(404).json({ error: "Not found" });
res.status(500).json({ error: "Server error" });
```

## Key Points:
- Sets HTTP status code.
- Chainable with other methods.
- Common: 200, 201, 400, 404, 500.
- Always set appropriate status codes.

## Interview Tip:
"`res.status()` is chainable â€” `res.status(201).json(data)` is the standard pattern."

---

## Question 30: What is the difference between `send()` and `json()`?

## Answer:
| Feature | `send()` | `json()` |
|---------|----------|----------|
| Types | Any (string, object, Buffer) | Objects only |
| Content-Type | Auto-detected | application/json |
| Use case | General responses | JSON APIs |

`json()` is clearer for APIs; `send()` is more versatile.

## Key Points:
- `send()`: any type, auto Content-Type.
- `json()`: objects only, JSON Content-Type.
- `json()` is clearer for APIs.
- Use `json()` for API responses.

## Interview Tip:
"Use `res.json()` for API responses â€” it's explicit and sets the correct Content-Type."

---

## Part 4 (31â€“40): Route Organization

---

## Question 31: What is `express.Router()`?

## Answer:
`express.Router()` creates modular, mountable route handlers. It's like a mini Express app.

```javascript
// routes/users.js
const router = express.Router();

router.get("/", getUsers);
router.post("/", createUser);
router.get("/:id", getUser);

module.exports = router;

// app.js
app.use("/api/users", require("./routes/users"));
```

## Key Points:
- Creates modular route handlers.
- Like a mini Express app.
- Mount with `app.use()`.
- Organizes routes by feature.
- Supports middleware per router.

## Interview Tip:
"`express.Router()` is the key to organizing large Express apps â€” one router per feature."

---

## Question 32: Why should you use Express Routers?

## Answer:
- **Modularity**: Separate routes into files.
- **Organization**: Group related routes.
- **Middleware**: Apply middleware per router.
- **Reusability**: Mount routers at different paths.
- **Testability**: Test routers independently.

## Key Points:
- Modular route organization.
- Group related routes.
- Per-router middleware.
- Reusable and mountable.
- Easier to test.

## Interview Tip:
"Routers keep your app organized â€” one router per feature (users, posts, auth)."

---

## Question 33: How do you create modular routes?

## Answer:
```javascript
// routes/auth.js
const router = express.Router();
router.post("/login", login);
router.post("/register", register);
router.post("/logout", logout);
module.exports = router;

// routes/users.js
const router = express.Router();
router.get("/", getUsers);
router.get("/:id", getUser);
router.put("/:id", updateUser);
module.exports = router;

// app.js
app.use("/api/auth", require("./routes/auth"));
app.use("/api/users", require("./routes/users"));
```

## Key Points:
- One file per feature.
- Create router per file.
- Mount with `app.use()`.
- Prefix with feature path.
- Export the router.

## Interview Tip:
"One router per feature file â€” auth.js, users.js, posts.js."

---

## Question 34: How do you organize routes in a large application?

## Answer:
```
src/
  routes/
    auth.routes.js
    user.routes.js
    post.routes.js
  controllers/
    auth.controller.js
    user.controller.js
  services/
    auth.service.js
    user.service.js
  app.js
```

## Key Points:
- Routes in `routes/` folder.
- Controllers in `controllers/` folder.
- Services in `services/` folder.
- One file per feature.
- Clean separation of concerns.

## Interview Tip:
"Routes, controllers, services â€” the three-layer architecture for Express apps."

---

## Question 35: What is route chaining?

## Answer:
Route chaining applies multiple handlers to the same route.

```javascript
router.route("/users")
  .get(authMiddleware, getUsers)
  .post(authMiddleware, validateUser, createUser);
```

## Key Points:
- Multiple handlers per route.
- Chain HTTP methods.
- Shared middleware.
- Cleaner code.
- `router.route()` for chaining.

## Interview Tip:
"`router.route()` lets you chain methods â€” cleaner than separate route definitions."

---

## Question 36: What are route parameters?

## Answer:
Dynamic URL segments that capture values.

```javascript
app.get("/users/:id", (req, res) => {
  req.params.id // "123"
});

app.get("/users/:userId/posts/:postId", (req, res) => {
  req.params.userId  // "123"
  req.params.postId  // "456"
});
```

## Key Points:
- `:param` syntax.
- Captured in `req.params`.
- Always strings.
- Multiple parameters supported.
- Used for resource identifiers.

## Interview Tip:
"Route parameters capture dynamic URL segments â€” always strings."

---

## Question 37: How do optional route parameters work?

## Answer:
Optional parameters use `?` suffix.

```javascript
app.get("/users/:id?", (req, res) => {
  if (req.params.id) {
    // Specific user
  } else {
    // All users
  }
});
```

## Key Points:
- `?` makes parameter optional.
- `req.params.id` is `undefined` if not provided.
- Single route handles both cases.
- Use with caution â€” can be confusing.

## Interview Tip:
"Optional parameters with `?` â€” but be careful, it can make routes ambiguous."

---

## Question 38: How do wildcard routes work?

## Answer:
Wildcard routes match any value in a segment.

```javascript
app.get("/files/*", (req, res) => {
  // Matches /files/any/thing/here
});

app.get("/api/*/users", (req, res) => {
  // Matches /api/v1/users, /api/v2/users
});
```

## Key Points:
- `*` matches any value.
- Useful for file paths.
- Versioning patterns.
- Use with caution.
- Can be ambiguous.

## Interview Tip:
"Wildcards are useful for file paths and versioning â€” but be careful with ambiguity."

---

## Question 39: How do nested routes work?

## Answer:
Nested routes represent resource relationships.

```javascript
// /users/:userId/posts
router.get("/:userId/posts", (req, res) => {
  const { userId } = req.params;
  // Get posts for user
});

// /users/:userId/posts/:postId
router.get("/:userId/posts/:postId", (req, res) => {
  const { userId, postId } = req.params;
  // Get specific post for user
});
```

## Key Points:
- Represent resource relationships.
- Multiple parameters.
- Clear URL structure.
- Can become deeply nested.
- Keep nesting shallow.

## Interview Tip:
"Nested routes represent relationships â€” but keep nesting shallow (2-3 levels max)."

---

## Question 40: What are common routing mistakes?

## Answer:
1. **No error handling**: Missing try/catch.
2. **Too many routes in one file**: No modularization.
3. **No validation**: Trusting client input.
4. **Wrong HTTP methods**: Using GET for mutations.
5. **Inconsistent naming**: `/getUser` vs `/users/:id`.
6. **No status codes**: Always sending 200.

## Key Points:
- Always handle errors.
- Modularize routes.
- Validate input.
- Use correct HTTP methods.
- Consistent naming.
- Appropriate status codes.

## Interview Tip:
"The biggest mistake is putting all routes in one file â€” use Router for modularity."

---

## Part 5 (41â€“50): Basic Express Features

---

## Question 41: How do you serve static files in Express?

## Answer:
```javascript
app.use(express.static("public"));

// With prefix
app.use("/static", express.static("public"));

// Absolute path
app.use(express.static(path.join(__dirname, "public")));
```

## Key Points:
- `express.static()` serves static files.
- Specify directory path.
- Optional URL prefix.
- Use absolute paths for reliability.
- Files in `public/` are served directly.

## Interview Tip:
"`express.static('public')` serves files from the `public` directory â€” simple and effective."

---

## Question 42: What is the `express.static()` middleware?

## Answer:
`express.static()` is built-in middleware that serves static files (HTML, CSS, JS, images).

```javascript
app.use(express.static("public"));
// GET /style.css â†’ serves public/style.css
```

## Key Points:
- Built-in middleware.
- Serves static files.
- Maps URL to file path.
- Caching headers by default.
- Multiple directories supported.

## Interview Tip:
"`express.static()` is the simplest way to serve static files in Express."

---

## Question 43: How do you parse JSON request bodies?

## Answer:
```javascript
app.use(express.json());

// Now req.body contains parsed JSON
app.post("/users", (req, res) => {
  const { name, email } = req.body;
});
```

## Key Points:
- `express.json()` parses JSON bodies.
- Must be applied before routes.
- Populates `req.body`.
- Sets size limit (default 100kb).
- Only parses JSON content type.

## Interview Tip:
"Always add `express.json()` before your routes â€” without it, `req.body` is undefined."

---

## Question 44: What is `express.json()`?

## Answer:
Built-in middleware that parses incoming JSON requests and populates `req.body`.

```javascript
app.use(express.json({ limit: "10mb" }));
```

## Key Points:
- Built-in since Express 4.16.
- Parses JSON request bodies.
- Populates `req.body`.
- Configurable size limit.
- Replaces `body-parser` for JSON.

## Interview Tip:
"`express.json()` replaced the `body-parser` package â€” it's built-in since Express 4.16."

---

## Question 45: What is `express.urlencoded()`?

## Answer:
Parses URL-encoded form data (HTML form submissions).

```javascript
app.use(express.urlencoded({ extended: true }));
```

## Key Points:
- Parses form data.
- `extended: true` for complex objects.
- Populates `req.body`.
- For HTML form submissions.
- Complementary to `express.json()`.

## Interview Tip:
"`express.urlencoded()` is for HTML forms â€” `express.json()` is for APIs."

---

## Question 46: How do you enable CORS?

## Answer:
```javascript
const cors = require("cors");
app.use(cors());

// With options
app.use(cors({
  origin: "https://example.com",
  methods: ["GET", "POST", "PUT", "DELETE"],
  credentials: true
}));
```

## Key Points:
- `cors` package for CORS.
- `app.use(cors())` enables all origins.
- Configure specific origins for security.
- `credentials: true` for cookies.
- Essential for frontend-backend communication.

## Interview Tip:
"Use the `cors` package â€” configure specific origins in production, not `cors()` without options."

---

## Question 47: What is the `cors` package?

## Answer:
The `cors` package is middleware that enables Cross-Origin Resource Sharing (CORS). It adds the necessary headers to allow or restrict cross-origin requests.

## Key Points:
- Middleware for CORS headers.
- Enables cross-origin requests.
- Configurable origins, methods, headers.
- Essential for frontend-backend communication.
- Security implications.

## Interview Tip:
"CORS is a security feature â€” configure it carefully, don't just allow all origins."

---

## Question 48: How do you configure environment variables?

## Answer:
```javascript
// .env
PORT=3000
DATABASE_URL=mongodb://localhost/myapp
JWT_SECRET=secret

// config.js
require("dotenv").config();
module.exports = {
  port: process.env.PORT || 3000,
  dbUrl: process.env.DATABASE_URL,
  jwtSecret: process.env.JWT_SECRET
};
```

## Key Points:
- `.env` file (gitignored).
- `dotenv` package to load.
- `process.env` to access.
- Different per environment.
- Never commit `.env` to git.

## Interview Tip:
"Use `dotenv` for environment variables â€” never commit `.env` to git."

---

## Question 49: How do you start and stop an Express server?

## Answer:
```javascript
const server = app.listen(3000, () => {
  console.log("Server running on port 3000");
});

// Graceful shutdown
process.on("SIGTERM", () => {
  server.close(() => {
    console.log("Server closed");
    process.exit(0);
  });
});
```

## Key Points:
- `app.listen(port, callback)` starts server.
- Returns server object.
- `server.close()` for graceful shutdown.
- Handle SIGTERM and SIGINT.
- Essential for production.

## Interview Tip:
"Always implement graceful shutdown â€” it prevents dropped connections during deployment."

---

## Question 50: What best practices do you follow when starting a new Express project?

## Answer:
1. **Structure**: Routes, controllers, services folders.
2. **Middleware**: CORS, body parser, error handler.
3. **Environment variables**: `dotenv` for config.
4. **Validation**: Zod or Joi for input validation.
5. **Error handling**: Global error handler.
6. **Logging**: Morgan or Pino.
7. **Security**: Helmet, rate limiting.

## Key Points:
- Structured folder layout.
- Essential middleware.
- Environment variables.
- Input validation.
- Error handling.
- Logging and security.

## Interview Tip:
"Start with structure, middleware, and error handling â€” add features as needed."

---

## Part 6 (51â€“60): Middleware

---

## Question 51: What is middleware in Express.js?

## Answer:
Middleware functions have access to `req`, `res`, and `next`. They execute during the request-response cycle and can:
- Execute code.
- Modify request/response.
- End the cycle.
- Call `next()` to pass control.

```javascript
app.use((req, res, next) => {
  console.log("Time:", Date.now());
  next();
});
```

## Key Points:
- Functions with `req`, `res`, `next`.
- Execute during request cycle.
- Can modify request/response.
- Can end the cycle.
- Call `next()` to continue.

## Interview Tip:
"Middleware is the backbone of Express â€” it processes requests before they reach route handlers."

---

## Question 52: How does middleware work?

## Answer:
Middleware functions are executed in order. Each middleware can:
1. Execute code.
2. Modify `req` or `res`.
3. End the request cycle (send response).
4. Call `next()` to pass to the next middleware.

```
Request â†’ Middleware 1 â†’ Middleware 2 â†’ Route Handler â†’ Response
```

## Key Points:
- Executed in order.
- Can modify request/response.
- Can end the cycle.
- `next()` passes control.
- Order matters.

## Interview Tip:
"Middleware is a pipeline â€” request flows through each middleware in order."

---

## Question 53: What is the middleware execution flow?

## Answer:
Middleware executes in the order it's registered:

```javascript
app.use(middleware1); // First
app.use(middleware2); // Second
app.get("/", handler); // Third (route handler)
```

Each must call `next()` to continue, or send a response to end the cycle.

## Key Points:
- Order of registration matters.
- Each calls `next()` to continue.
- Response ends the cycle.
- Route handlers are also middleware.
- Global middleware before routes.

## Interview Tip:
"Register global middleware first, then routes. Order matters."

---

## Question 54: What is the purpose of the `next()` function?

## Answer:
`next()` passes control to the next middleware in the stack. Without it, the request hangs.

```javascript
app.use((req, res, next) => {
  console.log("Middleware 1");
  next(); // Pass to next middleware
});
```

## Key Points:
- Passes control to next middleware.
- Without `next()`, request hangs.
- `next(err)` passes to error handler.
- Required in most middleware.
- Not needed if sending response.

## Interview Tip:
"Call `next()` to continue, or send a response to end. Never forget `next()`."

---

## Question 55: What happens if `next()` is not called?

## Answer:
The request hangs â€” the client never receives a response. The connection times out.

```javascript
// BAD: request hangs forever
app.use((req, res, next) => {
  console.log("This runs");
  // No next() and no res.send() â€” request hangs!
});
```

## Key Points:
- Request hangs without `next()`.
- Client receives no response.
- Connection times out.
- Always call `next()` or send response.
- Common beginner mistake.

## Interview Tip:
"Forgetting `next()` is the #1 Express mistake â€” the request hangs forever."

---

## Question 56: What is application-level middleware?

## Answer:
Applied to the entire application using `app.use()`.

```javascript
app.use(express.json());          // Parse JSON
app.use(cors());                   // Enable CORS
app.use(authMiddleware);           // Auth check
```

## Key Points:
- Applied to all routes.
- `app.use()` for global middleware.
- Runs before route handlers.
- Order matters.
- Common for parsing, auth, logging.

## Interview Tip:
"Application-level middleware runs on every request â€” use it for global concerns."

---

## Question 57: What is router-level middleware?

## Answer:
Applied only to specific routers.

```javascript
const router = express.Router();
router.use(authMiddleware); // Only for this router
router.get("/", getUsers);
```

## Key Points:
- Applied to specific router.
- `router.use()` for router middleware.
- Only runs for routes in that router.
- Good for feature-specific middleware.
- More granular than app-level.

## Interview Tip:
"Router-level middleware is for feature-specific concerns â€” like auth for user routes."

---

## Question 58: What is built-in middleware?

## Answer:
Express ships with built-in middleware:
- `express.json()`: Parse JSON.
- `express.urlencoded()`: Parse form data.
- `express.static()`: Serve static files.
- `express.raw()`: Parse raw data.
- `express.text()`: Parse text data.

## Key Points:
- Built-in to Express.
- No additional packages needed.
- `express.json()` for APIs.
- `express.static()` for files.
- Replaces `body-parser`.

## Interview Tip:
"Express has built-in middleware for JSON, forms, and static files â€” no need for `body-parser`."

---

## Question 59: What is third-party middleware?

## Answer:
External packages that add functionality:
- `cors`: CORS headers.
- `helmet`: Security headers.
- `morgan`: Request logging.
- `express-rate-limit`: Rate limiting.
- `multer`: File uploads.

## Key Points:
- External npm packages.
- Install and use with `app.use()`.
- Extend Express functionality.
- Security, logging, file handling.
- Large ecosystem.

## Interview Tip:
"Third-party middleware extends Express â€” `cors`, `helmet`, `morgan` are essentials."

---

## Question 60: How do you create custom middleware?

## Answer:
```javascript
// Simple logger
const logger = (req, res, next) => {
  console.log(`${req.method} ${req.path}`);
  next();
};

// Auth middleware
const auth = (req, res, next) => {
  const token = req.headers.authorization;
  if (!token) return res.status(401).json({ error: "Unauthorized" });
  // Verify token
  next();
};

app.use(logger);
app.use(auth);
```

## Key Points:
- Function with `req`, `res`, `next`.
- Call `next()` to continue.
- Send response to end cycle.
- Can modify `req`/`res`.
- Reusable across routes.

## Interview Tip:
"Custom middleware is just a function with `req`, `res`, and `next`."

---

## Part 7 (61â€“70): Request Processing

---

## Question 61: In what order is middleware executed?

## Answer:
Middleware executes in the order it's registered with `app.use()` or route methods.

```javascript
app.use(middleware1);  // 1st
app.use(middleware2);  // 2nd
app.get("/", handler); // 3rd
```

## Key Points:
- Registration order matters.
- Global before routes.
- Specific before general.
- `next()` passes control.
- Response ends the cycle.

## Interview Tip:
"Order matters â€” register global middleware first, then routes."

---

## Question 62: How do you apply middleware globally?

## Answer:
```javascript
app.use(express.json());   // All routes
app.use(cors());           // All routes
app.use(logger);           // All routes
```

`app.use()` without a path applies to all routes.

## Key Points:
- `app.use()` without path.
- Runs on every request.
- Before route handlers.
- Common for parsing, logging, CORS.

## Interview Tip:
"`app.use()` without a path applies to all routes â€” use it for global concerns."

---

## Question 63: How do you apply middleware to specific routes?

## Answer:
```javascript
// Specific route
app.get("/admin", authMiddleware, (req, res) => { ... });

// Specific path prefix
app.use("/api", authMiddleware);

// Router-level
router.use(authMiddleware);
```

## Key Points:
- Pass middleware as argument to route.
- `app.use(path, middleware)` for path prefix.
- Router-level for feature groups.
- More granular control.

## Interview Tip:
"Apply middleware to specific routes by passing it as an argument."

---

## Question 64: How do you chain multiple middleware functions?

## Answer:
```javascript
app.post("/users",
  authMiddleware,
  validateUser,
  createUser
);

// Or as array
app.post("/users", [authMiddleware, validateUser], createUser);
```

## Key Points:
- Multiple middleware as arguments.
- Or as an array.
- Execute in order.
- Each calls `next()`.
- Last one is the handler.

## Interview Tip:
"Chain middleware by passing multiple arguments â€” they execute in order."

---

## Question 65: What is the difference between middleware and route handlers?

## Answer:
- **Middleware**: Processes requests, can modify req/res, calls `next()`.
- **Route handler**: Handles specific route, sends response.

Both are functions with `req`, `res`, `next` â€” the difference is intent.

## Key Points:
- Middleware: processing, modification.
- Route handler: final response.
- Both have same signature.
- Middleware calls `next()`.
- Route handler sends response.

## Interview Tip:
"Middleware processes; route handlers respond. Both have the same function signature."

---

## Question 66: How do you skip middleware?

## Answer:
```javascript
// Skip for specific routes
app.use((req, res, next) => {
  if (req.path === "/health") return next();
  authMiddleware(req, res, next);
});

// Or use path
app.use("/api", authMiddleware);
// /health doesn't go through auth
```

## Key Points:
- Check `req.path` to skip.
- Use path-specific middleware.
- Conditional logic in middleware.
- `next()` to skip.

## Interview Tip:
"Skip middleware by checking `req.path` or using path-specific middleware."

---

## Question 67: How do you pass data between middleware?

## Answer:
Attach data to `req` object:

```javascript
const auth = (req, res, next) => {
  req.user = { id: 1, role: "admin" };
  next();
};

const handler = (req, res) => {
  res.json({ user: req.user });
};
```

## Key Points:
- Attach to `req` object.
- Available in subsequent middleware.
- Common for user data, timestamps.
- Custom properties on `req`.
- Clean and simple.

## Interview Tip:
"Attach data to `req` â€” it flows through the middleware chain."

---

## Question 68: What are common middleware use cases?

## Answer:
1. **Authentication**: Verify tokens.
2. **Authorization**: Check permissions.
3. **Logging**: Log requests.
4. **Validation**: Validate input.
5. **CORS**: Cross-origin headers.
6. **Rate limiting**: Prevent abuse.
7. **Error handling**: Catch errors.

## Key Points:
- Auth and authorization.
- Logging and monitoring.
- Input validation.
- CORS and security.
- Rate limiting.
- Error handling.

## Interview Tip:
"Middleware is for cross-cutting concerns â€” auth, logging, validation, security."

---

## Question 69: What are common mistakes when writing middleware?

## Answer:
1. **Forgetting `next()`**: Request hangs.
2. **Not sending response**: Request hangs.
3. **Async errors not caught**: Unhandled rejections.
4. **Wrong order**: Middleware runs in wrong order.
5. **Not ending cycle**: Both `next()` and `res.send()`.

## Key Points:
- Always call `next()` or send response.
- Catch async errors.
- Register in correct order.
- Don't call both `next()` and `res.send()`.
- Test middleware independently.

## Interview Tip:
"Forgetting `next()` is the most common middleware mistake â€” the request hangs forever."

---

## Question 70: How do you debug middleware execution?

## Answer:
```javascript
app.use((req, res, next) => {
  console.log("Before:", req.path);
  next();
});

// Or with Morgan
app.use(morgan("dev"));
```

## Key Points:
- Add logging middleware.
- Use Morgan for HTTP logging.
- Console.log in custom middleware.
- Check order of registration.
- Use debugger.

## Interview Tip:
"Add logging middleware to see the execution flow â€” Morgan is the standard."

---

## Part 8 (71â€“80): Error Handling

---

## Question 71: How does Express.js handle errors?

## Answer:
Express has a built-in error handling mechanism. Errors are passed to error-handling middleware (4 parameters).

```javascript
// Pass error with next()
app.get("/", (req, res, next) => {
  next(new Error("Something went wrong"));
});

// Error handler
app.use((err, req, res, next) => {
  res.status(500).json({ error: err.message });
});
```

## Key Points:
- `next(err)` passes to error handler.
- Error middleware has 4 parameters.
- Catches sync and async errors.
- Must be registered last.
- Custom error classes for different errors.

## Interview Tip:
"Use `next(err)` to pass errors to the error handler â€” never let errors go unhandled."

---

## Question 72: What is error-handling middleware?

## Answer:
Error-handling middleware has 4 parameters: `err`, `req`, `res`, `next`.

```javascript
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(err.status || 500).json({
    error: err.message || "Internal server error"
  });
});
```

## Key Points:
- 4 parameters: `err`, `req`, `res`, `next`.
- Must be registered last.
- Catches all errors.
- Custom error handling.
- Centralized error responses.

## Interview Tip:
"Error middleware has 4 parameters â€” that's how Express recognizes it as error handler."

---

## Question 73: Why does error middleware have four parameters?

## Answer:
Express uses the 4-parameter signature to identify error-handling middleware. The first parameter is the error object.

```javascript
app.use((err, req, res, next) => {
  // err is the error object
  // Express knows this is error middleware because of 4 params
});
```

## Key Points:
- 4 parameters = error handler.
- First param is error.
- Express identifies by parameter count.
- Must be registered last.
- Can have multiple error handlers.

## Interview Tip:
"4 parameters = error handler. That's how Express identifies it."

---

## Question 74: How do you create a global error handler?

## Answer:
```javascript
// At the end of app.js (after all routes)
app.use((err, req, res, next) => {
  const status = err.status || 500;
  const message = err.message || "Internal server error";
  
  console.error(`[${new Date().toISOString()}] ${status}: ${message}`);
  
  res.status(status).json({
    error: {
      message,
      ...(process.env.NODE_ENV === "development" && { stack: err.stack })
    }
  });
});
```

## Key Points:
- Register after all routes.
- Consistent error response format.
- Log errors.
- Include stack trace in development.
- Hide details in production.

## Interview Tip:
"Register the error handler last â€” it catches all errors from routes and middleware."

---

## Question 75: How do you handle asynchronous errors?

## Answer:
```javascript
// Option 1: try/catch
app.get("/users", async (req, res, next) => {
  try {
    const users = await User.find();
    res.json(users);
  } catch (err) {
    next(err);
  }
});

// Option 2: Wrapper function
const asyncHandler = (fn) => (req, res, next) => {
  Promise.resolve(fn(req, res, next)).catch(next);
};

app.get("/users", asyncHandler(async (req, res) => {
  const users = await User.find();
  res.json(users);
}));
```

## Key Points:
- Async errors need try/catch.
- `next(err)` passes to error handler.
- Wrapper function for DRY code.
- Express 5 handles async errors automatically.
- Always catch async errors.

## Interview Tip:
"Use a wrapper function to avoid try/catch in every route â€” `asyncHandler` is the standard."

---

## Question 76: What happens when an error is thrown inside an async route?

## Answer:
In Express 4, unhandled async errors crash the server. You must catch them manually.

In Express 5, async errors are automatically passed to the error handler.

```javascript
// Express 4: CRASHES without try/catch
app.get("/users", async (req, res) => {
  throw new Error("Crash!"); // Server crashes
});

// Express 4: Safe with wrapper
app.get("/users", asyncHandler(async (req, res) => {
  throw new Error("Caught!"); // Passed to error handler
}));
```

## Key Points:
- Express 4: async errors crash server.
- Express 5: async errors caught automatically.
- Use `asyncHandler` wrapper in Express 4.
- Always handle async errors.
- Never let errors go unhandled.

## Interview Tip:
"In Express 4, always use `asyncHandler` â€” without it, async errors crash the server."

---

## Question 77: How do you return consistent error responses?

## Answer:
```javascript
// Custom error class
class AppError extends Error {
  constructor(message, status) {
    super(message);
    this.status = status;
  }
}

// Usage
throw new AppError("User not found", 404);

// Error handler
app.use((err, req, res, next) => {
  res.status(err.status || 500).json({
    error: {
      message: err.message,
      status: err.status || 500
    }
  });
});
```

## Key Points:
- Custom error classes.
- Consistent response format.
- Include status code.
- Include error message.
- Include details in development.

## Interview Tip:
"Custom error classes ensure consistent error responses across your API."

---

## Question 78: How do you log application errors?

## Answer:
```javascript
// Winston logger
const winston = require("winston");
const logger = winston.createLogger({
  transports: [new winston.transports.Console()]
});

app.use((err, req, res, next) => {
  logger.error({
    message: err.message,
    stack: err.stack,
    path: req.path,
    method: req.method
  });
  res.status(500).json({ error: "Internal server error" });
});
```

## Key Points:
- Use Winston or Pino.
- Log message, stack, path, method.
- Don't expose stack to client.
- Structured logging for production.
- Log levels (error, warn, info).

## Interview Tip:
"Log errors with context (path, method, stack) â€” but never expose the stack to the client."

---

## Question 79: What HTTP status codes should be used for common API errors?

## Answer:
- **400**: Bad Request (validation errors).
- **401**: Unauthorized (no authentication).
- **403**: Forbidden (no permission).
- **404**: Not Found (resource doesn't exist).
- **409**: Conflict (duplicate data).
- **422**: Unprocessable Entity (business logic error).
- **429**: Too Many Requests (rate limited).
- **500**: Internal Server Error (server error).

## Key Points:
- 400: client error, validation.
- 401: no authentication.
- 403: no permission.
- 404: not found.
- 500: server error.

## Interview Tip:
"Use the most specific status code â€” 404 for not found, 400 for validation, 401 for auth."

---

## Question 80: What are Express.js error-handling best practices?

## Answer:
1. **Centralized error handler**: One error handler at the end.
2. **Custom error classes**: Different errors for different scenarios.
3. **Async error handling**: Use `asyncHandler` wrapper.
4. **Consistent responses**: Same format for all errors.
5. **Log errors**: Don't just send responses.
6. **Hide details**: No stack traces in production.
7. **Appropriate status codes**: Use correct HTTP codes.

## Key Points:
- Centralized error handling.
- Custom error classes.
- Async error wrapper.
- Consistent response format.
- Log errors.
- Hide details in production.
- Appropriate status codes.

## Interview Tip:
"Centralized error handling with custom error classes â€” that's the production standard."

---

## Part 9 (81â€“90): Authentication & Authorization

---

## Question 81: How do you implement authentication in Express.js?

## Answer:
1. **Register**: Create user with hashed password.
2. **Login**: Verify credentials, return JWT.
3. **Auth middleware**: Verify JWT on protected routes.
4. **Protected routes**: Use auth middleware.

```javascript
app.post("/login", async (req, res) => {
  const user = await User.findOne({ email: req.body.email });
  if (!user || !await bcrypt.compare(req.body.password, user.password)) {
    return res.status(401).json({ error: "Invalid credentials" });
  }
  const token = jwt.sign({ id: user.id }, process.env.JWT_SECRET);
  res.json({ token });
});
```

## Key Points:
- Register with hashed password.
- Login returns JWT.
- Auth middleware verifies token.
- Protected routes use middleware.
- Use bcrypt for passwords.

## Interview Tip:
"The auth flow is: register â†’ login â†’ get token â†’ send token with requests â†’ verify in middleware."

---

## Question 82: What is JWT authentication?

## Answer:
JWT (JSON Web Token) is a compact, self-contained token for securely transmitting information. It contains a payload signed with a secret.

```
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MSwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c
```

## Key Points:
- Compact, self-contained token.
- Contains payload (user data).
- Signed with secret.
- Stateless (no server storage).
- Sent in Authorization header.

## Interview Tip:
"JWT is stateless â€” the server doesn't store sessions, just verifies the token."

---

## Question 83: How does JWT work?

## Answer:
1. **User logs in**: Server verifies credentials.
2. **Server creates JWT**: Signs with secret.
3. **Client stores token**: localStorage or cookie.
4. **Client sends token**: In Authorization header.
5. **Server verifies token**: Checks signature and expiration.

## Key Points:
- Login creates token.
- Client stores and sends token.
- Server verifies on each request.
- Stateless authentication.
- Signed with secret.

## Interview Tip:
"JWT flow: login â†’ get token â†’ send with requests â†’ verify in middleware."

---

## Question 84: How do you verify a JWT?

## Answer:
```javascript
const jwt = require("jsonwebtoken");

const authMiddleware = (req, res, next) => {
  const token = req.headers.authorization?.split(" ")[1];
  if (!token) return res.status(401).json({ error: "No token" });
  
  try {
    const decoded = jwt.verify(token, process.env.JWT_SECRET);
    req.user = decoded;
    next();
  } catch (err) {
    res.status(401).json({ error: "Invalid token" });
  }
};
```

## Key Points:
- `jwt.verify(token, secret)`.
- Returns decoded payload.
- Throws on invalid/expired token.
- Attach user to `req`.
- Call `next()` on success.

## Interview Tip:
"`jwt.verify()` throws on invalid tokens â€” always wrap in try/catch."

---

## Question 85: Where should JWT tokens be stored?

## Answer:
- **HTTP-only cookies**: Most secure (XSS-resistant).
- **localStorage**: Convenient but vulnerable to XSS.
- **Memory**: Most secure but lost on refresh.

Best practice: HTTP-only cookies.

## Key Points:
- HTTP-only cookies: most secure.
- localStorage: convenient but risky.
- Memory: secure but not persistent.
- Always use HTTPS.
- Set secure and sameSite flags.

## Interview Tip:
"HTTP-only cookies are the most secure â€” they're invisible to JavaScript."

---

## Question 86: What is refresh token authentication?

## Answer:
Two tokens: short-lived access token + long-lived refresh token.

1. **Access token**: 15 minutes, used for API requests.
2. **Refresh token**: 7 days, used to get new access tokens.

When access token expires, use refresh token to get a new one.

## Key Points:
- Two tokens: access + refresh.
- Access token: short-lived.
- Refresh token: long-lived.
- Refresh token gets new access token.
- More secure than single long-lived token.

## Interview Tip:
"Access tokens are short-lived for security; refresh tokens are long-lived for UX."

---

## Question 87: What is the difference between authentication and authorization?

## Answer:
- **Authentication**: "Who are you?" (identity verification).
- **Authorization**: "What can you do?" (permission check).

## Key Points:
- Authentication: verify identity.
- Authorization: check permissions.
- Authentication first, then authorization.
- JWT for authentication.
- Middleware for authorization.

## Interview Tip:
"Authentication proves who you are; authorization determines what you can do."

---

## Question 88: How do you implement role-based access control (RBAC)?

## Answer:
```javascript
const authorize = (...roles) => {
  return (req, res, next) => {
    if (!roles.includes(req.user.role)) {
      return res.status(403).json({ error: "Forbidden" });
    }
    next();
  };
};

// Usage
app.delete("/users/:id", authMiddleware, authorize("admin"), deleteUser);
```

## Key Points:
- Roles: admin, user, moderator.
- Middleware checks role.
- 403 if insufficient permissions.
- Pass roles as arguments.
- Reusable across routes.

## Interview Tip:
"RBAC middleware checks user role â€” return 403 if insufficient permissions."

---

## Question 89: How do you protect private routes?

## Answer:
```javascript
// Auth middleware
const auth = (req, res, next) => {
  const token = req.headers.authorization?.split(" ")[1];
  if (!token) return res.status(401).json({ error: "Unauthorized" });
  
  try {
    req.user = jwt.verify(token, process.env.JWT_SECRET);
    next();
  } catch (err) {
    res.status(401).json({ error: "Invalid token" });
  }
};

// Protected route
app.get("/profile", auth, (req, res) => {
  res.json({ user: req.user });
});
```

## Key Points:
- Auth middleware before route.
- Verify token in middleware.
- Attach user to `req`.
- Return 401 if invalid.
- Call `next()` if valid.

## Interview Tip:
"Auth middleware protects routes â€” verify token, attach user, call `next()`."

---

## Question 90: What are common authentication mistakes?

## Answer:
1. **Storing passwords in plain text**: Always hash with bcrypt.
2. **Long-lived access tokens**: Use short-lived tokens.
3. **No HTTPS**: Tokens can be intercepted.
4. **Weak secrets**: Use strong JWT secrets.
5. **No token expiration**: Tokens should expire.
6. **Storing JWT in localStorage**: Vulnerable to XSS.

## Key Points:
- Hash passwords with bcrypt.
- Short-lived access tokens.
- Always use HTTPS.
- Strong JWT secrets.
- Token expiration.
- HTTP-only cookies for tokens.

## Interview Tip:
"The biggest mistake is storing passwords in plain text â€” always hash with bcrypt."

---

## Part 10 (91â€“100): Validation & Security

---

## Question 91: How do you validate incoming request data?

## Answer:
```javascript
const { z } = require("zod");

const UserSchema = z.object({
  name: z.string().min(1).max(100),
  email: z.string().email(),
  age: z.number().int().min(0).max(150)
});

app.post("/users", (req, res) => {
  const result = UserSchema.safeParse(req.body);
  if (!result.success) {
    return res.status(400).json({ errors: result.error.flatten() });
  }
  // result.data is validated and typed
});
```

## Key Points:
- Validate all external input.
- Zod for runtime validation.
- Return 400 for validation errors.
- Never trust client input.
- Validate at system boundaries.

## Interview Tip:
"Zod gives you runtime validation and TypeScript types in one step â€” use it everywhere."

---

## Question 92: What validation libraries have you used?

## Answer:
- **Zod**: TypeScript-first, runtime validation.
- **Joi**: Popular, schema-based validation.
- **Yup**: Similar to Joi, browser-friendly.
- **express-validator**: Express-specific validation.
- **class-validator**: Decorator-based (NestJS).

## Key Points:
- Zod: TypeScript-first.
- Joi: most popular.
- Yup: browser-friendly.
- express-validator: Express-specific.
- Choose based on needs.

## Interview Tip:
"Zod is my go-to â€” it's TypeScript-first and gives you runtime + compile-time safety."

---

## Question 93: How do you sanitize user input?

## Answer:
```javascript
const sanitizeHtml = require("sanitize-html");

app.post("/comments", (req, res) => {
  const clean = sanitizeHtml(req.body.content, {
    allowedTags: ["b", "i", "em", "strong"],
    allowedAttributes: {}
  });
  // Store clean content
});
```

## Key Points:
- Sanitize HTML to prevent XSS.
- Remove malicious scripts.
- Whitelist allowed tags.
- Sanitize before storing.
- Don't trust client input.

## Interview Tip:
"Sanitize HTML input â€” whitelist allowed tags, strip everything else."

---

## Question 94: How do you prevent SQL Injection?

## Answer:
```javascript
// BAD: string concatenation
const query = `SELECT * FROM users WHERE id = ${userId}`;

// GOOD: parameterized query
const query = "SELECT * FROM users WHERE id = $1";
const result = await db.query(query, [userId]);

// BETTER: use ORM
const user = await User.findById(userId);
```

## Key Points:
- Use parameterized queries.
- Use ORM (Prisma, TypeORM).
- Never concatenate user input.
- Validate input types.
- Least privilege database user.

## Interview Tip:
"Parameterized queries prevent SQL injection â€” never concatenate user input into SQL."

---

## Question 95: How do you prevent NoSQL Injection?

## Answer:
```javascript
// BAD: passing raw user input
const user = await User.findOne({ email: req.body.email });

// GOOD: validate and cast types
const email = String(req.body.email);
const user = await User.findOne({ email });
```

## Key Points:
- Validate input types.
- Cast to expected types.
- Use Mongoose validation.
- Don't pass raw objects to queries.
- Schema validation.

## Interview Tip:
"Validate that input is the expected type â€” a string should be a string, not an object."

---

## Question 96: How do you prevent Cross-Site Scripting (XSS)?

## Answer:
1. **Sanitize output**: Escape HTML in responses.
2. **Content Security Policy**: Restrict script sources.
3. **HTTP-only cookies**: Prevent JavaScript access.
4. **Input validation**: Reject malicious input.
5. **Helmet**: Security headers.

```javascript
app.use(helmet());
```

## Key Points:
- Sanitize output.
- CSP headers.
- HTTP-only cookies.
- Input validation.
- Helmet for security headers.

## Interview Tip:
"Helmet adds security headers including CSP â€” use it on every Express app."

---

## Question 97: How do you prevent Cross-Site Request Forgery (CSRF)?

## Answer:
1. **SameSite cookies**: Prevent cross-site requests.
2. **CSRF tokens**: Validate on mutations.
3. **Origin checks**: Verify request origin.

```javascript
const csrf = require("csurf");
app.use(csrf({ cookie: true }));
```

## Key Points:
- SameSite cookies.
- CSRF tokens.
- Origin verification.
- Most APIs use JWT (stateless), reducing CSRF risk.
- Essential for session-based auth.

## Interview Tip:
"JWT-based APIs are naturally CSRF-resistant â€” SameSite cookies add extra protection."

---

## Question 98: How do you implement rate limiting in Express.js?

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
- `express-rate-limit` package.
- Configure window and max.
- Apply to specific routes.
- Return 429 on limit.
- Prevent abuse and DDoS.

## Interview Tip:
"Rate limit login endpoints stricter than other routes â€” prevent brute force attacks."

---

## Question 99: What security middleware do you commonly use?

## Answer:
- **helmet**: Security headers.
- **cors**: CORS configuration.
- **express-rate-limit**: Rate limiting.
- **express-mongo-sanitize**: Prevent NoSQL injection.
- **hpp**: HTTP parameter pollution protection.

```javascript
app.use(helmet());
app.use(cors({ origin: "https://example.com" }));
app.use(mongoSanitize());
app.use(hpp());
```

## Key Points:
- Helmet: security headers.
- CORS: cross-origin configuration.
- Rate limiting: abuse prevention.
- mongo-sanitize: NoSQL injection.
- hpp: parameter pollution.

## Interview Tip:
"Helmet, CORS, rate limiting, and mongo-sanitize â€” the security middleware essentials."

---

## Question 100: What security best practices do you follow when building Express APIs?

## Answer:
1. **Helmet**: Security headers.
2. **CORS**: Restrict origins.
3. **Rate limiting**: Prevent abuse.
4. **Input validation**: Validate all input.
5. **HTTPS**: Encrypt in transit.
6. **HTTP-only cookies**: Secure token storage.
7. **Parameterized queries**: Prevent injection.
8. **Error handling**: Don't leak details.

## Key Points:
- Helmet for security headers.
- CORS for cross-origin control.
- Rate limiting for abuse prevention.
- Input validation for data integrity.
- HTTPS for encryption.
- HTTP-only cookies for tokens.
- Parameterized queries for injection prevention.

## Interview Tip:
"Security is defense in depth â€” Helmet, CORS, rate limiting, validation, and HTTPS."

---

## Part 11 (101â€“110): Project Architecture

---

## Question 101: How do you structure a large Express.js application?

## Answer:
```
src/
  routes/
    user.routes.js
    auth.routes.js
  controllers/
    user.controller.js
    auth.controller.js
  services/
    user.service.js
    auth.service.js
  models/
    user.model.js
  middleware/
    auth.js
    validate.js
  config/
    db.js
    env.js
  utils/
    helpers.js
  app.js
  server.js
```

## Key Points:
- Routes for URL mapping.
- Controllers for request handling.
- Services for business logic.
- Models for data access.
- Middleware for cross-cutting concerns.
- Config for configuration.

## Interview Tip:
"Routes â†’ Controllers â†’ Services â†’ Models â€” the four-layer architecture."

---

## Question 102: What folder structure do you recommend for enterprise Express.js projects?

## Answer:
Feature-based structure:

```
src/
  features/
    auth/
      auth.routes.js
      auth.controller.js
      auth.service.js
      auth.validation.js
    users/
      users.routes.js
      users.controller.js
      users.service.js
  shared/
    middleware/
    utils/
    config/
  app.js
```

## Key Points:
- Feature-based organization.
- Each feature is self-contained.
- Shared code in `shared/`.
- Easy to navigate.
- Scales well.

## Interview Tip:
"Feature-based structure scales better than type-based for large teams."

---

## Question 103: What is the MVC architecture pattern?

## Answer:
MVC = Model-View-Controller:
- **Model**: Data and business logic.
- **View**: UI (not applicable for APIs).
- **Controller**: Handles requests, coordinates Model and View.

For APIs: Controllers handle requests, Services contain business logic, Models handle data.

## Key Points:
- Model: data and logic.
- View: UI (not for APIs).
- Controller: request handling.
- For APIs: Controller + Service + Model.

## Interview Tip:
"For APIs, think Controller-Service-Model instead of traditional MVC."

---

## Question 104: What are the responsibilities of Controllers?

## Answer:
Controllers handle HTTP concerns:
- Parse request data.
- Call service layer.
- Send response.
- Handle errors.

```javascript
const getUsers = async (req, res, next) => {
  try {
    const users = await userService.getAll(req.query);
    res.json(users);
  } catch (err) {
    next(err);
  }
};
```

## Key Points:
- HTTP request/response handling.
- Call services for business logic.
- Parse request data.
- Send responses.
- Handle errors.

## Interview Tip:
"Controllers are thin â€” they parse requests, call services, and send responses."

---

## Question 105: What should be placed in the Service Layer?

## Answer:
Business logic belongs in services:
- Data validation rules.
- Business calculations.
- Data transformations.
- External API calls.
- Complex operations.

```javascript
class UserService {
  async createUser(data) {
    const hashedPassword = await bcrypt.hash(data.password, 12);
    return User.create({ ...data, password: hashedPassword });
  }
}
```

## Key Points:
- Business logic.
- Data validation.
- Calculations and transformations.
- External API integration.
- Reusable across controllers.

## Interview Tip:
"Services contain business logic â€” they're testable and reusable."

---

## Question 106: What is the Repository Pattern?

## Answer:
The Repository Pattern abstracts data access behind an interface.

```javascript
class UserRepository {
  async findById(id) {
    return User.findById(id);
  }
  async create(data) {
    return User.create(data);
  }
}
```

Services call repositories instead of directly using models.

## Key Points:
- Abstracts data access.
- Services call repositories.
- Easy to swap data sources.
- Testable with mocks.
- Clean separation.

## Interview Tip:
"Repositories abstract data access â€” swap databases without changing services."

---

## Question 107: Why should business logic not be written in controllers?

## Answer:
- **Testability**: Services are easier to test than controllers.
- **Reusability**: Logic in services can be reused.
- **Separation of concerns**: Controllers handle HTTP, services handle logic.
- **Maintainability**: Easier to find and modify logic.

## Key Points:
- Services are testable.
- Logic is reusable.
- Clean separation.
- Easier maintenance.
- Controllers stay thin.

## Interview Tip:
"Thin controllers, fat services â€” that's the golden rule."

---

## Question 108: How do you organize routes, controllers, services, and models?

## Answer:
```
routes â†’ controllers â†’ services â†’ models
```

- **Routes**: Map URLs to controllers.
- **Controllers**: Handle request/response.
- **Services**: Business logic.
- **Models**: Data access.

## Key Points:
- Routes for URL mapping.
- Controllers for HTTP handling.
- Services for business logic.
- Models for data access.
- Clear separation of concerns.

## Interview Tip:
"The flow is: Route â†’ Controller â†’ Service â†’ Model. Each layer has a single responsibility."

---

## Question 109: How do you manage configuration for different environments?

## Answer:
```javascript
// config/index.js
require("dotenv").config();

const config = {
  development: {
    db: "mongodb://localhost/myapp_dev",
    port: 3000
  },
  production: {
    db: process.env.DATABASE_URL,
    port: process.env.PORT
  }
};

module.exports = config[process.env.NODE_ENV || "development"];
```

## Key Points:
- Environment variables.
- Different config per environment.
- `.env` for development.
- Platform secrets for production.
- Config module for centralized access.

## Interview Tip:
"Use environment variables for all configuration â€” never hardcode values."

---

## Question 110: What Express.js architecture patterns have you used in production?

## Answer:
- **MVC**: Controllers, services, models.
- **Service Layer**: Business logic separation.
- **Repository Pattern**: Data access abstraction.
- **Middleware Pipeline**: Cross-cutting concerns.
- **Feature-based**: Organize by feature, not type.

## Key Points:
- MVC for traditional apps.
- Service Layer for business logic.
- Repository for data access.
- Middleware for cross-cutting concerns.
- Feature-based for large apps.

## Interview Tip:
"Start with MVC, add Service Layer and Repository as the app grows."

---

## Part 12 (111â€“120): API Design

---

## Question 111: How do you design a RESTful API?

## Answer:
1. **Resource-based URLs**: `/users`, `/posts`.
2. **HTTP methods**: GET, POST, PUT, DELETE.
3. **Status codes**: 200, 201, 400, 404, 500.
4. **JSON responses**: Consistent format.
5. **Versioning**: `/api/v1/users`.
6. **Pagination**: For list endpoints.

## Key Points:
- Resource-based URLs.
- Correct HTTP methods.
- Appropriate status codes.
- Consistent JSON format.
- API versioning.
- Pagination.

## Interview Tip:
"REST is about resources and HTTP methods â€” keep it simple and standard."

---

## Question 112: How do you version APIs?

## Answer:
```javascript
// URL versioning
app.use("/api/v1/users", v1UserRoutes);
app.use("/api/v2/users", v2UserRoutes);

// Header versioning
app.get("/api/users", (req, res) => {
  if (req.headers["accept-version"] === "2") {
    // v2 logic
  }
});
```

## Key Points:
- URL versioning: `/api/v1/`.
- Header versioning: `Accept-Version`.
- URL is most common.
- Maintain backward compatibility.
- Document version differences.

## Interview Tip:
"URL versioning (`/api/v1/`) is the most practical â€” visible and easy to test."

---

## Question 113: How do you structure consistent API responses?

## Answer:
```javascript
// Success
res.json({
  data: users,
  meta: { page: 1, total: 100 }
});

// Error
res.status(400).json({
  error: {
    message: "Validation failed",
    details: [{ field: "email", message: "Invalid email" }]
  }
});
```

## Key Points:
- `data` for success.
- `error` for failures.
- `meta` for pagination.
- Consistent structure.
- Document the format.

## Interview Tip:
"A consistent response format makes your API predictable and easy to consume."

---

## Question 114: How do you implement pagination?

## Answer:
```javascript
app.get("/users", async (req, res) => {
  const page = parseInt(req.query.page) || 1;
  const limit = parseInt(req.query.limit) || 10;
  const skip = (page - 1) * limit;
  
  const users = await User.find().skip(skip).limit(limit);
  const total = await User.countDocuments();
  
  res.json({
    data: users,
    meta: { page, limit, total, pages: Math.ceil(total / limit) }
  });
});
```

## Key Points:
- `page` and `limit` query params.
- `skip` and `limit` for database.
- Include total count.
- Include pagination metadata.
- Cursor-based for large datasets.

## Interview Tip:
"Always include pagination metadata â€” total count, current page, total pages."

---

## Question 115: How do you implement filtering, sorting, and searching?

## Answer:
```javascript
app.get("/users", async (req, res) => {
  const { role, sort, search } = req.query;
  
  let query = {};
  if (role) query.role = role;
  if (search) query.name = { $regex: search, $options: "i" };
  
  let sortOption = {};
  if (sort) sortOption[sort] = sort.startsWith("-") ? -1 : 1;
  
  const users = await User.find(query).sort(sortOption);
  res.json(users);
});
```

## Key Points:
- Query params for filtering.
- `$regex` for search.
- Sort direction with prefix.
- Validate filter values.
- Index filtered fields.

## Interview Tip:
"Use query params for filtering and sorting â€” validate all values."

---

## Question 116: How do you handle file uploads in Express.js?

## Answer:
```javascript
const multer = require("multer");
const upload = multer({ dest: "uploads/" });

app.post("/upload", upload.single("file"), (req, res) => {
  res.json({ filename: req.file.filename });
});

// Multiple files
app.post("/uploads", upload.array("files", 10), (req, res) => {
  res.json({ count: req.files.length });
});
```

## Key Points:
- `multer` for file uploads.
- `upload.single()` for one file.
- `upload.array()` for multiple.
- Configure destination.
- Validate file types.

## Interview Tip:
"Multer is the standard for Express file uploads â€” always validate file types and sizes."

---

## Question 117: How do you implement API documentation?

## Answer:
Use Swagger/OpenAPI:

```javascript
const swaggerUi = require("swagger-ui-express");
const swaggerDocument = require("./swagger.json");

app.use("/docs", swaggerUi.serve, swaggerUi.setup(swaggerDocument));
```

## Key Points:
- Swagger/OpenAPI for documentation.
- Interactive API docs.
- Auto-generated from annotations.
- Try-it-out feature.
- Keep docs in sync with code.

## Interview Tip:
"Swagger UI gives you interactive API documentation â€” it's a must-have for any API."

---

## Question 118: What tools have you used for API documentation?

## Answer:
- **Swagger UI**: Interactive API docs.
- **OpenAPI**: Specification standard.
- **Swagger JSDoc**: Generate from annotations.
- **Postman**: API testing and docs.
- **Redoc**: Alternative Swagger UI.

## Key Points:
- Swagger UI for interactive docs.
- OpenAPI for specification.
- Swagger JSDoc for auto-generation.
- Postman for testing.
- Redoc for alternative UI.

## Interview Tip:
"Swagger + OpenAPI is the standard â€” use annotations to keep docs in sync."

---

## Question 119: How do you implement request logging?

## Answer:
```javascript
const morgan = require("morgan");
app.use(morgan("dev")); // Short colored output
app.use(morgan("combined")); // Apache combined format
```

## Key Points:
- Morgan for HTTP logging.
- `dev` for development.
- `combined` for production.
- Log method, path, status, time.
- Custom formats available.

## Interview Tip:
"Morgan is the standard for Express request logging â€” `dev` in development, `combined` in production."

---

## Question 120: How do you monitor API usage?

## Answer:
1. **Request logging**: Morgan for HTTP logs.
2. **Error tracking**: Sentry for errors.
3. **Performance monitoring**: Datadog, New Relic.
4. **Custom metrics**: Track specific operations.
5. **Health checks**: `/health` endpoint.

## Key Points:
- Morgan for request logging.
- Sentry for error tracking.
- APM tools for performance.
- Custom metrics for business logic.
- Health checks for uptime.

## Interview Tip:
"Sentry for errors, APM for performance, Morgan for requests â€” the monitoring trifecta."

---

## Part 13 (121â€“130): Performance & Scalability

---

## Question 121: How do you improve the performance of an Express.js application?

## Answer:
1. **Compression**: gzip responses.
2. **Caching**: Redis for frequently accessed data.
3. **Connection pooling**: Database connections.
4. **Async operations**: Non-blocking I/O.
5. **Clustering**: Use all CPU cores.
6. **CDN**: Static assets.
7. **Pagination**: Limit response size.

## Key Points:
- Compression for smaller responses.
- Caching for frequent data.
- Connection pooling for databases.
- Clustering for multi-core.
- CDN for static assets.

## Interview Tip:
"Start with compression and caching â€” they give the biggest performance wins."

---

## Question 122: What causes slow Express.js APIs?

## Answer:
1. **Slow database queries**: Missing indexes.
2. **N+1 queries**: Multiple queries for related data.
3. **No caching**: Fetching same data repeatedly.
4. **Large responses**: No pagination.
5. **Synchronous operations**: Blocking the event loop.
6. **Too much middleware**: Heavy processing per request.

## Key Points:
- Database queries are the most common bottleneck.
- N+1 queries.
- Missing caching.
- Large responses.
- Synchronous operations.

## Interview Tip:
"Most slow APIs are caused by slow database queries â€” profile and optimize them."

---

## Question 123: How do you optimize database queries?

## Answer:
1. **Add indexes**: On frequently queried columns.
2. **Avoid N+1**: Use JOINs or batch loading.
3. **Select only needed columns**: Don't SELECT *.
4. **Connection pooling**: Reuse connections.
5. **Cache frequent queries**: Redis.
6. **Batch operations**: Insert/update multiple at once.

## Key Points:
- Indexes for speed.
- Avoid N+1 queries.
- Select only needed columns.
- Connection pooling.
- Cache frequent data.

## Interview Tip:
"Indexes are the most impactful optimization â€” most slow queries are missing an index."

---

## Question 124: How do you implement caching in Express.js?

## Answer:
```javascript
const Redis = require("ioredis");
const redis = new Redis();

app.get("/users", async (req, res) => {
  const cached = await redis.get("users");
  if (cached) return res.json(JSON.parse(cached));
  
  const users = await User.find();
  await redis.set("users", JSON.stringify(users), "EX", 3600);
  res.json(users);
});
```

## Key Points:
- Redis for caching.
- Check cache before database.
- Set expiration (TTL).
- Invalidate on updates.
- Cache frequently accessed data.

## Interview Tip:
"Cache expensive queries in Redis â€” check cache first, database second."

---

## Question 125: When would you use Redis?

## Answer:
- **Caching**: Frequently accessed data.
- **Session storage**: User sessions.
- **Rate limiting**: Request counters.
- **Real-time**: Pub/sub for notifications.
- **Job queues**: Background tasks.

## Key Points:
- Caching for performance.
- Sessions for multi-instance apps.
- Rate limiting for abuse prevention.
- Pub/sub for real-time.
- Job queues for background work.

## Interview Tip:
"Redis is the Swiss Army knife of backend infrastructure â€” caching, sessions, queues, and real-time."

---

## Question 126: How do you compress HTTP responses?

## Answer:
```javascript
const compression = require("compression");
app.use(compression());
```

Enables gzip compression for all responses.

## Key Points:
- `compression` middleware.
- Gzip for text responses.
- Reduces response size.
- Improves load times.
- Configurable.

## Interview Tip:
"`compression` middleware is a one-line performance boost â€” use it on every Express app."

---

## Question 127: How do you handle high traffic?

## Answer:
1. **Load balancing**: Distribute across instances.
2. **Caching**: Redis for frequent data.
3. **Connection pooling**: Database connections.
4. **Rate limiting**: Prevent abuse.
5. **CDN**: Static assets.
6. **Clustering**: Use all CPU cores.

## Key Points:
- Load balancing for distribution.
- Caching for reduced load.
- Connection pooling for efficiency.
- Rate limiting for protection.
- CDN for static content.

## Interview Tip:
"Load balancing + caching + connection pooling handles most high-traffic scenarios."

---

## Question 128: How do you implement load balancing?

## Answer:
```javascript
// Nginx upstream
upstream backend {
  server 127.0.0.1:3000;
  server 127.0.0.1:3001;
  server 127.0.0.1:3002;
}

// Or with PM2
pm2 start app.js -i max  // Cluster mode
```

## Key Points:
- Nginx as reverse proxy.
- PM2 for Node.js clustering.
- Multiple instances.
- Distribute requests.
- Health checks.

## Interview Tip:
"PM2 with cluster mode is the easiest way to load balance Node.js apps."

---

## Question 129: How do you scale an Express.js application horizontally?

## Answer:
1. **Stateless services**: No in-memory sessions.
2. **External session store**: Redis for sessions.
3. **Load balancer**: Distribute traffic.
4. **Multiple instances**: Run on different servers.
5. **Database scaling**: Read replicas.

## Key Points:
- Stateless services.
- Redis for sessions.
- Load balancer for distribution.
- Multiple instances.
- Database read replicas.

## Interview Tip:
"Stateless services scale horizontally â€” store sessions in Redis, not in memory."

---

## Question 130: What production performance best practices do you follow?

## Answer:
1. **Compression**: gzip all responses.
2. **Caching**: Redis for frequent data.
3. **Connection pooling**: Database connections.
4. **Clustering**: Use all CPU cores.
5. **Rate limiting**: Prevent abuse.
6. **CDN**: Static assets.
7. **Monitoring**: Track performance metrics.

## Key Points:
- Compression for smaller responses.
- Caching for reduced load.
- Connection pooling for efficiency.
- Clustering for multi-core.
- Rate limiting for protection.
- CDN for static content.
- Monitoring for visibility.

## Interview Tip:
"Compression, caching, and connection pooling â€” the performance trifecta."

---

## Part 14 (131â€“140): Testing & Deployment

---

## Question 131: How do you test Express.js APIs?

## Answer:
```javascript
const request = require("supertest");
const app = require("../app");

describe("GET /users", () => {
  it("returns list of users", async () => {
    const res = await request(app).get("/api/users");
    expect(res.status).toBe(200);
    expect(Array.isArray(res.body)).toBe(true);
  });
});
```

## Key Points:
- Supertest for HTTP testing.
- Test status codes and response body.
- Test happy path and error cases.
- Integration tests for full flow.
- Unit tests for services.

## Interview Tip:
"Supertest is the standard for Express API testing â€” test status codes and response bodies."

---

## Question 132: What testing frameworks have you used?

## Answer:
- **Jest**: Most popular test runner.
- **Mocha**: Flexible test framework.
- **Supertest**: HTTP assertions.
- **Chai**: Assertion library.
- **Sinon**: Mocking and stubbing.

## Key Points:
- Jest: most popular, batteries-included.
- Mocha: flexible, needs assertion library.
- Supertest: HTTP testing.
- Chai: assertions.
- Sinon: mocking.

## Interview Tip:
"Jest + Supertest is the standard for Express testing."

---

## Question 133: How do you write unit tests for controllers and services?

## Answer:
```javascript
// Service test
describe("UserService", () => {
  it("creates a user", async () => {
    const user = await userService.create({ name: "Alice", email: "alice@test.com" });
    expect(user.name).toBe("Alice");
  });
});

// Controller test (mock service)
describe("UserController", () => {
  it("returns users", async () => {
    jest.spyOn(userService, "getAll").mockResolvedValue([{ name: "Alice" }]);
    const res = await request(app).get("/api/users");
    expect(res.body[0].name).toBe("Alice");
  });
});
```

## Key Points:
- Test services directly.
- Mock dependencies for controllers.
- Test happy path and errors.
- Use Jest for mocking.
- Test business logic in services.

## Interview Tip:
"Test services directly â€” mock dependencies for controller tests."

---

## Question 134: How do you write integration tests for Express APIs?

## Answer:
```javascript
describe("POST /api/users", () => {
  it("creates a user", async () => {
    const res = await request(app)
      .post("/api/users")
      .send({ name: "Alice", email: "alice@test.com" });
    
    expect(res.status).toBe(201);
    expect(res.body.name).toBe("Alice");
  });

  it("returns 400 for invalid data", async () => {
    const res = await request(app)
      .post("/api/users")
      .send({ name: "" });
    
    expect(res.status).toBe(400);
  });
});
```

## Key Points:
- Test full request cycle.
- Test happy path and errors.
- Use real database (test DB).
- Clean up after tests.
- Test authentication.

## Interview Tip:
"Integration tests verify the full request cycle â€” use a test database."

---

## Question 135: How do you mock database calls during testing?

## Answer:
```javascript
// Mock Mongoose
jest.mock("../models/User");
const User = require("../models/User");

User.find.mockResolvedValue([{ name: "Alice" }]);

// Or use mongodb-memory-server
const { MongoMemoryServer } = require("mongodb-memory-server");
let mongoServer;

beforeAll(async () => {
  mongoServer = await MongoMemoryServer.create();
  await mongoose.connect(mongoServer.getUri());
});

afterAll(async () => {
  await mongoose.disconnect();
  await mongoServer.stop();
});
```

## Key Points:
- Jest mocking for unit tests.
- `mongodb-memory-server` for integration tests.
- Mock for speed; real DB for accuracy.
- Clean up after tests.
- Separate test database.

## Interview Tip:
"`mongodb-memory-server` is the best way to test MongoDB â€” fast and isolated."

---

## Question 136: How do you deploy an Express.js application?

## Answer:
1. **Build**: Prepare for production.
2. **Environment variables**: Set production values.
3. **Process manager**: PM2 for Node.js.
4. **Reverse proxy**: Nginx.
5. **SSL**: HTTPS with Let's Encrypt.
6. **Monitoring**: Track errors and performance.

## Key Points:
- PM2 for process management.
- Nginx as reverse proxy.
- SSL for security.
- Environment variables.
- Monitoring and logging.

## Interview Tip:
"PM2 + Nginx is the standard Express deployment stack."

---

## Question 137: How do you containerize an Express.js application using Docker?

## Answer:
```dockerfile
FROM node:20-alpine
WORKDIR /app
COPY package*.json ./
RUN npm ci --production
COPY . .
EXPOSE 3000
CMD ["node", "server.js"]
```

## Key Points:
- Multi-stage builds for smaller images.
- `npm ci` for reproducible installs.
- `.dockerignore` for unnecessary files.
- Alpine for smaller images.
- Environment variables.

## Interview Tip:
"Use `npm ci` in Docker â€” it's faster and more reproducible than `npm install`."

---

## Question 138: How do you manage environment variables in production?

## Answer:
- **Platform secrets**: Vercel, AWS, Heroku.
- **Docker secrets**: For containerized apps.
- **Never commit**: `.env` is gitignored.
- **Different per environment**: Dev, staging, production.

## Key Points:
- Platform-specific secrets management.
- Never commit credentials.
- Different values per environment.
- Use `dotenv` for development.

## Interview Tip:
"Use platform secrets in production â€” never commit `.env` to git."

---

## Question 139: How do you implement CI/CD for Express.js applications?

## Answer:
```yaml
# GitHub Actions
name: CI
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm ci
      - run: npm test
      - run: npm run lint
```

## Key Points:
- GitHub Actions for CI/CD.
- Run tests on every push.
- Lint before merging.
- Deploy on merge to main.
- Automated quality checks.

## Interview Tip:
"CI/CD automates testing and deployment â€” GitHub Actions is the standard."

---

## Question 140: How do you monitor production applications?

## Answer:
1. **Error tracking**: Sentry.
2. **Performance monitoring**: Datadog, New Relic.
3. **Logging**: Winston, Pino.
4. **Health checks**: `/health` endpoint.
5. **Uptime monitoring**: Pingdom, UptimeRobot.

## Key Points:
- Sentry for errors.
- APM for performance.
- Structured logging.
- Health checks.
- Uptime monitoring.

## Interview Tip:
"Sentry for errors, APM for performance, structured logging for debugging."

---

## Part 15 (141â€“150): Senior Real-World Interview Questions

---

## Question 141: Describe the largest Express.js application you've worked on.

## Answer:
Pick a real project and describe:
- **Scale**: Users, requests per second, data volume.
- **Architecture**: Services, databases, deployment.
- **Challenges**: What was hard and how you solved it.
- **Your role**: What you specifically contributed.
- **Results**: Performance improvements, features delivered.

## Key Points:
- Quantify the scale.
- Describe the architecture.
- Highlight challenges and solutions.
- Explain your contributions.
- Show impact.

## Interview Tip:
"Tell a story with a beginning (problem), middle (solution), and end (result)."

---

## Question 142: What was the most difficult Express.js bug you've fixed?

## Answer:
Describe:
1. **Symptoms**: What was happening.
2. **Investigation**: How you diagnosed it.
3. **Root cause**: What was actually wrong.
4. **Fix**: How you resolved it.
5. **Lesson**: What you learned.

## Key Points:
- Symptoms, investigation, root cause, fix, lesson.
- Systematic debugging approach.
- Tools used.
- What you learned.

## Interview Tip:
"Interviewers want to see your debugging process, not just the fix."

---

## Question 143: How do you debug production issues in Express.js?

## Answer:
1. **Check logs**: Winston/Pino logs.
2. **Error tracking**: Sentry for errors.
3. **APM**: Performance monitoring.
4. **Health checks**: Database connectivity.
5. **Profiling**: CPU and memory usage.
6. **Reproduce**: Try in staging.

## Key Points:
- Logs for context.
- Sentry for errors.
- APM for performance.
- Health checks for connectivity.
- Profiling for bottlenecks.

## Interview Tip:
"Start with logs and Sentry â€” they show you what went wrong."

---

## Question 144: How do you review Express.js pull requests?

## Answer:
Check for:
1. **Error handling**: Try/catch, error middleware.
2. **Validation**: Input validation present.
3. **Security**: SQL injection, XSS prevention.
4. **Performance**: N+1 queries, missing indexes.
5. **Code quality**: Naming, structure, tests.

## Key Points:
- Error handling.
- Input validation.
- Security checks.
- Performance considerations.
- Code quality.

## Interview Tip:
"Security and error handling are the most important things to check."

---

## Question 145: What coding standards do you enforce in your team?

## Answer:
1. **Linting**: ESLint with strict rules.
2. **Formatting**: Prettier.
3. **Type checking**: TypeScript.
4. **Testing**: Required for new features.
5. **Code review**: All PRs reviewed.
6. **Error handling**: All async operations.

## Key Points:
- ESLint for linting.
- Prettier for formatting.
- TypeScript for type safety.
- Tests required.
- Code review mandatory.

## Interview Tip:
"Automate what you can (linting, formatting) and enforce the rest through code review."

---

## Question 146: How do you mentor junior backend developers?

## Answer:
1. **Code review**: Detailed, educational feedback.
2. **Pair programming**: Work together on complex problems.
3. **Architecture discussions**: Explain why, not just what.
4. **Gradual responsibility**: Start small, increase complexity.
5. **Knowledge sharing**: Tech talks and documentation.

## Key Points:
- Educational code reviews.
- Pair programming.
- Explain the "why."
- Gradual responsibility.
- Knowledge sharing.

## Interview Tip:
"The best mentoring is patient, specific, and focuses on teaching principles."

---

## Question 147: How would you migrate a legacy Express.js application to a cleaner architecture?

## Answer:
1. **Assess current state**: Understand the codebase.
2. **Identify pain points**: Find the worst areas.
3. **Create a plan**: Prioritize by impact.
4. **Incremental migration**: One feature at a time.
5. **Add tests**: Before refactoring.
6. **Refactor gradually**: Don't rewrite everything.

## Key Points:
- Assess current state.
- Identify pain points.
- Incremental migration.
- Add tests first.
- Refactor gradually.

## Interview Tip:
"Never rewrite everything â€” migrate incrementally, one feature at a time."

---

## Question 148: If you were building a production REST API today, what architecture and tooling would you choose?

## Answer:
- **Express.js**: Web framework.
- **TypeScript**: Type safety.
- **Prisma/Mongoose**: Database ORM.
- **Zod**: Input validation.
- **JWT**: Authentication.
- **Winston/Pino**: Logging.
- **Jest + Supertest**: Testing.
- **Docker**: Containerization.
- **GitHub Actions**: CI/CD.

## Key Points:
- Express for web framework.
- TypeScript for type safety.
- Prisma/Mongoose for database.
- Zod for validation.
- JWT for auth.
- Docker for deployment.

## Interview Tip:
"Choose proven, well-documented technology â€” Express + TypeScript + Prisma is the standard."

---

## Question 149: What best practices do you always follow in production Express.js applications?

## Answer:
1. **Error handling**: Global error handler.
2. **Validation**: Zod for all input.
3. **Security**: Helmet, CORS, rate limiting.
4. **Logging**: Structured logging.
5. **Environment variables**: Never hardcode.
6. **Testing**: Unit and integration tests.
7. **Monitoring**: Sentry and APM.

## Key Points:
- Error handling.
- Input validation.
- Security middleware.
- Structured logging.
- Environment variables.
- Testing.
- Monitoring.

## Interview Tip:
"Error handling, validation, security, logging, and testing â€” the production essentials."

---

## Question 150: In your opinion, what separates a junior, mid-level, and senior Express.js developer?

## Answer:
- **Junior**: Knows basic routing and middleware. Can build simple APIs with guidance.
- **Mid-level**: Understands architecture, error handling, and testing. Can build features independently.
- **Senior**: Designs scalable architecture, handles production issues, mentors others. Understands trade-offs, security, and performance.

The biggest differentiator: a senior developer understands WHY, not just WHAT.

## Key Points:
- Junior: basic routing, guided work.
- Mid-level: architecture, error handling, testing.
- Senior: design, production, mentoring.
- Senior understands trade-offs.
- Senior thinks about security and performance.

## Interview Tip:
"The best answer shows self-awareness. Pick your level and explain what you're doing to grow."

---

# End of Express.js Interview Questions & Answers
