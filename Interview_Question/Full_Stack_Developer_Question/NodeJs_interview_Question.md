# Node.js Interview Questions (250 Total)

---

## Introduction

1. What is Node.js?
2. Why was Node.js created?
3. What problems does Node.js solve?
4. How does Node.js differ from browser JavaScript?
5. What are the advantages of Node.js?
6. What are the disadvantages of Node.js?
7. What is the V8 JavaScript engine?
8. How does the V8 engine work?
9. Why is Node.js considered fast?
10. Is Node.js single-threaded or multi-threaded?

---

## Architecture

11. How does Node.js handle multiple requests?
12. What is event-driven architecture?
13. What is non-blocking I/O?
14. What is asynchronous I/O?
15. What is synchronous I/O?
16. What is the event loop?
17. What are callbacks?
18. What are Promises?
19. What is async/await?
20. What makes Node.js scalable?

---

## Global Objects

21. What is the `global` object?
22. What is `globalThis`?
23. What is the `process` object?
24. What is the `Buffer` object?
25. What is the `console` object?
26. What is `__dirname`?
27. What is `__filename`?
28. What is `process.cwd()`?
29. What is `process.env`?
30. What is `process.argv`?

---

## Modules

31. What is a module in Node.js?
32. What are CommonJS modules?
33. What are ES Modules (ESM)?
34. What is the difference between CommonJS and ESM?
35. What is `require()`?
36. What is `module.exports`?
37. What is `exports`?
38. What is the `import` statement?
39. What is the `export` statement?
40. How does Node.js cache modules?

---

## npm & Packages

41. What is npm?
42. What is `package.json`?
43. What is `package-lock.json`?
44. What is the purpose of the `node_modules` folder?
45. What is semantic versioning (SemVer)?
46. What is the difference between dependencies and devDependencies?
47. What is `npx`?
48. How do you update npm packages safely?
49. How do you handle package vulnerabilities?
50. What best practices do you follow when managing dependencies?

---

# Event Loop

51. What is the Node.js Event Loop?
52. How does the Event Loop work internally?
53. Why is the Event Loop important?
54. What are the different phases of the Event Loop?
55. What happens in the Timers phase?
56. What happens in the Pending Callbacks phase?
57. What happens in the Poll phase?
58. What happens in the Check phase?
59. What happens in the Close Callbacks phase?
60. What is the difference between the Poll phase and the Check phase?

---

# Microtasks & Macrotasks

61. What is the Call Stack?
62. What is the Callback Queue?
63. What is the Microtask Queue?
64. What is the difference between the Microtask Queue and the Callback Queue?
65. Which executes first: microtasks or macrotasks?
66. How do Promises interact with the Event Loop?
67. How does `queueMicrotask()` work?
68. How does `process.nextTick()` work?
69. What is the difference between `process.nextTick()` and `Promise.resolve()`?
70. Why can overusing `process.nextTick()` cause problems?

---

# Timers

71. How does `setTimeout()` work?
72. How does `setInterval()` work?
73. How does `setImmediate()` work?
74. What is the difference between `setImmediate()` and `setTimeout(fn, 0)`?
75. When should you use `setImmediate()`?
76. How do you cancel a timer?
77. What is `clearTimeout()`?
78. What is `clearInterval()`?
79. Why is timer execution not guaranteed to be exact?
80. What factors can delay timer execution?

---

# EventEmitter

81. What is the `EventEmitter` class?
82. Why is `EventEmitter` important in Node.js?
83. How do you create a custom event?
84. What is the difference between `on()` and `once()`?
85. What is `emit()`?
86. How do you remove event listeners?
87. What is `removeListener()`?
88. What is `removeAllListeners()`?
89. What happens if too many listeners are attached?
90. What are common use cases for `EventEmitter`?

---

# Error Handling & Async Patterns

91. How do you handle errors in asynchronous code?
92. What is the difference between synchronous and asynchronous errors?
93. How do you catch Promise rejections?
94. What is an unhandled Promise rejection?
95. How do you use `try...catch` with `async/await`?
96. What is the difference between throwing an error and rejecting a Promise?
97. How do you create custom error classes?
98. What are operational errors vs programmer errors?
99. What are Node.js best practices for error handling?
100. How do you build a centralized error-handling strategy in a Node.js application?

---

# File System (`fs`)

101. What is the `fs` module in Node.js?
102. What is the difference between synchronous and asynchronous file operations?
103. How do you read a file in Node.js?
104. How do you write data to a file?
105. How do you append data to a file?
106. How do you delete a file?
107. How do you rename or move a file?
108. How do you check whether a file or directory exists?
109. How do you create and remove directories?
110. What are common file system best practices?

---

# Streams

111. What is a stream in Node.js?
112. Why are streams more efficient than reading an entire file into memory?
113. What are the four types of streams?
114. What is a Readable stream?
115. What is a Writable stream?
116. What is a Duplex stream?
117. What is a Transform stream?
118. How do you create a readable stream?
119. How do you create a writable stream?
120. What is stream backpressure, and how do you handle it?

---

# Buffers

121. What is a Buffer in Node.js?
122. Why are Buffers needed?
123. How do Buffers differ from strings?
124. How do you create a Buffer?
125. How do you convert a Buffer to a string?
126. How do you convert a string to a Buffer?
127. What is character encoding?
128. What encodings does Node.js support?
129. When would you use Buffers in real-world applications?
130. What are common mistakes when working with Buffers?

---

# Core Modules

131. What is the `path` module?
132. How do `path.join()` and `path.resolve()` differ?
133. What is the `os` module used for?
134. What information can you get from the `os` module?
135. What is the `crypto` module?
136. How do you generate a secure random value?
137. How do you hash passwords or data?
138. What is the `zlib` module used for?
139. How do you compress and decompress data?
140. What other built-in Node.js modules do you commonly use?

---

# HTTP, Child Processes & Worker Threads

141. What is the built-in `http` module?
142. How do you create a basic HTTP server using Node.js?
143. How do you handle incoming requests and responses?
144. What is the difference between the `http` module and Express.js?
145. When would you use the native `http` module instead of Express?
146. What are child processes in Node.js?
147. What is the difference between `spawn()`, `exec()`, `execFile()`, and `fork()`?
148. What are Worker Threads?
149. When should you use Worker Threads instead of Child Processes?
150. How do Worker Threads improve CPU-intensive applications?

---

# Performance Optimization

151. How do you improve the performance of a Node.js application?
152. What are the most common performance bottlenecks in Node.js?
153. How do you identify performance issues?
154. What tools do you use to profile a Node.js application?
155. What is the Node.js Inspector?
156. How do you analyze CPU usage in Node.js?
157. How do you analyze memory usage?
158. What causes high memory consumption in Node.js?
159. How do you optimize database queries in Node.js applications?
160. What are common performance optimization techniques for production systems?

---

# Memory Management

161. How does memory management work in Node.js?
162. What is stack memory?
163. What is heap memory?
164. How does V8 garbage collection work?
165. What are memory leaks in Node.js?
166. What are common causes of memory leaks?
167. How do you detect memory leaks?
168. How do closures contribute to memory leaks?
169. How do event listeners cause memory leaks?
170. What best practices help prevent memory leaks?

---

# Scaling Node.js Applications

171. What is clustering in Node.js?
172. Why would you use the Cluster module?
173. How does the Cluster module work?
174. What is load balancing?
175. How do you scale a Node.js application horizontally?
176. What is horizontal scaling?
177. What is vertical scaling?
178. When should you use Worker Threads instead of clustering?
179. How do you manage sessions in a clustered application?
180. What challenges arise when scaling Node.js applications?

---

# Security

181. How do you secure a Node.js application?
182. What are the most common security vulnerabilities in Node.js?
183. How do you prevent SQL Injection?
184. How do you prevent NoSQL Injection?
185. How do you prevent Cross-Site Scripting (XSS)?
186. How do you prevent Cross-Site Request Forgery (CSRF)?
187. How do you securely store passwords?
188. Why should you use environment variables for secrets?
189. How do you validate and sanitize user input?
190. What authentication and authorization best practices do you follow?

---

# Production & Deployment

191. How do you prepare a Node.js application for production?
192. How do you manage configuration across environments?
193. What logging libraries have you used?
194. What monitoring tools have you used?
195. How do you handle uncaught exceptions?
196. How do you handle unhandled Promise rejections?
197. What is graceful shutdown, and why is it important?
198. How do you deploy a Node.js application using Docker?
199. How do you deploy Node.js applications to cloud platforms such as AWS or DigitalOcean?
200. What production best practices do you follow before releasing a Node.js application?

---

# Project Architecture

201. How do you structure a large Node.js application?
202. What folder structure do you prefer for enterprise Node.js projects?
203. How do you separate business logic from controllers?
204. What is the Service Layer pattern?
205. What is the Repository pattern?
206. What is Dependency Injection (DI)?
207. What are the benefits of Dependency Injection?
208. How do you organize shared utilities and helper functions?
209. How do you manage configuration across environments?
210. What Node.js architecture patterns have you used in production?

---

# API Design

211. What are RESTful APIs?
212. What REST API design principles do you follow?
213. How do you version REST APIs?
214. What HTTP status codes do you commonly use?
215. How do you design consistent API responses?
216. How do you implement pagination?
217. How do you implement filtering and sorting?
218. How do you implement rate limiting?
219. How do you document APIs?
220. What are common REST API design mistakes?

---

# Caching & Messaging

221. What is caching?
222. When would you use Redis?
223. What data should be cached?
224. What cache invalidation strategies have you used?
225. What is a message queue?
226. When would you use RabbitMQ?
227. When would you use Apache Kafka?
228. What are background jobs in Node.js?
229. How do you schedule recurring tasks?
230. When should you use WebSockets instead of REST?

---

# Database & Scalability

231. How do you optimize database performance?
232. How do you handle database transactions?
233. How do you prevent race conditions?
234. How do you manage database connection pooling?
235. How do you scale a backend application?
236. How do you design a high-availability Node.js application?
237. What are the trade-offs between a monolith and microservices?
238. When would you choose microservices?
239. How do services communicate in a microservices architecture?
240. What challenges have you faced while scaling backend systems?

---

# Senior Real-World Interview Questions

241. Describe the largest Node.js application you've worked on.
242. What was the most difficult backend bug you've fixed?
243. How do you debug production issues in Node.js?
244. How do you review backend pull requests?
245. What coding standards do you enforce in your team?
246. How do you mentor junior backend developers?
247. If you joined a new project, how would you evaluate the existing Node.js codebase?
248. If you were building a production SaaS today, what backend architecture would you choose and why?
249. What best practices do you always follow in production Node.js applications?
250. In your opinion, what separates a junior, mid-level, and senior Node.js developer?

---

# ANSWERS


---

## Part 1 (1â€“10): Introduction

---

## Question 1: What is Node.js?

## Answer:
Node.js is a JavaScript runtime built on Chrome's V8 engine that lets you run JavaScript on the server side. Before Node.js, JavaScript only ran in browsers. Node.js took the V8 engine out of Chrome and paired it with a set of APIs for file system access, networking, and process management â€” making JavaScript a full-stack language.

I use it for building REST APIs, real-time applications, microservices, and CLI tools. It's the backbone of most modern full-stack JavaScript applications.

## Key Points:
- JavaScript runtime built on Chrome's V8 engine.
- Enables server-side JavaScript execution.
- Event-driven, non-blocking I/O model.
- Built-in modules for file system, networking, and process management.
- npm ecosystem with over 2 million packages.

## Interview Tip:
Don't just say "it runs JavaScript on the server." Mention the event-driven, non-blocking model â€” that's what makes Node.js unique compared to other server runtimes.

---

## Question 2: Why was Node.js created?

## Answer:
Ryan Dahl created Node.js in 2009 to solve a specific problem: handling thousands of concurrent connections efficiently. Traditional server frameworks like Apache used a thread-per-request model â€” each connection needed its own thread, which consumed a lot of memory. Node.js used an event-driven, non-blocking model that could handle many connections on a single thread.

The goal was to build I/O-heavy applications (chat servers, streaming, APIs) that could scale without the overhead of threads.

## Key Points:
- Created to handle concurrent I/O efficiently.
- Event-driven model replaces thread-per-request.
- Single-threaded but non-blocking.
- Designed for I/O-heavy workloads.
- Made JavaScript a server-side language.

## Interview Tip:
Mention the thread-per-request problem â€” it shows you understand WHY Node.js was created, not just WHAT it does.

---

## Question 3: What problems does Node.js solve?

## Answer:
- **Concurrency**: Handles thousands of simultaneous connections without threads.
- **Full-stack JavaScript**: Same language on client and server â€” shared code, types, and tooling.
- **I/O performance**: Non-blocking I/O is perfect for APIs, real-time apps, and streaming.
- **Developer productivity**: Fast iteration, huge ecosystem, rich tooling.
- **Scalability**: Lightweight processes scale horizontally easily.

## Key Points:
- Concurrency without thread overhead.
- Full-stack JavaScript reduces context switching.
- Non-blocking I/O for high-throughput applications.
- Massive npm ecosystem for rapid development.
- Lightweight and scalable.

## Interview Tip:
"Node.js solved the C10K problem â€” handling 10,000 concurrent connections efficiently."

---

## Question 4: How does Node.js differ from browser JavaScript?

## Answer:
| Feature | Browser JS | Node.js |
|---------|-----------|---------|
| Environment | Browser | Server/terminal |
| APIs | DOM, fetch, localStorage | fs, http, process, Buffer |
| Global object | `window` | `global` / `globalThis` |
| Module system | ES Modules | CommonJS + ESM |
| File system | Not available | Full access |
| Network | fetch API | http/https modules |

Both use the V8 engine and JavaScript language, but the APIs available are completely different.

## Key Points:
- Same language (JavaScript), different APIs.
- Browser: DOM manipulation, fetch, Web Storage.
- Node.js: File system, HTTP servers, process management.
- Node.js has full system access; browsers are sandboxed.
- Global objects differ (`window` vs `global`).

## Interview Tip:
"Same JavaScript, different playgrounds. Browser JS manipulates the DOM; Node.js manipulates the file system and network."

---

## Question 5: What are the advantages of Node.js?

## Answer:
- **Fast**: V8 engine compiles JavaScript to machine code.
- **Non-blocking I/O**: Handles thousands of concurrent connections.
- **Single language**: JavaScript on frontend and backend.
- **Huge ecosystem**: 2 million+ packages on npm.
- **Active community**: Large community, extensive documentation.
- **Lightweight**: Minimal resource usage per connection.
- **Cross-platform**: Runs on Windows, macOS, Linux.

## Key Points:
- V8 engine provides near-native performance.
- Event-driven model enables high concurrency.
- Full-stack JavaScript reduces development overhead.
- npm is the largest package registry.
- Excellent for I/O-heavy applications.

## Interview Tip:
Be specific about advantages. "Non-blocking I/O means I can handle 10,000 concurrent connections with minimal memory usage."

---

## Question 6: What are the disadvantages of Node.js?

## Answer:
- **CPU-intensive tasks**: Single-threaded, so heavy computation blocks the event loop.
- **Callback hell**: Deeply nested callbacks were common (async/await solved this).
- **Immature ecosystem**: Some packages are poorly maintained or abandoned.
- **Single-threaded limitations**: Can't leverage multiple cores without clustering.
- **Callback-based APIs**: Some core modules still use callbacks.
- **Not ideal for all tasks**: Not great for CPU-heavy processing like video encoding.

## Key Points:
- CPU-bound tasks block the event loop.
- Single-threaded nature limits multi-core usage.
- Some npm packages are low quality.
- Not suitable for CPU-intensive workloads.
- Worker Threads solve some CPU-bound issues.

## Interview Tip:
Honesty about disadvantages shows maturity. "Node.js isn't perfect â€” I wouldn't use it for a video processing server."

---

## Question 7: What is the V8 JavaScript engine?

## Answer:
V8 is Google's open-source JavaScript engine that compiles JavaScript to machine code. It's the engine inside Chrome and Node.js. V8 uses JIT (Just-In-Time) compilation â€” it compiles JavaScript to optimized machine code at runtime, which is why JavaScript runs much faster than interpreted languages.

V8 also implements the ECMAScript specification, garbage collection, and memory management.

## Key Points:
- Google's JavaScript engine, used in Chrome and Node.js.
- JIT compilation for near-native performance.
- Implements ECMAScript and WebAssembly.
- garbage collection for automatic memory management.
- Written in C++.

## Interview Tip:
"V8 is why Node.js is fast â€” it compiles JavaScript to machine code instead of interpreting it."

---

## Question 8: How does the V8 engine work?

## Answer:
V8 works in stages:
1. **Parsing**: JavaScript source code is parsed into an Abstract Syntax Tree (AST).
2. **Compilation**: The Ignition interpreter generates bytecode from the AST.
3. **Optimization**: The TurboFan optimizing compiler identifies hot code and compiles it to optimized machine code.
4. **Deoptimization**: If assumptions are violated, V8 falls back to bytecode.

This tiered compilation approach gives V8 both fast startup and high peak performance.

## Key Points:
- Parsing â†’ AST â†’ bytecode â†’ optimized machine code.
- Ignition interpreter for fast startup.
- TurboFan optimizing compiler for hot code.
- Deoptimization when assumptions are violated.
- JIT compilation happens at runtime.

## Interview Tip:
Mention the tiered approach â€” "V8 starts fast with bytecode, then optimizes hot code paths with TurboFan."

---

## Question 9: Why is Node.js considered fast?

## Answer:
Three reasons:
1. **V8 engine**: JIT compilation to machine code.
2. **Non-blocking I/O**: Doesn't wait for operations â€” handles thousands of concurrent connections.
3. **Event-driven architecture**: Single thread handles all I/O without context switching overhead.

For I/O-bound tasks, Node.js is extremely fast. For CPU-bound tasks, it can be slower than multi-threaded languages.

## Key Points:
- V8 JIT compilation for fast code execution.
- Non-blocking I/O eliminates waiting.
- Event-driven architecture avoids thread overhead.
- Fast for I/O-bound tasks, not CPU-bound tasks.
- Lightweight processes for high concurrency.

## Interview Tip:
"Node.js is fast for I/O â€” it can handle thousands of simultaneous database queries without breaking a sweat."

---

## Question 10: Is Node.js single-threaded or multi-threaded?

## Answer:
Node.js is single-threaded for JavaScript execution but uses multiple threads under the hood:
- **JavaScript execution**: Single-threaded (event loop).
- **libuv thread pool**: Multi-threaded for file system, DNS, and crypto operations (4 threads by default).
- **Worker Threads**: Optional multi-threading for CPU-intensive work.

The event loop is single-threaded, which makes programming simpler. But I/O operations are offloaded to background threads by libuv.

## Key Points:
- JavaScript execution is single-threaded.
- libuv provides a thread pool for I/O operations.
- Worker Threads allow true multi-threading.
- Single-threaded event loop simplifies concurrent programming.
- Clustering allows multiple processes for multi-core usage.

## Interview Tip:
"Single-threaded for JavaScript, multi-threaded for I/O. The event loop handles concurrency; libuv handles the heavy lifting."

---

## Part 2 (11â€“20): Architecture

---

## Question 11: How does Node.js handle multiple requests?

## Answer:
Node.js uses a single-threaded event loop with non-blocking I/O. When a request arrives, it's placed on the event loop. If the request requires I/O (database query, file read), Node.js delegates it to the libuv thread pool and continues processing other requests. When the I/O completes, a callback is placed on the event loop to handle the result.

This means Node.js can handle thousands of concurrent requests without spawning a new thread for each one.

## Key Points:
- Single event loop processes all requests.
- I/O operations are offloaded to the thread pool.
- Non-blocking â€” the event loop never waits.
- Callbacks handle results when I/O completes.
- Much more memory-efficient than thread-per-request.

## Interview Tip:
"Node.js doesn't block on I/O â€” it moves on to the next request and handles the result later via callbacks."

---

## Question 12: What is event-driven architecture?

## Answer:
Event-driven architecture means the program responds to events rather than following a linear sequence. Objects emit events, and listeners react to those events. In Node.js, everything is built on this pattern â€” HTTP requests, file operations, and stream data all emit events.

```js
const EventEmitter = require("events");
const emitter = new EventEmitter();
emitter.on("data", (chunk) => console.log(chunk));
emitter.emit("data", "hello");
```

## Key Points:
- Components communicate through events.
- Emitters produce events; listeners consume them.
- Decouples producers from consumers.
- Foundation of Node.js's core modules (http, streams, fs).
- Enables non-blocking, asynchronous programming.

## Interview Tip:
"Event-driven architecture decouples components â€” the emitter doesn't need to know who's listening."

---

## Question 13: What is non-blocking I/O?

## Answer:
Non-blocking I/O means the program doesn't wait for an operation to complete before moving on. When Node.js starts a file read or database query, it registers a callback and immediately continues executing the next line of code. When the I/O completes, the callback is invoked.

This is different from blocking I/O, where the program waits (blocks) until the operation finishes.

## Key Points:
- The program continues executing while I/O runs in the background.
- Callbacks handle results when operations complete.
- Enables high concurrency without threads.
- The event loop polls for completed I/O operations.
- Essential for scalable server applications.

## Interview Tip:
"Non-blocking I/O is why Node.js can handle 10,000 concurrent connections â€” it never waits for anything."

---

## Question 14: What is asynchronous I/O?

## Answer:
Asynchronous I/O is non-blocking I/O with callbacks, promises, or async/await. The operation starts, the program continues, and when the operation finishes, the result is delivered via a callback, resolved promise, or awaited value.

```js
// Asynchronous â€” doesn't block
fs.readFile("file.txt", (err, data) => {
  console.log(data); // Runs when file is read
});
console.log("This runs immediately");
```

## Key Points:
- Operations complete in the background.
- Results delivered via callbacks, promises, or async/await.
- The event loop manages the execution order.
- Essential for I/O-heavy applications.
- Non-blocking by nature.

## Interview Tip:
"Asynchronous means 'start now, finish later.' The event loop handles the timing."

---

## Question 15: What is synchronous I/O?

## Answer:
Synchronous I/O blocks the event loop until the operation completes. The program waits and can't do anything else until the I/O finishes.

```js
// Synchronous â€” blocks the event loop
const data = fs.readFileSync("file.txt"); // Waits here
console.log(data); // Only runs after file is read
console.log("This runs AFTER the file read");
```

Synchronous I/O is rarely used in production servers because it blocks all other requests.

## Key Points:
- Blocks the event loop until completion.
- Simple to write and reason about.
- Never use in request handlers â€” blocks all other requests.
- Useful for startup scripts and CLI tools.
- `readFileSync`, `writeFileSync` are synchronous versions.

## Interview Tip:
"Never use synchronous I/O in a server. One blocked request blocks ALL requests."

---

## Question 16: What is the event loop?

## Answer:
The event loop is the core mechanism that allows Node.js to perform non-blocking I/O. It continuously checks if there are any pending callbacks, timers, or I/O events to process. When the call stack is empty, the event loop picks the next callback from the appropriate queue and executes it.

The event loop runs in phases: timers, pending callbacks, idle/prepare, poll, check, and close callbacks.

## Key Points:
- Continuously runs checking for pending work.
- Processes callbacks from different queues in order.
- Enables non-blocking I/O on a single thread.
- Has distinct phases for different types of callbacks.
- Never blocks â€” always moving to the next task.

## Interview Tip:
"The event loop is the heartbeat of Node.js â€” it never stops, always checking for the next thing to do."

---

## Question 17: What are callbacks?

## Answer:
Callbacks are functions passed as arguments to other functions, to be executed when an asynchronous operation completes. They were the original way to handle async operations in Node.js.

```js
fs.readFile("file.txt", (err, data) => {
  if (err) throw err;
  console.log(data);
});
```

Callbacks can lead to "callback hell" when deeply nested, which is why Promises and async/await were introduced.

## Key Points:
- Functions passed as arguments to async operations.
- Called when the operation completes.
- Can lead to callback hell (deeply nested callbacks).
- Still used in some core Node.js APIs.
- Promises and async/await are preferred.

## Interview Tip:
"Callbacks are the foundation, but async/await is the modern approach. Know both."

---

## Question 18: What are Promises?

## Answer:
Promises represent the eventual completion or failure of an asynchronous operation. They provide `.then()` for success, `.catch()` for errors, and `.finally()` for cleanup.

```js
fetchUser(id)
  .then(user => fetchPosts(user.id))
  .then(posts => console.log(posts))
  .catch(err => console.error(err));
```

Promises eliminate callback hell by chaining, and they're the foundation for async/await.

## Key Points:
- Represent eventual completion or failure.
- Three states: pending, fulfilled, rejected.
- Chainable with `.then()` and `.catch()`.
- Foundation for async/await.
- `Promise.all()`, `Promise.race()` for concurrent operations.

## Interview Tip:
"Promises flattened callback hell into a chainable, readable pattern."

---

## Question 19: What is async/await?

## Answer:
Async/await is syntactic sugar over Promises that makes asynchronous code look and feel synchronous. `async` functions always return Promises, and `await` pauses execution until a Promise resolves.

```js
async function getUser(id) {
  const user = await db.user.findUnique({ where: { id } });
  const posts = await db.post.findMany({ where: { userId: id } });
  return { user, posts };
}
```

Error handling uses standard `try/catch`.

## Key Points:
- Syntactic sugar over Promises.
- `async` functions return Promises.
- `await` pauses until Promise resolves.
- `try/catch` for error handling.
- Makes async code readable and maintainable.

## Interview Tip:
"Async/await made async code readable. It's the modern standard â€” use it everywhere."

---

## Question 20: What makes Node.js scalable?

## Answer:
- **Non-blocking I/O**: Handles thousands of connections without threads.
- **Lightweight processes**: Minimal memory per connection.
- **Event-driven architecture**: No thread context switching overhead.
- **Clustering**: Can use multiple CPU cores.
- **Horizontal scaling**: Easy to add more instances behind a load balancer.

Node.js scales horizontally (more machines) rather than vertically (more CPU per machine).

## Key Points:
- Non-blocking I/O enables high concurrency.
- Lightweight memory footprint per connection.
- Clustering for multi-core usage.
- Horizontal scaling with load balancers.
- Designed for distributed, scalable systems.

## Interview Tip:
"Node.js scales by adding more instances, not more threads. Horizontal scaling is the Node.js way."

---

## Part 3 (21â€“30): Global Objects

---

## Question 21: What is the `global` object?

## Answer:
The `global` object in Node.js is the equivalent of `window` in browsers. It contains all global variables, functions, and modules. Anything attached to `global` is accessible from anywhere in the application without importing.

```js
global.myVar = "hello";
console.log(myVar); // "hello" â€” accessible everywhere
```

Avoid polluting the global object â€” it causes conflicts and makes code hard to reason about.

## Key Points:
- Node.js equivalent of browser's `window`.
- Global variables and functions live here.
- Avoid polluting it â€” use modules instead.
- `globalThis` is the modern, cross-platform way to access it.
- Process, console, Buffer, and other globals live here.

## Interview Tip:
"Think of `global` as the Node.js version of `window`. But unlike browsers, keep it clean â€” modules are the right way to share state."

---

## Question 22: What is `globalThis`?

## Answer:
`globalThis` is a standardized way to access the global object across all JavaScript environments â€” browser (`window`), Node.js (`global`), and web workers (`self`). It was introduced in ES2020.

```js
// Works in all environments
globalThis.myVar = "hello";
```

In Node.js, `globalThis === global`. In browsers, `globalThis === window`.

## Key Points:
- Standardized global object access across environments.
- `globalThis === global` in Node.js.
- `globalThis === window` in browsers.
- Introduced in ES2020 for cross-platform code.
- Use `globalThis` when writing isomorphic code.

## Interview Tip:
"`globalThis` is the one true global â€” it works everywhere. Use it when writing code that runs in both Node.js and browsers."

---

## Question 23: What is the `process` object?

## Answer:
The `process` object provides information about and control over the current Node.js process. It's a global object available everywhere.

Common uses:
```js
process.env.NODE_ENV // Environment variables
process.cwd()        // Current working directory
process.argv         // Command-line arguments
process.exit(0)      // Exit the process
process.pid          // Process ID
process.memoryUsage() // Memory usage info
```

## Key Points:
- Global object representing the current process.
- Access environment variables, arguments, and PID.
- Control process lifecycle (exit, signal handling).
- Get system information (memory, uptime).
- Handle process-level events (exit, uncaughtException).

## Interview Tip:
"`process.env` is the most commonly used part â€” it's how you access environment variables in Node.js."

---

## Question 24: What is the `Buffer` object?

## Answer:
Buffers handle binary data in Node.js. Since JavaScript was designed for text, Node.js introduced Buffers to work with raw binary data â€” file contents, network packets, images, and cryptographic operations.

```js
// Create a buffer from a string
const buf = Buffer.from("hello");
console.log(buf); // <Buffer 68 65 6c 6c 6f>

// Create an empty buffer of 10 bytes
const empty = Buffer.alloc(10);
```

## Key Points:
- Handles binary data in Node.js.
- Fixed-size memory allocation.
- Created from strings, arrays, or allocated empty.
- Converts between binary and text with encoding.
- Used for file I/O, networking, and crypto.

## Interview Tip:
"Buffers are Node.js's way of dealing with binary data â€” images, file contents, and network packets."

---

## Question 25: What is the `console` object?

## Answer:
The `console` object provides logging functionality. It's globally available in Node.js and outputs to `stdout` (standard output) or `stderr` (standard error).

```js
console.log("Info message");      // stdout
console.error("Error message");   // stderr
console.warn("Warning message");  // stderr
console.time("timer");
// ... code ...
console.timeEnd("timer");         // prints elapsed time
```

In production, use a logging library (Winston, Pino) instead of `console.log`.

## Key Points:
- Globally available logging utility.
- `log` outputs to stdout, `error`/`warn` to stderr.
- `time`/`timeEnd` for performance measurement.
- `table` for tabular data display.
- Use structured logging (Winston/Pino) in production.

## Interview Tip:
"`console.log` is fine for development. In production, use structured logging with Winston or Pino."

---

## Question 26: What is `__dirname`?

## Answer:
`__dirname` is a Node.js variable that holds the directory path of the current module file. It's only available in CommonJS modules.

```js
const path = require("path");
console.log(__dirname); // e.g., /home/user/project/src
console.log(path.join(__dirname, "config", "db.json"));
```

In ES Modules, use `import.meta.dirname` (Node.js 21+) or `path.dirname(fileURLToPath(import.meta.url))`.

## Key Points:
- Directory path of the current module file.
- Only available in CommonJS modules.
- Use `import.meta.dirname` in ES Modules.
- Essential for resolving file paths relative to the module.
- Always use `path.join()` for cross-platform paths.

## Interview Tip:
"`__dirname` doesn't exist in ES Modules â€” use `import.meta.dirname` instead. This is a common gotcha."

---

## Question 27: What is `__filename`?

## Answer:
`__filename` is a Node.js variable that holds the full file path of the current module. It's only available in CommonJS modules.

```js
console.log(__filename); // e.g., /home/user/project/src/server.js
```

In ES Modules, use `import.meta.filename` or construct it from `import.meta.url`.

## Key Points:
- Full file path of the current module.
- Only available in CommonJS modules.
- Use `import.meta.filename` in ES Modules.
- Useful for logging and debugging.
- Always use `path.join()` when combining with other paths.

## Interview Tip:
"`__filename` and `__dirname` are CommonJS-only. ES Modules use `import.meta` instead."

---

## Question 28: What is `process.cwd()`?

## Answer:
`process.cwd()` returns the current working directory of the Node.js process. This is the directory from which you ran the `node` command, not necessarily the directory where the script file lives.

```js
console.log(process.cwd()); // e.g., /home/user/project
```

This is different from `__dirname` â€” `process.cwd()` is where you ran the command; `__dirname` is where the file is.

## Key Points:
- Returns the directory where the Node process was started.
- Different from `__dirname` (which is the file's directory).
- Can be changed with `process.chdir()`.
- Useful for resolving relative paths from the command line.
- Commonly used in configuration and CLI tools.

## Interview Tip:
"`process.cwd()` â‰  `__dirname`. The former is where you ran the command; the latter is where the file is."

---

## Question 29: What is `process.env`?

## Answer:
`process.env` is an object containing the current environment variables. It's how Node.js accesses configuration values, secrets, and environment-specific settings.

```js
const dbUrl = process.env.DATABASE_URL;
const port = process.env.PORT || 3000;
const isProd = process.env.NODE_ENV === "production";
```

Use `.env` files with `dotenv` package in development, and set real environment variables in production.

## Key Points:
- Object containing all environment variables.
- Access secrets, config, and environment flags.
- Use `dotenv` to load `.env` files in development.
- Never commit `.env` files to git.
- All values are strings â€” parse numbers and booleans.

## Interview Tip:
"`process.env` values are always strings. `process.env.PORT` is `"3000"`, not `3000`. Parse with `Number()`."

---

## Question 30: What is `process.argv`?

## Answer:
`process.argv` is an array containing the command-line arguments passed to the Node.js process.

```bash
node server.js --port 3000 --verbose
```

```js
console.log(process.argv);
// ["node", "server.js", "--port", "3000", "--verbose"]

const port = process.argv[2]; // "--port" â€” not useful as-is
```

For complex CLI argument parsing, use libraries like `yargs` or `commander`.

## Key Points:
- Array of command-line arguments.
- First two elements: `node` executable and script path.
- Remaining elements: user-provided arguments.
- All values are strings.
- Use `yargs` or `commander` for complex CLI parsing.

## Interview Tip:
"For anything beyond simple flags, use `yargs` or `commander`. Parsing `process.argv` manually is error-prone."

---

## Part 4 (31â€“40): Modules

---

## Question 31: What is a module in Node.js?

## Answer:
A module is a reusable piece of JavaScript code that encapsulates related functionality. Node.js uses the module system to organize code, share functionality between files, and maintain separation of concerns.

Each file in Node.js is treated as a separate module. You export functionality from one module and import it in another.

## Key Points:
- Each file is a module in Node.js.
- Modules encapsulate related functionality.
- Export and import to share between files.
- Prevents global namespace pollution.
- Two module systems: CommonJS and ES Modules.

## Interview Tip:
"Modules are the building blocks of Node.js applications â€” they keep code organized and reusable."

---

## Question 32: What are CommonJS modules?

## Answer:
CommonJS (CJS) is Node.js's original module system. It uses `require()` to import and `module.exports` to export. It's synchronous and loads modules at runtime.

```js
// Exporting
module.exports = { createUser, findUser };

// Importing
const { createUser, findUser } = require("./users");
```

CommonJS is still the default in Node.js, though ES Modules are becoming more common.

## Key Points:
- Node.js's original module system.
- `require()` for importing, `module.exports` for exporting.
- Synchronous module loading.
- Each module is wrapped in a function (module wrapper).
- Still the default in Node.js.

## Interview Tip:
"CommonJS is synchronous â€” `require()` blocks execution until the module is loaded. ES Modules are asynchronous."

---

## Question 33: What are ES Modules (ESM)?

## Answer:
ES Modules (ESM) is the official JavaScript module system standardized in ES2015. It uses `import` and `export` syntax. In Node.js, you enable ESM by adding `"type": "module"` to `package.json` or using `.mjs` file extensions.

```js
// Exporting
export function createUser() { /* ... */ }
export default class UserService { /* ... */ }

// Importing
import { createUser } from "./users.js";
import UserService from "./users.js";
```

## Key Points:
- Official JavaScript module system (ES2015).
- `import`/`export` syntax.
- Asynchronous module loading.
- Enable with `"type": "module"` in package.json.
- Static analysis enables tree-shaking.

## Interview Tip:
"ES Modules are the future â€” static imports enable tree-shaking and better optimization."

---

## Question 34: What is the difference between CommonJS and ESM?

## Answer:
| Feature | CommonJS | ES Modules |
|---------|----------|------------|
| Syntax | `require()` / `module.exports` | `import` / `export` |
| Loading | Synchronous | Asynchronous |
| Resolution | Runtime | Static (compile-time) |
| Tree-shaking | No | Yes |
| Async | No | Top-level `await` |
| File extension | `.js` | `.mjs` or `"type": "module"` |

ESM is the standard going forward, but CommonJS is still widely used.

## Key Points:
- CommonJS: synchronous, runtime resolution, no tree-shaking.
- ESM: asynchronous, static resolution, enables tree-shaking.
- ESM supports top-level `await`.
- Both work in Node.js â€” they can coexist.
- ESM is the official JavaScript standard.

## Interview Tip:
"ESM enables tree-shaking because imports are static â€” the bundler knows what to include at compile time."

---

## Question 35: What is `require()`?

## Answer:
`require()` is CommonJS's function for importing modules. It's synchronous and loads the module at runtime.

```js
const fs = require("fs");           // Built-in module
const express = require("express"); // npm package
const users = require("./users");   // Local file
```

`require()` caches modules â€” the second `require()` of the same module returns the cached export.

## Key Points:
- Synchronous module loading.
- Resolves built-in modules, npm packages, and local files.
- Caches modules after first load.
- Can be used conditionally (inside if blocks).
- Returns `module.exports` of the required module.

## Interview Tip:
"`require()` is synchronous â€” it blocks execution until the module is loaded. Use dynamic `import()` for async loading."

---

## Question 36: What is `module.exports`?

## Answer:
`module.exports` is how CommonJS modules export functionality. You assign values to `module.exports` to make them available to other modules.

```js
// Named exports via object
module.exports = { createUser, findUser };

// Single export
module.exports = class UserService { /* ... */ };
```

When another module does `require("./file")`, it gets whatever `module.exports` points to.

## Key Points:
- Default export object for CommonJS modules.
- Assign functions, classes, or values to export them.
- `require()` returns the `module.exports` object.
- Can be replaced entirely or have properties added.

## Interview Tip:
"`module.exports` and `exports` are the same object initially â€” but reassigning `exports` breaks the link."

---

## Question 37: What is `exports`?

## Answer:
`exports` is a shortcut for `module.exports`. It starts as the same object reference, so adding properties to `exports` also adds them to `module.exports`.

```js
exports.createUser = () => { /* ... */ }; // Works
exports.findUser = () => { /* ... */ };   // Works

// But reassigning breaks it:
exports = { createUser }; // Broken! module.exports is unchanged
```

Always use `module.exports` for reassignment. Use `exports` only for adding individual properties.

## Key Points:
- `exports` is a shorthand for `module.exports`.
- Adding properties works fine.
- Reassigning `exports` breaks the link â€” avoid it.
- Prefer `module.exports` for clarity.
- Both are available in every CommonJS module.

## Interview Tip:
"`exports` is a convenience alias. If you need to reassign, use `module.exports` directly."

---

## Question 38: What is the `import` statement?

## Answer:
The `import` statement is ESM syntax for importing modules. It's static â€” the import is resolved at parse time, not runtime.

```js
import { createUser } from "./users.js";
import UserService from "./users.js";        // Default import
import * as utils from "./utils.js";         // Namespace import
import("./dynamic-module.js").then(mod => {}); // Dynamic import
```

Static imports enable tree-shaking. Dynamic `import()` loads modules on demand.

## Key Points:
- Static imports resolved at parse time.
- Supports named, default, and namespace imports.
- Dynamic `import()` for lazy loading.
- Enables tree-shaking in bundlers.
- Must be at the top level (not inside conditionals).

## Interview Tip:
"Static `import` is for most cases. Dynamic `import()` is for conditional or lazy loading."

---

## Question 39: What is the `export` statement?

## Answer:
The `export` statement is ESM syntax for exporting functionality from a module.

```js
// Named exports
export function createUser() { /* ... */ }
export const API_URL = "https://api.example.com";

// Default export
export default class UserService { /* ... */ }

// Re-export
export { createUser } from "./users.js";
```

Named exports are imported by name; default exports are imported without a name.

## Key Points:
- Named exports: exported by name, imported by name.
- Default export: one per module, imported without braces.
- Re-exports: forward exports from other modules.
- Static analysis enables tree-shaking.

## Interview Tip:
"Named exports are better for tree-shaking â€” bundlers can determine exactly which exports are used."

---

## Question 40: How does Node.js cache modules?

## Answer:
Node.js caches modules after the first `require()` call. Subsequent `require()` calls for the same module return the cached export without re-executing the module code.

```js
// First call: loads and executes the module
const users = require("./users");
// Second call: returns cached export (module code doesn't run again)
const users2 = require("./users");
console.log(users === users2); // true
```

This means module-level code (like database connections) runs only once.

## Key Points:
- Modules are cached after first `require()`.
- Cached by resolved file path.
- Module-level code executes only once.
- `require.cache` contains the cache (can be cleared).
- ES Modules also cache, but with different semantics.

## Interview Tip:
"The module cache is why database connections at module level are created once â€” `require()` returns the same export every time."

---

## Part 5 (41â€“50): npm & Packages

---

## Question 41: What is npm?

## Answer:
npm (Node Package Manager) is the default package manager for Node.js. It's a registry of over 2 million open-source packages and a command-line tool for installing, managing, and publishing packages.

```bash
npm init                  # Initialize a new project
npm install express       # Install a package
npm install -D jest        # Install a dev dependency
npm run build             # Run a script
npm publish               # Publish a package
```

## Key Points:
- Default package manager for Node.js.
- 2 million+ packages on the registry.
- `package.json` defines project dependencies.
- `node_modules/` stores installed packages.
- Alternative package managers: yarn, pnpm, bun.

## Interview Tip:
"npm is the most popular package manager, but I've also used yarn and pnpm â€” pnpm is great for monorepos."

---

## Question 42: What is `package.json`?

## Answer:
`package.json` is the manifest file for a Node.js project. It defines metadata (name, version, description), dependencies, scripts, and configuration.

```json
{
  "name": "my-app",
  "version": "1.0.0",
  "scripts": {
    "dev": "node --watch src/server.js",
    "build": "tsc",
    "start": "node dist/server.js",
    "test": "jest"
  },
  "dependencies": { "express": "^4.18.0" },
  "devDependencies": { "jest": "^29.0.0" }
}
```

## Key Points:
- Project manifest: metadata, dependencies, scripts.
- `dependencies`: production packages.
- `devDependencies`: development-only packages.
- `scripts`: custom commands you can run.
- Created with `npm init`.

## Interview Tip:
"The `scripts` section is your project's command center â€” `dev`, `build`, `start`, `test` are the standard ones."

---

## Question 43: What is `package-lock.json`?

## Answer:
`package-lock.json` locks the exact versions of all dependencies and their sub-dependencies. It ensures that every `npm install` produces the same `node_modules` tree, regardless of when it runs.

Without it, `^4.18.0` might resolve to `4.18.2` today and `4.19.0` next week â€” potentially introducing bugs.

## Key Points:
- Locks exact dependency versions.
- Ensures reproducible installs across environments.
- Auto-generated by npm.
- Commit to version control.
- Prevents "works on my machine" issues.

## Interview Tip:
"Always commit `package-lock.json`. It ensures every developer and CI/CD pipeline installs identical dependencies."

---

## Question 44: What is the purpose of the `node_modules` folder?

## Answer:
`node_modules/` contains all installed npm packages and their dependencies. When you run `npm install`, npm downloads packages from the registry and stores them here.

It can be extremely large â€” thousands of files and hundreds of megabytes. That's why you never commit it to git â€” regenerate it with `npm install`.

## Key Points:
- Stores all installed npm packages.
- Generated by `npm install` â€” never commit to git.
- Can be very large (hundreds of MB).
- Add `node_modules/` to `.gitignore`.
- Regenerate with `npm install` from `package-lock.json`.

## Interview Tip:
"`node_modules` is the largest folder in most Node.js projects â€” that's why `.gitignore` exists."

---

## Question 45: What is semantic versioning (SemVer)?

## Answer:
SemVer uses a three-part version number: `MAJOR.MINOR.PATCH` (e.g., `4.18.2`).

- **MAJOR**: Breaking changes (4.0.0 â†’ 5.0.0).
- **MINOR**: New features, backward-compatible (4.18.0 â†’ 4.19.0).
- **PATCH**: Bug fixes, backward-compatible (4.18.0 â†’ 4.18.1).

The `^` and `~` prefixes in `package.json` control version ranges:
- `^4.18.0`: allows patches and minors (4.18.x, 4.19.x).
- `~4.18.0`: allows only patches (4.18.x).

## Key Points:
- MAJOR.MINOR.PATCH format.
- MAJOR = breaking, MINOR = features, PATCH = fixes.
- `^` allows minor and patch updates.
- `~` allows only patch updates.
- `package-lock.json` pins exact versions.

## Interview Tip:
"`^4.18.0` can introduce breaking changes in minor versions (rare but possible). `package-lock.json` prevents surprises."

---

## Question 46: What is the difference between dependencies and devDependencies?

## Answer:
- **dependencies**: Packages needed in production (Express, Prisma, React).
- **devDependencies**: Packages needed only in development (Jest, TypeScript, ESLint).

```json
{
  "dependencies": { "express": "^4.18.0" },
  "devDependencies": { "jest": "^29.0.0", "typescript": "^5.0.0" }
}
```

`npm install` installs both. `npm install --production` installs only dependencies.

## Key Points:
- `dependencies`: needed in production.
- `devDependencies`: needed only in development/testing.
- `npm install --production` skips devDependencies.
- Testing frameworks, linters, and build tools are devDependencies.
- Frameworks and libraries are dependencies.

## Interview Tip:
"If the package isn't needed in production, it's a devDependency."

---

## Question 47: What is `npx`?

## Answer:
`npx` is a package runner that comes with npm. It executes npm packages without installing them globally.

```bash
npx create-next-app my-app     # Run without installing
npx prisma migrate dev         # Run project-local binary
npx eslint src/                # Run without global install
```

It's also used to run project-local binaries from `node_modules/.bin/`.

## Key Points:
- Runs npm packages without global installation.
- Executes project-local binaries automatically.
- Avoids global package pollution.
- Can run specific package versions: `npx package@version`.
- Bundled with npm 5.2+.

## Interview Tip:
"`npx` is why you don't need `npm install -g` for most tools. It runs them on demand."

---

## Question 48: How do you update npm packages safely?

## Answer:
1. **Check outdated packages**: `npm outdated`
2. **Update minor/patch**: `npm update` (respects SemVer ranges)
3. **Update to latest**: `npm install package@latest`
4. **Check changelog**: Read the package changelog for breaking changes.
5. **Run tests**: Verify nothing breaks after updating.
6. **Update lock file**: Commit the updated `package-lock.json`.

For major version bumps, test thoroughly before updating.

## Key Points:
- `npm outdated` shows available updates.
- `npm update` updates within SemVer ranges.
- `npm install package@latest` for major updates.
- Always run tests after updating.
- Check changelogs for breaking changes.

## Interview Tip:
"Update strategically â€” minor/patch updates are usually safe. Major updates need testing."

---

## Question 49: How do you handle package vulnerabilities?

## Answer:
1. **Run `npm audit`**: Check for known vulnerabilities.
2. **Fix automatically**: `npm audit fix` (applies safe fixes).
3. **Review manually**: Some fixes require manual intervention.
4. **Update packages**: Vulnerabilities are often fixed in newer versions.
5. **Replace packages**: If a package is abandoned, find an alternative.
6. **Monitor continuously**: Use GitHub Dependabot or Snyk.

## Key Points:
- `npm audit` scans for known vulnerabilities.
- `npm audit fix` applies safe automatic fixes.
- Some vulnerabilities require manual package updates.
- GitHub Dependabot provides automated alerts.
- Snyk offers deeper security scanning.

## Interview Tip:
"I run `npm audit` in CI/CD and block deploys on critical vulnerabilities."

---

## Question 50: What best practices do you follow when managing dependencies?

## Answer:
- **Minimize dependencies**: Don't install a package for something you can write in 10 lines.
- **Check maintenance**: Look at last publish date, open issues, and contributor count.
- **Lock versions**: Always commit `package-lock.json`.
- **Audit regularly**: Run `npm audit` in CI/CD.
- **Update carefully**: Check changelogs before major updates.
- **Pin versions**: For critical dependencies, pin exact versions.
- **Use devDependencies**: Testing and build tools belong in devDependencies.

## Key Points:
- Fewer dependencies = smaller attack surface.
- Check package health before installing.
- Lock file is essential for reproducible builds.
- Regular audits prevent security issues.
- Pin critical dependencies for stability.

## Interview Tip:
"Every dependency is a liability â€” I evaluate the trade-off before adding each one."

---

## Part 6 (51â€“60): Event Loop

---

## Question 51: What is the Node.js Event Loop?

## Answer:
The event loop is Node.js's mechanism for handling asynchronous operations. It continuously checks for pending tasks (callbacks, timers, I/O) and executes them when the call stack is empty. It's what allows Node.js to perform non-blocking I/O on a single thread.

The event loop runs in phases, each processing a specific type of callback.

## Key Points:
- Single-threaded loop that processes asynchronous callbacks.
- Runs continuously until the process exits.
- Each iteration is called a "tick."
- Different phases handle different types of callbacks.
- Enables non-blocking I/O.

## Interview Tip:
"The event loop is what makes Node.js non-blocking â€” it never waits for I/O, always moving to the next task."

---

## Question 52: How does the Event Loop work internally?

## Answer:
The event loop has six phases, executed in order:
1. **Timers**: `setTimeout` and `setInterval` callbacks.
2. **Pending callbacks**: I/O callbacks deferred to the next loop.
3. **Idle/prepare**: Internal use only.
4. **Poll**: Retrieve new I/O events; execute I/O callbacks.
5. **Check**: `setImmediate` callbacks.
6. **Close callbacks**: Close event callbacks (e.g., `socket.on('close')`).

After each phase, the event loop checks for microtasks (Promises, `process.nextTick`) and processes them before moving to the next phase.

## Key Points:
- Six phases executed in order.
- Each phase has its own callback queue.
- Microtasks are processed between phases.
- The loop never blocks â€” always moving forward.
- Each phase delegates to the next when its queue is empty.

## Interview Tip:
"The event loop is a cycle of phases. Microtasks (Promises) run between phases, not within them."

---

## Question 53: Why is the Event Loop important?

## Answer:
The event loop is the reason Node.js can handle thousands of concurrent connections with a single thread. Without it, Node.js would need threads for each connection (like traditional servers). The event loop processes I/O asynchronously, so the thread never blocks.

Understanding the event loop is essential for debugging timing issues, performance bottlenecks, and unexpected behavior.

## Key Points:
- Enables single-threaded concurrency.
- Processes I/O without blocking.
- Essential for understanding Node.js behavior.
- Key to debugging timing-related issues.
- Differentiates Node.js from thread-per-request servers.

## Interview Tip:
"If you understand the event loop, you understand 80% of Node.js. Everything else builds on it."

---

## Question 54: What are the different phases of the Event Loop?

## Answer:
1. **Timers phase**: Executes `setTimeout()` and `setInterval()` callbacks.
2. **Pending callbacks phase**: Executes I/O callbacks deferred from the previous cycle.
3. **Idle/prepare phase**: Internal use only (libuv internals).
4. **Poll phase**: Retrieves new I/O events and executes callbacks. Blocks here if no timers or check callbacks.
5. **Check phase**: Executes `setImmediate()` callbacks.
6. **Close callbacks phase**: Executes close event callbacks (e.g., `socket.on('close')`).

Between each phase, Node.js processes all microtasks.

## Key Points:
- Each phase has a specific callback type.
- The poll phase is where Node.js waits for I/O.
- `setImmediate` runs in the check phase, after poll.
- `setTimeout` runs in the timers phase.
- Microtasks run between every phase.

## Interview Tip:
"The poll phase is the heart of the event loop â€” it's where Node.js spends most of its time waiting for I/O."

---

## Question 55: What happens in the Timers phase?

## Answer:
The timers phase executes callbacks scheduled by `setTimeout()` and `setInterval()`. When the timer's delay has elapsed, its callback is placed in the timers queue and executed during this phase.

Note: `setTimeout(fn, 0)` doesn't execute immediately â€” it schedules the callback for the next timers phase iteration.

## Key Points:
- Executes `setTimeout` and `setInterval` callbacks.
- Timers are checked against the current time.
- `setTimeout(fn, 0)` runs in the next timers phase.
- Timer accuracy depends on system load.
- Multiple timers may batch together.

## Interview Tip:
"`setTimeout(fn, 0)` doesn't mean 'run immediately' â€” it means 'run in the next timers phase.'"

---

## Question 56: What happens in the Pending Callbacks phase?

## Answer:
The pending callbacks phase executes I/O callbacks that were deferred from the previous cycle. This includes some TCP errors and other system-level callbacks. In practice, most developers rarely interact with this phase directly.

## Key Points:
- Executes deferred I/O callbacks from the previous cycle.
- Handles system-level callbacks (TCP errors, etc.).
- Most developers don't interact with this phase directly.
- Part of the normal event loop lifecycle.

## Interview Tip:
"This phase is mostly internal â€” focus on timers, poll, and check for practical understanding."

---

## Question 57: What happens in the Poll phase?

## Answer:
The poll phase has two main responsibilities:
1. Process I/O events that have completed.
2. Block here waiting for new I/O events if there are no timers or `setImmediate` callbacks pending.

If the poll queue is empty:
- If there are `setImmediate` callbacks pending, move to the check phase.
- If there are timers pending, wait until the earliest timer expires, then move to the timers phase.
- Otherwise, poll waits for new I/O events.

## Key Points:
- Processes completed I/O callbacks.
- Blocks waiting for new I/O if nothing else is pending.
- Transitions to check phase if `setImmediate` is pending.
- Transitions to timers phase if timers are pending.
- This is where Node.js waits for new work.

## Interview Tip:
"The poll phase is where Node.js sleeps when there's nothing to do â€” it waits for I/O or timers."

---

## Question 58: What happens in the Check phase?

## Answer:
The check phase executes `setImmediate()` callbacks. `setImmediate` is specifically designed to run after the poll phase, making it useful for executing code after I/O callbacks are processed.

```js
const fs = require("fs");
fs.readFile("file.txt", () => {
  // I/O callback (poll phase)
  setImmediate(() => {
    // Runs in check phase â€” after poll
  });
});
```

## Key Points:
- Executes `setImmediate()` callbacks.
- Runs after the poll phase.
- Useful for code that should run after I/O callbacks.
- `setImmediate` vs `setTimeout(fn, 0)`: `setImmediate` always runs after poll.

## Interview Tip:
"`setImmediate` runs after I/O callbacks. `setTimeout(fn, 0)` runs before I/O callbacks. That's the key difference."

---

## Question 59: What happens in the Close Callbacks phase?

## Answer:
The close callbacks phase handles close event callbacks, like `socket.on('close', ...)`. If a socket is abruptly closed (e.g., `socket.destroy()`), the close event is emitted in this phase.

```js
const server = require("net").createServer();
server.on("connection", (socket) => {
  socket.on("close", () => {
    // This callback runs in the close phase
  });
});
```

## Key Points:
- Handles close event callbacks.
- Runs for abruptly closed sockets and resources.
- Last phase before the loop restarts.
- Important for cleanup logic.

## Interview Tip:
"Close callbacks handle cleanup â€” releasing resources when connections end."

---

## Question 60: What is the difference between the Poll phase and the Check phase?

## Answer:
- **Poll phase**: Processes I/O callbacks and waits for new I/O events. This is where Node.js spends most of its time.
- **Check phase**: Executes `setImmediate()` callbacks. Only runs after the poll phase when `setImmediate` callbacks are pending.

The poll phase is about I/O; the check phase is about executing code after I/O.

```js
// I/O callback runs in poll phase
fs.readFile("file.txt", () => {
  // setImmediate runs in check phase
  setImmediate(() => console.log("check phase"));
});
```

## Key Points:
- Poll: I/O callbacks and waiting for new I/O.
- Check: `setImmediate` callbacks after poll.
- Poll is where Node.js waits; check is what happens after.
- `setImmediate` is specifically tied to the check phase.

## Interview Tip:
"Poll waits for I/O; check runs after I/O. That's the fundamental difference."

---

## Part 7 (61â€“70): Microtasks & Macrotasks

---

## Question 61: What is the Call Stack?

## Answer:
The call stack is a LIFO (Last In, First Out) stack that tracks function execution. When a function is called, it's pushed onto the stack. When it returns, it's popped off. The event loop only processes new callbacks when the call stack is empty.

```js
function a() { b(); }
function b() { c(); }
function c() { console.log("done"); }
a(); // Stack: a â†’ b â†’ c â†’ empty
```

## Key Points:
- LIFO stack tracking function execution.
- Functions are pushed on call, popped on return.
- Only one function executes at a time.
- Event loop checks the stack before processing callbacks.
- Deep recursion can cause stack overflow.

## Interview Tip:
"The call stack is single-threaded â€” only one function runs at a time. The event loop manages what runs next."

---

## Question 62: What is the Callback Queue?

## Answer:
The callback queue (also called the task queue or macrotask queue) stores callbacks from completed asynchronous operations (timers, I/O, etc.). When the call stack is empty, the event loop picks the next callback from this queue and pushes it onto the call stack.

```js
setTimeout(() => console.log("timer"), 0);
console.log("first");
// Output: "first" â†’ "timer"
```

## Key Points:
- Stores completed async operation callbacks.
- Event loop processes it when the call stack is empty.
- Macrotasks include setTimeout, setInterval, I/O callbacks.
- Processed one callback at a time.
- Microtasks have priority over this queue.

## Interview Tip:
"The callback queue is where macrotasks wait. Microtasks get priority and run before macrotasks."

---

## Question 63: What is the Microtask Queue?

## Answer:
The microtask queue stores callbacks from Promises, `queueMicrotask()`, and `process.nextTick()`. Microtasks are processed between event loop phases â€” after the current operation completes and before the next macrotask.

```js
Promise.resolve().then(() => console.log("micro"));
setTimeout(() => console.log("macro"), 0);
console.log("sync");
// Output: "sync" â†’ "micro" â†’ "macro"
```

## Key Points:
- Higher priority than the macrotask queue.
- Processed after each operation and between event loop phases.
- Includes Promise callbacks, `queueMicrotask()`, `process.nextTick()`.
- All microtasks run before the next macrotask.
- Can starve the event loop if microtasks are too many.

## Interview Tip:
"Microtasks always run before macrotasks. That's why Promise callbacks execute before setTimeout callbacks."

---

## Question 64: What is the difference between the Microtask Queue and the Callback Queue?

## Answer:
| Feature | Microtask Queue | Callback Queue (Macrotask) |
|---------|----------------|---------------------------|
| Priority | Higher | Lower |
| Timing | After each operation | After event loop phase |
| Examples | Promise, `queueMicrotask()` | `setTimeout`, I/O, `setImmediate` |
| Processing | All microtasks before next macrotask | One macrotask per loop iteration |

Microtasks are processed greedily â€” all of them run before the next macrotask.

## Key Points:
- Microtasks have higher priority.
- All microtasks run before the next macrotask.
- Microtasks include Promises and `process.nextTick()`.
- Macrotasks include timers and I/O callbacks.
- Overusing microtasks can starve the event loop.

## Interview Tip:
"Microtasks: process all of them. Macrotasks: process one at a time per loop iteration."

---

## Question 65: Which executes first: microtasks or macrotasks?

## Answer:
Microtasks always execute before macrotasks. After the current synchronous code completes, all microtasks are processed first, then the next macrotask is picked from the callback queue.

```js
setTimeout(() => console.log("macrotask"), 0);
Promise.resolve().then(() => console.log("microtask"));
console.log("sync");
// Output: "sync" â†’ "microtask" â†’ "macrotask"
```

## Key Points:
- Microtasks have priority over macrotasks.
- All microtasks run before the next macrotask.
- `process.nextTick()` runs before Promise callbacks.
- Microtasks are processed between event loop phases.

## Interview Tip:
"Synchronous â†’ Microtasks â†’ Macrotasks. That's the execution order."

---

## Question 66: How do Promises interact with the Event Loop?

## Answer:
When a Promise resolves (or rejects), its `.then()` / `.catch()` callback is placed in the microtask queue. The event loop processes it after the current operation completes, before the next macrotask.

```js
const promise = new Promise((resolve) => {
  resolve("done");
});
promise.then((val) => console.log(val)); // Microtask
setTimeout(() => console.log("timeout"), 0); // Macrotask
// Output: "done" â†’ "timeout"
```

## Key Points:
- Promise callbacks are microtasks.
- Processed after current operation, before macrotasks.
- `.then()` callbacks don't execute immediately when resolved.
- Promise chain callbacks are all microtasks.
- `Promise.all()` resolves when all promises resolve.

## Interview Tip:
"Promise callbacks are microtasks â€” they always run before setTimeout and I/O callbacks."

---

## Question 67: How does `queueMicrotask()` work?

## Answer:
`queueMicrotask()` adds a callback to the microtask queue. It runs after the current operation completes and before the next macrotask â€” same timing as Promise callbacks.

```js
queueMicrotask(() => console.log("microtask"));
Promise.resolve().then(() => console.log("promise microtask"));
setTimeout(() => console.log("macrotask"), 0);
// Output: "microtask" â†’ "promise microtask" â†’ "macrotask"
```

## Key Points:
- Adds a callback to the microtask queue.
- Runs after current operation, before macrotasks.
- Same queue as Promise callbacks.
- Useful for running code that needs microtask timing.
- Available in both Node.js and browsers.

## Interview Tip:
"`queueMicrotask()` is the explicit way to add to the microtask queue â€” Promises do it implicitly."

---

## Question 68: How does `process.nextTick()` work?

## Answer:
`process.nextTick()` adds a callback to the "next tick queue" â€” a queue that's processed after the current operation but BEFORE the microtask queue (Promises).

```js
process.nextTick(() => console.log("nextTick"));
Promise.resolve().then(() => console.log("promise"));
setTimeout(() => console.log("timeout"), 0);
// Output: "nextTick" â†’ "promise" â†’ "timeout"
```

`process.nextTick` has the highest priority of all async callbacks.

## Key Points:
- Runs before Promise callbacks (higher priority than microtasks).
- Processed after current operation, before microtasks.
- Node.js-specific â€” not available in browsers.
- Can starve I/O if overused.
- Useful for ensuring callbacks run immediately after the current operation.

## Interview Tip:
"`process.nextTick` > Promises > setTimeout. It's the highest-priority async callback in Node.js."

---

## Question 69: What is the difference between `process.nextTick()` and `Promise.resolve()`?

## Answer:
Both schedule callbacks for the next iteration of the event loop, but `process.nextTick()` runs before Promise callbacks.

```js
process.nextTick(() => console.log("nextTick"));
Promise.resolve().then(() => console.log("promise"));
// Output: "nextTick" â†’ "promise"
```

`process.nextTick` is Node.js-specific. `Promise.resolve().then()` works in all JavaScript environments.

## Key Points:
- `process.nextTick` runs before Promise callbacks.
- `process.nextTick` is Node.js-specific.
- Promise callbacks are portable across environments.
- `process.nextTick` can starve I/O if overused.
- Prefer Promises for portability; `nextTick` for Node.js-specific timing.

## Interview Tip:
"`process.nextTick` is faster than Promises but Node.js-specific. Use Promise callbacks for portable code."

---

## Question 70: Why can overusing `process.nextTick()` cause problems?

## Answer:
`process.nextTick()` callbacks are processed before I/O callbacks. If you keep adding `nextTick` callbacks, the event loop never reaches the I/O phase â€” starving I/O operations, timers, and other callbacks.

```js
// This starves the event loop
function loop() {
  process.nextTick(loop);
}
loop(); // I/O never processes
```

This can cause your server to stop responding to requests.

## Key Points:
- `nextTick` callbacks are processed before I/O.
- Infinite `nextTick` loops starve the event loop.
- I/O callbacks, timers, and `setImmediate` never execute.
- Can cause the server to become unresponsive.
- Use `setImmediate` instead for long-running operations.

## Interview Tip:
"If you need to break up long-running work, use `setImmediate` â€” not `process.nextTick`."

---

## Part 8 (71â€“80): Timers

---

## Question 71: How does `setTimeout()` work?

## Answer:
`setTimeout()` schedules a callback to run after a specified delay (in milliseconds). The callback is placed in the timers queue and executed during the timers phase of the event loop.

```js
setTimeout(() => console.log("after 1 second"), 1000);
console.log("immediately");
// Output: "immediately" â†’ "after 1 second"
```

The delay is a minimum â€” the actual execution depends on the call stack and event loop.

## Key Points:
- Schedules a callback after a delay (ms).
- Callback is placed in the timers queue.
- Delay is a minimum, not a guarantee.
- Returns a timer ID for cancellation.
- `setTimeout(fn, 0)` doesn't execute immediately.

## Interview Tip:
"`setTimeout(fn, 0)` runs after the current code and microtasks â€” not immediately."

---

## Question 72: How does `setInterval()` work?

## Answer:
`setInterval()` repeatedly calls a callback at a specified interval (in milliseconds). It continues until `clearInterval()` is called or the process exits.

```js
let count = 0;
const interval = setInterval(() => {
  console.log(count++);
  if (count >= 5) clearInterval(interval);
}, 1000);
```

Like `setTimeout`, the interval is a minimum â€” not exact.

## Key Points:
- Repeatedly calls a callback at an interval.
- Continues until cleared or process exits.
- Interval is a minimum, not exact.
- Use `clearInterval()` to stop.
- If a callback takes longer than the interval, callbacks stack up.

## Interview Tip:
"If a callback takes longer than the interval, callbacks queue up. Use a flag to prevent overlapping execution."

---

## Question 73: How does `setImmediate()` work?

## Answer:
`setImmediate()` schedules a callback to run after the current poll phase of the event loop. It's useful for executing code after I/O callbacks are processed.

```js
const fs = require("fs");
fs.readFile("file.txt", () => {
  // I/O callback (poll phase)
  setImmediate(() => {
    console.log("runs after I/O callback");
  });
});
```

## Key Points:
- Executes callback after the current poll phase.
- Useful for code that should run after I/O.
- Faster than `setTimeout(fn, 0)` in I/O callbacks.
- Returns a handle for cancellation.
- Only available in Node.js.

## Interview Tip:
"`setImmediate` is faster than `setTimeout(fn, 0)` inside I/O callbacks because it runs in the check phase, not the timers phase."

---

## Question 74: What is the difference between `setImmediate()` and `setTimeout(fn, 0)`?

## Answer:
- `setTimeout(fn, 0)` is placed in the timers queue â€” runs in the timers phase.
- `setImmediate(fn)` is placed in the check queue â€” runs in the check phase.

The execution order depends on context:
- **Outside I/O**: `setTimeout(fn, 0)` usually runs first.
- **Inside I/O**: `setImmediate()` always runs first.

```js
// Outside I/O â€” order is non-deterministic
setTimeout(() => console.log("timeout"), 0);
setImmediate(() => console.log("immediate"));

// Inside I/O â€” setImmediate always runs first
const fs = require("fs");
fs.readFile("file.txt", () => {
  setImmediate(() => console.log("immediate")); // First
  setTimeout(() => console.log("timeout"), 0);  // Second
});
```

## Key Points:
- `setTimeout(fn, 0)`: timers phase.
- `setImmediate`: check phase (after poll).
- Inside I/O, `setImmediate` always runs first.
- Outside I/O, the order is non-deterministic.
- `setImmediate` is generally more predictable.

## Interview Tip:
"Inside I/O callbacks, `setImmediate` is always faster. Outside I/O, the order is unpredictable."

---

## Question 75: When should you use `setImmediate()`?

## Answer:
Use `setImmediate` when you need to defer work until after the current I/O callbacks are processed:
- Breaking up long-running operations without blocking I/O.
- Scheduling work that should run after all I/O callbacks.
- As a more predictable alternative to `setTimeout(fn, 0)`.

```js
const fs = require("fs");
fs.readFile("file.txt", () => {
  // Heavy processing â€” use setImmediate to not block I/O
  setImmediate(() => {
    processData(data);
  });
});
```

## Key Points:
- Defer work until after I/O callbacks.
- Break up long-running operations.
- More predictable than `setTimeout(fn, 0)`.
- Use for CPU-intensive work that shouldn't block I/O.

## Interview Tip:
"`setImmediate` is the Node.js equivalent of 'do this next, after I/O is done.'"

---

## Question 76: How do you cancel a timer?

## Answer:
Both `setTimeout` and `setInterval` return a timer ID. Pass it to `clearTimeout()` or `clearInterval()` to cancel.

```js
const timer = setTimeout(() => {
  console.log("This will never run");
}, 5000);

clearTimeout(timer); // Cancel the timer

const interval = setInterval(() => {
  console.log("Repeated");
}, 1000);

clearInterval(interval); // Stop the interval
```

## Key Points:
- `clearTimeout(id)` cancels a setTimeout.
- `clearInterval(id)` cancels a setInterval.
- Both return a timer ID when created.
- Clearing prevents the callback from executing.
- Important to clean up intervals to prevent memory leaks.

## Interview Tip:
"Always clear your timers and intervals when they're no longer needed â€” they can cause memory leaks."

---

## Question 77: What is `clearTimeout()`?

## Answer:
`clearTimeout()` cancels a timer previously created by `setTimeout()`. The callback will not execute.

```js
const timer = setTimeout(() => {
  console.log("This won't run");
}, 5000);

clearTimeout(timer);
```

If the timer has already fired, `clearTimeout()` has no effect.

## Key Points:
- Cancels a setTimeout timer.
- Takes the timer ID as argument.
- No effect if the timer already fired.
- Important for cleanup in components and subscriptions.

## Interview Tip:
"`clearTimeout` is like hanging up a phone call before someone answers â€” the callback never happens."

---

## Question 78: What is `clearInterval()`?

## Answer:
`clearInterval()` cancels a timer previously created by `setInterval()`. The callback stops repeating.

```js
let count = 0;
const interval = setInterval(() => {
  console.log(count++);
  if (count >= 5) clearInterval(interval);
}, 1000);
```

Always clear intervals when they're no longer needed â€” they continue running until explicitly cleared.

## Key Points:
- Cancels a setInterval timer.
- Stops the repeated callback execution.
- Must be explicitly called â€” intervals don't stop on their own.
- Important for cleanup to prevent memory leaks.
- Use a reference to the interval ID.

## Interview Tip:
"Forget to clear an interval and you've got a memory leak. Always clean up."

---

## Question 79: Why is timer execution not guaranteed to be exact?

## Answer:
Several factors affect timer accuracy:
1. **Event loop congestion**: Other callbacks may be running when the timer fires.
2. **System load**: High CPU usage delays callback execution.
3. **Minimum delay**: Browsers/Node.js enforce minimum delays (1ms for setTimeout).
4. **Timer resolution**: The system clock has limited precision.
5. **Timer batching**: Multiple timers with the same delay may batch together.

Timer callbacks are scheduled, not guaranteed.

## Key Points:
- Event loop congestion delays execution.
- System load affects timing accuracy.
- Minimum delays are enforced.
- Timer batching can cause simultaneous execution.
- Never rely on exact timing for critical logic.

## Interview Tip:
"Timers are approximate â€” never build logic that depends on exact timing."

---

## Question 80: What factors can delay timer execution?

## Answer:
- **Call stack blocking**: Synchronous code running too long.
- **Event loop congestion**: Many pending callbacks.
- **High system load**: CPU or memory pressure.
- **GC pauses**: Garbage collection pauses the event loop.
- **I/O operations**: Heavy I/O processing delays the event loop.
- **`process.nextTick` and microtask starvation**: Too many microtasks delay macrotasks.

## Key Points:
- Synchronous code blocks the event loop.
- Many pending callbacks delay processing.
- System load affects all operations.
- GC pauses the event loop briefly.
- Microtask starvation delays macrotasks.

## Interview Tip:
"The event loop is single-threaded â€” anything that blocks it delays all timers."

---

## Part 9 (81â€“90): EventEmitter

---

## Question 81: What is the `EventEmitter` class?

## Answer:
`EventEmitter` is a class in Node.js that implements the publish-subscribe pattern. Objects can emit events, and other objects can listen for and respond to those events. Most of Node.js's core modules (http, streams, fs) are built on EventEmitter.

```js
const EventEmitter = require("events");
const emitter = new EventEmitter();

emitter.on("data", (msg) => console.log(msg));
emitter.emit("data", "hello world"); // "hello world"
```

## Key Points:
- Implements the publish-subscribe pattern.
- Core of Node.js's event-driven architecture.
- Used by http, streams, and other core modules.
- `on()` to listen, `emit()` to trigger events.
- Supports multiple listeners per event.

## Interview Tip:
"EventEmitter is the foundation of Node.js â€” HTTP servers, streams, and processes all extend it."

---

## Question 82: Why is `EventEmitter` important in Node.js?

## Answer:
EventEmitter is the foundation of Node.js's event-driven architecture. It enables:
- **Decoupled code**: Emitters don't know who's listening.
- **Flexible communication**: Multiple listeners per event.
- **Custom events**: Create domain-specific events.
- **Core module foundation**: HTTP, streams, and processes use it.

Without EventEmitter, Node.js couldn't have its non-blocking, event-driven model.

## Key Points:
- Foundation of Node.js's event-driven model.
- Decouples event producers from consumers.
- Enables custom events for domain logic.
- Core modules are built on it.
- Enables the observer pattern in JavaScript.

## Interview Tip:
"If you understand EventEmitter, you understand how Node.js's core modules work."

---

## Question 83: How do you create a custom event?

## Answer:
Extend or instantiate `EventEmitter`, then use `on()` to listen and `emit()` to trigger:

```js
const EventEmitter = require("events");

class OrderService extends EventEmitter {
  placeOrder(order) {
    // Process order
    this.emit("orderPlaced", order);
  }
}

const service = new OrderService();
service.on("orderPlaced", (order) => {
  console.log(`Order ${order.id} placed`);
});

service.placeOrder({ id: 123 }); // Triggers the event
```

## Key Points:
- Extend `EventEmitter` or create instances.
- `on(event, listener)` to subscribe.
- `emit(event, data)` to trigger.
- Pass data to listeners via emit arguments.
- Custom events for domain-specific communication.

## Interview Tip:
"Extending EventEmitter is the standard pattern for creating event emitters in Node.js."

---

## Question 84: What is the difference between `on()` and `once()`?

## Answer:
- `on()`: The listener fires every time the event is emitted.
- `once()`: The listener fires only the first time the event is emitted, then automatically removes itself.

```js
emitter.on("connect", () => console.log("connected")); // Fires every time
emitter.once("connect", () => console.log("first time")); // Fires once

emitter.emit("connect"); // Both fire
emitter.emit("connect"); // Only on() fires
```

## Key Points:
- `on()`: persistent listener, fires every emission.
- `once()`: one-time listener, auto-removes after first fire.
- `once()` is useful for initialization or connection events.
- Both accept event name and callback.

## Interview Tip:
"`once()` is great for 'do this one time' patterns â€” like initializing a connection."

---

## Question 85: What is `emit()`?

## Answer:
`emit()` triggers an event, calling all registered listeners for that event. You can pass data to listeners as additional arguments.

```js
emitter.on("message", (text, sender) => {
  console.log(`${sender}: ${text}`);
});

emitter.emit("message", "Hello", "Alice"); // "Alice: Hello"
```

`emit()` returns `true` if there are listeners, `false` if there are none.

## Key Points:
- Triggers an event and calls all listeners.
- Pass data to listeners as arguments.
- Returns `true` if listeners exist, `false` otherwise.
- Events with no listeners are silently ignored.
- Synchronous â€” listeners execute in order.

## Interview Tip:
"`emit()` is synchronous â€” listeners run one after another, not in parallel."

---

## Question 86: How do you remove event listeners?

## Answer:
```js
function onData(data) { console.log(data); }

emitter.on("data", onData);
emitter.removeListener("data", onData);  // Remove specific listener
emitter.removeAllListeners("data");       // Remove all listeners for "data"
emitter.removeAllListeners();             // Remove ALL listeners
```

Always remove listeners when they're no longer needed to prevent memory leaks.

## Key Points:
- `removeListener(event, fn)` removes a specific listener.
- `removeAllListeners(event)` removes all listeners for an event.
- Always clean up listeners in cleanup code.
- Memory leaks occur when listeners aren't removed.
- `once()` auto-removes after first emission.

## Interview Tip:
"Forget to remove listeners and you've got a memory leak. Clean up in cleanup functions."

---

## Question 87: What is `removeListener()`?

## Answer:
`removeListener()` (alias: `off()`) removes a specific listener from an event. You must pass the same function reference that was used in `on()`.

```js
function onData(data) { console.log(data); }

emitter.on("data", onData);
emitter.removeListener("data", onData); // Works â€” same reference
emitter.removeListener("data", () => {}); // Doesn't work â€” different reference
```

## Key Points:
- Removes a specific listener by function reference.
- Must pass the exact same function used in `on()`.
- Alias: `off()` (same method).
- Returns the EventEmitter for chaining.
- No effect if the listener was already removed.

## Interview Tip:
"You need the exact function reference â€” anonymous functions can't be removed."

---

## Question 88: What is `removeAllListeners()`?

## Answer:
`removeAllListeners()` removes all listeners from an event, or all events if no event name is provided.

```js
emitter.removeAllListeners("data"); // Remove all "data" listeners
emitter.removeAllListeners();       // Remove ALL listeners
```

Use this sparingly â€” it can remove listeners added by other parts of the code. Prefer `removeListener()` for specific cleanup.

## Key Points:
- Removes all listeners for a specific event.
- Without arguments, removes all listeners for all events.
- Can remove listeners added by other code.
- Use with caution â€” prefer `removeListener()` for specific cleanup.
- Returns the EventEmitter for chaining.

## Interview Tip:
"`removeAllListeners()` is nuclear â€” it removes everything. Use `removeListener()` for targeted cleanup."

---

## Question 89: What happens if too many listeners are attached?

## Answer:
Node.js emits a warning when more than 10 listeners are attached to a single event. This is called a "memory leak warning" â€” it suggests you may have forgotten to remove listeners.

```js
// MaxListenersExceededWarning: Possible EventEmitter memory leak detected.
// 11 listeners added. Use emitter.setMaxListeners() to increase limit
```

You can increase the limit or set it to 0 for unlimited:

```js
emitter.setMaxListeners(20); // Increase limit
emitter.setMaxListeners(0);  // Unlimited (use with caution)
```

## Key Points:
- Warning triggered at 11+ listeners per event.
- Indicates possible memory leak.
- `setMaxListeners(n)` increases the limit.
- `setMaxListeners(0)` removes the limit (use carefully).
- Usually means you forgot to remove listeners.

## Interview Tip:
"The memory leak warning exists for a reason â€” don't just increase the limit. Fix the leak."

---

## Question 90: What are common use cases for `EventEmitter`?

## Answer:
- **HTTP servers**: `'request'`, `'connection'`, `'error'` events.
- **Streams**: `'data'`, `'end'`, `'error'` events.
- **Custom domain events**: `'orderPlaced'`, `'userCreated'`.
- **Process communication**: `'exit'`, `'uncaughtException'`.
- **Chat applications**: `'message'`, `'join'`, `'leave'` events.
- **Real-time features**: `'update'`, `'notification'` events.

## Key Points:
- HTTP servers emit request and connection events.
- Streams emit data and end events.
- Custom events for domain-specific communication.
- Process events for lifecycle management.
- Real-time applications for live updates.

## Interview Tip:
"If you're building a real-time feature, EventEmitter is your foundation."

---

## Part 10 (91â€“100): Error Handling & Async Patterns

---

## Question 91: How do you handle errors in asynchronous code?

## Answer:
Three main approaches:
1. **Callbacks**: Pass an error as the first argument (error-first callback).
2. **Promises**: Use `.catch()` or `try/catch` with `async/await`.
3. **Async/await**: Wrap in `try/catch`.

```js
// Callback
fs.readFile("file.txt", (err, data) => {
  if (err) return console.error(err);
});

// Promise
fetchData()
  .then(data => console.log(data))
  .catch(err => console.error(err));

// Async/await
async function getData() {
  try {
    const data = await fetchData();
  } catch (err) {
    console.error(err);
  }
}
```

## Key Points:
- Error-first callbacks: `callback(err, result)`.
- Promise `.catch()` for rejected promises.
- `try/catch` with `async/await` for clean error handling.
- Always handle errors â€” unhandled errors crash the process.
- `async/await` + `try/catch` is the modern standard.

## Interview Tip:
"Async/await + try/catch is the cleanest error handling pattern. Use it everywhere."

---

## Question 92: What is the difference between synchronous and asynchronous errors?

## Answer:
- **Synchronous errors**: Thrown immediately, caught with `try/catch`.
- **Asynchronous errors**: Occur in callbacks, promises, or timers â€” caught differently.

```js
// Synchronous â€” try/catch works
try {
  JSON.parse("invalid");
} catch (err) {
  console.error(err);
}

// Asynchronous â€” try/catch doesn't work
try {
  setTimeout(() => { throw new Error("async"); }, 1000);
} catch (err) {
  console.error(err); // Never catches!
}
```

## Key Points:
- Synchronous errors are caught by `try/catch`.
- `try/catch` doesn't catch errors in async callbacks.
- Promise rejections need `.catch()` or `try/catch` with `async/await`.
- Unhandled async errors can crash the process.
- Different error handling for different contexts.

## Interview Tip:
"`try/catch` only works synchronously. For async code, use Promises or async/await."

---

## Question 93: How do you catch Promise rejections?

## Answer:
Three ways:
1. **`.catch()`**: Attach to the promise chain.
2. **`try/catch`**: Use with `async/await`.
3. **`unhandledRejection` event**: Global fallback (not recommended as primary).

```js
// .catch()
fetchData()
  .then(data => process(data))
  .catch(err => handleError(err));

// try/catch with async/await
async function getData() {
  try {
    const data = await fetchData();
    process(data);
  } catch (err) {
    handleError(err);
  }
}

// Global fallback
process.on("unhandledRejection", (err) => {
  console.error("Unhandled rejection:", err);
});
```

## Key Points:
- `.catch()` for promise chains.
- `try/catch` for async/await.
- `unhandledRejection` event as a safety net.
- Always handle rejections â€” unhandled ones crash Node.js 15+.
- Never leave promises without error handling.

## Interview Tip:
"`unhandledRejection` is a safety net, not a strategy. Handle errors explicitly with try/catch or .catch()."

---

## Question 94: What is an unhandled Promise rejection?

## Answer:
An unhandled Promise rejection occurs when a Promise rejects and no `.catch()` handler or `try/catch` block catches it. In Node.js 15+, unhandled rejections crash the process by default.

```js
// Unhandled rejection â€” crashes in Node.js 15+
fetch("https://api.example.com/data")
  .then(res => res.json());
// If the network fails, this crashes!
```

Always add error handling to every Promise chain.

## Key Points:
- Promise rejects without a `.catch()` or `try/catch`.
- Crashes the process in Node.js 15+.
- Previously just logged a warning.
- Add `.catch()` or use `async/await` with `try/catch`.
- Global `unhandledRejection` handler as last resort.

## Interview Tip:
"Node.js 15+ treats unhandled rejections like uncaught exceptions â€” they crash your server."

---

## Question 95: How do you use `try...catch` with `async/await`?

## Answer:
Wrap `await` calls in a `try/catch` block. The `catch` receives any rejected promise value.

```js
async function getUser(id) {
  try {
    const user = await db.user.findUnique({ where: { id } });
    if (!user) throw new Error("User not found");
    return user;
  } catch (err) {
    console.error("Error fetching user:", err.message);
    throw err; // Re-throw or handle
  }
}
```

Multiple `await` calls can share a single `try/catch` or have separate ones.

## Key Points:
- `try` wraps `await` calls.
- `catch` receives the rejection value.
- Re-throw or handle the error in catch.
- Multiple awaits can share one try/catch.
- Clean and readable error handling.

## Interview Tip:
"Async/await + try/catch makes async error handling look like synchronous code."

---

## Question 96: What is the difference between throwing an error and rejecting a Promise?

## Answer:
- **Throwing**: Stops function execution, propagates up the call stack (synchronous).
- **Rejecting**: Creates a rejected Promise, propagates to `.catch()` or `try/catch` with `await`.

```js
// Throwing (synchronous)
function doWork() {
  throw new Error("sync error"); // Stops here
}

// Rejecting (async)
async function doAsyncWork() {
  throw new Error("async error"); // Creates rejected Promise
}
```

In `async` functions, `throw` creates a rejected Promise â€” they're equivalent.

## Key Points:
- Throw: synchronous error propagation.
- Reject: async error propagation via Promise.
- In async functions, throw = reject.
- Both use the same error handling (try/catch).
- Reject propagates to the nearest `.catch()`.

## Interview Tip:
"In an async function, `throw` creates a rejected Promise. They're the same thing."

---

## Question 97: How do you create custom error classes?

## Answer:
Extend the built-in `Error` class:

```js
class NotFoundError extends Error {
  constructor(message, resource) {
    super(message);
    this.name = "NotFoundError";
    this.resource = resource;
    this.statusCode = 404;
  }
}

class ValidationError extends Error {
  constructor(message, fields) {
    super(message);
    this.name = "ValidationError";
    this.fields = fields;
    this.statusCode = 400;
  }
}
```

Custom error classes make error handling more precise.

## Key Points:
- Extend the `Error` class.
- Set `name`, `statusCode`, and custom properties.
- Preserves stack trace via `super()`.
- Enables specific error handling by type.
- Common: NotFoundError, ValidationError, UnauthorizedError.

## Interview Tip:
"Custom error classes make error handling precise â€” `if (err instanceof ValidationError)` is better than checking error messages."

---

## Question 98: What are operational errors vs programmer errors?

## Answer:
- **Operational errors**: Expected failures â€” network timeouts, invalid user input, file not found. These should be handled gracefully.
- **Programmer errors**: Bugs â€” null reference, undefined property, type errors. These should crash the process and be fixed.

```js
// Operational error â€” handle gracefully
try {
  const data = await readFile("config.json");
} catch (err) {
  if (err.code === "ENOENT") {
    console.log("Config file not found, using defaults");
  }
}

// Programmer error â€” let it crash
function processUser(user) {
  return user.name.toUpperCase(); // Bug if user is null â€” should crash
}
```

## Key Points:
- Operational: expected failures, handle gracefully.
- Programmer: bugs, let them crash and fix.
- Operational errors have predictable causes.
- Programmer errors indicate code defects.
- Never hide programmer errors with catch blocks.

## Interview Tip:
"Don't catch programmer errors â€” let them crash. Catch operational errors and handle them gracefully."

---

## Question 99: What are Node.js best practices for error handling?

## Answer:
1. **Always handle errors**: Never leave promises unhandled.
2. **Use async/await + try/catch**: Cleanest error handling pattern.
3. **Create custom errors**: Specific error types for different scenarios.
4. **Don't catch programmer errors**: Let them crash.
5. **Handle operational errors gracefully**: Return meaningful messages.
6. **Use error boundaries**: Catch errors at appropriate levels.
7. **Log errors**: Use structured logging (Winston/Pino).
8. **Validate input early**: Prevent errors before they happen.

## Key Points:
- Handle all promise rejections.
- Async/await + try/catch is the standard.
- Custom errors for precise handling.
- Don't hide bugs with catch blocks.
- Log errors for debugging.

## Interview Tip:
"Error handling is not optional â€” it's a core part of production-quality code."

---

## Question 100: How do you build a centralized error-handling strategy in a Node.js application?

## Answer:
1. **Custom error classes**: Define error types (NotFound, Validation, Auth).
2. **Error middleware**: Express error-handling middleware catches all errors.
3. **Error response formatter**: Consistent error response format.
4. **Error logging**: Log all errors with context.
5. **Error monitoring**: Send errors to Sentry or similar.

```js
// Express error middleware
app.use((err, req, res, next) => {
  const status = err.statusCode || 500;
  const message = err.message || "Internal server error";
  
  logger.error({ err, req: req.path });
  
  res.status(status).json({
    error: { message, code: err.name, ...(isDev && { stack: err.stack }) }
  });
});
```

## Key Points:
- Custom error classes for different error types.
- Centralized error middleware catches all errors.
- Consistent error response format.
- Structured error logging.
- Error monitoring in production.

## Interview Tip:
"A centralized error handler means every error is handled consistently â€” no forgotten catch blocks."

---

## Part 11 (101â€“110): File System (`fs`)

---

## Question 101: What is the `fs` module in Node.js?

## Answer:
The `fs` (file system) module provides APIs for interacting with the file system â€” reading, writing, deleting, renaming, and stat'ing files and directories.

```js
const fs = require("fs");
const fsPromises = require("fs").promises;

// Callback-based
fs.readFile("file.txt", (err, data) => { /* ... */ });

// Promise-based
const data = await fsPromises.readFile("file.txt", "utf-8");
```

## Key Points:
- Provides file system operations.
- Callback-based and promise-based APIs.
- Synchronous versions available (`readFileSync`).
- Supports reading, writing, deleting, renaming files.
- Cross-platform (works on Windows, macOS, Linux).

## Interview Tip:
"Use `fs.promises` for modern async code. Callback-based `fs` is legacy."

---

## Question 102: What is the difference between synchronous and asynchronous file operations?

## Answer:
- **Synchronous** (`readFileSync`, `writeFileSync`): Blocks the event loop until completion. Simple but blocks all other requests.
- **Asynchronous** (`readFile`, `writeFile`): Non-blocking â€” callback or promise handles the result when ready.

```js
// Synchronous â€” blocks event loop
const data = fs.readFileSync("file.txt", "utf-8");

// Asynchronous â€” non-blocking
fs.readFile("file.txt", "utf-8", (err, data) => { /* ... */ });

// Promise-based async
const data = await fs.promises.readFile("file.txt", "utf-8");
```

## Key Points:
- Synchronous: blocks the event loop.
- Asynchronous: non-blocking, callback or promise.
- Never use sync operations in request handlers.
- Async operations are essential for scalable servers.
- Promise-based async is the modern standard.

## Interview Tip:
"Never use `readFileSync` in a request handler â€” it blocks every other request."

---

## Question 103: How do you read a file in Node.js?

## Answer:
```js
// Promise-based (recommended)
const fs = require("fs").promises;
const data = await fs.readFile("file.txt", "utf-8");

// Callback-based
const fs = require("fs");
fs.readFile("file.txt", "utf-8", (err, data) => {
  if (err) throw err;
  console.log(data);
});

// Synchronous
const data = fs.readFileSync("file.txt", "utf-8");
```

## Key Points:
- `fs.promises.readFile()` for async/await.
- `fs.readFile()` for callbacks.
- `fs.readFileSync()` for synchronous (avoid in servers).
- Second argument specifies encoding (e.g., "utf-8").
- Returns a Buffer by default; specify encoding for string.

## Interview Tip:
"Use `fs.promises.readFile()` with `await` â€” it's the cleanest approach."

---

## Question 104: How do you write data to a file?

## Answer:
```js
// Promise-based
const fs = require("fs").promises;
await fs.writeFile("output.txt", "Hello, World!");

// With options
await fs.writeFile("data.json", JSON.stringify(data), "utf-8");

// Callback-based
fs.writeFile("output.txt", "Hello", (err) => {
  if (err) throw err;
});

// Synchronous
fs.writeFileSync("output.txt", "Hello");
```

## Key Points:
- `fs.promises.writeFile()` for async/await.
- Overwrites the entire file by default.
- Use `appendFile()` to add to existing files.
- Specify encoding for string data.
- Always handle errors.

## Interview Tip:
"`writeFile` overwrites the entire file. Use `appendFile` to add to existing files."

---

## Question 105: How do you append data to a file?

## Answer:
```js
// Promise-based
const fs = require("fs").promises;
await fs.appendFile("log.txt", "New log entry\n");

// Callback-based
fs.appendFile("log.txt", "New log entry\n", (err) => {
  if (err) throw err;
});
```

`appendFile` adds data to the end of the file without overwriting existing content.

## Key Points:
- Adds data to the end of a file.
- Creates the file if it doesn't exist.
- `fs.promises.appendFile()` for async/await.
- Common for log files and append-only data.
- Does not overwrite existing content.

## Interview Tip:
"`appendFile` is perfect for log files â€” it adds entries without overwriting."

---

## Question 106: How do you delete a file?

## Answer:
```js
// Promise-based
const fs = require("fs").promises;
await fs.unlink("file.txt");

// Callback-based
fs.unlink("file.txt", (err) => {
  if (err) throw err;
});
```

`unlink` is the Node.js equivalent of "delete file." It's named after the Unix system call.

## Key Points:
- `fs.promises.unlink()` for async/await.
- Named after Unix `unlink` system call.
- Throws error if file doesn't exist.
- Always check if the file exists first (or handle the error).
- Use `rmdir` or `rm` for directories.

## Interview Tip:
"`unlink` deletes files â€” the name comes from Unix, not from what it does."

---

## Question 107: How do you rename or move a file?

## Answer:
```js
// Rename or move
const fs = require("fs").promises;
await fs.rename("old-path.txt", "new-path.txt");

// Move to a different directory
await fs.rename("./uploads/temp.jpg", "./uploads/images/photo.jpg");
```

`rename` can rename a file, move it to a different directory, or both.

## Key Points:
- `fs.promises.rename()` for async/await.
- Can rename and/or move files.
- Moving across filesystems may fail (use copy + delete).
- Works for files and directories.
- Throws error if the destination already exists.

## Interview Tip:
"`rename` is both rename and move. For cross-filesystem moves, copy the file first, then delete the original."

---

## Question 108: How do you check whether a file or directory exists?

## Answer:
```js
// Promise-based
const fs = require("fs").promises;
try {
  await fs.access("file.txt");
  console.log("File exists");
} catch {
  console.log("File does not exist");
}

// Synchronous
const fs = require("fs");
if (fs.existsSync("file.txt")) {
  console.log("File exists");
}
```

Note: `fs.exists()` is deprecated â€” use `fs.access()` or `fs.existsSync()` instead.

## Key Points:
- `fs.promises.access()` checks existence.
- `fs.existsSync()` is synchronous.
- `fs.exists()` is deprecated.
- `access` throws if the file doesn't exist.
- Use `stat()` to get file info (size, permissions).

## Interview Tip:
"`fs.exists()` is deprecated. Use `fs.access()` or check for errors in `readFile()`."

---

## Question 109: How do you create and remove directories?

## Answer:
```js
const fs = require("fs").promises;

// Create directory
await fs.mkdir("new-folder");

// Create nested directories
await fs.mkdir("a/b/c", { recursive: true });

// Remove empty directory
await fs.rmdir("empty-folder");

// Remove directory and contents
await fs.rm("folder", { recursive: true, force: true });
```

## Key Points:
- `mkdir()` creates directories.
- `{ recursive: true }` creates parent directories.
- `rmdir()` removes empty directories only.
- `rm()` with `{ recursive: true }` removes everything.
- `force: true` ignores errors if the directory doesn't exist.

## Interview Tip:
"`fs.rm()` with `recursive: true` is the modern way to delete directories. `rmdir()` only works on empty directories."

---

## Question 110: What are common file system best practices?

## Answer:
1. **Use async operations**: Never block the event loop with sync operations.
2. **Use `fs.promises`**: Cleaner async code with async/await.
3. **Handle errors**: Always catch file operation errors.
4. **Use path.join()**: Don't concatenate paths manually.
5. **Validate paths**: Prevent path traversal attacks.
6. **Use streams for large files**: Don't read entire large files into memory.
7. **Close file handles**: Always close after reading/writing.

## Key Points:
- Async operations for non-blocking I/O.
- `fs.promises` for modern async/await.
- `path.join()` for cross-platform paths.
- Streams for large files.
- Error handling is essential.

## Interview Tip:
"Never read an entire large file into memory â€” use streams instead."

---

## Part 12 (111â€“120): Streams

---

## Question 111: What is a stream in Node.js?

## Answer:
Streams are objects that let you read or write data continuously, piece by piece, instead of loading everything into memory at once. They're ideal for processing large files, network data, or any data that comes in chunks.

```js
const readable = fs.createReadStream("large-file.txt");
const writable = fs.createWriteStream("output.txt");
readable.pipe(writable);
```

## Key Points:
- Process data in chunks, not all at once.
- Memory-efficient for large data.
- Can be read, written, transformed, or duplicated.
- Built on EventEmitter.
- Four types: Readable, Writable, Duplex, Transform.

## Interview Tip:
"Streams are how Node.js handles large data â€” they're memory-efficient and composable."

---

## Question 112: Why are streams more efficient than reading an entire file into memory?

## Answer:
Reading an entire file loads it all into RAM â€” a 4GB file uses 4GB of memory. Streams process data in small chunks (typically 64KB), using constant memory regardless of file size.

```js
// Bad: loads entire file into memory
const data = await fs.promises.readFile("4gb-file.mp4");

// Good: processes in chunks
const stream = fs.createReadStream("4gb-file.mp4");
stream.pipe(res); // Sends to response in chunks
```

## Key Points:
- Constant memory usage regardless of file size.
- Processes data in small chunks (64KB default).
- Essential for large files (video, logs, datasets).
- Pipes connect readable and writable streams.
- Memory-efficient and scalable.

## Interview Tip:
"Streams use constant memory â€” whether the file is 1MB or 4GB."

---

## Question 113: What are the four types of streams?

## Answer:
1. **Readable**: Source of data (e.g., `fs.createReadStream`, HTTP request).
2. **Writable**: Destination for data (e.g., `fs.createWriteStream`, HTTP response).
3. **Duplex**: Both readable and writable (e.g., TCP socket).
4. **Transform**: Duplex that modifies data in transit (e.g., zlib compression).

```js
const readable = fs.createReadStream("input.txt");     // Readable
const writable = fs.createWriteStream("output.txt");   // Writable
const transform = zlib.createGzip();                    // Transform
readable.pipe(transform).pipe(writable);               // Pipeline
```

## Key Points:
- Readable: data source.
- Writable: data destination.
- Duplex: both read and write.
- Transform: modify data in transit.
- All are built on EventEmitter.

## Interview Tip:
"Readable + Writable = Duplex. Duplex + transformation = Transform."

---

## Question 114: What is a Readable stream?

## Answer:
A Readable stream produces data that you can consume. It emits `'data'` events for each chunk and `'end'` when there's no more data.

```js
const readable = fs.createReadStream("file.txt", { encoding: "utf-8" });
readable.on("data", (chunk) => console.log(chunk));
readable.on("end", () => console.log("Done"));
readable.on("error", (err) => console.error(err));
```

## Key Points:
- Produces data chunks via `'data'` events.
- `'end'` event when all data is consumed.
- `'error'` event for read errors.
- Can be paused and resumed.
- Sources: files, HTTP requests, TCP sockets.

## Interview Tip:
"Readable streams emit `'data'` and `'end'` events â€” that's how you consume data."

---

## Question 115: What is a Writable stream?

## Answer:
A Writable stream consumes data that you write to it. It emits `'drain'` when it's ready for more data and `'finish'` when all data has been flushed.

```js
const writable = fs.createWriteStream("output.txt");
writable.write("Hello, ");
writable.write("World!");
writable.end(); // No more data
writable.on("finish", () => console.log("Done"));
```

## Key Points:
- Consumes data via `write()` method.
- `'drain'` event when ready for more data.
- `'finish'` event when all data is written.
- `end()` signals no more data.
- Sources: files, HTTP responses, TCP sockets.

## Interview Tip:
"Writable streams use `write()` to send data and `end()` to signal completion."

---

## Question 116: What is a Duplex stream?

## Answer:
A Duplex stream is both readable and writable â€” it can receive and send data. A TCP socket is the classic example.

```js
const socket = require("net").createConnection(3000, "localhost");
socket.write("Hello server");      // Writable
socket.on("data", (chunk) => {     // Readable
  console.log("Received:", chunk.toString());
});
```

## Key Points:
- Both readable and writable.
- Can read and write simultaneously.
- Classic example: TCP sockets.
- Implements both Readable and Writable interfaces.
- Data written can be independent of data read.

## Interview Tip:
"Duplex = two-way communication. TCP sockets are the most common Duplex stream."

---

## Question 117: What is a Transform stream?

## Answer:
A Transform stream is a Duplex stream that modifies data in transit. Data written to it is transformed and can be read from the other end. Examples: zlib compression, crypto hashing.

```js
const { createGzip } = require("zlib");
const gzip = createGzip();

const input = fs.createReadStream("file.txt");
const output = fs.createWriteStream("file.txt.gz");

input.pipe(gzip).pipe(output); // Compress and write
```

## Key Points:
- Modifies data as it passes through.
- Both readable and writable.
- Used for compression, encryption, encoding.
- `pipe()` connects streams together.
- zlib and crypto provide transform streams.

## Interview Tip:
"Transform streams are the 'middleware' of streams â€” they modify data in the pipeline."

---

## Question 118: How do you create a readable stream?

## Answer:
```js
// From a file
const readable = fs.createReadStream("file.txt", {
  encoding: "utf-8",
  highWaterMark: 16 * 1024  // 16KB chunks
});

// From an array
const { Readable } = require("stream");
const readable = Readable.from(["chunk1", "chunk2", "chunk3"]);

// Listen for data
readable.on("data", (chunk) => {
  console.log(chunk);
});
```

## Key Points:
- `fs.createReadStream()` for files.
- `Readable.from()` for arrays or iterables.
- `highWaterMark` controls chunk size.
- Emits `'data'`, `'end'`, `'error'` events.
- Can be piped to writable streams.

## Interview Tip:
"`Readable.from()` is useful for creating streams from arrays or generators."

---

## Question 119: How do you create a writable stream?

## Answer:
```js
// To a file
const writable = fs.createWriteStream("output.txt");

// Write data
writable.write("Hello, ");
writable.write("World!");

// End the stream
writable.end();
writable.on("finish", () => console.log("Done writing"));

// Pipe from readable to writable
const readable = fs.createReadStream("input.txt");
readable.pipe(writable);
```

## Key Points:
- `fs.createWriteStream()` for files.
- `write()` to send data chunks.
- `end()` to signal completion.
- `pipe()` connects readable to writable.
- `'finish'` event when writing is complete.

## Interview Tip:
"`pipe()` is the simplest way to connect streams â€” it handles backpressure automatically."

---

## Question 120: What is stream backpressure, and how do you handle it?

## Answer:
Backpressure occurs when the writable stream can't keep up with the readable stream. The readable stream produces data faster than the writable stream can consume it, causing memory to grow unbounded.

Node.js handles this automatically with `pipe()` â€” it pauses the readable stream when the writable stream's buffer is full and resumes when it drains.

```js
// pipe() handles backpressure automatically
readable.pipe(writable);

// Manual handling
readable.on("data", (chunk) => {
  const canContinue = writable.write(chunk);
  if (!canContinue) {
    readable.pause();
    writable.once("drain", () => readable.resume());
  }
});
```

## Key Points:
- Readable produces faster than writable consumes.
- `pipe()` handles backpressure automatically.
- Manual: check `write()` return value, pause/resume.
- `'drain'` event signals the writable is ready for more.
- Ignoring backpressure causes memory issues.

## Interview Tip:
"`pipe()` handles backpressure for you. If you're writing manually, check the return value of `write()`."

---

## Part 13 (121â€“130): Buffers

---

## Question 121: What is a Buffer in Node.js?

## Answer:
A Buffer is a fixed-size block of memory that holds binary data. Since JavaScript was designed for text, Node.js introduced Buffers to handle raw binary data â€” file contents, network packets, images, and cryptographic operations.

```js
const buf = Buffer.from("hello");
console.log(buf);        // <Buffer 68 65 6c 6c 6f>
console.log(buf.length); // 5
```

## Key Points:
- Fixed-size memory block for binary data.
- Created from strings, arrays, or allocated empty.
- Converts between binary and text with encoding.
- Used for file I/O, networking, and crypto.
- Backed by V8's ArrayBuffer.

## Interview Tip:
"Buffers are Node.js's way of dealing with binary data â€” the raw bytes that make up files, images, and network packets."

---

## Question 122: Why are Buffers needed?

## Answer:
JavaScript was designed for text and doesn't have a native way to represent binary data. Buffers provide a way to work with raw bytes â€” essential for:
- Reading/writing files (binary content).
- Network protocols (TCP, HTTP).
- Cryptographic operations.
- Image and media processing.
- Interacting with the operating system.

## Key Points:
- JavaScript lacks native binary data support.
- Buffers handle raw bytes for file I/O.
- Essential for networking and crypto.
- Needed for image and media processing.
- Bridge between JavaScript and binary data.

## Interview Tip:
"Without Buffers, Node.js couldn't read files, process images, or handle network protocols."

---

## Question 123: How do Buffers differ from strings?

## Answer:
- **Strings**: UTF-16 encoded, immutable, variable-width characters.
- **Buffers**: Binary data, fixed-size, raw bytes.

```js
// String â€” UTF-16
const str = "hello";
console.log(str.length); // 5 characters

// Buffer â€” raw bytes
const buf = Buffer.from("hello");
console.log(buf.length); // 5 bytes
```

Buffers can represent any binary data; strings are limited to text.

## Key Points:
- Strings: text, UTF-16, immutable.
- Buffers: binary, raw bytes, mutable.
- Buffers can represent any binary data.
- Strings are limited to valid text.
- Convert between them with encoding.

## Interview Tip:
"Strings are for text; Buffers are for bytes. When you need raw binary data, use Buffers."

---

## Question 124: How do you create a Buffer?

## Answer:
```js
// From a string
const buf1 = Buffer.from("hello");

// From an array
const buf2 = Buffer.from([0x68, 0x65, 0x6c, 0x6c, 0x6f]);

// From another buffer (copy)
const buf3 = Buffer.from(buf1);

// Allocate empty buffer
const buf4 = Buffer.alloc(10);      // 10 bytes, zero-filled
const buf5 = Buffer.allocUnsafe(10); // 10 bytes, uninitialized (faster)
```

## Key Points:
- `Buffer.from()` for creating from data.
- `Buffer.alloc()` for zero-filled buffers.
- `Buffer.allocUnsafe()` for uninitialized (faster but may contain old data).
- `allocUnsafe` is faster but not secure â€” use `alloc` for sensitive data.

## Interview Tip:
"Use `Buffer.alloc()` for sensitive data â€” `allocUnsafe` may contain leftover memory."

---

## Question 125: How do you convert a Buffer to a string?

## Answer:
```js
const buf = Buffer.from([0x48, 0x65, 0x6c, 0x6c, 0x6f]);

// Default UTF-8
const str1 = buf.toString();       // "Hello"

// Specific encoding
const str2 = buf.toString("hex");  // "48656c6c6f"
const str3 = buf.toString("base64"); // "SGVsbG8="
```

## Key Points:
- `buf.toString()` converts to UTF-8 string.
- Specify encoding for different formats.
- Common encodings: "utf-8", "hex", "base64".
- Useful for debugging and data conversion.

## Interview Tip:
"`buf.toString("hex")` and `buf.toString("base64")` are commonly used for debugging and data encoding."

---

## Question 126: How do you convert a string to a Buffer?

## Answer:
```js
const str = "Hello, World!";

// UTF-8 (default)
const buf1 = Buffer.from(str);

// Specific encoding
const buf2 = Buffer.from(str, "utf-8");
const buf3 = Buffer.from(str, "base64");
```

## Key Points:
- `Buffer.from(string)` creates a Buffer.
- Default encoding is UTF-8.
- Specify encoding as second argument.
- Used before writing binary data.

## Interview Tip:
"`Buffer.from()` is the standard way to convert strings to Buffers."

---

## Question 127: What is character encoding?

## Character encoding maps characters to binary representations. Different encodings use different schemes:
- **UTF-8**: Variable-width (1-4 bytes per character). Most common.
- **UTF-16**: Fixed 2 or 4 bytes per character.
- **ASCII**: 1 byte per character (limited to 128 characters).
- **Latin-1**: 1 byte per character (256 characters).

```js
Buffer.from("hello", "utf-8");   // 5 bytes
Buffer.from("hello", "utf-16le"); // 10 bytes
```

## Key Points:
- Encoding maps characters to bytes.
- UTF-8 is the most widely used encoding.
- Different encodings produce different byte sequences.
- Node.js supports many encodings (utf-8, ascii, hex, base64).
- Always specify encoding when converting between strings and Buffers.

## Interview Tip:
"UTF-8 is the default and most common encoding â€” it's variable-width and backward-compatible with ASCII."

---

## Question 128: What encodings does Node.js support?

## Answer:
Common encodings:
- **utf-8**: Default, variable-width (1-4 bytes).
- **ascii**: 1 byte, limited to 128 characters.
- **utf-16le**: 2 bytes per character (little-endian).
- **base64**: Binary to text encoding (4 characters per 3 bytes).
- **hex**: Two hex characters per byte.

```js
Buffer.from("hello", "utf-8");
Buffer.from("hello", "base64");
Buffer.from("hello", "hex");
```

## Key Points:
- UTF-8 is the default encoding.
- base64 for encoding binary data as text.
- hex for debugging and binary data display.
- ASCII for simple text.
- UTF-16 for specific use cases.

## Interview Tip:
"Know the common ones: utf-8, base64, hex. You'll use them regularly."

---

## Question 129: When would you use Buffers in real-world applications?

## Answer:
- **File processing**: Reading/writing binary files (images, PDFs, videos).
- **Network protocols**: TCP/UDP communication.
- **Cryptographic operations**: Hashing, encryption, decryption.
- **Image processing**: Manipulating image data.
- **Data serialization**: Converting data to binary formats.
- **API responses**: Streaming binary data.

## Key Points:
- File processing (images, media, documents).
- Network protocols (TCP, UDP).
- Cryptographic operations.
- Image and media processing.
- Data serialization and encoding.

## Interview Tip:
"If you're dealing with binary data â€” files, images, network packets â€” you're using Buffers."

---

## Question 130: What are common mistakes when working with Buffers?

## Answer:
1. **Using `allocUnsafe` for sensitive data**: It may contain old memory.
2. **Not specifying encoding**: Default is UTF-8, which may not be what you want.
3. **Comparing buffers with `===`**: Buffers are objects â€” use `buf.equals()` instead.
4. **Not handling encoding mismatches**: Reading binary data as UTF-8 produces garbage.
5. **Forgetting Buffer is mutable**: `buf[0] = 0x48` modifies the buffer.

## Key Points:
- `allocUnsafe` may contain leftover memory â€” use `alloc` for security.
- Always specify encoding when converting.
- Use `buf.equals()` for comparison, not `===`.
- Handle encoding mismatches carefully.
- Buffers are mutable â€” be careful with modifications.

## Interview Tip:
"`buf.equals()` for comparison, not `===`. That's a common gotcha."

---

## Part 14 (131â€“140): Core Modules

---

## Question 131: What is the `path` module?

## Answer:
The `path` module provides utilities for working with file and directory paths. It handles cross-platform path differences (Windows uses `\`, Unix uses `/`).

```js
const path = require("path");

path.join("/users", "alice", "file.txt");  // Cross-platform join
path.resolve("src", "utils", "index.js"); // Absolute path
path.extname("file.txt");                 // ".txt"
path.basename("/users/alice/file.txt");   // "file.txt"
```

## Key Points:
- Cross-platform path manipulation.
- `join()`: joins path segments.
- `resolve()`: resolves to an absolute path.
- `extname()`, `basename()`, `dirname()`: path parsing.
- Always use `path.join()` instead of string concatenation.

## Interview Tip:
"Never concatenate paths with `+` â€” use `path.join()`. It handles cross-platform differences."

---

## Question 132: How do `path.join()` and `path.resolve()` differ?

## Answer:
- **`path.join()`**: Concatenates path segments into one path.
- **`path.resolve()`**: Resolves to an absolute path from right to left.

```js
path.join("src", "utils", "index.js");
// "src/utils/index.js" (relative)

path.resolve("src", "utils", "index.js");
// "/home/user/project/src/utils/index.js" (absolute)
```

`resolve()` stops when it hits an absolute path; `join()` just concatenates.

## Key Points:
- `join()` concatenates segments (may be relative).
- `resolve()` produces an absolute path.
- `resolve()` processes from right to left.
- `resolve()` stops at the first absolute path.
- Use `join()` for joining; `resolve()` for getting absolute paths.

## Interview Tip:
"`join()` is for building paths; `resolve()` is for finding absolute paths."

---

## Question 133: What is the `os` module used for?

## Answer:
The `os` module provides operating system-related utilities â€” platform info, CPU details, memory usage, and system information.

```js
const os = require("os");

os.platform();     // "win32", "darwin", "linux"
os.cpus();         // CPU information
os.totalmem();     // Total system memory
os.freemem();      // Free system memory
os.hostname();     // Computer name
os.uptime();       // System uptime in seconds
os.userInfo();     // Current user info
```

## Key Points:
- System information: platform, hostname, uptime.
- Hardware info: CPUs, memory.
- User info: current user details.
- Network info: network interfaces.
- Useful for monitoring and diagnostics.

## Interview Tip:
"`os.cpus()` and `os.freemem()` are useful for monitoring system health."

---

## Question 134: What information can you get from the `os` module?

## Answer:
- `os.platform()`: Operating system (`win32`, `darwin`, `linux`).
- `os.arch()`: CPU architecture (`x64`, `arm64`).
- `os.cpus()`: Detailed CPU information.
- `os.totalmem()` / `os.freemem()`: Memory info.
- `os.uptime()`: System uptime.
- `os.hostname()`: Machine hostname.
- `os.networkInterfaces()`: Network interface details.
- `os.userInfo()`: Current user info.

## Key Points:
- Platform, architecture, and OS version.
- CPU count, model, and speed.
- Total and free memory.
- System uptime.
- Network interfaces and user info.

## Interview Tip:
"The `os` module is great for monitoring â€” CPU usage, memory, and uptime."

---

## Question 135: What is the `crypto` module?

## Answer:
The `crypto` module provides cryptographic functionality â€” hashing, encryption, decryption, signing, and verification. It wraps OpenSSL's functionality.

```js
const crypto = require("crypto");

// Hashing
const hash = crypto.createHash("sha256").update("password").digest("hex");

// Random bytes
const token = crypto.randomBytes(32).toString("hex");
```

## Key Points:
- Cryptographic operations: hashing, encryption, signing.
- Wraps OpenSSL functionality.
- Secure random number generation.
- HMAC, RSA, AES support.
- Use for password hashing, token generation, data encryption.

## Interview Tip:
"Never roll your own crypto â€” use the `crypto` module or a library like bcrypt."

---

## Question 136: How do you generate a secure random value?

## Answer:
```js
const crypto = require("crypto");

// Secure random bytes
const token = crypto.randomBytes(32).toString("hex");
console.log(token); // 64-character hex string

// Random UUID
const { v4: uuidv4 } = require("uuid");
const id = uuidv4();

// Random integer between min and max
const randomInt = crypto.randomInt(1, 101); // 1-100
```

Always use `crypto.randomBytes()` â€” never `Math.random()` for security-sensitive values.

## Key Points:
- `crypto.randomBytes()` for secure random data.
- `crypto.randomUUID()` for UUID generation.
- `crypto.randomInt()` for secure random integers.
- Never use `Math.random()` for security.
- Essential for tokens, session IDs, and cryptographic keys.

## Interview Tip:
"`Math.random()` is not cryptographically secure. Use `crypto.randomBytes()` for anything security-related."

---

## Question 137: How do you hash passwords or data?

## Answer:
```js
const crypto = require("crypto");

// Simple hash (NOT for passwords â€” use bcrypt)
const hash = crypto.createHash("sha256").update("password").digest("hex");

// For passwords â€” use bcrypt
const bcrypt = require("bcrypt");
const hashedPassword = await bcrypt.hash("password", 12);
const isMatch = await bcrypt.compare("password", hashedPassword);
```

Never use plain SHA-256 for passwords â€” use bcrypt, scrypt, or argon2.

## Key Points:
- SHA-256 for data integrity, not passwords.
- bcrypt, scrypt, or argon2 for password hashing.
- bcrypt auto-generates and verifies salt.
- Hashing is one-way â€” can't reverse it.
- Always salt passwords before hashing.

## Interview Tip:
"Never hash passwords with plain SHA-256 â€” use bcrypt. It handles salting and is slow by design."

---

## Question 138: What is the `zlib` module used for?

## Answer:
The `zlib` module provides compression and decompression â€” gzip, deflate, and brotli. It's commonly used for compressing HTTP responses and file data.

```js
const zlib = require("zlib");
const { gzip, gunzip } = require("zlib").promises;

// Compress
const compressed = await gzip(Buffer.from("Hello, World!"));

// Decompress
const decompressed = await gunzip(compressed);
```

## Key Points:
- Compression and decompression.
- Supports gzip, deflate, and brotli.
- Used in HTTP middleware for response compression.
- Stream-based and callback-based APIs.
- Reduces data size for storage and transfer.

## Interview Tip:
"`zlib` is what Express's compression middleware uses under the hood."

---

## Question 139: How do you compress and decompress data?

## Answer:
```js
const zlib = require("zlib");
const { promisify } = require("util");
const gzip = promisify(zlib.gzip);
const gunzip = promisify(zlib.gunzip);

// Compress
const data = "Large amount of text...";
const compressed = await gzip(Buffer.from(data));

// Decompress
const decompressed = await gunzip(compressed);
const original = decompressed.toString();
```

Stream-based for large data:
```js
const fs = require("fs");
const zlib = require("zlib");
fs.createReadStream("input.txt")
  .pipe(zlib.createGzip())
  .pipe(fs.createWriteStream("input.txt.gz"));
```

## Key Points:
- `gzip`/`gunzip` for compression/decompression.
- Callback, promise, and stream APIs.
- Stream-based for large files.
- `deflate`/`inflate` for raw compression.
- `brotliCompress`/`brotliDecompress` for modern compression.

## Interview Tip:
"For large files, use stream-based compression â€” don't load the entire file into memory."

---

## Question 140: What other built-in Node.js modules do you commonly use?

## Answer:
- **`path`**: File path utilities.
- **`http`/`https`**: HTTP server and client.
- **`fs`**: File system operations.
- **`crypto`**: Cryptographic operations.
- **`os`**: Operating system information.
- **`events`**: Event emitter.
- **`stream`**: Stream utilities.
- **`url`**: URL parsing.
- **`querystring`**: Query string parsing.
- **`util`**: Utility functions (promisify, etc.).
- **`child_process`**: Spawning child processes.
- **`worker_threads`**: Multi-threading.

## Key Points:
- `path`, `fs`, `http` are the most commonly used.
- `crypto` for security operations.
- `events` for event-driven patterns.
- `stream` for data processing.
- `child_process` and `worker_threads` for parallelism.

## Interview Tip:
"Know the core modules â€” you'll use `path`, `fs`, `http`, and `crypto` in almost every Node.js project."

---

## Part 15 (141â€“150): HTTP, Child Processes & Worker Threads

---

## Question 141: What is the built-in `http` module?

## Answer:
The `http` module provides HTTP server and client functionality. It's the foundation for frameworks like Express.js.

```js
const http = require("http");

const server = http.createServer((req, res) => {
  res.writeHead(200, { "Content-Type": "text/plain" });
  res.end("Hello, World!");
});

server.listen(3000, () => console.log("Server running on port 3000"));
```

## Key Points:
- Built-in HTTP server and client.
- Foundation for Express.js and other frameworks.
- `createServer()` creates an HTTP server.
- Handles requests and responses.
- Also includes `http.request()` for making HTTP requests.

## Interview Tip:
"Express.js wraps the `http` module with routing, middleware, and convenience methods."

---

## Question 142: How do you create a basic HTTP server using Node.js?

## Answer:
```js
const http = require("http");

const server = http.createServer((req, res) => {
  if (req.url === "/" && req.method === "GET") {
    res.writeHead(200, { "Content-Type": "application/json" });
    res.end(JSON.stringify({ message: "Hello, World!" }));
  } else if (req.url === "/users" && req.method === "GET") {
    res.writeHead(200, { "Content-Type": "application/json" });
    res.end(JSON.stringify([{ id: 1, name: "Alice" }]));
  } else {
    res.writeHead(404);
    res.end("Not Found");
  }
});

server.listen(3000);
```

## Key Points:
- `http.createServer()` creates a server.
- Callback receives `req` (request) and `res` (response).
- Set headers with `writeHead()`.
- Send response with `end()`.
- Manual routing based on `req.url` and `req.method`.

## Interview Tip:
"For anything beyond a simple server, use Express.js. The native `http` module requires manual routing."

---

## Question 143: How do you handle incoming requests and responses?

## Answer:
```js
const http = require("http");

const server = http.createServer((req, res) => {
  // Request info
  console.log(req.method);  // "GET", "POST"
  console.log(req.url);     // "/users"
  console.log(req.headers); // Request headers

  // Read request body
  let body = "";
  req.on("data", (chunk) => { body += chunk; });
  req.on("end", () => {
    const data = JSON.parse(body);
    // Process data
  });

  // Response
  res.writeHead(200, { "Content-Type": "application/json" });
  res.end(JSON.stringify({ success: true }));
});
```

## Key Points:
- `req.method`: HTTP method (GET, POST, etc.).
- `req.url`: Request URL path.
- `req.headers`: Request headers.
- `req.on("data")`: Read request body chunks.
- `res.writeHead()`: Set status and headers.
- `res.end()`: Send response.

## Interview Tip:
"Request bodies come in chunks â€” collect them with `req.on('data')` and process in `req.on('end')`."

---

## Question 144: What is the difference between the `http` module and Express.js?

## Answer:
| Feature | `http` module | Express.js |
|---------|--------------|------------|
| Routing | Manual URL checking | Built-in router |
| Middleware | None | Rich middleware ecosystem |
| Request parsing | Manual | Automatic (body-parser) |
| Error handling | Manual | Error middleware |
| Learning curve | Steep | Moderate |
| Flexibility | Maximum | Framework conventions |

Express.js is built on top of `http` and provides a much better developer experience.

## Key Points:
- `http`: low-level, manual everything.
- Express: high-level, routing, middleware, parsing.
- Express is built on `http`.
- Express has a massive middleware ecosystem.
- Use `http` for minimal servers; Express for real applications.

## Interview Tip:
"Express is the `http` module with superpowers â€” routing, middleware, and conventions."

---

## Question 145: When would you use the native `http` module instead of Express?

## Answer:
- **Minimal servers**: Simple proxy or health check endpoint.
- **Performance-critical**: Avoiding Express overhead for high-throughput services.
- **Learning purposes**: Understanding how HTTP works under the hood.
- **Serverless functions**: Where minimal bundle size matters.
- **Custom middleware**: When you need full control over request processing.

For most applications, Express (or Fastify) is the better choice.

## Key Points:
- Minimal, lightweight servers.
- Performance-critical applications.
- Learning and understanding HTTP fundamentals.
- Serverless where bundle size matters.
- Custom processing without framework overhead.

## Interview Tip:
"For production APIs, I'd choose Express or Fastify over raw `http`. The `http` module is for learning or very specific use cases."

---

## Question 146: What are child processes in Node.js?

## Answer:
Child processes let you spawn separate processes from Node.js â€” useful for running shell commands, executing scripts in other languages, or offloading CPU-heavy work.

```js
const { exec } = require("child_process");

exec("ls -la", (err, stdout, stderr) => {
  console.log(stdout);
});
```

Child processes have their own memory and V8 instance, independent from the parent.

## Key Points:
- Spawn separate OS processes.
- Independent memory and V8 instance.
- Useful for shell commands and scripts.
- Four methods: `spawn`, `exec`, `execFile`, `fork`.
- Communication via stdin/stdout or IPC.

## Interview Tip:
"Child processes are for running external commands â€” shell scripts, system utilities, or CPU-heavy operations."

---

## Question 147: What is the difference between `spawn()`, `exec()`, `execFile()`, and `fork()`?

## Answer:
| Method | Use Case | Returns |
|--------|----------|---------|
| `spawn()` | Large data, streaming | Child process object |
| `exec()` | Shell commands, small output | Buffer via callback |
| `execFile()` | Execute a file without shell | Buffer via callback |
| `fork()` | Node.js modules, IPC | Child process with IPC channel |

- `spawn`: streams output, doesn't buffer.
- `exec`: buffers output (max 1MB), uses shell.
- `execFile`: like `exec` but no shell.
- `fork`: for Node.js modules, enables IPC.

## Key Points:
- `spawn`: streaming, no buffering, shell optional.
- `exec`: buffers output, uses shell.
- `execFile`: no shell, buffers output.
- `fork`: Node.js-specific, IPC channel for communication.
- Use `spawn` for large data; `exec` for small commands.

## Interview Tip:
"`spawn` for streaming, `exec` for small commands, `fork` for Node.js modules with IPC."

---

## Question 148: What are Worker Threads?

## Answer:
Worker Threads enable true multi-threading in Node.js. Each Worker runs in its own thread with its own V8 instance, event loop, and memory. Workers communicate with the main thread via message passing.

```js
const { Worker, isMainThread, parentPort } = require("worker_threads");

if (isMainThread) {
  const worker = new Worker(__filename);
  worker.on("message", (msg) => console.log(msg));
  worker.postMessage("start");
} else {
  parentPort.on("message", (msg) => {
    parentPort.postMessage("Worker done");
  });
}
```

## Key Points:
- True multi-threading in Node.js.
- Each Worker has its own V8 instance and memory.
- Communication via message passing.
- Useful for CPU-intensive tasks.
- Don't share memory (SharedArrayBuffer for shared memory).

## Interview Tip:
"Worker Threads are Node.js's answer to CPU-bound tasks â€” they run JavaScript in separate threads."

---

## Question 149: When should you use Worker Threads instead of Child Processes?

## Answer:
- **Worker Threads**: CPU-intensive JavaScript tasks (parsing, computation, data processing). Lighter than child processes.
- **Child Processes**: Running external commands, shell scripts, or non-JavaScript programs.

Worker Threads share memory more efficiently and are faster to spawn than Child Processes.

## Key Points:
- Worker Threads: CPU-intensive JavaScript.
- Child Processes: External commands and scripts.
- Worker Threads are lighter and faster to spawn.
- Worker Threads can share memory (SharedArrayBuffer).
- Child Processes are better for system-level operations.

## Interview Tip:
"Worker Threads for JavaScript CPU work; Child Processes for shell commands and external programs."

---

## Question 150: How do Worker Threads improve CPU-intensive applications?

## Answer:
Without Worker Threads, CPU-intensive work blocks the event loop â€” no other requests can be processed. Worker Threads offload CPU work to separate threads, keeping the main thread responsive.

```js
// Main thread â€” stays responsive
const { Worker } = require("worker_threads");

app.get("/process", (req, res) => {
  const worker = new Worker("./heavy-computation.js");
  worker.on("message", (result) => res.json(result));
  worker.postMessage(data);
});
```

## Key Points:
- CPU work runs in separate threads.
- Main thread stays responsive for I/O.
- Multiple CPU cores are utilized.
- Prevents event loop blocking.
- Ideal for data processing, image manipulation, etc.

## Interview Tip:
"Without Worker Threads, a single CPU-heavy request blocks ALL other requests. Worker Threads prevent that."

---

## Part 16 (151â€“160): Performance Optimization

---

## Question 151: How do you improve the performance of a Node.js application?

## Answer:
- **Non-blocking I/O**: Always use async operations.
- **Caching**: Redis, in-memory cache for frequently accessed data.
- **Database optimization**: Indexes, query optimization, connection pooling.
- **Code splitting**: Load only what's needed.
- **Compression**: gzip/brotli for HTTP responses.
- **Clustering**: Use all CPU cores.
- **Worker Threads**: Offload CPU-intensive work.
- **Monitoring**: Profile and identify bottlenecks.

## Key Points:
- Async I/O is the foundation.
- Caching reduces database load.
- Database optimization prevents slow queries.
- Clustering utilizes multiple cores.
- Worker Threads prevent event loop blocking.

## Interview Tip:
"Start with async I/O and caching â€” they give the biggest performance wins."

---

## Question 152: What are the most common performance bottlenecks in Node.js?

## Answer:
- **Synchronous operations**: Blocking the event loop.
- **Slow database queries**: Missing indexes, N+1 queries.
- **Memory leaks**: Growing memory usage over time.
- **Event loop blocking**: CPU-intensive tasks on the main thread.
- **No caching**: Hitting the database for every request.
- **Large payloads**: Sending/receiving huge data without streaming.
- **Too many dependencies**: Large bundle sizes.

## Key Points:
- Synchronous code blocks the event loop.
- Database queries are the most common bottleneck.
- Memory leaks cause crashes over time.
- CPU work on the main thread blocks everything.
- Caching prevents redundant computation.

## Interview Tip:
"Profile first, optimize second. Don't guess â€” measure."

---

## Question 153: How do you identify performance issues?

## Answer:
1. **Profiling**: Use Node.js inspector to profile CPU and memory.
2. **APM tools**: Datadog, New Relic, or PM2 for monitoring.
3. **Logging**: Track response times and slow queries.
4. **Load testing**: Artillery or k6 to simulate traffic.
5. **Process monitoring**: `process.memoryUsage()` and `process.cpuUsage()`.

## Key Points:
- Profiling identifies CPU bottlenecks.
- APM tools provide real-time monitoring.
- Load testing simulates production traffic.
- Logging tracks slow operations.
- Process monitoring catches memory issues.

## Interview Tip:
"Use the Node.js inspector and Chrome DevTools to profile â€” it's built-in and powerful."

---

## Question 154: What tools do you use to profile a Node.js application?

## Answer:
- **Node.js Inspector**: Built-in, connect with Chrome DevTools.
- **Clinic.js**: Performance profiling and diagnosis.
- **0x**: Flame graph profiling.
- **Autocannon**: HTTP load testing.
- **Clinic Doctor**: Diagnoses common issues.
- **process.memoryUsage()**: Runtime memory monitoring.

```bash
node --inspect server.js
# Open chrome://inspect in Chrome
```

## Key Points:
- Node.js Inspector: built-in profiling.
- Clinic.js: comprehensive profiling suite.
- 0x: flame graphs for CPU analysis.
- Autocannon: HTTP load testing.
- Chrome DevTools for visual profiling.

## Interview Tip:
"`node --inspect` + Chrome DevTools is the quickest way to profile Node.js performance."

---

## Question 155: What is the Node.js Inspector?

## Answer:
The Node.js Inspector is a built-in debugging and profiling interface. It uses the Chrome DevTools Protocol, allowing you to connect Chrome DevTools to a running Node.js process.

```bash
node --inspect server.js           # Start with inspector
node --inspect-brk server.js       # Break on first line
```

Then open `chrome://inspect` in Chrome to connect.

## Key Points:
- Built-in debugging and profiling tool.
- Uses Chrome DevTools Protocol.
- Connect via `chrome://inspect`.
- Provides CPU profiling, memory snapshots, and debugging.
- No external tools needed.

## Interview Tip:
"The Node.js Inspector is Chrome DevTools for the server â€” it's incredibly powerful and built-in."

---

## Question 156: How do you analyze CPU usage in Node.js?

## Answer:
1. Start with `node --inspect server.js`.
2. Open Chrome DevTools â†’ Profiler tab.
3. Record a CPU profile while the issue occurs.
4. View the flame graph to find hot functions.
5. Optimize the identified bottlenecks.

```bash
# Or use 0x for flame graphs
npx 0x server.js
```

## Key Points:
- Chrome DevTools profiler for CPU analysis.
- Flame graphs show where CPU time is spent.
- 0x is a simpler alternative for flame graphs.
- Profile under realistic load.
- Focus on the hottest functions first.

## Interview Tip:
"Flame graphs make CPU bottlenecks obvious â€” wide bars are where time is spent."

---

## Question 157: How do you analyze memory usage?

## Answer:
```js
// Check memory usage
console.log(process.memoryUsage());
// { rss, heapTotal, heapUsed, external, arrayBuffers }

// Take heap snapshots with Chrome DevTools
// Memory tab â†’ Take heap snapshot
```

Monitor over time to detect memory leaks:
- `rss`: Total memory allocated to the process.
- `heapTotal`: V8 heap total size.
- `heapUsed`: V8 heap used size.
- `external`: C++ objects bound to JavaScript.

## Key Points:
- `process.memoryUsage()` for current memory.
- Chrome DevTools heap snapshots for analysis.
- Compare snapshots over time to find leaks.
- Growing `heapUsed` indicates a memory leak.
- `rss` includes all memory (heap, stack, etc.).

## Interview Tip:
"Take two heap snapshots â€” one at startup, one after running for a while. Diff them to find leaks."

---

## Question 158: What causes high memory consumption in Node.js?

## Answer:
- **Memory leaks**: Objects not being garbage collected.
- **Large data in memory**: Reading entire files or datasets.
- **Event listener leaks**: Not removing listeners.
- **Closures holding references**: Keeping objects alive unnecessarily.
- **Global variables**: Accumulating data in global scope.
- **Streams not properly closed**: Unclosed file handles.

## Key Points:
- Memory leaks grow over time.
- Large data should be streamed, not loaded.
- Event listener leaks prevent garbage collection.
- Global variables persist indefinitely.
- Monitor memory to catch issues early.

## Interview Tip:
"Memory leaks are the silent killers â€” they work fine in testing but crash in production after hours."

---

## Question 159: How do you optimize database queries in Node.js applications?

## Answer:
1. **Add indexes**: On frequently queried columns.
2. **Avoid N+1 queries**: Use `JOIN` or batch loading.
3. **Use connection pooling**: Reuse database connections.
4. **Select only needed columns**: Don't `SELECT *`.
5. **Cache frequent queries**: Use Redis or in-memory cache.
6. **Batch inserts**: Insert multiple rows in one query.
7. **Use ORM query optimization**: Avoid N+1 with `include`.

```js
// N+1 problem
const users = await db.user.findMany();
for (const user of users) {
  user.posts = await db.post.findMany({ where: { userId: user.id } });
}

// Optimized
const users = await db.user.findMany({ include: { posts: true } });
```

## Key Points:
- Indexes are the most impactful optimization.
- N+1 queries are the most common problem.
- Connection pooling reduces connection overhead.
- Select only needed columns.
- Cache frequently accessed data.

## Interview Tip:
"The N+1 query problem is the most common database performance issue â€” use `include` or batch loading."

---

## Question 160: What are common performance optimization techniques for production systems?

## Answer:
- **Enable compression**: gzip/brotli for HTTP responses.
- **Use a CDN**: Cache static assets globally.
- **Implement caching**: Redis for database queries.
- **Use clustering**: Utilize all CPU cores.
- **Rate limiting**: Prevent abuse and overload.
- **Monitor and alert**: Track metrics and set up alerts.
- **Optimize images**: Compress and resize on the server.
- **Use HTTP/2 or HTTP/3**: Multiplexing and header compression.

## Key Points:
- Compression reduces response size.
- CDN caches static assets globally.
- Redis caching reduces database load.
- Clustering utilizes multiple cores.
- Monitoring catches issues early.

## Interview Tip:
"The best performance optimization is caching â€” it's the cheapest way to reduce server load."

---

## Part 17 (161â€“170): Memory Management

---

## Question 161: How does memory management work in Node.js?

## Answer:
Node.js uses V8's garbage collector for automatic memory management. Memory is divided into:
- **Stack**: Primitive values, function calls (fast, limited size).
- **Heap**: Objects, closures, arrays (larger, garbage collected).

V8's garbage collector automatically frees memory that's no longer referenced. You don't manually allocate or free memory.

## Key Points:
- Automatic memory management via garbage collection.
- Stack for primitives and function calls.
- Heap for objects and complex data.
- V8's GC runs periodically.
- Memory is freed when objects are no longer referenced.

## Interview Tip:
"You don't manage memory manually in Node.js â€” V8's garbage collector handles it. But memory leaks can still happen."

---

## Question 162: What is stack memory?

## Answer:
Stack memory stores primitive values (numbers, strings, booleans) and function call frames. It's fast but limited in size. Each function call adds a frame to the stack; when the function returns, the frame is removed.

```js
function a() {
  let x = 10;       // x is on the stack
  function b() {
    let y = 20;     // y is on the stack
  }
  b();
}
a();
```

Stack overflow happens when too many function calls stack up (infinite recursion).

## Key Points:
- Stores primitives and function call frames.
- Fast access â€” LIFO structure.
- Limited in size.
- Automatically managed â€” no cleanup needed.
- Stack overflow occurs with deep recursion.

## Interview Tip:
"Stack memory is fast but small. Deep recursion can cause stack overflow."

---

## Question 163: What is heap memory?

## Answer:
Heap memory stores objects, closures, arrays, and other complex data structures. It's larger than stack memory but slower to access. V8's garbage collector manages heap memory.

```js
const obj = { name: "Alice" };  // obj is on the stack, { name: "Alice" } is on the heap
const arr = [1, 2, 3];         // arr is on the stack, the array is on the heap
```

The heap is divided into generations for efficient garbage collection.

## Key Points:
- Stores objects, closures, arrays, and complex data.
- Larger than stack but slower access.
- Managed by V8's garbage collector.
- Divided into generations (young and old).
- Most memory leaks happen in the heap.

## Interview Tip:
"Most objects live on the heap â€” that's where memory leaks happen."

---

## Question 164: How does V8 garbage collection work?

## Answer:
V8 uses a generational garbage collector:
- **Young generation**: New objects. Scavenged frequently (fast, short-lived objects).
- **Old generation**: Objects that survived multiple collections. Mark-and-sweep less frequently.

The Mark-and-Sweep algorithm:
1. Mark all reachable objects (from roots like global, stack).
2. Sweep (free) all unmarked objects.

## Key Points:
- Generational GC: young and old generations.
- Young generation: frequent, fast collections.
- Old generation: less frequent, mark-and-sweep.
- Roots: global object, call stack, current scope.
- Unreachable objects are garbage collected.

## Interview Tip:
"V8's GC is generational â€” short-lived objects are collected quickly; long-lived objects are collected less frequently."

---

## Question 165: What are memory leaks in Node.js?

## Answer:
Memory leaks occur when objects are no longer needed but are still referenced, preventing garbage collection. The application's memory usage grows over time until it crashes.

Common causes:
- Event listeners not removed.
- Closures holding references.
- Global variables accumulating data.
- Unclosed file handles or connections.
- Caches without size limits.

## Key Points:
- Objects referenced but no longer needed.
- GC can't free them â€” memory grows.
- Common causes: event listeners, closures, globals.
- Accumulates over time â€” crashes in production.
- Monitor memory to detect leaks.

## Interview Tip:
"Memory leaks are invisible during testing â€” they only show up after running for hours or days."

---

## Question 166: What are common causes of memory leaks?

## Answer:
1. **Event listener leaks**: Adding listeners without removing them.
2. **Closures**: Functions that capture and hold large objects.
3. **Global variables**: Accumulating data in global scope.
4. **Unclosed resources**: File handles, database connections.
5. **Unbounded caches**: Caches that grow without limits.
6. **Timers**: `setInterval` not cleared.
7. **Streams not closed**: Unclosed readable/writable streams.

## Key Points:
- Event listeners are the most common cause.
- Closures keep objects alive longer than expected.
- Global variables persist indefinitely.
- Always close resources (files, connections, streams).
- Set size limits on caches.

## Interview Tip:
"Event listener leaks are the most common memory leak in Node.js â€” always remove them."

---

## Question 167: How do you detect memory leaks?

## Answer:
1. **Monitor memory over time**: Track `process.memoryUsage()` â€” growing `heapUsed` indicates a leak.
2. **Heap snapshots**: Take snapshots with Chrome DevTools and compare.
3. **Clinic.js**: Automated memory leak detection.
4. **Node.js `--inspect`**: Profile memory usage.
5. **Process monitoring**: PM2, Datadog, or similar tools.

```js
setInterval(() => {
  const { heapUsed } = process.memoryUsage();
  console.log(`Heap used: ${Math.round(heapUsed / 1024 / 1024)} MB`);
}, 10000);
```

## Key Points:
- Monitor heap usage over time.
- Compare heap snapshots to find growing objects.
- Clinic.js automates leak detection.
- Growing heap = likely memory leak.
- Profile in production-like conditions.

## Interview Tip:
"If heap usage keeps growing, you have a memory leak. Take snapshots and diff them."

---

## Question 168: How do closures contribute to memory leaks?

## Answer:
A closure captures variables from its outer scope. If the closure is long-lived (e.g., stored in a global variable or event listener), it keeps the captured variables alive â€” even if nothing else references them.

```js
function createHandler() {
  const largeData = new Array(1000000).fill("data");
  return function handler() {
    // largeData is captured and can't be garbage collected
    console.log("handling");
  };
}
const handler = createHandler(); // largeData is still in memory
```

## Key Points:
- Closures capture outer scope variables.
- Long-lived closures keep captured objects alive.
- Prevents garbage collection of captured data.
- Solution: minimize captured data or nullify references.

## Interview Tip:
"Closures are powerful but can keep objects alive longer than expected â€” be careful with what you capture."

---

## Question 169: How do event listeners cause memory leaks?

## Answer:
When you add event listeners with `on()` and never remove them, the listener function and everything it references stays in memory. Over time, accumulating listeners consume more and more memory.

```js
// Leak: listener never removed
emitter.on("data", () => console.log("data"));
emitter.on("data", () => console.log("data"));
// After 1000 emits, 1000 listeners exist

// Fix: use once() or removeListener()
emitter.once("data", () => console.log("data")); // Auto-removes
```

## Key Points:
- Each listener stays in memory until removed.
- Accumulating listeners consume memory.
- `once()` auto-removes after first emission.
- Always remove listeners in cleanup code.
- MaxListeners warning indicates a potential leak.

## Interview Tip:
"Event listener leaks are the #1 memory leak in Node.js. Use `once()` or always call `removeListener()`."

---

## Question 170: What best practices help prevent memory leaks?

## Answer:
1. **Remove event listeners** when done.
2. **Use `once()`** for one-time listeners.
3. **Set cache size limits** (e.g., LRU cache with max size).
4. **Close file handles and connections** after use.
5. **Avoid global variables** for accumulating data.
6. **Nullify references** when objects are no longer needed.
7. **Monitor memory** in production.
8. **Use weak references** when appropriate (`WeakMap`, `WeakSet`).

## Key Points:
- Always clean up event listeners.
- Set limits on caches.
- Close resources when done.
- Avoid global state.
- Monitor memory in production.
- `WeakMap` and `WeakSet` don't prevent garbage collection.

## Interview Tip:
"Prevention is better than detection â€” clean up resources and set limits from the start."

---

## Part 18 (171â€“180): Scaling Node.js Applications

---

## Question 171: What is clustering in Node.js?

## Answer:
Clustering lets you run multiple Node.js instances (workers) on a single machine, each handling requests independently. The master process distributes incoming connections across workers.

```js
const cluster = require("cluster");
const http = require("http");
const numCPUs = require("os").cpus().length;

if (cluster.isPrimary) {
  for (let i = 0; i < numCPUs; i++) {
    cluster.fork();
  }
} else {
  http.createServer((req, res) => {
    res.end("Hello from worker " + process.pid);
  }).listen(3000);
}
```

## Key Points:
- Run multiple Node.js instances on one machine.
- Master process distributes connections.
- Each worker has its own event loop and memory.
- Utilizes all CPU cores.
- Increases throughput and fault tolerance.

## Interview Tip:
"Clustering is how Node.js uses multiple CPU cores â€” one process per core."

---

## Question 172: Why would you use the Cluster module?

## Answer:
Node.js is single-threaded â€” it can only use one CPU core. Clustering lets you use all available cores by running multiple worker processes. This:
- Increases throughput (more requests per second).
- Provides fault tolerance (if one worker crashes, others continue).
- Utilizes all CPU cores on the machine.

## Key Points:
- Node.js uses only one core by default.
- Clustering utilizes all available cores.
- Increases throughput proportionally.
- Provides fault tolerance.
- Each worker is an independent process.

## Interview Tip:
"A single Node.js process uses one core. Clustering gives you N cores for N workers."

---

## Question 173: How does the Cluster module work?

## Answer:
1. The **master process** forks worker processes.
2. Each **worker** runs an independent Node.js instance.
3. The master uses the OS to distribute connections (round-robin by default).
4. Workers share the same port (the master listens, workers handle requests).
5. Workers communicate with the master via IPC.

```js
if (cluster.isPrimary) {
  // Master: fork workers
  for (let i = 0; i < numCPUs; i++) cluster.fork();
} else {
  // Worker: handle requests
  server.listen(3000);
}
```

## Key Points:
- Master forks workers.
- Workers share the same port.
- Round-robin distribution by default.
- Workers communicate via IPC.
- Workers are independent processes.

## Interview Tip:
"Workers share the port through the master â€” the OS handles distribution."

---

## Question 174: What is load balancing?

## Answer:
Load balancing distributes incoming requests across multiple servers or processes. In Node.js clustering, the master process acts as a load balancer, distributing requests across workers.

Common load balancers:
- **Node.js cluster**: Built-in, single machine.
- **Nginx**: Reverse proxy, multiple machines.
- **AWS ALB**: Cloud load balancing.
- **PM2**: Process manager with clustering.

## Key Points:
- Distributes requests across multiple instances.
- Increases throughput and availability.
- Node.js cluster: built-in, single machine.
- Nginx, ALB: multi-machine load balancing.
- Prevents any single instance from being overwhelmed.

## Interview Tip:
"Load balancing is essential for scaling â€” whether it's clustering on one machine or multiple servers."

---

## Question 175: How do you scale a Node.js application horizontally?

## Answer:
Horizontal scaling means adding more machines (or containers) behind a load balancer:

1. **Containerize** the app with Docker.
2. **Deploy multiple instances** on different machines.
3. **Use a load balancer** (Nginx, ALB) to distribute traffic.
4. **Externalize state**: Use Redis for sessions, not in-memory.
5. **Use a shared database**: All instances connect to the same DB.

```bash
# Run multiple instances on different ports
PORT=3001 node server.js &
PORT=3002 node server.js &
PORT=3003 node server.js &
```

## Key Points:
- Add more machines behind a load balancer.
- Containerize with Docker for consistency.
- Externalize state (Redis, databases).
- Don't store sessions in memory â€” use Redis.
- Each instance should be stateless.

## Interview Tip:
"Stateless services scale horizontally. If you store sessions in memory, you're stuck with one machine."

---

## Question 176: What is horizontal scaling?

## Answer:
Horizontal scaling (scaling out) means adding more machines to handle increased load. Each machine runs its own instance of the application, and a load balancer distributes traffic across them.

Contrast with vertical scaling (scaling up) â€” adding more CPU/RAM to a single machine.

## Key Points:
- Add more machines (not more power per machine).
- Each machine runs an independent instance.
- Load balancer distributes traffic.
- More resilient â€” if one machine fails, others continue.
- More cost-effective at scale.

## Interview Tip:
"Horizontal scaling = more machines. Vertical scaling = bigger machine. Horizontal is usually better for large-scale systems."

---

## Question 177: What is vertical scaling?

## Answer:
Vertical scaling (scaling up) means adding more CPU, RAM, or storage to a single machine. It's simpler than horizontal scaling but has limits â€” a single machine can only be so powerful.

## Key Points:
- Add more resources to a single machine.
- Simpler than horizontal scaling.
- Limited by hardware maximums.
- No load balancer needed.
- Single point of failure.

## Interview Tip:
"Vertical scaling is fine for small to medium apps. For large-scale, you need horizontal scaling."

---

## Question 178: When should you use Worker Threads instead of clustering?

## Answer:
- **Worker Threads**: CPU-intensive JavaScript tasks (parsing, computation). Lighter, share memory more efficiently.
- **Clustering**: Scaling I/O across CPU cores. Each worker handles HTTP requests independently.

Use Worker Threads for CPU work within a single process. Use clustering to scale across cores for I/O.

## Key Points:
- Worker Threads: CPU-intensive tasks.
- Clustering: I/O scaling across cores.
- Worker Threads are lighter and faster.
- Clustering is better for HTTP server scaling.
- They can be used together.

## Interview Tip:
"Worker Threads for computation; Clustering for I/O scaling. They complement each other."

---

## Question 179: How do you manage sessions in a clustered application?

## Answer:
Don't store sessions in memory â€” each worker has its own memory. Use an external session store:

- **Redis**: Most common for session storage.
- **Database**: PostgreSQL, MongoDB for session persistence.
- **JWT**: Stateless sessions â€” no server-side storage needed.

```js
const session = require("express-session");
const RedisStore = require("connect-redis").default;
const redis = require("redis");

const client = redis.createClient();
app.use(session({
  store: new RedisStore({ client }),
  secret: "your-secret"
}));
```

## Key Points:
- Don't use in-memory sessions in clustering.
- Redis is the most common session store.
- JWT provides stateless sessions.
- Database-backed sessions for persistence.
- All workers share the same session store.

## Interview Tip:
"Sessions in memory + clustering = lost sessions. Use Redis or JWT."

---

## Question 180: What challenges arise when scaling Node.js applications?

## Answer:
- **Session management**: Can't use in-memory sessions.
- **State sharing**: Workers don't share state.
- **Database connection limits**: Too many connections overwhelm the DB.
- **Deployment complexity**: More instances = more deployment work.
- **Monitoring**: Need to monitor multiple instances.
- **Debugging**: Harder to reproduce issues across instances.
- **Rate limiting**: Need distributed rate limiting (Redis).

## Key Points:
- Session management requires external stores.
- Database connections need pooling.
- Deployment complexity increases.
- Monitoring and debugging become harder.
- Distributed state management is challenging.

## Interview Tip:
"Scaling isn't just adding machines â€” it's solving the problems that come with multiple instances."

---

## Part 19 (181â€“190): Security

---

## Question 181: How do you secure a Node.js application?

## Answer:
1. **Input validation**: Validate and sanitize all user input.
2. **Authentication**: Use JWT or sessions with secure cookies.
3. **Authorization**: Check permissions on every request.
4. **HTTPS**: Encrypt data in transit.
5. **Rate limiting**: Prevent brute force and DDoS.
6. **Security headers**: Use Helmet.js.
7. **Dependency auditing**: Check for vulnerabilities.
8. **Environment variables**: Keep secrets out of code.
9. **SQL injection prevention**: Use parameterized queries.
10. **XSS prevention**: Escape output, use CSP.

## Key Points:
- Validate all input server-side.
- Use HTTPS everywhere.
- Rate limiting prevents abuse.
- Security headers with Helmet.
- Audit dependencies regularly.
- Never expose secrets to the client.

## Interview Tip:
"Security is defense in depth â€” no single measure is enough. Layer multiple protections."

---

## Question 182: What are the most common security vulnerabilities in Node.js?

## Answer:
- **SQL/NoSQL injection**: Unsanitized user input in queries.
- **XSS**: Injecting malicious scripts into pages.
- **CSRF**: Forged requests from other sites.
- **Broken authentication**: Weak passwords, exposed tokens.
- **Sensitive data exposure**: Secrets in code or logs.
- **Dependency vulnerabilities**: Outdated packages with known issues.
- **Path traversal**: Accessing files outside intended directories.

## Key Points:
- Injection attacks are the most common.
- Authentication issues are frequent.
- Dependency vulnerabilities affect many apps.
- Sensitive data exposure is catastrophic.
- OWASP Top 10 applies to Node.js.

## Interview Tip:
"The OWASP Top 10 applies to Node.js just like any other web framework."

---

## Question 183: How do you prevent SQL Injection?

## Answer:
Use parameterized queries or an ORM â€” never concatenate user input into SQL strings.

```js
// VULNERABLE â€” never do this
const query = `SELECT * FROM users WHERE id = '${userId}'`;

// Safe â€” parameterized query
const query = "SELECT * FROM users WHERE id = $1";
const result = await db.query(query, [userId]);

// Safe â€” ORM (Prisma)
const user = await prisma.user.findUnique({ where: { id: userId } });
```

## Key Points:
- Never concatenate user input into SQL.
- Use parameterized queries or prepared statements.
- ORMs (Prisma, TypeORM) handle this automatically.
- Sanitize input before using in queries.
- Least privilege: DB user should have minimal permissions.

## Interview Tip:
"Parameterized queries prevent SQL injection â€” it's that simple."

---

## Question 184: How do you prevent NoSQL Injection?

## Answer:
NoSQL injection occurs when user input is used directly in MongoDB queries. Attackers can inject operators like `$gt`, `$ne`, or `$regex`.

```js
// VULNERABLE
const user = await User.findOne({ username: req.body.username });

// Safe â€” validate types
const username = String(req.body.username);
const user = await User.findOne({ username });

// Safe â€” use Mongoose validation
const user = await User.findOne({ username: { $type: "string", $eq: username } });
```

## Key Points:
- Validate input types before queries.
- Don't pass raw user input to queries.
- Use schema validation (Mongoose, Joi).
- Sanitize and cast input to expected types.
- Use `$eq` operator for explicit comparison.

## Interview Tip:
"Validate that input is the expected type â€” a string should be a string, not an object."

---

## Question 185: How do you prevent Cross-Site Scripting (XSS)?

## Answer:
1. **Escape output**: React escapes JSX by default; in templates, escape HTML.
2. **Content Security Policy (CSP)**: Restrict which scripts can run.
3. **HTTP-only cookies**: Prevent JavaScript access to auth cookies.
4. **Sanitize HTML**: Use DOMPurify for user-generated HTML.
5. **Input validation**: Reject or sanitize potentially malicious input.

```js
const helmet = require("helmet");
app.use(helmet()); // Adds security headers including CSP
```

## Key Points:
- Escape output to prevent script injection.
- CSP headers restrict script sources.
- HTTP-only cookies prevent cookie theft.
- Sanitize user-generated HTML with DOMPurify.
- Input validation prevents malicious content.

## Interview Tip:
"Helmet.js adds security headers including CSP â€” it's a quick win for XSS prevention."

---

## Question 186: How do you prevent Cross-Site Request Forgery (CSRF)?

## Answer:
1. **SameSite cookies**: Set `SameSite=Strict` or `SameSite=Lax`.
2. **CSRF tokens**: Generate per-session tokens, validate on mutations.
3. **Origin/Referer checks**: Verify request origin.
4. **Double Submit Cookie**: Token in both cookie and header.

```js
const csrf = require("csurf");
const csrfProtection = csrf({ cookie: true });
app.use(csrfProtection);
```

## Key Points:
- SameSite cookies are the primary defense.
- CSRF tokens add a second layer.
- Origin checks verify request source.
- Most frameworks provide CSRF protection.
- SameSite=Lax prevents most CSRF attacks.

## Interview Tip:
"SameSite cookies prevent most CSRF attacks automatically. Add CSRF tokens as a second layer."

---

## Question 187: How do you securely store passwords?

## Answer:
Use bcrypt, scrypt, or argon2 â€” never plain text or MD5/SHA.

```js
const bcrypt = require("bcrypt");

// Hash password (cost factor 12)
const hashedPassword = await bcrypt.hash("userPassword", 12);

// Verify password
const isMatch = await bcrypt.compare("userPassword", hashedPassword);
```

- **bcrypt**: Auto-salts, slow by design (brute-force resistant).
- **scrypt**: Memory-hard, resistant to GPU attacks.
- **argon2**: Modern, memory-hard, winner of the Password Hashing Competition.

## Key Points:
- Use bcrypt, scrypt, or argon2.
- Never MD5 or SHA for passwords.
- bcrypt auto-salts and is slow by design.
- Cost factor (12+) controls hashing speed.
- Compare with `bcrypt.compare()`, not `hash()`.

## Interview Tip:
"Never roll your own password hashing â€” use bcrypt. It's slow on purpose to prevent brute-force attacks."

---

## Question 188: Why should you use environment variables for secrets?

## Answer:
Environment variables keep secrets out of your codebase. If secrets are in code, they're visible to anyone with repository access. Environment variables:
- Are not committed to version control.
- Can be different per environment (dev, staging, prod).
- Are managed by the deployment platform.
- Can be rotated without code changes.

```js
const dbUrl = process.env.DATABASE_URL; // Not in code
```

## Key Points:
- Secrets in code = public secrets.
- Environment variables are not in version control.
- Different values per environment.
- Can be rotated without deploying code.
- Use `.env` files in development (gitignored).

## Interview Tip:
"Never commit secrets to git. Use environment variables and .env files."

---

## Question 189: How do you validate and sanitize user input?

## Answer:
Use Zod, Joi, or similar validation libraries:

```js
const { z } = require("zod");

const UserSchema = z.object({
  name: z.string().min(1).max(100),
  email: z.string().email(),
  age: z.number().int().min(0).max(150)
});

const result = UserSchema.safeParse(req.body);
if (!result.success) {
  return res.status(400).json({ errors: result.error.flatten() });
}
```

## Key Points:
- Validate all external input server-side.
- Use schema validation (Zod, Joi, Yup).
- Validate types, ranges, and formats.
- Sanitize HTML input to prevent XSS.
- Never trust client-side validation alone.

## Interview Tip:
"Zod is my go-to for validation â€” it gives me runtime safety and TypeScript types in one step."

---

## Question 190: What authentication and authorization best practices do you follow?

## Answer:
1. **Use established libraries**: Auth.js, Passport.js, Lucia.
2. **Hash passwords**: bcrypt with cost factor 12+.
3. **Use HTTP-only cookies**: For session tokens.
4. **Implement rate limiting**: On login endpoints.
5. **Use MFA**: Multi-factor authentication for sensitive accounts.
6. **Least privilege**: Users only get necessary permissions.
7. **Audit logs**: Track authentication events.
8. **Rotate secrets**: Regularly rotate tokens and keys.

## Key Points:
- Use established auth libraries.
- Hash passwords with bcrypt.
- Secure token storage (HTTP-only cookies).
- Rate limit authentication endpoints.
- Implement MFA for security.
- Track authentication events.

## Interview Tip:
"Don't build auth from scratch â€” use Auth.js or Passport.js. They handle the edge cases you'd miss."

---

## Part 20 (191â€“200): Production & Deployment

---

## Question 191: How do you prepare a Node.js application for production?

## Answer:
1. **Environment variables**: Use `.env` for development, platform secrets for production.
2. **Error handling**: Centralized error handler, `uncaughtException` and `unhandledRejection` handlers.
3. **Logging**: Structured logging (Pino/Winston).
4. **Security**: Helmet, CORS, rate limiting, input validation.
5. **Graceful shutdown**: Handle SIGTERM/SIGINT signals.
6. **Health checks**: `/health` endpoint for monitoring.
7. **Process manager**: PM2 for clustering and restarts.
8. **Monitoring**: Sentry for errors, APM for performance.

## Key Points:
- Environment configuration for each stage.
- Graceful shutdown handling.
- Structured logging for debugging.
- Security middleware and headers.
- Process management with PM2.
- Health checks for load balancers.

## Interview Tip:
"Production-ready means: error handling, logging, security, graceful shutdown, and monitoring."

---

## Question 192: How do you manage configuration across environments?

## Answer:
Use environment variables with a configuration module:

```js
// config.js
module.exports = {
  port: process.env.PORT || 3000,
  dbUrl: process.env.DATABASE_URL,
  jwtSecret: process.env.JWT_SECRET,
  logLevel: process.env.LOG_LEVEL || "info",
  isProd: process.env.NODE_ENV === "production"
};
```

- Development: `.env` file (gitignored).
- Staging/Production: Platform secrets (Vercel, AWS, Docker).
- Never commit `.env` files.

## Key Points:
- Environment variables for all configuration.
- `.env` file for local development.
- Platform secrets for production.
- Config module for centralized access.
- Default values for optional settings.

## Interview Tip:
"Use a config module that reads from environment variables â€” it centralizes configuration and provides defaults."

---

## Question 193: What logging libraries have you used?

## Answer:
- **Pino**: Fast, structured JSON logging. My preferred choice.
- **Winston**: Feature-rich, multiple transports.
- **Bunyan**: JSON logging, similar to Pino.
- **Morgan**: HTTP request logging for Express.

```js
const pino = require("pino");
const logger = pino({ level: "info" });

logger.info({ userId: 123, action: "login" }, "User logged in");
```

## Key Points:
- Pino: fast, structured, JSON output.
- Winston: flexible, multiple transports.
- Morgan: HTTP request logging.
- Structured logging (JSON) is essential for production.
- Never use `console.log` in production.

## Interview Tip:
"Pino is my go-to for production logging â€” it's fast and outputs structured JSON."

---

## Question 194: What monitoring tools have you used?

## Answer:
- **Sentry**: Error tracking and performance monitoring.
- **Datadog**: Full-stack APM and infrastructure monitoring.
- **New Relic**: Application performance monitoring.
- **PM2**: Process monitoring and management.
- **Prometheus + Grafana**: Metrics and dashboards.
- **Uptime monitoring**: Pingdom, UptimeRobot.

## Key Points:
- Sentry for error tracking.
- APM tools for performance monitoring.
- PM2 for process management.
- Prometheus + Grafana for custom metrics.
- Set up alerts for critical issues.

## Interview Tip:
"Sentry for errors, PM2 for process management, Datadog for APM â€” that's my monitoring stack."

---

## Question 195: How do you handle uncaught exceptions?

## Answer:
```js
process.on("uncaughtException", (err) => {
  logger.fatal({ err }, "Uncaught exception");
  // Log the error, then exit gracefully
  process.exit(1);
});
```

Uncaught exceptions indicate bugs â€” the process state is unreliable. Log the error and restart the process.

## Key Points:
- Uncaught exceptions indicate programmer errors.
- Log the error with full context.
- Exit the process â€” state may be corrupted.
- Let the process manager (PM2) restart it.
- Don't try to continue â€” the state is unreliable.

## Interview Tip:
"Uncaught exceptions mean the process state is unreliable â€” log it and restart. Don't try to continue."

---

## Question 196: How do you handle unhandled Promise rejections?

## Answer:
```js
process.on("unhandledRejection", (reason, promise) => {
  logger.fatal({ reason }, "Unhandled promise rejection");
  // In Node.js 15+, this crashes the process by default
});
```

Prevention: Always handle promise rejections with `.catch()` or `try/catch` with `async/await`.

## Key Points:
- Unhandled rejections crash in Node.js 15+.
- Always handle rejections explicitly.
- Log with full context for debugging.
- Global handler is a safety net, not a strategy.
- Use `try/catch` with `async/await`.

## Interview Tip:
"Node.js 15+ crashes on unhandled rejections â€” handle them explicitly or your server will crash."

---

## Question 197: What is graceful shutdown, and why is it important?

## Answer:
Graceful shutdown means finishing in-flight requests before closing the server. Without it, active connections are abruptly terminated, causing data loss or errors.

```js
process.on("SIGTERM", async () => {
  logger.info("SIGTERM received, shutting down gracefully");
  server.close(() => {
    logger.info("Server closed");
    process.exit(0);
  });
  // Close database connections, flush logs, etc.
});
```

## Key Points:
- Finish in-flight requests before closing.
- Close database connections cleanly.
- Flush logs and buffers.
- Handle SIGTERM and SIGINT signals.
- Essential for zero-downtime deployments.

## Interview Tip:
"Graceful shutdown means no request is lost during deployment â€” finish what's in progress, then close."

---

## Question 198: How do you deploy a Node.js application using Docker?

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

```bash
docker build -t my-app .
docker run -p 3000:3000 -e DATABASE_URL=... my-app
```

## Key Points:
- Multi-stage build for smaller images.
- `npm ci` for reproducible installs.
- `.dockerignore` to exclude unnecessary files.
- Use alpine images for smaller size.
- Environment variables via `-e` flag or secrets.

## Interview Tip:
"Use `npm ci` instead of `npm install` in Docker â€” it's faster and more reproducible."

---

## Question 199: How do you deploy Node.js applications to cloud platforms such as AWS or DigitalOcean?

## Answer:
- **AWS**: EC2 (VMs), ECS (containers), Lambda (serverless), Elastic Beanstalk (managed).
- **DigitalOcean**: Droplets (VMs), App Platform (PaaS), Kubernetes.
- **Railway/Render**: Simple PaaS for quick deploys.
- **Vercel/Netlify**: Serverless deployment for APIs.

Steps:
1. Containerize with Docker.
2. Push to container registry (ECR, Docker Hub).
3. Deploy to container service (ECS, DigitalOcean Kubernetes).
4. Set environment variables.
5. Configure health checks and auto-scaling.

## Key Points:
- AWS: EC2, ECS, Lambda, Beanstalk.
- DigitalOcean: Droplets, App Platform, Kubernetes.
- PaaS options: Railway, Render.
- Containerize with Docker for portability.
- Environment variables for configuration.

## Interview Tip:
"For most projects, a PaaS like Railway or Render is faster than managing EC2. Use ECS when you need more control."

---

## Question 200: What production best practices do you follow before releasing a Node.js application?

## Answer:
1. **Type checking**: `tsc --noEmit` for TypeScript projects.
2. **Linting**: ESLint with strict rules.
3. **Testing**: Unit, integration, and E2E tests.
4. **Security audit**: `npm audit` for vulnerabilities.
5. **Performance profiling**: Identify bottlenecks.
6. **Error handling**: Verify all error paths work.
7. **Logging**: Structured logging in place.
8. **Graceful shutdown**: Handle SIGTERM.
9. **Health checks**: `/health` endpoint.
10. **Environment variables**: All secrets configured.

## Key Points:
- Type checking and linting catch bugs early.
- Tests verify correctness.
- Security audit prevents vulnerabilities.
- Error handling prevents crashes.
- Graceful shutdown prevents data loss.
- Health checks enable monitoring.

## Interview Tip:
"I have a pre-deploy checklist: type check, lint, test, audit, profile, and verify error handling."

---

## Part 21 (201â€“210): Project Architecture

---

## Question 201: How do you structure a large Node.js application?

## Answer:
```
src/
  controllers/     # Request handlers
  services/        # Business logic
  repositories/    # Database access
  models/          # Data models/schemas
  middleware/      # Express middleware
  routes/          # Route definitions
  utils/           # Helper functions
  config/          # Configuration
  validators/      # Input validation schemas
  errors/          # Custom error classes
  app.js           # Express app setup
  server.js        # Server startup
```

Separation of concerns: controllers handle HTTP, services handle logic, repositories handle data.

## Key Points:
- Separate concerns: controllers, services, repositories.
- Each layer has a single responsibility.
- Business logic in services, not controllers.
- Database access in repositories.
- Configuration separated from code.

## Interview Tip:
"Controllers handle HTTP, services handle business logic, repositories handle data. Never mix these."

---

## Question 202: What folder structure do you prefer for enterprise Node.js projects?

## Answer:
Feature-based structure for large projects:

```
src/
  features/
    auth/
      auth.controller.js
      auth.service.js
      auth.routes.js
      auth.validation.js
    users/
      users.controller.js
      users.service.js
      users.repository.js
      users.routes.js
  shared/
    middleware/
    utils/
    errors/
    config/
  app.js
```

Each feature is self-contained. Shared code in `shared/`.

## Key Points:
- Feature-based organization for scalability.
- Each feature has its own controller, service, routes.
- Shared code in `shared/` directory.
- Easy to navigate and maintain.
- Scales well with team size.

## Interview Tip:
"Feature-based structure scales better than type-based. Each feature is a module that can be understood independently."

---

## Question 203: How do you separate business logic from controllers?

## Answer:
Controllers handle HTTP concerns (parsing requests, sending responses). Services handle business logic (validation rules, calculations, data transformations).

```js
// Controller â€” HTTP concerns only
async function createUser(req, res, next) {
  try {
    const user = await userService.create(req.body);
    res.status(201).json(user);
  } catch (err) {
    next(err);
  }
}

// Service â€” business logic
async function create(userData) {
  const validated = validateUser(userData);
  const hashedPassword = await bcrypt.hash(validated.password, 12);
  return userRepository.create({ ...validated, password: hashedPassword });
}
```

## Key Points:
- Controllers: HTTP request/response handling.
- Services: Business logic, validation, transformations.
- Repositories: Database access.
- Each layer is independently testable.
- Services can be reused across controllers.

## Interview Tip:
"If you can test the service without HTTP, you've properly separated concerns."

---

## Question 204: What is the Service Layer pattern?

## Answer:
The Service Layer encapsulates business logic in dedicated service classes or modules. Services are called by controllers and use repositories for data access.

```js
class UserService {
  constructor(userRepository, emailService) {
    this.userRepository = userRepository;
    this.emailService = emailService;
  }

  async createUser(data) {
    const user = await this.userRepository.create(data);
    await this.emailService.sendWelcome(user.email);
    return user;
  }
}
```

## Key Points:
- Encapsulates business logic.
- Independent of HTTP (testable without Express).
- Uses dependency injection for dependencies.
- Can be reused across controllers.
- Central place for business rules.

## Interview Tip:
"Services are where business logic lives â€” they're testable, reusable, and framework-independent."

---

## Question 205: What is the Repository pattern?

## Answer:
The Repository pattern abstracts database access behind an interface. Services call repositories instead of directly using the database client.

```js
class UserRepository {
  constructor(prisma) {
    this.prisma = prisma;
  }

  async findById(id) {
    return this.prisma.user.findUnique({ where: { id } });
  }

  async create(data) {
    return this.prisma.user.create({ data });
  }
}
```

## Key Points:
- Abstracts database access.
- Service calls repository, not database directly.
- Easy to swap database without changing services.
- Testable with mock repositories.
- Centralizes database queries.

## Interview Tip:
"Repositories make it easy to swap databases â€” change the repository, not every service."

---

## Question 206: What is Dependency Injection (DI)?

## Answer:
Dependency Injection means passing dependencies (services, repositories) as arguments instead of creating them inside the module. This makes code loosely coupled and testable.

```js
// Without DI â€” tightly coupled
class UserService {
  constructor() {
    this.db = new Database(); // Created inside
  }
}

// With DI â€” loosely coupled
class UserService {
  constructor(db) {
    this.db = db; // Passed in
  }
}

const service = new UserService(database);
```

## Key Points:
- Pass dependencies as arguments.
- Don't create dependencies inside modules.
- Makes code loosely coupled and testable.
- Easy to swap implementations.
- Frameworks like NestJS have built-in DI.

## Interview Tip:
"DI makes testing easy â€” pass mock dependencies instead of real ones."

---

## Question 207: What are the benefits of Dependency Injection?

## Answer:
- **Testability**: Inject mocks for unit testing.
- **Loose coupling**: Modules don't create their dependencies.
- **Flexibility**: Swap implementations easily.
- **Reusability**: Same service works with different dependencies.
- **Maintainability**: Changes in one module don't affect others.

## Key Points:
- Easy to test with mock dependencies.
- Reduces coupling between modules.
- Enables swapping implementations.
- Improves code maintainability.
- Foundation of clean architecture.

## Interview Tip:
"DI is the foundation of testable, maintainable code. If you're not using it, you should be."

---

## Question 208: How do you organize shared utilities and helper functions?

## Answer:
Use a `utils/` or `lib/` directory:

```
src/
  utils/
    date.js         # Date formatting helpers
    string.js       # String manipulation
    validation.js   # Validation helpers
    errors.js       # Custom error classes
  lib/
    logger.js       # Logger configuration
    db.js           # Database client
```

Keep utilities pure (no side effects) and testable.

## Key Points:
- `utils/` for pure helper functions.
- `lib/` for shared infrastructure (logger, DB).
- Keep utilities pure and testable.
- Group by concern, not by file type.
- Use path aliases for clean imports.

## Interview Tip:
"Utils should be pure functions â€” no side effects, no dependencies. Easy to test and reuse."

---

## Question 209: How do you manage configuration across environments?

## Answer:
Use a config module that reads from environment variables:

```js
// config/index.js
const config = {
  port: parseInt(process.env.PORT) || 3000,
  db: { url: process.env.DATABASE_URL },
  jwt: { secret: process.env.JWT_SECRET, expiresIn: "7d" },
  logLevel: process.env.LOG_LEVEL || "info"
};

module.exports = config;
```

- Development: `.env` file (gitignored).
- Production: Platform environment variables.
- Never hardcode values.

## Key Points:
- Centralized config module.
- Reads from environment variables.
- Default values for optional settings.
- `.env` for development.
- Platform secrets for production.

## Interview Tip:
"A single config module that reads environment variables keeps configuration centralized and consistent."

---

## Question 210: What Node.js architecture patterns have you used in production?

## Answer:
- **MVC**: Model-View-Controller for traditional apps.
- **Service Layer**: Business logic separation.
- **Repository Pattern**: Database abstraction.
- **Event-Driven**: EventEmitter for decoupled components.
- **CQRS**: Command Query Responsibility Segregation for complex domains.
- **Microservices**: Service decomposition for large systems.

For most projects, a layered architecture (Controller â†’ Service â†’ Repository) is sufficient.

## Key Points:
- MVC for traditional applications.
- Service Layer for business logic.
- Repository for database abstraction.
- Event-driven for decoupled systems.
- Layered architecture for most projects.

## Interview Tip:
"Don't over-architect. Start with a layered architecture and add patterns as needed."

---

## Part 22 (211â€“220): API Design

---

## Question 211: What are RESTful APIs?

## Answer:
REST (Representational State Transfer) is an architectural style for APIs. RESTful APIs use HTTP methods to perform CRUD operations on resources identified by URLs.

- `GET /users` â€” List users
- `GET /users/:id` â€” Get a user
- `POST /users` â€” Create a user
- `PUT /users/:id` â€” Update a user
- `DELETE /users/:id` â€” Delete a user

## Key Points:
- Resource-based URLs (`/users`, `/posts`).
- HTTP methods for operations (GET, POST, PUT, DELETE).
- Stateless â€” each request contains all needed info.
- Uses standard HTTP status codes.
- JSON for data exchange.

## Interview Tip:
"REST is about resources and HTTP methods â€” keep it simple and standard."

---

## Question 212: What REST API design principles do you follow?

## Answer:
1. **Resource-based URLs**: `/users`, `/users/:id/posts`.
2. **Use HTTP methods correctly**: GET reads, POST creates, PUT updates, DELETE removes.
3. **Proper status codes**: 200 OK, 201 Created, 400 Bad Request, 404 Not Found.
4. **Consistent naming**: Plural nouns for collections (`/users`, not `/user`).
5. **Versioning**: `/api/v1/users`.
6. **Pagination**: For list endpoints.
7. **Error responses**: Consistent error format.

## Key Points:
- Resource-based, not action-based URLs.
- Proper HTTP methods and status codes.
- Plural nouns for collections.
- Versioning for breaking changes.
- Pagination for lists.

## Interview Tip:
"Follow HTTP conventions â€” use the right method, the right status code, and resource-based URLs."

---

## Question 213: How do you version REST APIs?

## Answer:
URL versioning is the most common approach:

```
/api/v1/users
/api/v2/users
```

Or header versioning:
```
GET /api/users
Accept: application/vnd.myapp.v2+json
```

URL versioning is simpler and more visible. Header versioning is cleaner but harder to test.

## Key Points:
- URL versioning: `/api/v1/...` (most common).
- Header versioning: `Accept` header.
- Version breaking changes, not every change.
- Maintain old versions for backward compatibility.
- Document version differences.

## Interview Tip:
"URL versioning is the most practical â€” it's visible, testable, and easy to route."

---

## Question 214: What HTTP status codes do you commonly use?

## Answer:
- **200**: OK â€” request succeeded.
- **201**: Created â€” resource created.
- **204**: No Content â€” success, no response body.
- **400**: Bad Request â€” invalid input.
- **401**: Unauthorized â€” authentication required.
- **403**: Forbidden â€” authenticated but not authorized.
- **404**: Not Found â€” resource doesn't exist.
- **409**: Conflict â€” resource already exists.
- **422**: Unprocessable Entity â€” validation error.
- **429**: Too Many Requests â€” rate limited.
- **500**: Internal Server Error â€” server error.

## Key Points:
- 2xx: success.
- 4xx: client errors.
- 5xx: server errors.
- Use the most specific status code.
- Don't return 200 for errors.

## Interview Tip:
"Use specific status codes â€” 400 for validation errors, 404 for not found, 500 for server errors."

---

## Question 215: How do you design consistent API responses?

## Answer:
Use a standard response format:

```js
// Success
{
  "data": { "id": 1, "name": "Alice" },
  "meta": { "page": 1, "total": 100 }
}

// Error
{
  "error": {
    "code": "VALIDATION_ERROR",
    "message": "Invalid input",
    "details": { "email": "Invalid email format" }
  }
}
```

Consistency makes API consumption predictable.

## Key Points:
- `data` field for successful responses.
- `error` field for error responses.
- `meta` for pagination and metadata.
- Consistent error codes and messages.
- Documentation for response format.

## Interview Tip:
"A consistent response format makes your API predictable and easy to consume."

---

## Question 216: How do you implement pagination?

## Answer:
Offset-based:
```
GET /api/users?page=1&limit=10
```

Cursor-based:
```
GET /api/users?cursor=abc123&limit=10
```

Response:
```json
{
  "data": [...],
  "meta": {
    "page": 1,
    "limit": 10,
    "total": 100,
    "totalPages": 10
  }
}
```

Cursor-based is better for real-time data; offset-based is simpler.

## Key Points:
- Offset-based: `page` and `limit` parameters.
- Cursor-based: `cursor` for position.
- Include pagination metadata in response.
- Cursor-based avoids issues with data changes between pages.
- Default limit should be reasonable (10-50).

## Interview Tip:
"Cursor-based pagination is better for real-time data â€” offset pagination can skip or duplicate items."

---

## Question 217: How do you implement filtering and sorting?

## Answer:
```
GET /api/users?role=admin&status=active&sort=-createdAt&fields=name,email
```

```js
// Parse query parameters
const { role, status, sort, fields } = req.query;

const filter = {};
if (role) filter.role = role;
if (status) filter.status = status;

const orderBy = {};
if (sort) {
  const [field, direction] = sort.startsWith("-") 
    ? [sort.slice(1), "desc"] 
    : [sort, "asc"];
  orderBy[field] = direction;
}
```

## Key Points:
- Query parameters for filtering: `?role=admin`.
- Sorting with direction: `?sort=-createdAt` (descending).
- Field selection: `?fields=name,email`.
- Parse and apply filters server-side.
- Validate filter values.

## Interview Tip:
"Use query parameters for filtering and sorting â€” it's the REST standard."

---

## Question 218: How do you implement rate limiting?

## Answer:
```js
const rateLimit = require("express-rate-limit");
const RedisStore = require("rate-limit-redis");
const redis = require("redis");

const client = redis.createClient();

const limiter = rateLimit({
  store: new RedisStore({ sendCommand: (...args) => client.sendCommand(args) }),
  windowMs: 15 * 60 * 1000, // 15 minutes
  max: 100, // 100 requests per window
  message: { error: "Too many requests" }
});

app.use("/api/", limiter);
```

## Key Points:
- Limit requests per IP or user per time window.
- Redis store for distributed rate limiting.
- Return 429 status when rate limited.
- Different limits for different endpoints.
- Login endpoints should have stricter limits.

## Interview Tip:
"Rate limiting prevents abuse. Use Redis for distributed rate limiting across multiple instances."

---

## Question 219: How do you document APIs?

## Answer:
Use OpenAPI (Swagger):

```js
const swagger = require("swagger-jsdoc");
const swaggerUi = require("swagger-ui-express");

const options = {
  definition: {
    openapi: "3.0.0",
    info: { title: "My API", version: "1.0.0" }
  },
  apis: ["./routes/*.js"]
};

const specs = swagger(options);
app.use("/docs", swaggerUi.serve, swaggerUi.setup(specs));
```

Or use JSDoc annotations in your route files.

## Key Points:
- OpenAPI (Swagger) is the standard.
- Auto-generate docs from code annotations.
- Swagger UI for interactive documentation.
- Document endpoints, parameters, and responses.
- Keep docs in sync with code.

## Interview Tip:
"Swagger UI gives you interactive API documentation for free â€” use it."

---

## Question 220: What are common REST API design mistakes?

## Answer:
1. **Not using proper HTTP methods**: Using GET for everything.
2. **Wrong status codes**: Returning 200 for errors.
3. **Inconsistent responses**: Different formats per endpoint.
4. **No pagination**: Returning all records at once.
5. **Not versioning**: Breaking changes without versioning.
6. **Exposing internal IDs**: Using database IDs in URLs.
7. **No rate limiting**: Vulnerable to abuse.
8. **Verb-based URLs**: `/getUsers` instead of `GET /users`.

## Key Points:
- Use proper HTTP methods and status codes.
- Consistent response format across all endpoints.
- Always paginate list endpoints.
- Version your API for breaking changes.
- Resource-based URLs, not verb-based.

## Interview Tip:
"REST is about conventions â€” follow them and your API will be predictable and easy to use."

---

## Part 23 (221â€“230): Caching & Messaging

---

## Question 221: What is caching?

## Answer:
Caching stores frequently accessed data in a fast storage layer (memory, Redis) to avoid expensive operations (database queries, API calls, computations).

```js
const cache = new Map();

async function getUser(id) {
  if (cache.has(id)) return cache.get(id);
  const user = await db.user.findUnique({ where: { id } });
  cache.set(id, user);
  return user;
}
```

## Key Points:
- Stores fast-access copies of expensive data.
- Reduces database load and response times.
- In-memory cache (Map, LRU) for single instance.
- Redis for distributed caching.
- Cache invalidation is the hard part.

## Interview Tip:
"There are only two hard things in computer science: cache invalidation and naming things."

---

## Question 222: When would you use Redis?

## Answer:
- **Session storage**: Shared sessions across instances.
- **Caching**: Fast data caching with TTL.
- **Rate limiting**: Distributed rate limiting.
- **Message queues**: Pub/sub and task queues.
- **Real-time**: Pub/sub for real-time features.
- **Leaderboards**: Sorted sets for rankings.
- **Counting**: Atomic counters for analytics.

## Key Points:
- Session storage for clustered apps.
- Caching with automatic expiration.
- Distributed rate limiting.
- Message queuing and pub/sub.
- Incredibly fast (in-memory).

## Interview Tip:
"Redis is the Swiss Army knife of backend infrastructure â€” sessions, caching, queues, and real-time."

---

## Question 223: What data should be cached?

## Answer:
- **Database query results**: Frequently accessed, rarely changed.
- **API responses**: External API calls with known freshness.
- **Computed values**: Expensive calculations.
- **Session data**: User sessions.
- **Configuration**: Static configuration data.
- **HTML fragments**: Server-side rendered components.

Don't cache: rapidly changing data, user-specific data (unless per-user cache), or data that must be real-time.

## Key Points:
- Frequently accessed, rarely changed data.
- Expensive computations and queries.
- External API responses.
- Session and authentication data.
- Avoid caching real-time or rapidly changing data.

## Interview Tip:
"Cache what's expensive to compute and doesn't change often."

---

## Question 224: What cache invalidation strategies have you used?

## Answer:
1. **TTL (Time-To-Live)**: Cache expires after a set time.
2. **Event-based**: Invalidate when data changes (write-through).
3. **LRU (Least Recently Used)**: Evict oldest items when cache is full.
4. **Write-behind**: Write to cache first, flush to DB later.
5. **Tag-based**: Invalidate related items by tag.

```js
// TTL-based
await redis.set("user:1", JSON.stringify(user), "EX", 3600); // 1 hour

// Event-based
await db.user.update({ data });
await redis.del(`user:${id}`); // Invalidate cache
```

## Key Points:
- TTL: automatic expiration.
- Event-based: invalidate on data change.
- LRU: evict oldest when full.
- Tag-based: invalidate groups of items.
- Choose based on data freshness requirements.

## Interview Tip:
"TTL is simplest. Event-based is most accurate. Use a combination for best results."

---

## Question 225: What is a message queue?

## Answer:
A message queue is a system for asynchronous communication between services. Producers send messages to a queue, and consumers process them independently.

```js
// Producer
await queue.publish("email", { to: "user@example.com", subject: "Welcome" });

// Consumer
queue.consume("email", async (message) => {
  await sendEmail(message.to, message.subject);
});
```

## Key Points:
- Asynchronous communication between services.
- Decouples producers from consumers.
- Handles load spikes by buffering messages.
- Ensures reliability â€” messages aren't lost.
- Examples: RabbitMQ, Kafka, Redis queues.

## Interview Tip:
"Message queues decouple services and handle load spikes â€” they're essential for microservices."

---

## Question 226: When would you use RabbitMQ?

## Answer:
RabbitMQ is a traditional message broker for:
- **Task queues**: Background jobs (email, image processing).
- **Request-reply**: RPC-style communication.
- **Fanout**: Broadcasting to multiple consumers.
- **Routing**: Directing messages to specific queues.

Choose RabbitMQ when you need reliable message delivery, complex routing, and acknowledgment-based processing.

## Key Points:
- Traditional message broker.
- Reliable message delivery with acknowledgments.
- Complex routing with exchanges and queues.
- Good for task queues and background jobs.
- Simpler than Kafka for most use cases.

## Interview Tip:
"RabbitMQ is great for task queues and background jobs â€” reliable and easy to set up."

---

## Question 227: When would you use Apache Kafka?

## Answer:
Kafka is a distributed event streaming platform for:
- **Event sourcing**: Storing all state changes as events.
- **Log aggregation**: Centralized logging from multiple services.
- **Real-time analytics**: Stream processing.
- **High-throughput**: Millions of messages per second.
- **Event replay**: Re-process events from the past.

Choose Kafka when you need high throughput, event replay, and stream processing.

## Key Points:
- Distributed event streaming platform.
- High throughput (millions of messages/second).
- Event replay â€” re-process past events.
- Log aggregation and stream processing.
- More complex than RabbitMQ.

## Interview Tip:
"Kafka is for high-throughput event streaming. RabbitMQ is for task queues. Pick based on your needs."

---

## Question 228: What are background jobs in Node.js?

## Answer:
Background jobs are tasks that run asynchronously, outside the request-response cycle. They're used for:
- Sending emails
- Processing images
- Generating reports
- Syncing data
- Cleaning up resources

```js
// Using Bull (Redis-based job queue)
const Queue = require("bull");
const emailQueue = new Queue("emails");

// Add job
await emailQueue.add({ to: "user@example.com", subject: "Welcome" });

// Process job
emailQueue.process(async (job) => {
  await sendEmail(job.data.to, job.data.subject);
});
```

## Key Points:
- Run asynchronously outside request cycle.
- Use job queues (Bull, Agenda, BullMQ).
- Process in background without blocking the server.
- Handle retries and failures.
- Redis-based for distributed job processing.

## Interview Tip:
"Background jobs keep your API fast â€” heavy work happens in the queue, not in the request."

---

## Question 229: How do you schedule recurring tasks?

## Answer:
Use `node-cron` or `bull` for scheduled jobs:

```js
const cron = require("node-cron");

// Run every day at midnight
cron.schedule("0 0 * * *", async () => {
  await cleanupOldRecords();
  await generateDailyReport();
});
```

Or use Bull with repeatable jobs:

```js
await emailQueue.add(
  { type: "weekly-report" },
  { repeat: { every: 7 * 24 * 60 * 60 * 1000 } } // Weekly
);
```

## Key Points:
- `node-cron` for simple cron scheduling.
- Bull for distributed scheduled jobs.
- Cron syntax for flexible scheduling.
- Run cleanup, reports, syncs on schedule.
- Consider timezone handling.

## Interview Tip:
"`node-cron` for simple scheduling. Bull for distributed, reliable recurring jobs."

---

## Question 230: When should you use WebSockets instead of REST?

## Answer:
Use WebSockets for:
- **Real-time updates**: Chat, notifications, live feeds.
- **Bidirectional communication**: Client and server both send messages.
- **Low latency**: Immediate push without polling.
- **Collaborative editing**: Real-time document editing.
- **Live dashboards**: Real-time metrics and monitoring.

Use REST for:
- CRUD operations.
- Request-response patterns.
- Stateless operations.

## Key Points:
- WebSockets: real-time, bidirectional, low latency.
- REST: request-response, stateless, CRUD.
- WebSockets for chat, live feeds, real-time updates.
- REST for standard API operations.
- Can use both in the same application.

## Interview Tip:
"If the server needs to push data to the client in real-time, use WebSockets. For request-response, use REST."

---

## Part 24 (231â€“240): Database & Scalability

---

## Question 231: How do you optimize database performance?

## Answer:
1. **Indexes**: Add indexes on frequently queried columns.
2. **Connection pooling**: Reuse database connections.
3. **Query optimization**: Avoid N+1 queries, select only needed columns.
4. **Caching**: Cache frequent queries in Redis.
5. **Read replicas**: Distribute read queries across replicas.
6. **Batch operations**: Insert/update multiple rows in one query.
7. **Lazy loading**: Load related data only when needed.

## Key Points:
- Indexes are the most impactful optimization.
- Connection pooling reduces overhead.
- Avoid N+1 queries with eager loading.
- Cache frequently accessed data.
- Read replicas distribute read load.

## Interview Tip:
"Start with indexes â€” they usually give the biggest performance improvement."

---

## Question 232: How do you handle database transactions?

## Answer:
```js
// Prisma transaction
const result = await prisma.$transaction(async (tx) => {
  const user = await tx.user.create({ data: { name: "Alice" } });
  const account = await tx.account.create({ data: { userId: user.id, balance: 100 } });
  return { user, account };
});
```

Transactions ensure multiple operations succeed or fail together (ACID properties).

## Key Points:
- Transactions group multiple operations.
- All operations succeed or all fail (ACID).
- Use for data consistency across multiple tables.
- Prisma, TypeORM, and Knex support transactions.
- Keep transactions short â€” long transactions cause locks.

## Interview Tip:
"Use transactions when multiple operations must succeed or fail together â€” like transferring money between accounts."

---

## Question 233: How do you prevent race conditions?

## Answer:
1. **Database transactions**: Ensure atomic operations.
2. **Optimistic locking**: Version field to detect conflicts.
3. **Pessimistic locking**: Lock rows during updates.
4. **Atomic operations**: Use database-level atomicity.

```js
// Optimistic locking
const user = await db.user.findUnique({ where: { id } });
const updated = await db.user.update({
  where: { id, version: user.version },
  data: { balance: user.balance - 100, version: user.version + 1 }
});
if (!updated) throw new Error("Conflict â€” retry");
```

## Key Points:
- Race conditions occur with concurrent modifications.
- Transactions ensure atomicity.
- Optimistic locking detects conflicts.
- Pessimistic locking prevents conflicts.
- Database-level atomicity is the safest.

## Interview Tip:
"Optimistic locking is usually best â€” detect conflicts and retry, don't lock rows."

---

## Question 234: How do you manage database connection pooling?

## Answer:
Connection pooling maintains a pool of reusable database connections instead of creating a new connection per request.

```js
// Prisma â€” built-in connection pooling
datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
  connection_limit = 10
}

// pg (node-postgres)
const { Pool } = require("pg");
const pool = new Pool({ max: 20, idleTimeoutMillis: 30000 });
```

## Key Points:
- Reuse connections instead of creating new ones.
- Configurable pool size (max connections).
- Idle timeout closes unused connections.
- Prevents connection exhaustion under load.
- Most ORMs handle pooling automatically.

## Interview Tip:
"Connection pooling prevents connection exhaustion â€” configure the pool size based on your database limits."

---

## Question 235: How do you scale a backend application?

## Answer:
1. **Horizontal scaling**: Add more instances behind a load balancer.
2. **Vertical scaling**: Increase resources on a single instance.
3. **Database scaling**: Read replicas, sharding, connection pooling.
4. **Caching**: Redis for frequently accessed data.
5. **CDN**: Cache static assets globally.
6. **Async processing**: Background jobs for heavy work.
7. **Microservices**: Decompose into independent services.

## Key Points:
- Horizontal scaling is the primary approach.
- Database is usually the bottleneck.
- Caching reduces database load.
- Async processing offloads heavy work.
- CDN reduces server load for static assets.

## Interview Tip:
"Start with horizontal scaling and caching â€” they give the biggest scaling wins."

---

## Question 236: How do you design a high-availability Node.js application?

## Answer:
1. **Multiple instances**: At least 2-3 instances behind a load balancer.
2. **Health checks**: Load balancer routes away from unhealthy instances.
3. **Graceful shutdown**: Finish requests before closing.
4. **Externalized state**: Sessions and cache in Redis.
5. **Database replication**: Primary + read replicas.
6. **Monitoring and alerting**: Detect issues quickly.
7. **Auto-scaling**: Add instances under load.

## Key Points:
- Multiple instances eliminate single points of failure.
- Health checks detect and replace failed instances.
- Externalized state enables instance independence.
- Database replication provides failover.
- Monitoring catches issues before users do.

## Interview Tip:
"High availability means no single point of failure â€” multiple instances, external state, and health checks."

---

## Question 237: What are the trade-offs between a monolith and microservices?

## Answer:
| Aspect | Monolith | Microservices |
|--------|----------|---------------|
| Complexity | Simple to start | Complex infrastructure |
| Deployment | Single deploy | Per-service deployment |
| Scaling | Scale entire app | Scale individual services |
| Team | Easier coordination | Independent teams |
| Debugging | Easier | Distributed tracing needed |
| Tech stack | Single stack | Polyglot (any language per service) |

## Key Points:
- Monolith: simpler, faster to develop, easier to debug.
- Microservices: scalable, independent, polyglot.
- Start with monolith, split when needed.
- Microservices add operational complexity.
- Most teams should start with a well-structured monolith.

## Interview Tip:
"Don't start with microservices â€” start with a monolith and split when you have a clear reason."

---

## Question 238: When would you choose microservices?

## Answer:
- **Large teams**: Multiple teams working independently.
- **Different scaling needs**: Some services need more resources.
- **Different tech stacks**: Some services need Python, others Node.js.
- **Independent deployment**: Services deploy independently.
- **Fault isolation**: One service failure doesn't bring down everything.

Don't choose microservices for small teams or simple applications.

## Key Points:
- Large teams with independent ownership.
- Different scaling requirements per service.
- Need for polyglot technology stacks.
- Independent deployment cycles.
- Fault isolation between services.

## Interview Tip:
"Choose microservices when the operational complexity is worth the benefits â€” usually at scale."

---

## Question 239: How do services communicate in a microservices architecture?

## Answer:
- **HTTP/REST**: Synchronous request-response.
- **Message queues**: Asynchronous communication (RabbitMQ, Kafka).
- **gRPC**: High-performance RPC protocol.
- **WebSockets**: Real-time bidirectional communication.
- **Event-driven**: Pub/sub patterns.

Each has trade-offs â€” HTTP is simple, queues are reliable, gRPC is fast.

## Key Points:
- HTTP/REST: simple, widely supported.
- Message queues: reliable, asynchronous.
- gRPC: fast, typed, efficient.
- WebSockets: real-time, bidirectional.
- Event-driven: decoupled, scalable.

## Interview Tip:
"HTTP for simplicity, queues for reliability, gRPC for performance, WebSockets for real-time."

---

## Question 240: What challenges have you faced while scaling backend systems?

## Answer:
Common challenges:
- **Database bottlenecks**: Queries that worked at small scale fail at large scale.
- **Distributed state**: Sessions and cache across multiple instances.
- **Service communication**: Reliability and latency between services.
- **Monitoring**: Observing across multiple services and instances.
- **Deployment**: Zero-downtime deployments at scale.
- **Data consistency**: Maintaining consistency across services.

## Key Points:
- Database is usually the first bottleneck.
- Distributed state requires external stores (Redis).
- Service communication adds latency.
- Monitoring becomes critical at scale.
- Zero-downtime deployments are harder.

## Interview Tip:
"The database is almost always the bottleneck. Caching and read replicas solve most scaling issues."

---

## Part 25 (241â€“250): Senior Real-World Interview Questions

---

## Question 241: Describe the largest Node.js application you've worked on.

## Answer:
Pick a real project and describe:
- **Scale**: Users, requests per second, data volume.
- **Architecture**: Monolith or microservices, tech stack.
- **Challenges**: What was hard and how you solved it.
- **Your role**: What you specifically contributed.
- **Results**: Performance improvements, features delivered.

Focus on the technical decisions and trade-offs you made.

## Key Points:
- Quantify the scale (users, RPS, data).
- Describe the architecture and tech stack.
- Highlight challenges and solutions.
- Explain your specific contributions.
- Show the impact of your work.

## Interview Tip:
"Tell a story with a beginning (problem), middle (solution), and end (result). Quantify everything."

---

## Question 242: What was the most difficult backend bug you've fixed?

## Answer:
Describe:
1. **The symptoms**: What was happening.
2. **The investigation**: How you diagnosed it.
3. **The root cause**: What was actually wrong.
4. **The fix**: How you resolved it.
5. **The lesson**: What you learned.

Choose a bug that shows your debugging process and technical depth.

## Key Points:
- Describe symptoms, investigation, root cause, fix, and lesson.
- Show your systematic debugging approach.
- Mention tools you used.
- Explain what you learned.
- Choose a technically interesting bug.

## Interview Tip:
"Interviewers want to see your debugging process, not just the fix. Walk through your investigation steps."

---

## Question 243: How do you debug production issues in Node.js?

## Answer:
1. **Check logs**: Structured logs with context (Pino/Winston).
2. **Check metrics**: CPU, memory, response times (APM tools).
3. **Reproduce**: Try to reproduce in staging.
4. **Profile**: CPU and memory profiling.
5. **Check dependencies**: Database, external APIs, caches.
6. **Rollback**: If recent deployment, consider rollback.
7. **Monitor**: Watch for patterns and correlations.

## Key Points:
- Logs are the first line of debugging.
- Metrics show trends and anomalies.
- Reproduce in staging when possible.
- Profile CPU and memory for performance issues.
- Check dependencies â€” they're often the cause.

## Interview Tip:
"Start with logs, then metrics, then profiling. Don't guess â€” use data."

---

## Question 244: How do you review backend pull requests?

## Answer:
Check for:
1. **Security**: SQL injection, XSS, secrets exposure.
2. **Error handling**: All errors handled gracefully.
3. **Performance**: N+1 queries, missing indexes, blocking code.
4. **Testing**: Adequate test coverage.
5. **Code quality**: Readability, naming, separation of concerns.
6. **Database changes**: Migrations, indexes, data integrity.
7. **API design**: Consistent with existing patterns.

## Key Points:
- Security is the top priority.
- Error handling prevents crashes.
- Performance issues caught early.
- Tests verify correctness.
- Consistent patterns reduce cognitive load.

## Interview Tip:
"Security and error handling are the most important things to check in every PR."

---

## Question 245: What coding standards do you enforce in your team?

## Answer:
1. **Linting**: ESLint with strict rules.
2. **Formatting**: Prettier for consistent style.
3. **Type checking**: TypeScript strict mode.
4. **Testing**: Required for new features.
5. **Error handling**: All async operations must handle errors.
6. **Code review**: All PRs reviewed before merge.
7. **Documentation**: API docs and README updates.

## Key Points:
- Automated linting and formatting.
- TypeScript for type safety.
- Tests are required, not optional.
- Consistent error handling patterns.
- Code review for all changes.

## Interview Tip:
"Automate what you can (linting, formatting) and enforce the rest through code review."

---

## Question 246: How do you mentor junior backend developers?

## Answer:
1. **Code review**: Detailed, educational feedback.
2. **Pair programming**: Work together on complex problems.
3. **Architecture discussions**: Explain why, not just what.
4. **Gradual responsibility**: Start with small features, increase complexity.
5. **Knowledge sharing**: Tech talks, documentation, READMEs.
6. **Safe environment**: Encourage questions and mistakes.

## Key Points:
- Educational code reviews.
- Pair programming for learning.
- Explain the "why" behind decisions.
- Gradually increase responsibility.
- Create a safe environment for questions.

## Interview Tip:
"The best mentoring is patient, specific, and focuses on teaching principles, not just fixing code."

---

## Question 247: If you joined a new project, how would you evaluate the existing Node.js codebase?

## Answer:
1. **Run the app**: Does it start and work?
2. **Check dependencies**: Outdated, vulnerable packages.
3. **Read tests**: Are there tests? What's the coverage?
4. **Check architecture**: Is it well-organized?
5. **Review error handling**: How are errors handled?
6. **Check security**: Vulnerabilities, secrets exposure.
7. **Profile performance**: Any obvious bottlenecks?
8. **Talk to the team**: Understand the context.

## Key Points:
- Start by running the application.
- Check for security vulnerabilities.
- Evaluate test coverage and quality.
- Understand the architecture.
- Talk to the team for context.

## Interview Tip:
"Run the app first, check security second, and talk to the team for context."

---

## Question 248: If you were building a production SaaS today, what backend architecture would you choose and why?

## Answer:
- **Node.js + Express/Fastify**: API server.
- **PostgreSQL**: Primary database.
- **Redis**: Caching, sessions, queues.
- **Prisma**: Type-safe ORM.
- **Auth.js**: Authentication.
- **Bull**: Background job processing.
- **Docker + AWS ECS**: Deployment.
- **Sentry**: Error tracking.
- **Pino**: Structured logging.

Start monolith, split to microservices only when needed.

## Key Points:
- Proven, boring technology stack.
- PostgreSQL for reliability.
- Redis for caching and queues.
- Monolith first, microservices when needed.
- Focus on shipping, not architecture astronautics.

## Interview Tip:
"Choose boring, proven technology. The latest trendy library is rarely worth the risk in production."

---

## Question 249: What best practices do you always follow in production Node.js applications?

## Answer:
1. **Structured logging**: Pino with JSON output.
2. **Error handling**: Centralized error handler.
3. **Graceful shutdown**: Handle SIGTERM.
4. **Health checks**: `/health` endpoint.
5. **Rate limiting**: Protect endpoints from abuse.
6. **Input validation**: Zod for all external input.
7. **Security headers**: Helmet.js.
8. **Environment variables**: Secrets out of code.
9. **Monitoring**: Sentry + APM.
10. **Testing**: Unit + integration tests.

## Key Points:
- Structured logging for debugging.
- Error handling prevents crashes.
- Graceful shutdown prevents data loss.
- Health checks enable monitoring.
- Security is non-negotiable.

## Interview Tip:
"Production best practices aren't optional â€” they're what separates hobby projects from production systems."

---

## Question 250: In your opinion, what separates a junior, mid-level, and senior Node.js developer?

## Answer:
- **Junior**: Knows the basics â€” Node.js, Express, database CRUD. Can build features with guidance. Needs help with architecture decisions.
- **Mid-level**: Understands the event loop, async patterns, and database optimization. Can build features independently. Knows when to use which tool.
- **Senior**: Designs architecture, makes technology decisions, mentors others. Understands trade-offs, security, and performance from day one. Thinks about scalability and maintainability.

The biggest differentiator: a senior developer can explain WHY, not just WHAT.

## Key Points:
- Junior: learns the framework, builds with guidance.
- Mid-level: understands the architecture, builds independently.
- Senior: designs the architecture, makes decisions, mentors.
- Senior understands trade-offs, not just features.
- Senior thinks about security, performance, and scalability.

## Interview Tip:
"The best answer shows self-awareness. Pick the level you're at and explain what you're doing to grow."

---

# End of Node.js Interview Questions & Answers
