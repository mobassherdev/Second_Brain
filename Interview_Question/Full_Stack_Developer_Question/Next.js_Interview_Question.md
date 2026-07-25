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
143. Where should API calls be madeâ€”server or client?
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

# ANSWERS

---

## Part 1 (1â€“10): Introduction

---

## Question 1: What is Next.js?

## Answer:
Next.js is a React framework built by Vercel that adds server-side rendering, static site generation, file-based routing, and many other production features out of the box. It's built on top of React but handles all the complex configuration that you'd otherwise do manually â€” bundling, routing, SSR, API routes, and more.

I use Next.js for almost every new React project because it gives me everything I need without assembling 15 different libraries together.

## Key Points:
- Next.js is a full-stack React framework, not just a library.
- Built on top of React with additional features like SSR, SSG, ISR, and App Router.
- Developed and maintained by Vercel.
- Supports both server-side and client-side rendering strategies.
- Has built-in API routes for backend logic.

## Interview Tip:
Don't just say "it's a React framework." Mention specific features like SSR, file-based routing, and built-in optimizations. Show that you understand why it exists beyond just "it's popular."

---

## Question 2: Why was Next.js created?

## Answer:
React by itself is just a UI library â€” it gives you components and a virtual DOM but doesn't handle routing, server rendering, code splitting, or deployment. Every team using React had to assemble their own stack: React Router for routing, a custom webpack config, SSR setup, and so on. Next.js was created to solve this by providing a batteries-included framework with sensible defaults.

It also solves the SEO problem that plain React has â€” since React renders in the browser, search engine crawlers often can't index the content. Next.js renders on the server first, so crawlers get fully rendered HTML.

## Key Points:
- React is a library, not a framework â€” it lacks routing, SSR, and build tooling.
- Next.js provides a complete solution with file-based routing, SSR, SSG, and more.
- Solves React's SEO problem by rendering content on the server.
- Reduces the number of decisions a team needs to make when starting a project.

## Interview Tip:
Frame it as "React is the engine, Next.js is the car." You need a car to actually drive â€” Next.js gives you the complete experience.

---

## Question 3: What problems does Next.js solve?

## Answer:
- **SEO**: React renders in the browser, so crawlers see empty HTML. Next.js pre-renders pages on the server.
- **Routing**: React Router requires manual setup. Next.js uses file-based routing automatically.
- **Performance**: Manual code splitting, image optimization, and font loading are complex. Next.js handles them built-in.
- **Build configuration**: Webpack and Babel configs are pre-configured and optimized.
- **API backend**: You can build your entire API in the same project using API routes or Route Handlers.

## Key Points:
- Solves SEO through server-side rendering and static generation.
- Eliminates need for React Router â€” file system becomes your router.
- Built-in code splitting, image optimization, and font optimization.
- Removes complex build configuration (Webpack, Babel, etc.).
- Enables full-stack development with API routes.

## Interview Tip:
Mention 2-3 of these problems with brief explanations rather than just listing them. Interviewers want depth, not a bulleted list.

---

## Question 4: What are the advantages of Next.js over React?

## Answer:
Next.js gives you server-side rendering out of the box, which React doesn't. You get automatic code splitting per page, built-in image optimization with `next/image`, font optimization with `next/font`, file-based routing, and API routes for your backend. It also has built-in SEO support with metadata APIs.

In plain React, you'd need to set up Webpack, React Router, SSR with something like `react-dom/server`, and a separate image optimization solution. Next.js handles all of this.

## Key Points:
- Server-side rendering and static generation built-in.
- Automatic code splitting â€” only loads JavaScript needed for each page.
- `next/image` handles image optimization (resizing, lazy loading, modern formats).
- File-based routing instead of manual route configuration.
- API routes or Route Handlers for serverless backend logic.

## Interview Tip:
Be specific. "SSR out of the box" is better than "better performance." Mention concrete features like `next/image` and file-based routing.

---

## Question 5: What are the disadvantages of Next.js?

## Answer:
- **Learning curve**: The App Router, Server Components, and caching model are complex to master.
- **Opinionated structure**: File-based routing is convenient but rigid â€” complex routing patterns can be harder than with React Router.
- **Overkill for SPAs**: If you just need a simple single-page app, Next.js adds unnecessary complexity.
- **Hosting dependency**: Some features work best on Vercel; other hosts may require extra configuration.
- **Frequent API changes**: The framework evolves fast â€” APIs change between major versions (Pages Router â†’ App Router).

## Key Points:
- Complex mental model with Server Components, Client Components, and caching.
- Not ideal for pure SPAs that don't need SSR or SEO.
- Some advanced features are optimized for Vercel hosting.
- Migration between router versions (Pages â†’ App) requires significant effort.

## Interview Tip:
Acknowledge the downsides honestly. It shows you've actually used the framework and aren't just repeating marketing points.

---

## Question 6: What is the difference between React and Next.js?

## Answer:
React is a JavaScript library for building user interfaces. Next.js is a full-stack framework built on top of React that adds routing, server rendering, API routes, and build optimizations.

React gives you components and state management. Next.js gives you those plus routing, SSR, SSG, ISR, middleware, image optimization, font optimization, and API routes.

## Key Points:
- React = library (UI only).
- Next.js = framework (full-stack).
- Next.js adds routing, SSR, SSG, API routes, and optimizations.
- React requires additional libraries for routing, SSR, etc.
- Next.js is built on top of React.

## Interview Tip:
Use an analogy: "React is the engine; Next.js is the complete car with wheels, chassis, and steering."

---

## Question 7: When would you choose React instead of Next.js?

## Answer:
- **Simple SPAs**: If you don't need SSR or SEO, React with Vite is simpler.
- **Existing architecture**: If you already have a backend and build system.
- **Mobile apps**: React Native uses React, not Next.js.
- **Widget/embedded**: If you're building a widget embedded in another app.
- **Learning**: If you're just learning React, start simple.

## Key Points:
- Simple SPAs without SEO needs.
- Existing backend infrastructure.
- Mobile development with React Native.
- Embedded widgets.
- Learning purposes.

## Interview Tip:
Show that you understand when NOT to use Next.js â€” it demonstrates maturity.

---

## Question 8: When would you choose Next.js instead of React?

## Answer:
- **SEO matters**: Blogs, e-commerce, marketing sites.
- **Full-stack app**: When you want API routes in the same project.
- **Performance**: When you need SSR, SSG, or ISR.
- **Team productivity**: File-based routing and built-in features speed up development.
- **Content-heavy sites**: When content changes frequently and needs indexing.

## Key Points:
- SEO-critical applications.
- Full-stack applications.
- Performance-sensitive applications.
- Content-heavy websites.
- Teams that want conventions over configuration.

## Interview Tip:
Give specific examples: "For an e-commerce site, I'd choose Next.js for SEO and performance. For a simple dashboard, React with Vite might be enough."

---

## Question 9: What is the App Router?

## Answer:
The App Router is Next.js's newer routing system introduced in version 13. It uses the `app` directory and supports React Server Components, nested layouts, loading states, error boundaries, and more.

It's the recommended approach for new Next.js projects and provides better performance, smaller bundle sizes, and more flexible data fetching compared to the Pages Router.

## Key Points:
- Introduced in Next.js 13.
- Uses `app` directory.
- Supports React Server Components.
- Nested layouts, loading states, error boundaries.
- Recommended for new projects.

## Interview Tip:
"The App Router is the future of Next.js â€” it's more powerful but has a steeper learning curve."

---

## Question 10: What is the Pages Router?

## Answer:
The Pages Router is the original routing system in Next.js that uses the `pages` directory. It's simpler and more familiar to developers who used Next.js before version 13.

It uses `getServerSideProps`, `getStaticProps`, and `getStaticPaths` for data fetching, and doesn't support React Server Components natively.

## Key Points:
- Original Next.js routing system.
- Uses `pages` directory.
- Data fetching with `getServerSideProps`, `getStaticProps`.
- Simpler but less powerful than App Router.
- Still supported but not recommended for new projects.

## Interview Tip:
"The Pages Router is still supported â€” many production apps use it. But the App Router is the future."

---

## Part 2 (11â€“20): App Router

---

## Question 11: What are the main features of the App Router?

## Answer:
- **React Server Components**: Components that run on the server.
- **Nested layouts**: Share UI across routes without re-rendering.
- **Loading states**: Built-in loading UI with `loading.tsx`.
- **Error handling**: Error boundaries with `error.tsx`.
- **Server Actions**: Form handling without API routes.
- **Streaming**: Progressive rendering for better performance.

## Key Points:
- Server Components for better performance.
- Nested layouts for shared UI.
- Built-in loading and error states.
- Server Actions for form handling.
- Streaming for progressive rendering.

## Interview Tip:
"The App Router adds Server Components, nested layouts, and streaming â€” all of which improve performance."

---

## Question 12: Why did Next.js introduce the App Router?

## Answer:
The App Router was introduced to:
1. **Leverage React Server Components**: Move rendering to the server for better performance.
2. **Improve developer experience**: Nested layouts, loading states, error boundaries.
3. **Enable streaming**: Progressive rendering for faster perceived performance.
4. **Simplify data fetching**: Async components, no `getServerSideProps` boilerplate.

## Key Points:
- Leverage React Server Components.
- Improve developer experience.
- Enable streaming.
- Simplify data fetching.

## Interview Tip:
"The App Router is Next.js's answer to the evolving React ecosystem â€” Server Components are the future."

---

## Question 13: What is the difference between the App Router and the Pages Router?

## Answer:
| Feature | App Router | Pages Router |
|---------|-----------|--------------|
| Directory | `app` | `pages` |
| Server Components | Yes | No |
| Nested Layouts | Yes | Limited |
| Data Fetching | Async components | getServerSideProps |
| Streaming | Yes | No |
| Server Actions | Yes | No |

## Key Points:
- App Router uses `app` directory; Pages Router uses `pages`.
- App Router supports Server Components; Pages Router doesn't.
- App Router has nested layouts; Pages Router has limited layout support.
- App Router uses async components; Pages Router uses getServerSideProps.
- App Router supports streaming; Pages Router doesn't.

## Interview Tip:
"The App Router is more powerful but has a steeper learning curve. Choose based on your project needs."

---

## Question 14: Which router would you use for a new project?

## Answer:
I would use the App Router for a new project. It's the recommended approach and provides better performance, smaller bundle sizes, and more flexible data fetching. The Server Components model reduces client-side JavaScript, and nested layouts make shared UI easier.

However, if the team is more familiar with the Pages Router and the project doesn't need Server Components, the Pages Router is still a solid choice.

## Key Points:
- App Router for new projects (recommended).
- Better performance with Server Components.
- Nested layouts for shared UI.
- Pages Router still valid for existing teams.

## Interview Tip:
"The App Router is the future, but the Pages Router is still production-ready. Choose based on your team's familiarity."

---

## Question 15: What is the `app` directory?

## Answer:
The `app` directory is where you define routes in the App Router. Each folder inside `app` represents a route segment. Special files like `page.tsx`, `layout.tsx`, `loading.tsx`, and `error.tsx` define the UI for each route.

```
app/
  page.tsx          â†’ /
  about/
    page.tsx        â†’ /about
  blog/
    [slug]/
      page.tsx      â†’ /blog/:slug
```

## Key Points:
- Defines routes in App Router.
- Each folder = route segment.
- Special files: page.tsx, layout.tsx, loading.tsx, error.tsx.
- File-based routing.

## Interview Tip:
"The `app` directory is your file-based router â€” each folder is a route."

---

## Question 16: What is the `page.tsx` file?

## Answer:
`page.tsx` defines the UI for a route segment. Without it, the route doesn't exist. It's the equivalent of a page component in the Pages Router.

```tsx
// app/page.tsx â†’ /
export default function Home() {
  return <h1>Home Page</h1>;
}
```

## Key Points:
- Defines UI for a route.
- Required for the route to exist.
- Export a React component as default.

## Interview Tip:
"No page.tsx, no route â€” it's that simple."

---

## Question 17: What is the `layout.tsx` file?

## Answer:
`layout.tsx` defines shared UI that wraps child routes. It persists across navigations and doesn't re-render when navigating between child routes.

```tsx
// app/layout.tsx
export default function RootLayout({ children }) {
  return (
    <html>
      <body>
        <nav>...</nav>
        {children}
      </body>
    </html>
  );
}
```

## Key Points:
- Shared UI across child routes.
- Persists across navigations.
- Doesn't re-render on navigation.
- Nested layouts supported.

## Interview Tip:
"Layouts are the killer feature â€” they persist across routes and don't re-render."

---

## Question 18: What is the `template.tsx` file?

## Answer:
`template.tsx` is similar to `layout.tsx` but re-renders on every navigation. Use it when you need fresh state or effects on each page.

```tsx
// app/template.tsx
export default function Template({ children }) {
  return <div>{children}</div>;
}
```

## Key Points:
- Similar to layout.tsx.
- Re-renders on every navigation.
- Use for fresh state/effects.
- Less common than layout.tsx.

## Interview Tip:
"Templates re-render on navigation; layouts don't. Use templates when you need fresh state."

---

## Question 19: What is the `loading.tsx` file?

## Answer:
`loading.tsx` defines a loading UI that shows while the page content is being fetched. It wraps the page in a React Suspense boundary automatically.

```tsx
// app/dashboard/loading.tsx
export default function Loading() {
  return <div>Loading dashboard...</div>;
}
```

## Key Points:
- Shows loading UI while page loads.
- Automatic Suspense boundary.
- Better user experience.
- Simple to implement.

## Interview Tip:
"loading.tsx gives users instant feedback while the page loads."

---

## Question 20: What is the `error.tsx` file?

## Answer:
`error.tsx` defines an error boundary for a route segment. When an error occurs, it catches the error and shows the fallback UI.

```tsx
// app/dashboard/error.tsx
'use client'
export default function Error({ error, reset }) {
  return (
    <div>
      <p>Error: {error.message}</p>
      <button onClick={() => reset()}>Try again</button>
    </div>
  );
}
```

## Key Points:
- Catches errors in route segment.
- Shows fallback UI.
- Must be a Client Component.
- Has access to error and reset.

## Interview Tip:
"error.tsx is your safety net â€” it catches errors and shows a user-friendly message."

---

## Part 3 (21â€“30): Components

---

## Question 21: What are Server Components?

## Answer:
Server Components are React components that run only on the server. They can directly access databases, file systems, and other server resources without exposing them to the client. They don't add JavaScript to the client bundle.

```tsx
// This runs on the server
async function UserProfile({ userId }) {
  const user = await db.user.findById(userId);
  return <div>{user.name}</div>;
}
```

## Key Points:
- Run only on the server.
- Can access server resources directly.
- Don't add to client JavaScript bundle.
- Can be async (use await).
- Default component type in App Router.

## Interview Tip:
"Server Components reduce client-side JavaScript â€” they're the default in the App Router."

---

## Question 22: What are Client Components?

## Answer:
Client Components are React components that run on both the client and server. They support interactivity (onClick, useState, useEffect) and are marked with `'use client'` at the top.

```tsx
'use client'
import { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);
  return <button onClick={() => setCount(count + 1)}>{count}</button>;
}
```

## Key Points:
- Run on client and server.
- Support interactivity.
- Mark with 'use client'.
- Add to client JavaScript bundle.
- Use for interactive UI.

## Interview Tip:
"Client Components are for interactivity â€” forms, buttons, state, effects."

---

## Question 23: What is the `"use client"` directive?

## Answer:
`'use client'` marks a component as a Client Component. It tells the bundler to include it in the client JavaScript bundle and allow client-side features like useState, useEffect, and event handlers.

```tsx
'use client'
// This is now a Client Component
```

## Key Points:
- Marks component as Client Component.
- Enables client-side features.
- Required for useState, useEffect, event handlers.
- Must be at the top of the file.

## Interview Tip:
"'use client' is the boundary between server and client â€” everything below it is client-side."

---

## Question 24: When should you use a Client Component?

## Answer:
Use Client Components when you need:
- **Interactivity**: onClick, onChange, onSubmit.
- **State**: useState, useReducer.
- **Effects**: useEffect, useLayoutEffect.
- **Browser APIs**: localStorage, window, document.
- **Third-party libraries** that use client features.

## Key Points:
- Interactive UI elements.
- State management.
- Side effects.
- Browser APIs.
- Client-side libraries.

## Interview Tip:
"If it needs interactivity, make it a Client Component. Otherwise, keep it as a Server Component."

---

## Question 25: When should you use a Server Component?

## Answer:
Use Server Components when you need:
- **Data fetching**: Direct database access.
- **Sensitive data**: API keys, secrets.
- **Large dependencies**: Keep them server-side.
- **Static content**: No interactivity needed.
- **Performance**: Reduce client-side JavaScript.

## Key Points:
- Data fetching.
- Sensitive data.
- Large dependencies.
- Static content.
- Performance optimization.

## Interview Tip:
"Server Components are the default â€” use them unless you need client-side features."

---

## Question 26: What are the benefits of Server Components?

## Answer:
- **Smaller bundle size**: No JavaScript sent to client.
- **Direct data access**: Query databases directly.
- **Security**: Sensitive code stays server-side.
- **Performance**: Faster initial page loads.
- **SEO**: Content rendered on server.

## Key Points:
- Reduced client-side JavaScript.
- Direct server resource access.
- Better security.
- Faster performance.
- Better SEO.

## Interview Tip:
"Server Components = less JavaScript, better performance, better security."

---

## Question 27: What are the limitations of Server Components?

## Answer:
- **No interactivity**: Can't use onClick, useState, useEffect.
- **No browser APIs**: Can't access localStorage, window.
- **Async only**: Must be async if fetching data.
- **No context**: Can't use React Context directly.
- **Limited third-party support**: Many libraries require client features.

## Key Points:
- No interactivity.
- No browser APIs.
- No React hooks (except async patterns).
- No React Context.
- Limited library support.

## Interview Tip:
"Server Components can't be interactive â€” that's the trade-off for better performance."

---

## Question 28: Can a Server Component import a Client Component?

## Answer:
Yes! Server Components can import and render Client Components. This is the recommended pattern â€” keep most of your app as Server Components and only use Client Components where needed.

```tsx
// Server Component
import LikeButton from './LikeButton'; // Client Component

function Post() {
  return (
    <div>
      <h1>Post Title</h1>
      <LikeButton /> {/* Client Component */}
    </div>
  );
}
```

## Key Points:
- Server Components can import Client Components.
- Recommended pattern.
- Keep most app as Server Components.
- Use Client Components only for interactivity.

## Interview Tip:
"Import Client Components into Server Components â€” don't make the entire app client-side."

---

## Question 29: Can a Client Component import a Server Component?

## Answer:
No! Client Components cannot import Server Components directly. However, you can pass Server Components as children or props to Client Components.

```tsx
// Client Component
'use client'
function Layout({ children }) {
  return <div>{children}</div>; // children can be Server Components
}
```

## Key Points:
- Client Components cannot import Server Components.
- Pass Server Components as children or props.
- Use the composition pattern.

## Interview Tip:
"You can't import Server Components into Client Components â€” use composition instead."

---

## Question 30: How do Server and Client Components communicate?

## Answer:
- **Props**: Server Components pass data as props to Client Components.
- **Children**: Server Components render as children of Client Components.
- **Server Actions**: Client Components call Server Actions for mutations.
- **URL**: Both can read URL parameters.

## Key Points:
- Props for data passing.
- Children for composition.
- Server Actions for mutations.
- URL for shared state.

## Interview Tip:
"Server and Client Components communicate through props, children, and Server Actions."

---

## Part 4 (31â€“40): Routing

---

## Question 31: How does file-based routing work?

## Answer:
File-based routing maps files and folders in the `app` directory to URL routes. Each `page.tsx` file defines a route, and folder structure determines the URL.

```
app/
  page.tsx          â†’ /
  about/
    page.tsx        â†’ /about
  blog/
    page.tsx        â†’ /blog
    [slug]/
      page.tsx      â†’ /blog/:slug
```

## Key Points:
- Files and folders map to routes.
- page.tsx defines a route.
- Folder structure = URL structure.
- Dynamic routes with [param].

## Interview Tip:
"File-based routing means your folder structure IS your URL structure."

---

## Question 32: What are dynamic routes?

## Answer:
Dynamic routes use square brackets `[param]` to capture URL parameters. The parameter value is available via `params`.

```tsx
// app/blog/[slug]/page.tsx
export default function BlogPost({ params }) {
  return <h1>Post: {params.slug}</h1>;
}
```

## Key Points:
- Use [param] syntax.
- Capture URL parameters.
- Access via params prop.
- Can have multiple dynamic segments.

## Interview Tip:
"Dynamic routes use [param] â€” the folder name becomes the parameter name."

---

## Question 33: What are nested routes?

## Answer:
Nested routes are routes inside other routes. They share the parent route's layout and URL segment.

```
app/
  dashboard/
    layout.tsx       â†’ shared dashboard layout
    page.tsx         â†’ /dashboard
    settings/
      page.tsx       â†’ /dashboard/settings
    analytics/
      page.tsx       â†’ /dashboard/analytics
```

## Key Points:
- Routes inside other routes.
- Share parent layout.
- URL segments nest.
- Layouts persist across nested routes.

## Interview Tip:
"Nested routes share layouts â€” the dashboard layout persists across settings and analytics."

---

## Question 34: What are catch-all routes?

## Answer:
Catch-all routes use `[...param]` to match any number of segments. The parameter is an array of all segments.

```tsx
// app/docs/[...slug]/page.tsx
export default function Docs({ params }) {
  // /docs/a/b/c â†’ params.slug = ['a', 'b', 'c']
  return <div>{params.slug.join('/')}</div>;
}
```

## Key Points:
- Match multiple segments.
- Parameter is an array.
- Useful for documentation, file browsers.
- [...param] syntax.

## Interview Tip:
"Catch-all routes match any depth â€” use them for documentation or file browsing."

---

## Question 35: What are optional catch-all routes?

## Answer:
Optional catch-all routes use `[[...param]]` to match zero or more segments. The parameter can be undefined.

```tsx
// app/shop/[[...slug]]/page.tsx
export default function Shop({ params }) {
  // /shop â†’ params.slug = undefined
  // /shop/shoes â†’ params.slug = ['shoes']
  // /shop/shoes/nike â†’ params.slug = ['shoes', 'nike']
  return <div>...</div>;
}
```

## Key Points:
- Match zero or more segments.
- Parameter can be undefined.
- [[...param]] syntax.
- More flexible than catch-all.

## Interview Tip:
"Optional catch-all routes handle both /shop and /shop/shoes/nike."

---

## Question 36: What is route grouping?

## Answer:
Route grouping uses parentheses `(folder)` to organize routes without affecting the URL structure. Grouped folders don't create URL segments.

```
app/
  (marketing)/
    about/page.tsx   â†’ /about
    contact/page.tsx â†’ /contact
  (shop)/
    products/page.tsx â†’ /products
    cart/page.tsx     â†’ /cart
```

## Key Points:
- Organize routes without URL impact.
- Use (folder) syntax.
- Don't create URL segments.
- Useful for organizing by feature.

## Interview Tip:
"Route groups organize your code without changing URLs â€” use them for feature-based organization."

---

## Question 37: What are parallel routes?

## Answer:
Parallel routes use `@folder` syntax to render multiple pages simultaneously in the same layout. They're useful for dashboards, modals, and split views.

```tsx
// app/dashboard/layout.tsx
export default function DashboardLayout({ children, analytics }) {
  return (
    <div>
      {children}
      {analytics}
    </div>
  );
}
```

## Key Points:
- Render multiple pages simultaneously.
- Use @folder syntax.
- Useful for dashboards and modals.
- Independent route segments.

## Interview Tip:
"Parallel routes let you render multiple pages side by side â€” great for dashboards."

---

## Question 38: What are intercepted routes?

## Answer:
Intercepted routes use `(..)` syntax to show a route segment in the current layout while keeping the URL. They're useful for modals that should maintain the URL.

```
app/
  feed/
    page.tsx          â†’ /feed
    [id]/
      page.tsx        â†’ /feed/:id
  (..)photo/
    [id]/
      page.tsx        â†’ intercepts /photo/:id in /feed layout
```

## Key Points:
- Show route in current layout.
- Maintain URL.
- Use (..) syntax.
- Great for modals.

## Interview Tip:
"Intercepted routes let you show a modal while keeping the URL â€” the best of both worlds."

---

## Question 39: What is the `Link` component?

## Answer:
`Link` is a Next.js component that enables client-side navigation. It prefetches pages for faster transitions and handles routing without full page reloads.

```tsx
import Link from 'next/link';

<Link href="/about">About</Link>
```

## Key Points:
- Client-side navigation.
- Prefetches pages.
- No full page reloads.
- Better performance than `<a>`.

## Interview Tip:
"Always use Link instead of <a> â€” it enables client-side navigation and prefetching."

---

## Question 40: Why should you use `Link` instead of `<a>`?

## Answer:
- **Client-side navigation**: No full page reload.
- **Prefetching**: Links are prefetched in the background.
- **Performance**: Faster transitions.
- **Scroll preservation**: Maintains scroll position.
- **Active state**: Easier to detect active links.

## Key Points:
- Client-side navigation.
- Prefetching.
- Better performance.
- Scroll preservation.
- Active state detection.

## Interview Tip:
"Link = client-side navigation with prefetching. <a> = full page reload."

---

## Part 5 (41â€“50): Navigation & Layouts

---

## Question 41: What is `useRouter()`?

## Answer:
`useRouter()` is a hook that gives you access to the router object for programmatic navigation.

```tsx
'use client'
import { useRouter } from 'next/navigation';

function Button() {
  const router = useRouter();
  return <button onClick={() => router.push('/dashboard')}>Go</button>;
}
```

## Key Points:
- Programmatic navigation.
- router.push() for navigation.
- router.replace() for replacement.
- router.back() for history.
- Must be a Client Component.

## Interview Tip:
"useRouter() is for programmatic navigation â€” use it in event handlers."

---

## Question 42: What is `usePathname()`?

## Answer:
`usePathname()` returns the current URL pathname as a string.

```tsx
'use client'
import { usePathname } from 'next/navigation';

function Navbar() {
  const pathname = usePathname();
  return <p>Current path: {pathname}</p>;
}
```

## Key Points:
- Returns current pathname.
- Reactive (updates on navigation).
- Useful for active link detection.
- Must be a Client Component.

## Interview Tip:
"usePathname() tells you where the user is â€” use it for active states."

---

## Question 43: What is `useSearchParams()`?

## Answer:
`useSearchParams()` returns the URL search parameters as a read-only URLSearchParams object.

```tsx
'use client'
import { useSearchParams } from 'next/navigation';

function Search() {
  const searchParams = useSearchParams();
  const query = searchParams.get('q');
  return <p>Search: {query}</p>;
}
```

## Key Points:
- Returns URL search parameters.
- Read-only.
- Reactive.
- Must be a Client Component.

## Interview Tip:
"useSearchParams() reads URL query parameters â€” great for search pages."

---

## Question 44: How do you navigate programmatically?

## Answer:
Use `useRouter()` hook for programmatic navigation:

```tsx
'use client'
import { useRouter } from 'next/navigation';

function Navigation() {
  const router = useRouter();
  
  return (
    <button onClick={() => router.push('/dashboard')}>
      Go to Dashboard
    </button>
  );
}
```

## Key Points:
- Use useRouter() hook.
- router.push() for navigation.
- router.replace() to replace history.
- router.back() to go back.

## Interview Tip:
"Programmatic navigation = useRouter() + router.push()."

---

## Question 45: What are nested layouts?

## Answer:
Nested layouts are layouts inside other layouts. They wrap child routes and persist across navigations. Each layout only re-renders when its own segment changes.

```
app/
  layout.tsx          â†’ Root layout (persists everywhere)
  dashboard/
    layout.tsx        â†’ Dashboard layout (persists in /dashboard)
    settings/
      layout.tsx      â†’ Settings layout (persists in /dashboard/settings)
```

## Key Points:
- Layouts inside other layouts.
- Persist across navigations.
- Only re-render when their segment changes.
- Share UI without re-rendering.

## Interview Tip:
"Nested layouts persist â€” the dashboard layout doesn't re-render when navigating to settings."

---

## Question 46: Why are layouts useful?

## Answer:
- **Performance**: Don't re-render on navigation.
- **Consistency**: Shared UI across routes.
- **State preservation**: Layout state persists.
- **Code reuse**: Write once, use everywhere.
- **Better UX**: Faster navigation.

## Key Points:
- Better performance (no re-render).
- Consistent UI.
- State preservation.
- Code reuse.
- Faster navigation.

## Interview Tip:
"Layouts are the killer feature â€” they persist and don't re-render."

---

## Question 47: How do layouts improve performance?

## Answer:
Layouts don't re-render when navigating between child routes. Only the child components re-render. This means:
- Less JavaScript execution.
- Faster navigation.
- Preserved layout state (scroll, form state).
- Shared components stay mounted.

## Key Points:
- No re-render on navigation.
- Less JavaScript execution.
- Faster transitions.
- State preservation.
- Shared components stay mounted.

## Interview Tip:
"Layouts improve performance by avoiding re-renders on navigation."

---

## Question 48: What is shared UI in Next.js?

## Answer:
Shared UI is UI that persists across multiple routes without re-rendering. In Next.js, this is achieved through layouts. Common examples:
- Navigation bars
- Sidebars
- Footers
- Authentication state

## Key Points:
- UI that persists across routes.
- Achieved through layouts.
- No re-render on navigation.
- Examples: nav, sidebar, footer.

## Interview Tip:
"Shared UI = layouts. They persist and don't re-render."

---

## Question 49: What is partial rendering?

## Answer:
Partial rendering means only the parts of the page that change are re-rendered during navigation. Layouts persist, and only the child components between layouts update.

When navigating from `/dashboard` to `/dashboard/settings`:
1. Root layout stays.
2. Dashboard layout stays.
3. Only the page content changes.

## Key Points:
- Only changed parts re-render.
- Layouts persist.
- Child components update.
- Faster navigation.

## Interview Tip:
"Partial rendering = only the changing parts re-render. Layouts stay."

---

## Question 50: What happens when navigating between pages in Next.js?

## Answer:
1. **Client-side navigation**: No full page reload.
2. **Layouts persist**: Only child components re-render.
3. **Prefetched**: Link components prefetch the target page.
4. **Loading states**: loading.tsx shows while new content loads.
5. **Partial rendering**: Only changed parts update.

## Key Points:
- Client-side navigation.
- Layouts persist.
- Prefetching.
- Loading states.
- Partial rendering.

## Interview Tip:
"Next.js navigation is client-side, partial rendering with prefetching."

---
