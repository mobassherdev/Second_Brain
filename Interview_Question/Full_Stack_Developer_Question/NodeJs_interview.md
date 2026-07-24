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
