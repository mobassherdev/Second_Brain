## React Interview Questions (300 Total)

---

### Part 1: React Fundamentals (1–50)

1. What is React?
2. Why was React created?
3. What problems does React solve?
4. What are the advantages of React?
5. What are the disadvantages of React?
6. What is the Virtual DOM?
7. How does the Virtual DOM work?
8. What is the difference between the Virtual DOM and the Real DOM?
9. What is reconciliation in React?
10. What is React Fiber?
11. What is JSX?
12. Why do we use JSX?
13. Can React work without JSX?
14. How does JSX get converted into JavaScript?
15. What is Babel, and what role does it play in React?
16. What is a React element?
17. What is the difference between a React element and a React component?
18. What are functional components?
19. What are class components?
20. Why are functional components preferred today?
21. What is the difference between functional and class components?
22. What is the render process in React?
23. What causes a React component to re-render?
24. What is the difference between rendering and re-rendering?
25. What is the React component lifecycle?
26. What are the lifecycle methods in class components?
27. How do lifecycle methods map to Hooks?
28. What is the difference between mounting, updating, and unmounting?
29. What are props in React?
30. Are props immutable? Why?
31. What is prop drilling?
32. How can you avoid prop drilling?
33. What is state in React?
34. What is the difference between props and state?
35. When should you use props versus state?
36. What is lifting state up?
37. What is controlled data flow in React?
38. What is one-way data binding?
39. What are controlled components?
40. What are uncontrolled components?
41. What are refs in React?
42. When should you use refs?
43. What is `React.Fragment`?
44. Why do we use fragments?
45. What are keys in React?
46. Why are keys important?
47. Why shouldn't you use array indexes as keys?
48. What happens if keys are missing or duplicated?
49. What are synthetic events in React?
50. How do synthetic events differ from native browser events?

---

### Components & JSX

51. What are reusable components in React?
52. What makes a good React component?
53. What is component composition?
54. What is the difference between composition and inheritance in React?
55. Why does React recommend composition over inheritance?
56. What is a higher-order component (HOC)?
57. When would you use a higher-order component?
58. What are the disadvantages of HOCs?
59. What is the render props pattern?
60. What is the difference between HOCs and render props?
61. What are compound components?
62. What is the children prop?
63. How do you use `props.children`?
64. What is `React.cloneElement()`?
65. When should you use `React.cloneElement()`?
66. What is `React.Children`?
67. What is `React.Children.map()`?
68. What is `React.Children.only()`?
69. What is `React.createElement()`?
70. How does JSX become `React.createElement()` calls?

---

### Rendering

71. What is conditional rendering?
72. How can you conditionally render components?
73. What is short-circuit rendering (`&&`)?
74. When should you use the ternary operator instead of `&&`?
75. What is null rendering?
76. What happens when a component returns `null`?
77. What is list rendering?
78. How do you render lists in React?
79. Why should every list item have a unique key?
80. What happens when keys change between renders?
81. What happens if two elements have the same key?
82. Why are random keys a bad idea?
83. Why shouldn't array indexes be used as keys?
84. What is dynamic rendering?
85. What is recursive rendering?
86. What is portal rendering?
87. What are React Portals?
88. When should you use React Portals?
89. How do portals differ from normal rendering?
90. What are common portal use cases?

---

### Forms

91. What are controlled components?
92. What are uncontrolled components?
93. What is the difference between controlled and uncontrolled components?
94. Which approach is recommended and why?
95. How do you handle form input in React?
96. How do you handle multiple form fields?
97. How do you validate forms in React?
98. What are the most popular React form libraries?
99. How do you reset a form in React?
100. How do you upload files in a React form?

---

## useState

101. What is the `useState` Hook?
102. Why do we use `useState`?
103. How does `useState` work internally?
104. What happens when `setState` is called?
105. Is `setState` synchronous or asynchronous?
106. What is functional state update?
107. When should you use the functional updater form of `setState`?
108. Can you store objects in state?
109. Can you store arrays in state?
110. Why shouldn't you mutate state directly?

---

## useEffect

111. What is the `useEffect` Hook?
112. Why do we use `useEffect`?
113. What are the different dependency array options in `useEffect`?
114. What happens if the dependency array is omitted?
115. What happens if the dependency array is empty (`[]`)?
116. What happens if dependencies change?
117. What is the cleanup function in `useEffect`?
118. When does the cleanup function run?
119. Why is cleanup important?
120. What are common mistakes when using `useEffect`?

---

## Dependency Arrays & Effects

121. What causes an infinite loop in `useEffect`?
122. How do you prevent infinite loops?
123. Why should all dependencies be included in the dependency array?
124. What is the `eslint-plugin-react-hooks` rule?
125. Can you ignore dependency warnings? When, if ever?
126. What is a stale closure in React?
127. How do stale closures happen?
128. How do you fix stale closure issues?
129. Can you make API calls inside `useEffect`?
130. How do you cancel an API request in `useEffect`?

---

## useRef

131. What is the `useRef` Hook?
132. What is the difference between `useRef` and `useState`?
133. When should you use `useRef`?
134. How do you focus an input using `useRef`?
135. Can updating a ref trigger a re-render?
136. What is `forwardRef`?
137. When should you use `forwardRef`?
138. What is `useImperativeHandle`?
139. When should you use `useImperativeHandle`?
140. What are common use cases for refs?

---

## Memoization Hooks

141. What is the `useMemo` Hook?
142. When should you use `useMemo`?
143. What is the `useCallback` Hook?
144. What is the difference between `useMemo` and `useCallback`?
145. When is memoization unnecessary?
146. What is `React.memo`?
147. What is the difference between `React.memo` and `useMemo`?
148. How do `React.memo` and `useCallback` work together?
149. What are the performance costs of memoization?
150. How do you decide whether to optimize with memoization?

---

## Context API

151. What is the Context API?
152. Why was Context API introduced?
153. What problems does Context API solve?
154. When should you use Context API?
155. When should you avoid Context API?
156. How do you create a Context?
157. What is a Provider?
158. What is a Consumer?
159. What is the `useContext` Hook?
160. How does Context trigger re-renders?

---

## useReducer

161. What is the `useReducer` Hook?
162. When should you use `useReducer` instead of `useState`?
163. What is a reducer function?
164. What are actions in `useReducer`?
165. How does dispatch work?
166. What are the advantages of `useReducer`?
167. Can `useReducer` replace Redux?
168. What are common use cases for `useReducer`?
169. Can `useReducer` be combined with Context API?
170. What are the limitations of `useReducer`?

---

## Custom Hooks

171. What is a custom Hook?
172. Why do we create custom Hooks?
173. What naming convention should custom Hooks follow?
174. Can one custom Hook use another custom Hook?
175. What are common real-world custom Hooks?
176. How do custom Hooks share logic?
177. Do custom Hooks share state?
178. What are the benefits of custom Hooks over HOCs?
179. What are the benefits of custom Hooks over render props?
180. What are common mistakes when writing custom Hooks?

---

## Advanced React Hooks

181. What is `useLayoutEffect`?
182. What is the difference between `useEffect` and `useLayoutEffect`?
183. When should you use `useLayoutEffect`?
184. What is `useTransition`?
185. What problems does `useTransition` solve?
186. What is `useDeferredValue`?
187. When should you use `useDeferredValue`?
188. What is `useId`?
189. Why is `useId` useful?
190. What is `useSyncExternalStore`?

---

## Performance & Optimization

191. What causes unnecessary re-renders in React?
192. How do you identify unnecessary re-renders?
193. How can you optimize React performance?
194. What is code splitting in React?
195. What is lazy loading?
196. What is `React.lazy()`?
197. What is `Suspense`?
198. What are Error Boundaries?
199. What tools do you use to profile React performance?
200. What performance optimization techniques have you used in production React applications?

---

## React Internals

201. What is React Fiber?
202. Why was React Fiber introduced?
203. How does the React Fiber architecture work?
204. What is reconciliation in React?
205. How does React's diffing algorithm work?
206. Why does React use the Virtual DOM?
207. How does React decide which components to re-render?
208. What is the commit phase in React?
209. What is the render phase in React?
210. What is concurrent rendering?

---

## Rendering Strategies

211. What is client-side rendering (CSR)?
212. What is server-side rendering (SSR)?
213. What is static site generation (SSG)?
214. What is incremental static regeneration (ISR)?
215. What are the advantages and disadvantages of CSR?
216. What are the advantages and disadvantages of SSR?
217. When would you choose CSR over SSR?
218. What causes hydration in React?
219. What is hydration mismatch?
220. How do you debug hydration issues?

---

## React 18 & React 19

221. What are the major features introduced in React 18?
222. What are concurrent features in React?
223. What is automatic batching?
224. How does automatic batching improve performance?
225. What are React Server Components?
226. What are Client Components?
227. What is the difference between Server Components and Client Components?
228. When should you use Server Components?
229. What new features were introduced in React 19?
230. How do React 18 and React 19 improve developer experience?

---

## Design Patterns

231. What is component composition?
232. What are compound components?
233. What is the Higher-Order Component (HOC) pattern?
234. When should you use HOCs?
235. What are the drawbacks of HOCs?
236. What is the Render Props pattern?
237. When should you use Render Props?
238. What are the advantages of custom Hooks over HOCs?
239. What are the advantages of custom Hooks over Render Props?
240. Which React design pattern do you prefer and why?

---

## Architecture & Best Practices

241. How do you structure a large React application?
242. How do you organize components in a scalable project?
243. How do you decide where state should live?
244. How do you avoid prop drilling in large applications?
245. How do you manage shared business logic?
246. What are common React anti-patterns?
247. How do you write reusable React components?
248. How do you debug complex React applications?
249. What React best practices do you follow in production?
250. How would you architect a large enterprise React application?

---

# Production & Debugging

251. How do you debug a React application in production?
252. A React page is re-rendering continuously. How would you debug it?
253. A component is rendering too slowly. How do you identify the bottleneck?
254. How do you debug unnecessary re-renders?
255. How do you profile React performance using React DevTools?
256. How do you debug memory leaks in React?
257. What are common causes of memory leaks in React applications?
258. How do you debug hydration errors in React?
259. How do you debug state synchronization issues?
260. How do you debug race conditions caused by asynchronous API calls?

---

# State Management Decisions

261. When is local component state enough?
262. When would you choose Context API?
263. When would you choose Redux Toolkit?
264. When would you choose Zustand?
265. When would you choose React Query or TanStack Query?
266. How do you decide whether state should be global or local?
267. What data should never be stored in global state?
268. How do you avoid overusing Context API?
269. How do you organize application state in a large React project?
270. How do you handle shared state across multiple pages?

---

# Testing

271. How do you test React components?
272. What is the difference between unit, integration, and end-to-end testing?
273. What is React Testing Library?
274. Why is React Testing Library preferred over Enzyme?
275. What is Jest?
276. How do you test asynchronous React components?
277. How do you mock API requests in tests?
278. What should you test in a React component?
279. What should you avoid testing?
280. How much test coverage is enough?

---

# Accessibility (A11y)

281. What is accessibility in React?
282. Why is accessibility important?
283. How do you make React applications accessible?
284. What are ARIA attributes?
285. How do you build accessible forms?
286. How do you ensure keyboard accessibility?
287. How do you test accessibility?
288. What tools do you use to check accessibility?
289. What are common accessibility mistakes in React applications?
290. How does semantic HTML improve accessibility in React?

---

# Real Senior Interview Questions

291. What are the biggest mistakes developers make in React?
292. What React features do you use most frequently in production?
293. What is the most challenging React bug you've fixed?
294. How do you review React code during a pull request?
295. What React best practices do you enforce in your team?
296. How do you onboard a new developer to a large React codebase?
297. If React didn't exist, what alternative would you choose and why?
298. What React features are you most excited about in the future?
299. How would you explain React to a junior developer?
300. If you were building a production React application today, what architecture, tools, and best practices would you choose, and why?

---
