# Next.js Interview Questions (250 Total)

---

### Introduction

1. What is Next.js?
2. Why was Next.js created?
3. What problems does Next.js solve?
4. What are the advantages of Next.js over React?
5. What are the disadvantages of Next.js?
6. What is the difference between React and Next.js?
7. When would you choose React instead of Next.js?
8. When would you choose Next.js instead of React?
9. What is the App Router?
10. What is the Pages Router?

---

### App Router

11. What are the main features of the App Router?
12. Why did Next.js introduce the App Router?
13. What is the difference between the App Router and the Pages Router?
14. Which router would you use for a new project?
15. What is the `app` directory?
16. What is the `page.tsx` file?
17. What is the `layout.tsx` file?
18. What is the `template.tsx` file?
19. What is the `loading.tsx` file?
20. What is the `error.tsx` file?

---

### Components

21. What are Server Components?
22. What are Client Components?
23. What is the `"use client"` directive?
24. When should you use a Client Component?
25. When should you use a Server Component?
26. What are the benefits of Server Components?
27. What are the limitations of Server Components?
28. Can a Server Component import a Client Component?
29. Can a Client Component import a Server Component?
30. How do Server and Client Components communicate?

---

### Routing

31. How does file-based routing work?
32. What are dynamic routes?
33. What are nested routes?
34. What are catch-all routes?
35. What are optional catch-all routes?
36. What is route grouping?
37. What are parallel routes?
38. What are intercepted routes?
39. What is the `Link` component?
40. Why should you use `Link` instead of `<a>`?

---

### Navigation & Layouts

41. What is `useRouter()`?
42. What is `usePathname()`?
43. What is `useSearchParams()`?
44. How do you navigate programmatically?
45. What are nested layouts?
46. Why are layouts useful?
47. How do layouts improve performance?
48. What is shared UI in Next.js?
49. What is partial rendering?
50. What happens when navigating between pages in Next.js?

---

# Rendering Strategies

51. What is Client-Side Rendering (CSR)?
52. What is Server-Side Rendering (SSR)?
53. What is Static Site Generation (SSG)?
54. What is Incremental Static Regeneration (ISR)?
55. What is Partial Prerendering (PPR)?
56. What is the difference between SSR, SSG, ISR, and CSR?
57. When should you choose SSR over SSG?
58. When should you choose CSR over SSR?
59. When should you use ISR?
60. What rendering strategy would you choose for an e-commerce website?

---

# Hydration & Streaming

61. What is hydration in Next.js?
62. What causes hydration mismatches?
63. How do you fix hydration errors?
64. What is streaming in Next.js?
65. What are the benefits of streaming?
66. How does React Suspense work with Next.js?
67. What is selective hydration?
68. What is progressive rendering?
69. What are common hydration pitfalls?
70. How do you debug hydration issues?

---

# Data Fetching

71. How do you fetch data in the App Router?
72. What is the difference between server-side and client-side data fetching?
73. When should data be fetched on the server?
74. When should data be fetched on the client?
75. How does the native `fetch()` API work in Next.js?
76. What caching behavior does `fetch()` have by default in the App Router?
77. What does `cache: "no-store"` do?
78. What does `next: { revalidate }` do?
79. What is request memoization?
80. What is data cache in Next.js?

---

# Route Handlers

81. What are Route Handlers?
82. How do Route Handlers differ from API Routes?
83. How do you create a GET Route Handler?
84. How do you create a POST Route Handler?
85. How do you read request parameters in a Route Handler?
86. How do you return JSON responses?
87. How do you handle errors in Route Handlers?
88. How do you validate request data?
89. When should you use Route Handlers instead of Express?
90. Can Route Handlers access databases directly?

---

# SEO & Metadata

91. Why is Next.js considered SEO-friendly?
92. What is the Metadata API?
93. How do you define page metadata?
94. How do you create dynamic metadata?
95. How do you add Open Graph metadata?
96. How do you generate dynamic page titles?
97. How do you create XML sitemaps in Next.js?
98. How do you configure robots.txt?
99. How do you improve SEO in Next.js applications?
100. What are the biggest SEO mistakes developers make in Next.js?

---

# Server Actions

101. What are Server Actions?
102. Why were Server Actions introduced?
103. How do Server Actions work?
104. What does the `"use server"` directive do?
105. When should you use a Server Action?
106. How do Server Actions differ from Route Handlers?
107. Can Server Actions access a database directly?
108. How do you submit forms using Server Actions?
109. How do you validate data in Server Actions?
110. What are the limitations of Server Actions?

---

# Middleware

111. What is Middleware in Next.js?
112. When should you use Middleware?
113. How does Middleware work?
114. What requests pass through Middleware?
115. How do you protect routes with Middleware?
116. How do you redirect users in Middleware?
117. How do you rewrite URLs in Middleware?
118. How do you read cookies in Middleware?
119. What are common Middleware use cases?
120. What are the limitations of Middleware?

---

# Authentication & Authorization

121. How do you implement authentication in Next.js?
122. What is the difference between authentication and authorization?
123. Where should JWT tokens be stored?
124. Why are HTTP-only cookies preferred over localStorage?
125. How do you protect Server Components?
126. How do you protect Client Components?
127. How do you implement role-based access control (RBAC)?
128. How do you handle login and logout in Next.js?
129. How do you refresh expired access tokens?
130. What authentication libraries are commonly used with Next.js?

---

# Cookies, Headers & Sessions

131. How do you read cookies in Server Components?
132. How do you set cookies in Next.js?
133. How do you delete cookies?
134. How do you read request headers?
135. How do you set response headers?
136. What is the difference between cookies and sessions?
137. How do you manage user sessions?
138. How do you securely store sensitive information?
139. What are secure cookie attributes?
140. How do you prevent CSRF attacks?

---

# APIs & External Services

141. How do you consume REST APIs in Next.js?
142. How do you consume GraphQL APIs?
143. Where should API calls be made—server or client?
144. How do you handle loading states?
145. How do you handle API errors?
146. How do you implement pagination?
147. How do you implement infinite scrolling?
148. How do you upload files in Next.js?
149. How do you integrate third-party APIs securely?
150. How do you avoid exposing API keys in Next.js?

---

# Image Optimization

151. What is the `next/image` component?
152. Why should you use `next/image` instead of `<img>`?
153. How does image optimization work in Next.js?
154. What image formats does Next.js support?
155. How do you optimize remote images?
156. What is lazy loading in `next/image`?
157. What is the `priority` prop?
158. What is the difference between `fill` and fixed dimensions?
159. How do you configure image domains?
160. What are common mistakes when using `next/image`?

---

# Font Optimization

161. What is `next/font`?
162. Why should you use `next/font`?
163. What are the advantages of self-hosted fonts?
164. What is layout shift caused by fonts?
165. How does Next.js reduce font loading issues?
166. What is font preloading?
167. How do you load Google Fonts using `next/font`?
168. How do you load local fonts?
169. What is `display: swap`?
170. What are font loading best practices?

---

# Performance Optimization

171. How do you improve performance in a Next.js application?
172. What causes slow page loads?
173. How do you reduce JavaScript bundle size?
174. What is code splitting?
175. How does automatic code splitting work in Next.js?
176. What is dynamic import?
177. When should you use dynamic imports?
178. What is lazy loading?
179. How do you optimize third-party scripts?
180. How do you measure application performance?

---

# Caching & Revalidation

181. What types of caching exist in Next.js?
182. What is the Data Cache?
183. What is the Full Route Cache?
184. What is the Router Cache?
185. What is request memoization?
186. What is cache revalidation?
187. What is time-based revalidation?
188. What is on-demand revalidation?
189. What is `revalidatePath()`?
190. What is `revalidateTag()`?

---

# Deployment & Production

191. How do you deploy a Next.js application?
192. Why is Vercel the recommended platform for Next.js?
193. How do you deploy Next.js with Docker?
194. How do you deploy Next.js on AWS?
195. How do you manage environment variables?
196. What is the Edge Runtime?
197. When should you use the Edge Runtime?
198. How do you monitor a production Next.js application?
199. What are common production issues in Next.js applications?
200. What best practices do you follow before deploying a Next.js application?

---

# Architecture & Project Structure

201. How do you structure a large Next.js application?
202. How do you organize the `app` directory in a scalable project?
203. What folder structure do you prefer for enterprise Next.js applications?
204. How do you organize reusable UI components?
205. How do you separate business logic from UI components?
206. Where should API calls be placed in a Next.js project?
207. How do you organize utility functions and shared libraries?
208. How do you structure feature-based modules?
209. How do you handle shared layouts across large applications?
210. How do you decide whether code belongs in a Server Component or Client Component?

---

# State Management

211. When is React Context enough in a Next.js application?
212. When would you choose Redux Toolkit?
213. When would you choose Zustand?
214. When would you choose TanStack Query (React Query)?
215. What data should stay on the server instead of global state?
216. How do you avoid unnecessary global state?
217. How do you share authenticated user data across the application?
218. How do you manage server state vs client state?
219. How do you persist client state after page refresh?
220. What state management mistakes do developers commonly make?

---

# Security

221. How do you secure a Next.js application?
222. How do you prevent XSS attacks in Next.js?
223. How do you prevent CSRF attacks?
224. How do you protect sensitive environment variables?
225. Why should secrets never be exposed to the client?
226. How do you securely handle file uploads?
227. How do you validate user input?
228. How do you implement rate limiting?
229. How do you secure API routes and Route Handlers?
230. What are the most common security mistakes in Next.js applications?

---

# Testing & Debugging

231. How do you test a Next.js application?
232. What testing libraries do you use with Next.js?
233. How do you test Server Components?
234. How do you test Client Components?
235. How do you test Route Handlers?
236. How do you debug hydration mismatch errors?
237. How do you debug performance issues in production?
238. How do you debug caching problems?
239. How do you debug Middleware issues?
240. What tools do you use for monitoring and logging?

---

# Senior Real-World Interview Questions

241. What are the biggest mistakes developers make when building Next.js applications?
242. What are the most common performance issues you've solved in Next.js?
243. Describe a challenging Next.js bug you've fixed.
244. How would you migrate a React application to Next.js?
245. How would you migrate from the Pages Router to the App Router?
246. How do you review a Next.js pull request?
247. What best practices do you enforce in your team for Next.js development?
248. How would you build a production-ready SaaS application with Next.js?
249. If you were starting a new Next.js project today, what architecture, libraries, and tooling would you choose, and why?
250. In your opinion, what separates a junior, mid-level, and senior Next.js developer?

---


