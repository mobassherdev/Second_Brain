## React Interview Questions (300 Total)

---

### Part 1: React Fundamentals (1â€“50)

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

# ANSWERS


---

## Part 1 (1â€“50): React Fundamentals

---

## Question 1: What is React?

## Answer:
React is a JavaScript library for building user interfaces, primarily for single-page applications. It was created by Facebook (now Meta) and is maintained by Meta and the open-source community.

React uses a component-based architecture where UIs are built from small, reusable pieces called components.

```jsx
function App() {
  return <h1>Hello, World!</h1>;
}
```

## Key Points:
- JavaScript library for building UIs.
- Component-based architecture.
- Created by Facebook (Meta).
- Uses Virtual DOM for performance.
- Declarative approach to UI.

## Interview Tip:
"React is a library, not a framework â€” it focuses on the view layer and gives you freedom for the rest."

---

## Question 2: Why was React created?

## Answer:
React was created at Facebook in 2011 by Jordan Walke to solve the challenge of building dynamic, data-driven UIs that update efficiently. Traditional DOM manipulation was slow and error-prone with complex UIs.

React introduced:
- **Declarative UI**: Describe what the UI should look like.
- **Component model**: Break UI into reusable pieces.
- **Virtual DOM**: Efficient updates.

## Key Points:
- Created at Facebook in 2011.
- Solve complex UI update problems.
- Declarative approach.
- Component-based architecture.
- Virtual DOM for performance.

## Interview Tip:
"React was created because building complex UIs with vanilla JavaScript was painful and error-prone."

---

## Question 3: What problems does React solve?

## Answer:
1. **Complex DOM manipulation**: Declarative UI instead of imperative DOM updates.
2. **UI state management**: Components manage their own state.
3. **Code reusability**: Components can be reused across the app.
4. **Performance**: Virtual DOM minimizes actual DOM updates.
5. **Data flow**: One-way data flow makes debugging easier.

## Key Points:
- Declarative UI.
- Component-based state management.
- Reusable components.
- Virtual DOM performance.
- Predictable data flow.

## Interview Tip:
"React solves the complexity of building interactive UIs with a declarative, component-based approach."

---

## Question 4: What are the advantages of React?

## Answer:
- **Declarative**: Describe UI, React handles updates.
- **Component-based**: Reusable, modular UI pieces.
- **Virtual DOM**: Efficient updates.
- **Rich ecosystem**: Redux, React Router, Next.js.
- **Large community**: Extensive resources and support.
- **React Native**: Share code with mobile apps.
- **JSX**: HTML-like syntax in JavaScript.

## Key Points:
- Declarative approach.
- Component reusability.
- Virtual DOM performance.
- Huge ecosystem.
- Cross-platform (React Native).

## Interview Tip:
"React's biggest advantages are its declarative nature, component model, and massive ecosystem."

---

## Question 5: What are the disadvantages of React?

## Answer:
- **Learning curve**: JSX, hooks, state management.
- **Boilerplate**: Need additional libraries for routing, state, etc.
- **Rapid changes**: Frequent API changes.
- **SEO challenges**: CSR requires SSR for SEO (Next.js solves this).
- **No opinionated structure**: Must choose your own patterns.

## Key Points:
- Learning curve for beginners.
- Need additional libraries.
- Fast-moving ecosystem.
- SEO needs SSR.
- Unopinionated.

## Interview Tip:
"React's main disadvantage is that it's unopinionated â€” you need to make many decisions yourself."

---

## Question 6: What is the Virtual DOM?

## Answer:
The Virtual DOM is a lightweight JavaScript representation of the actual DOM. React uses it to minimize expensive DOM operations by computing the minimal set of changes needed.

```
State Change â†’ New Virtual DOM â†’ Diff with Old Virtual DOM â†’ Update only changed nodes
```

## Key Points:
- Lightweight JS representation of DOM.
- Computes minimal changes.
- Minimizes expensive DOM operations.
- React's performance optimization.
- In-memory representation.

## Interview Tip:
"The Virtual DOM is React's performance secret â€” it computes the diff and updates only what changed."

---

## Question 7: How does the Virtual DOM work?

## Answer:
1. **State changes**: Component state updates.
2. **New Virtual DOM**: React creates a new Virtual DOM tree.
3. **Diffing**: React compares new and old Virtual DOM.
4. **Minimal updates**: Only changed nodes are updated in the real DOM.

## Key Points:
- State change triggers re-render.
- New Virtual DOM created.
- Diffing algorithm finds changes.
- Minimal real DOM updates.
- Batch updates for efficiency.

## Interview Tip:
"The Virtual DOM is a diffing mechanism â€” it finds what changed and updates only that."

---

## Question 8: What is the difference between the Virtual DOM and the Real DOM?

## Answer:
| Feature | Virtual DOM | Real DOM |
|---------|------------|----------|
| Type | JavaScript object | Browser API |
| Updates | Fast (in-memory) | Slow (reflow/repaint) |
| Manipulation | Declarative | Imperative |
| Performance | Optimized | Slower |

## Key Points:
- Virtual DOM: JS object, fast updates.
- Real DOM: Browser API, slow updates.
- Virtual DOM minimizes real DOM operations.
- React uses Virtual DOM for performance.

## Interview Tip:
"The Virtual DOM is a fast, in-memory representation â€” the real DOM is the slow browser API."

---

## Question 9: What is reconciliation in React?

## Answer:
Reconciliation is React's algorithm for comparing two Virtual DOM trees and determining what needs to change. It's the process of diffing the old and new Virtual DOM.

## Key Points:
- Algorithm for comparing Virtual DOM trees.
- Determines minimal changes.
- Uses heuristics for efficiency.
- O(n) complexity with assumptions.
- Part of React's rendering process.

## Interview Tip:
"Reconciliation is React's diffing algorithm â€” it finds what changed efficiently."

---

## Question 10: What is React Fiber?

## Answer:
React Fiber is the reconciliation engine introduced in React 16. It enables:
- **Incremental rendering**: Split work into chunks.
- **Prioritization**: Important updates first.
- **Pause and resume**: Non-blocking rendering.

## Key Points:
- Reconciliation engine (React 16+).
- Incremental rendering.
- Priority-based updates.
- Non-blocking rendering.
- Enables concurrent features.

## Interview Tip:
"Fiber enables concurrent rendering â€” React can pause and resume rendering for better UX."

---

## Question 11: What is JSX?

## Answer:
JSX is a syntax extension for JavaScript that looks like HTML. It's used in React to describe UI.

```jsx
const element = <h1 className="title">Hello, World!</h1>;
```

JSX is transpiled to `React.createElement()` calls by Babel.

## Key Points:
- Syntax extension for JavaScript.
- Looks like HTML in JavaScript.
- Transpiled by Babel.
- Produces `React.createElement()` calls.
- Not required but recommended.

## Interview Tip:
"JSX is syntactic sugar â€” it makes writing React components feel like writing HTML."

---

## Question 12: Why do we use JSX?

## Answer:
- **Readability**: HTML-like syntax is familiar.
- **Expressiveness**: Embed JavaScript expressions with `{}`.
- **Type safety**: Babel catches syntax errors.
- **Tooling**: Better IDE support and autocompletion.
- **Component composition**: Easy to nest components.

## Key Points:
- Familiar HTML-like syntax.
- Embed JS with `{}`.
- Better tooling support.
- Easier component composition.
- Not required but preferred.

## Interview Tip:
"JSX makes React code readable and expressive â€” it's the preferred way to write React."

---

## Question 13: Can React work without JSX?

## Answer:
Yes. JSX is syntactic sugar for `React.createElement()`. You can write React without JSX:

```jsx
// With JSX
const element = <h1 className="title">Hello</h1>;

// Without JSX
const element = React.createElement("h1", { className: "title" }, "Hello");
```

## Key Points:
- JSX is optional.
- `React.createElement()` is the underlying API.
- JSX is more readable.
- Both produce the same result.
- JSX is the standard practice.

## Interview Tip:
"React works without JSX, but JSX is much more readable â€” use it."

---

## Question 14: How does JSX get converted into JavaScript?

## Answer:
Babel (a JavaScript compiler) transpiles JSX into `React.createElement()` calls:

```jsx
// JSX
const el = <div className="box">Hello</div>;

// Compiled
const el = React.createElement("div", { className: "box" }, "Hello");
```

## Key Points:
- Babel transpiles JSX.
- Produces `React.createElement()` calls.
- Happens at build time.
- Modern React uses JSX transform (no need to import React).

## Interview Tip:
"Babel transforms JSX into `React.createElement()` calls at build time."

---

## Question 15: What is Babel, and what role does it play in React?

## Answer:
Babel is a JavaScript compiler that:
- **Transpiles JSX**: Converts JSX to `React.createElement()`.
- **Modern JS**: Converts ES6+ to browser-compatible JavaScript.
- **Polyfills**: Adds missing features for older browsers.

## Key Points:
- JavaScript compiler.
- Transpiles JSX.
- Converts modern JS.
- Build-time tool.
- Essential for React development.

## Interview Tip:
"Babel makes modern JavaScript and JSX work in all browsers."

---

## Question 16: What is a React element?

## Answer:
A React element is a plain JavaScript object that describes what should appear on screen. It's the smallest building block of React UI.

```jsx
const element = <h1>Hello</h1>;
// element is a plain JS object
```

## Key Points:
- Plain JavaScript object.
- Describes UI.
- Immutable.
- Created by `React.createElement()` or JSX.
- Building block of React UI.

## Interview Tip:
"Elements are the smallest units â€” they describe what to render."

---

## Question 17: What is the difference between a React element and a React component?

## Answer:
- **Element**: Plain object describing UI (immutable).
- **Component**: Function or class that returns elements (reusable).

```jsx
// Element
const el = <h1>Hello</h1>;

// Component
function Greeting() {
  return <h1>Hello</h1>;
}
```

## Key Points:
- Element: immutable object.
- Component: function/class returning elements.
- Components produce elements.
- Elements are the output; components are the factory.

## Interview Tip:
"Components produce elements â€” components are the recipe, elements are the dish."

---

## Question 18: What are functional components?

## Answer:
Functional components are JavaScript functions that return JSX. They're the modern way to write React components.

```jsx
function Greeting({ name }) {
  return <h1>Hello, {name}!</h1>;
}
```

## Key Points:
- JavaScript functions.
- Return JSX.
- Modern React standard.
- Use hooks for state and effects.
- Simpler than class components.

## Interview Tip:
"Functional components are the standard â€” use them with hooks for all new code."

---

## Question 19: What are class components?

## Answer:
Class components use ES6 classes and have access to lifecycle methods and state.

```jsx
class Greeting extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}!</h1>;
  }
}
```

## Key Points:
- ES6 classes.
- Extend `React.Component`.
- Lifecycle methods.
- `this.state` for state.
- Legacy pattern (hooks replaced them).

## Interview Tip:
"Class components are legacy â€” functional components with hooks are the standard."

---

## Question 20: Why are functional components preferred today?

## Answer:
- **Simpler syntax**: No `this` binding.
- **Hooks**: Access to state and lifecycle.
- **Smaller bundle**: Less code.
- **Easier to test**: Pure functions.
- **Better performance**: React optimizes functional components.
- **Concurrent features**: Better support for React 18+ features.

## Key Points:
- Simpler code.
- Hooks replace lifecycle methods.
- Smaller bundle size.
- Easier testing.
- Better concurrent support.

## Interview Tip:
"Functional components are simpler, smaller, and better optimized â€” use them."

---

## Question 21: What is the difference between functional and class components?

## Answer:
| Feature | Functional | Class |
|---------|-----------|-------|
| Syntax | Function | Class |
| State | `useState` | `this.state` |
| Lifecycle | `useEffect` | Lifecycle methods |
| `this` | No | Yes |
| Hooks | Yes | No |
| Simplicity | Simpler | More verbose |

## Key Points:
- Functional: hooks, simpler, modern.
- Class: lifecycle methods, `this`, legacy.
- Functional is the standard.
- Class components still work but aren't preferred.

## Interview Tip:
"Functional components with hooks are the modern standard â€” class components are legacy."

---

## Question 22: What is the render process in React?

## Answer:
1. **Trigger**: State or props change.
2. **Render phase**: Component function executes, Virtual DOM created.
3. **Reconciliation**: Diff old and new Virtual DOM.
4. **Commit phase**: Apply changes to real DOM.

## Key Points:
- Trigger â†’ Render â†’ Reconciliation â†’ Commit.
- Render phase creates Virtual DOM.
- Commit phase updates real DOM.
- Render phase can be interrupted (Fiber).
- Commit phase is synchronous.

## Interview Tip:
"React renders in two phases: render (Virtual DOM) and commit (real DOM)."

---

## Question 23: What causes a React component to re-render?

## Answer:
1. **State change**: `setState` or `useState` setter.
2. **Props change**: Parent re-renders with new props.
3. **Context change**: Context value changes.
4. **Parent re-render**: Parent component re-renders.

## Key Points:
- State changes.
- Props changes.
- Context changes.
- Parent re-renders.
- Not caused by variable mutations.

## Interview Tip:
"State, props, context, or parent re-render â€” those are the four triggers."

---

## Question 24: What is the difference between rendering and re-rendering?

## Answer:
- **Rendering**: Initial render of a component (first mount).
- **Re-rendering**: Subsequent renders due to state/props/context changes.

## Key Points:
- Rendering: first mount.
- Re-rendering: updates after mount.
- Both go through render and commit phases.
- Re-rendering is React's core mechanism.

## Interview Tip:
"Rendering is the first time; re-rendering is every update after that."

---

## Question 25: What is the React component lifecycle?

## Answer:
The lifecycle has three phases:
1. **Mounting**: Component is created and inserted into DOM.
2. **Updating**: Component re-renders due to state/props/context changes.
3. **Unmounting**: Component is removed from DOM.

## Key Points:
- Mounting: creation.
- Updating: re-renders.
- Unmounting: removal.
- Hooks handle all phases in functional components.

## Interview Tip:
"Mount â†’ Update â†’ Unmount â€” the three lifecycle phases."

---

## Question 26: What are the lifecycle methods in class components?

## Answer:
- **Mounting**: `constructor`, `componentDidMount`, `render`.
- **Updating**: `componentDidUpdate`, `render`.
- **Unmounting**: `componentWillUnmount`.
- **Error handling**: `componentDidCatch`.

## Key Points:
- `componentDidMount`: after mount.
- `componentDidUpdate`: after update.
- `componentWillUnmount`: before unmount.
- `componentDidCatch`: error handling.
- `render`: required method.

## Interview Tip:
"componentDidMount, componentDidUpdate, componentWillUnmount â€” the three main lifecycle methods."

---

## Question 27: How do lifecycle methods map to Hooks?

## Answer:
| Lifecycle Method | Hook Equivalent |
|-----------------|----------------|
| `componentDidMount` | `useEffect(() => {}, [])` |
| `componentDidUpdate` | `useEffect(() => {}, [deps])` |
| `componentWillUnmount` | `useEffect(() => { return () => {} }, [])` |
| `componentDidCatch` | `useErrorBoundary` (custom) |

## Key Points:
- `useEffect` handles most lifecycle scenarios.
- Empty `[]` for mount only.
- Dependencies for update.
- Cleanup function for unmount.

## Interview Tip:
"`useEffect` replaces most lifecycle methods â€” it's the hook equivalent."

---

## Question 28: What is the difference between mounting, updating, and unmounting?

## Answer:
- **Mounting**: Component created, inserted into DOM.
- **Updating**: Component re-renders due to state/props/context.
- **Unmounting**: Component removed from DOM.

## Key Points:
- Mounting: first render.
- Updating: re-renders.
- Unmounting: cleanup and removal.
- Each phase has specific hooks/methods.

## Interview Tip:
"Mount = create, Update = re-render, Unmount = cleanup."

---

## Question 29: What are props in React?

## Answer:
Props (properties) are read-only data passed from parent to child components.

```jsx
function Greeting({ name }) {
  return <h1>Hello, {name}!</h1>;
}

<Greeting name="Alice" />
```

## Key Points:
- Read-only data from parent.
- Passed as attributes.
- Immutable within component.
- One-way data flow.
- Can be any JavaScript value.

## Interview Tip:
"Props are how components communicate â€” parent to child, read-only."

---

## Question 30: Are props immutable? Why?

## Answer:
Yes, props are immutable. A component should never modify its own props. This ensures:
- **Predictability**: Data flows one way.
- **Debugging**: Easy to trace data source.
- **Reusability**: Components work with any data.

## Key Points:
- Props are read-only.
- Never modify props directly.
- One-way data flow.
- Parent controls the data.
- Predictable behavior.

## Interview Tip:
"Props are a contract â€” the parent provides them, the child reads them."

---

## Question 31: What is prop drilling?

## Answer:
Prop drilling is passing props through multiple intermediate components that don't need them, just to reach a deeply nested component.

```jsx
<App user={user} /> â†’ <Layout user={user} /> â†’ <Sidebar user={user} /> â†’ <Profile user={user} />
```

## Key Points:
- Passing props through many levels.
- Intermediate components don't use the props.
- Makes code harder to maintain.
- Solved by Context, Redux, or composition.

## Interview Tip:
"Prop drilling is passing data through components that don't need it â€” Context or state management solves it."

---

## Question 32: How can you avoid prop drilling?

## Answer:
1. **Context API**: Share data without prop drilling.
2. **State management**: Redux, Zustand.
3. **Component composition**: Use `children` prop.
4. **Custom hooks**: Encapsulate shared logic.

## Key Points:
- Context API for global data.
- State management for complex state.
- Composition for layout patterns.
- Custom hooks for logic reuse.

## Interview Tip:
"Context API is the built-in solution for prop drilling."

---

## Question 33: What is state in React?

## Answer:
State is mutable data managed within a component. When state changes, the component re-renders.

```jsx
const [count, setCount] = useState(0);
```

## Key Points:
- Mutable data within component.
- Triggers re-render on change.
- Managed with `useState` hook.
- Local to the component.
- Can be passed down as props.

## Interview Tip:
"State is the component's memory â€” when it changes, the component re-renders."

---

## Question 34: What is the difference between props and state?

## Answer:
| Feature | Props | State |
|---------|-------|-------|
| Source | Parent component | Component itself |
| Mutability | Immutable | Mutable |
| Purpose | Pass data down | Manage internal data |
| Update | Parent updates | Component updates |

## Key Points:
- Props: external, immutable, from parent.
- State: internal, mutable, managed locally.
- Props for configuration; state for data.
- Both trigger re-renders when changed.

## Interview Tip:
"Props are configuration from parent; state is internal data managed by the component."

---

## Question 35: When should you use props versus state?

## Answer:
- **Props**: Data from parent, configuration, callbacks.
- **State**: Internal data, UI state, form inputs, toggles.

## Key Points:
- Props for external data.
- State for internal data.
- Props for configuration.
- State for interactive data.

## Interview Tip:
"If the data comes from outside, use props. If the component manages it, use state."

---

## Question 36: What is lifting state up?

## Answer:
Lifting state up means moving state from a child component to a common parent so multiple children can share it.

```jsx
function Parent() {
  const [value, setValue] = useState("");
  return (
    <>
      <Input value={value} onChange={setValue} />
      <Display value={value} />
    </>
  );
}
```

## Key Points:
- Move state to common parent.
- Share state between siblings.
- Parent controls the data flow.
- Common pattern in React.

## Interview Tip:
"Lift state up when siblings need to share data â€” move it to their common parent."

---

## Question 37: What is controlled data flow in React?

## Answer:
Controlled data flow means React controls the form data through state. The input value is driven by React state, and changes go through event handlers.

```jsx
const [value, setValue] = useState("");
<input value={value} onChange={(e) => setValue(e.target.value)} />
```

## Key Points:
- React state controls input value.
- Event handlers update state.
- Single source of truth.
- Predictable behavior.
- Recommended approach.

## Interview Tip:
"Controlled components = React state is the source of truth for form data."

---

## Question 38: What is one-way data binding?

## Answer:
One-way data binding means data flows in one direction: parent to child (via props). Changes in the child don't automatically update the parent â€” the parent must pass callbacks.

## Key Points:
- Data flows parent â†’ child.
- Props down, events up.
- Predictable data flow.
- Easier to debug.
- React's design principle.

## Interview Tip:
"React's one-way data flow makes debugging easier â€” you always know where data comes from."

---

## Question 39: What are controlled components?

## Answer:
Controlled components have their value controlled by React state. The input value is set by state, and changes are handled by event handlers.

```jsx
const [name, setName] = useState("");
<input value={name} onChange={(e) => setName(e.target.value)} />
```

## Key Points:
- Value from React state.
- Changes via event handlers.
- React is the source of truth.
- Recommended approach.
- Predictable behavior.

## Interview Tip:
"Controlled components = React controls the value. Use them for forms."

---

## Question 40: What are uncontrolled components?

## Answer:
Uncontrolled components store their own state in the DOM. You use refs to access the value.

```jsx
const inputRef = useRef();
<input ref={inputRef} />
// Access: inputRef.current.value
```

## Key Points:
- DOM stores the value.
- Refs to access values.
- Less React control.
- Use for file inputs or simple forms.
- Not recommended for most cases.

## Interview Tip:
"Uncontrolled components use refs â€” use them only for file inputs or simple cases."

---

## Question 41: What are refs in React?

## Answer:
Refs (references) provide a way to access DOM elements or component instances directly.

```jsx
const inputRef = useRef(null);
<input ref={inputRef} />
```

## Key Points:
- Access DOM elements directly.
- `useRef` hook in functional components.
- Don't trigger re-renders.
- Use for DOM manipulation, focus, measurements.
- Avoid for data that affects rendering.

## Interview Tip:
"Refs are escape hatches â€” use them for DOM access, not for state."

---

## Question 42: When should you use refs?

## Answer:
- **Focus management**: Focus an input programmatically.
- **DOM measurements**: Get element dimensions.
- **Animations**: Integrate with animation libraries.
- **Third-party libraries**: Integrate non-React libraries.
- **Timers**: Store interval/timeout IDs.

## Key Points:
- Focus management.
- DOM measurements.
- Third-party integration.
- Timer storage.
- Not for rendering data.

## Interview Tip:
"Use refs for imperative actions â€” focus, measurements, and third-party integration."

---

## Question 43: What is `React.Fragment`?

## Answer:
`React.Fragment` lets you group elements without adding extra DOM nodes.

```jsx
// Short syntax
return (
  <>
    <h1>Title</h1>
    <p>Content</p>
  </>
);
```

## Key Points:
- Groups elements without extra DOM.
- Short syntax: `<>...</>`.
- Can have `key` prop (use `<Fragment key={}>`).
- Avoids unnecessary wrapper divs.

## Interview Tip:
"Fragments avoid unnecessary DOM nodes â€” use `<>...</>` for grouping."

---

## Question 44: Why do we use fragments?

## Answer:
- **Clean DOM**: No extra wrapper elements.
- **Flexibility**: Return multiple elements without a parent div.
- **Styling**: Avoid layout issues from wrapper divs.
- **Semantic HTML**: Keep HTML structure clean.

## Key Points:
- No extra DOM nodes.
- Return multiple elements.
- Cleaner HTML.
- Avoid layout issues.

## Interview Tip:
"Fragments keep the DOM clean â€” no unnecessary wrapper divs."

---

## Question 45: What are keys in React?

## Answer:
Keys are unique identifiers for elements in a list. They help React identify which items changed, were added, or were removed.

```jsx
{items.map(item => <li key={item.id}>{item.name}</li>)}
```

## Key Points:
- Unique identifiers for list items.
- Help React track changes.
- Must be unique among siblings.
- Should be stable (not array indexes).
- Essential for list rendering performance.

## Interview Tip:
"Keys help React efficiently update lists â€” use stable, unique IDs."

---

## Question 46: Why are keys important?

## Answer:
- **Performance**: React can efficiently update only changed items.
- **Identity**: React knows which element is which.
- **State preservation**: Component state is preserved correctly.
- **List reconciliation**: Enables efficient diffing.

## Key Points:
- Efficient list updates.
- Element identity.
- State preservation.
- Enables reconciliation.
- Critical for performance.

## Interview Tip:
"Without keys, React can't efficiently update lists â€” it would re-render everything."

---

## Question 47: Why shouldn't you use array indexes as keys?

## Answer:
Array indexes as keys cause issues when:
- **Items are reordered**: React thinks items changed.
- **Items are inserted/removed**: State gets mixed up.
- **Items have state**: State follows the wrong item.

```jsx
// Bad: index as key
{items.map((item, index) => <li key={index}>{item.name}</li>)}

// Good: stable ID
{items.map(item => <li key={item.id}>{item.name}</li>)}
```

## Key Points:
- Indexes change on reorder/insert/delete.
- State gets mixed up.
- Use stable, unique IDs.
- Only use indexes for static lists.

## Interview Tip:
"Use stable IDs as keys â€” indexes cause state bugs when lists change."

---

## Question 48: What happens if keys are missing or duplicated?

## Answer:
- **Missing**: React uses index as fallback (same problems).
- **Duplicated**: React can't distinguish elements, causes bugs.
- **Console warning**: React warns about missing/duplicate keys.

## Key Points:
- Missing keys trigger warnings.
- Duplicated keys cause bugs.
- Always provide unique keys.
- React warns in development.

## Interview Tip:
"Always provide unique keys â€” missing or duplicate keys cause subtle bugs."

---

## Question 49: What are synthetic events in React?

## Answer:
Synthetic events are React's cross-browser wrapper around native browser events. They have the same interface as native events but work consistently across browsers.

```jsx
function handleClick(e) {
  e.preventDefault(); // Works across browsers
  console.log(e.target);
}
```

## Key Points:
- Cross-browser event wrappers.
- Same interface as native events.
- Consistent behavior across browsers.
- React pools events (React 16).
- Use like native events.

## Interview Tip:
"Synthetic events are React's cross-browser event wrappers â€” they ensure consistent behavior."

---

## Question 50: How do synthetic events differ from native browser events?

## Answer:
- **Cross-browser**: Synthetic events work consistently.
- **Naming**: `onClick` vs `onclick`.
- **Pooling**: React 16 pooled events (React 17+ doesn't).
- **Propagation**: Same bubbling behavior.

## Key Points:
- Cross-browser consistency.
- camelCase naming.
- Same event interface.
- React handles event delegation.

## Interview Tip:
"Synthetic events are just cross-browser wrappers â€” use them like native events."

---

## Part 2 (51â€“70): Components & JSX

---

## Question 51: What are reusable components in React?

## Answer:
Reusable components are designed to be used in multiple places with different data. They accept props to customize their behavior.

```jsx
function Button({ label, onClick, variant = "primary" }) {
  return (
    <button className={`btn btn-${variant}`} onClick={onClick}>
      {label}
    </button>
  );
}
```

## Key Points:
- Used in multiple places.
- Accept props for customization.
- Single responsibility.
- Well-documented API.
- Testable in isolation.

## Interview Tip:
"Reusable components accept props and have a single responsibility."

---

## Question 52: What makes a good React component?

## Answer:
- **Single responsibility**: Does one thing well.
- **Reusable**: Works with different data.
- **Testable**: Easy to test in isolation.
- **Self-contained**: Manages its own concerns.
- **Clear API**: Well-defined props.

## Key Points:
- Single responsibility.
- Reusable and testable.
- Clear props API.
- Self-contained.
- Well-documented.

## Interview Tip:
"A good component does one thing well and is easy to reuse."

---

## Question 53: What is component composition?

## Answer:
Component composition is combining simple components to build complex UIs.

```jsx
function App() {
  return (
    <Layout>
      <Header />
      <Content />
      <Footer />
    </Layout>
  );
}
```

## Key Points:
- Combine simple components.
- Build complex UIs from pieces.
- React's core pattern.
- More flexible than inheritance.
- Use `children` prop.

## Interview Tip:
"Composition is React's core pattern â€” build complex UIs from simple pieces."

---

## Question 54: What is the difference between composition and inheritance in React?

## Answer:
- **Composition**: Combine components using `children` or props.
- **Inheritance**: Extend component classes.

React recommends composition over inheritance.

## Key Points:
- Composition: combine with props/children.
- Inheritance: extend classes.
- React prefers composition.
- More flexible and simpler.

## Interview Tip:
"React recommends composition â€” use `children` and props instead of inheritance."

---

## Question 55: Why does React recommend composition over inheritance?

## Answer:
- **Flexibility**: Components can render anything via props.
- **Simplicity**: No complex class hierarchies.
- **Reusability**: Components are more reusable.
- **Testability**: Easier to test.

## Key Points:
- More flexible.
- Simpler code.
- Better reusability.
- Easier testing.
- React's design philosophy.

## Interview Tip:
"Composition is more flexible â€” you can render anything via props."

---

## Question 56: What is a higher-order component (HOC)?

## Answer:
A HOC is a function that takes a component and returns a new component with enhanced functionality.

```jsx
function withAuth(Component) {
  return function AuthenticatedComponent(props) {
    if (!isAuthenticated) return <Redirect to="/login" />;
    return <Component {...props} />;
  };
}

const ProtectedDashboard = withAuth(Dashboard);
```

## Key Points:
- Function that takes a component, returns enhanced component.
- Adds functionality without modifying original.
- Pattern from functional programming.
- Used for cross-cutting concerns.
- Being replaced by custom hooks.

## Interview Tip:
"HOCs add functionality to components â€” but custom hooks are usually better today."

---

## Question 57: When would you use a higher-order component?

## Answer:
- **Authentication**: Protect routes.
- **Data fetching**: Add loading/error states.
- **Logging**: Track component usage.
- **Theming**: Inject theme props.

## Key Points:
- Cross-cutting concerns.
- Authentication wrappers.
- Data fetching abstractions.
- Logging and analytics.
- Being replaced by hooks.

## Interview Tip:
"HOCs are for cross-cutting concerns â€” but custom hooks are usually preferred."

---

## Question 58: What are the disadvantages of HOCs?

## Answer:
- **Wrapper hell**: Deep nesting of HOCs.
- **Prop collisions**: Multiple HOCs may use same prop names.
- **Static composition**: Can't use hooks inside.
- **Ref forwarding**: Requires `forwardRef`.
- **Debugging**: Harder to trace in DevTools.

## Key Points:
- Wrapper hell.
- Prop collisions.
- No hooks inside.
- Ref forwarding issues.
- Custom hooks are cleaner.

## Interview Tip:
"HOCs cause wrapper hell and prop collisions â€” custom hooks avoid these issues."

---

## Question 59: What is the render props pattern?

## Answer:
Render props is a pattern where a component receives a function as a prop and calls it to render content.

```jsx
function MouseTracker({ render }) {
  const [pos, setPos] = useState({ x: 0, y: 0 });
  return render(pos);
}

<MouseTracker render={({ x, y }) => <p>{x}, {y}</p>} />
```

## Key Points:
- Function as a prop.
- Component calls the function to render.
- Shares data with the caller.
- Flexible rendering.
- Being replaced by hooks.

## Interview Tip:
"Render props share data via a function â€” but hooks are usually cleaner."

---

## Question 60: What is the difference between HOCs and render props?

## Answer:
- **HOCs**: Function that wraps a component.
- **Render props**: Component that takes a render function.

Both share data with components, but render props are more explicit.

## Key Points:
- HOCs: wrap components.
- Render props: function as prop.
- Both share data.
- Both being replaced by hooks.

## Interview Tip:
"Both are patterns for sharing logic â€” hooks are usually better."

---

## Question 61: What are compound components?

## Answer:
Compound components work together to form a complete UI. They share implicit state.

```jsx
<Select>
  <Select.Option value="1">Option 1</Select.Option>
  <Select.Option value="2">Option 2</Select.Option>
</Select>
```

## Key Points:
- Components work together.
- Share implicit state.
- Clean API for consumers.
- Flexible composition.
- Common in UI libraries.

## Interview Tip:
"Compound components share state implicitly â€” they work together as a unit."

---

## Question 62: What is the children prop?

## Answer:
`children` is a special prop that contains the content between a component's opening and closing tags.

```jsx
function Card({ children }) {
  return <div className="card">{children}</div>;
}

<Card>
  <h1>Title</h1>
  <p>Content</p>
</Card>
```

## Key Points:
- Special prop for nested content.
- Can be any React node.
- Enables composition.
- Fundamental pattern.

## Interview Tip:
"`children` is how components compose â€” it's the content between tags."

---

## Question 63: How do you use `props.children`?

## Answer:
```jsx
function Layout({ children }) {
  return (
    <div className="layout">
      <Header />
      <main>{children}</main>
      <Footer />
    </div>
  );
}
```

## Key Points:
- Render nested content.
- Enables layout patterns.
- Can be any React node.
- Fundamental composition pattern.

## Interview Tip:
"`props.children` enables layout patterns â€” wrap content with shared UI."

---

## Question 64: What is `React.cloneElement()`?

## Answer:
`React.cloneElement()` clones a React element and merges new props.

```jsx
const enhanced = React.cloneElement(element, { className: "extra" });
```

## Key Points:
- Clones element with new props.
- Merges existing and new props.
- Use sparingly.
- Common in HOCs and libraries.

## Interview Tip:
"`cloneElement` is for advanced patterns â€” use sparingly."

---

## Question 65: When should you use `React.cloneElement()`?

## Answer:
- **Injecting props**: Add props to children in libraries.
- **Enhancing elements**: Modify child elements.
- **Library patterns**: When building component libraries.

## Key Points:
- Library patterns.
- Injecting props into children.
- Use sparingly.
- Prefer composition.

## Interview Tip:
"`cloneElement` is for library authors â€” prefer composition in application code."

---

## Question 66: What is `React.Children`?

## Answer:
`React.Children` provides utilities for working with the `children` prop.

```jsx
React.Children.map(children, child => ...)
React.Children.forEach(children, child => ...)
React.Children.count(children)
React.Children.only(children)
```

## Key Points:
- Utilities for `children` prop.
- Map, forEach, count, only.
- Handles edge cases.
- Use for library patterns.

## Interview Tip:
"`React.Children` utilities handle edge cases when working with children."

---

## Question 67: What is `React.Children.map()`?

## Answer:
`React.Children.map()` iterates over children, handling arrays, fragments, and null.

```jsx
React.Children.map(children, (child, index) => {
  return React.cloneElement(child, { index });
});
```

## Key Points:
- Iterates over children safely.
- Handles arrays and fragments.
- Returns new array.
- Better than `children.map()`.

## Interview Tip:
"`React.Children.map()` handles edge cases that `children.map()` doesn't."

---

## Question 68: What is `React.Children.only()`?

## Answer:
`React.Children.only()` returns the only child or throws an error if there are multiple children.

```jsx
function Wrapper({ children }) {
  return React.Children.only(children);
}
```

## Key Points:
- Returns single child.
- Throws if multiple children.
- Enforces single child.
- Use for wrapper components.

## Interview Tip:
"`React.Children.only()` enforces a single child â€” useful for wrapper components."

---

## Question 69: What is `React.createElement()`?

## Answer:
`React.createElement()` creates a React element. JSX compiles to this.

```jsx
React.createElement("div", { className: "box" }, "Hello");
// Same as: <div className="box">Hello</div>
```

## Key Points:
- Creates React elements.
- JSX compiles to this.
- Low-level API.
- Rarely used directly.

## Interview Tip:
"`React.createElement()` is what JSX compiles to â€” you rarely use it directly."

---

## Question 70: How does JSX become `React.createElement()` calls?

## Answer:
Babel transforms JSX during build:

```jsx
// JSX
<div className="box">Hello</div>

// Compiled
React.createElement("div", { className: "box" }, "Hello")
```

## Key Points:
- Babel transpiles JSX.
- Produces `React.createElement()` calls.
- Build-time transformation.
- Same result either way.

## Interview Tip:
"Babel transforms JSX into `React.createElement()` calls at build time."

---

## Part 3 (71â€“90): Rendering

---

## Question 71: What is conditional rendering?

## Answer:
Conditional rendering shows different UI based on conditions.

```jsx
function Greeting({ isLoggedIn }) {
  if (isLoggedIn) return <h1>Welcome back!</h1>;
  return <h1>Please sign in.</h1>;
}
```

## Key Points:
- Show different UI based on conditions.
- Use `if`, ternary, or `&&`.
- Common pattern in React.
- Clean and declarative.

## Interview Tip:
"Conditional rendering is just JavaScript â€” use `if`, ternary, or `&&`."

---

## Question 72: How can you conditionally render components?

## Answer:
```jsx
// If/else
if (loading) return <Spinner />;
if (error) return <Error />;
return <Content />;

// Ternary
{isLoggedIn ? <Dashboard /> : <Login />}

// Logical AND
{hasPermission && <AdminPanel />}
```

## Key Points:
- `if/else` for early returns.
- Ternary for two options.
- `&&` for show/hide.
- Clean and declarative.

## Interview Tip:
"Ternary for two options, `&&` for show/hide, `if/else` for early returns."

---

## Question 73: What is short-circuit rendering (`&&`)?

## Answer:
Short-circuit rendering shows content only when a condition is true.

```jsx
{isLoggedIn && <Dashboard />}
```

If `isLoggedIn` is false, nothing renders.

## Key Points:
- Show content when condition is true.
- Uses `&&` operator.
- False condition renders nothing.
- Common pattern.

## Interview Tip:
"`&&` renders the right side only when the left side is truthy."

---

## Question 74: When should you use the ternary operator instead of `&&`?

## Answer:
Use ternary when you have two options (true and false). Use `&&` when you only show content on true.

```jsx
// Ternary: two options
{isLoggedIn ? <Dashboard /> : <Login />}

// &&: only true
{hasPermission && <AdminPanel />}
```

## Key Points:
- Ternary: two options.
- `&&`: only true case.
- Choose based on use case.

## Interview Tip:
"Ternary for two options; `&&` for show/hide."

---

## Question 75: What is null rendering?

## Answer:
Returning `null` from a component renders nothing.

```jsx
function Warning({ show }) {
  if (!show) return null;
  return <div className="warning">Warning!</div>;
}
```

## Key Points:
- `return null` renders nothing.
- Component is still mounted.
- Common for conditional components.
- Doesn't affect parent.

## Interview Tip:
"`return null` means render nothing â€” the component is still mounted."

---

## Question 76: What happens when a component returns `null`?

## Answer:
Nothing is rendered to the DOM. The component is still mounted and its lifecycle hooks still run.

## Key Points:
- Nothing rendered.
- Component still mounted.
- Effects still run.
- Common for conditional UI.

## Interview Tip:
"Returning `null` hides the component visually but it's still alive."

---

## Question 77: What is list rendering?

## Answer:
List rendering displays a collection of items using `.map()`.

```jsx
function TodoList({ todos }) {
  return (
    <ul>
      {todos.map(todo => (
        <li key={todo.id}>{todo.text}</li>
      ))}
    </ul>
  );
}
```

## Key Points:
- Use `.map()` for lists.
- Always provide `key` prop.
- Keys must be unique.
- Efficient updates with keys.

## Interview Tip:
"List rendering = `.map()` with unique keys."

---

## Question 78: How do you render lists in React?

## Answer:
```jsx
{items.map(item => (
  <Item key={item.id} {...item} />
))}
```

Always provide a unique `key` for each item.

## Key Points:
- `.map()` to iterate.
- `key` for each item.
- Unique, stable keys.
- Component per item.

## Interview Tip:
"`map()` with unique keys â€” that's the pattern."

---

## Question 79: Why should every list item have a unique key?

## Answer:
Keys help React:
- **Identify items**: Know which item is which.
- **Efficient updates**: Only update changed items.
- **Preserve state**: Keep component state correct.
- **Reorder correctly**: Handle list reordering.

## Key Points:
- Item identity.
- Efficient updates.
- State preservation.
- Correct reordering.

## Interview Tip:
"Keys give React a stable identity for each list item."

---

## Question 80: What happens when keys change between renders?

## Answer:
React treats items with changed keys as new elements â€” it unmounts the old and mounts the new. This causes:
- **State loss**: Component state is reset.
- **Performance**: Unnecessary mount/unmount.
- **Animation issues**: Transitions break.

## Key Points:
- Changed key = new element.
- State is lost.
- Performance impact.
- Use stable keys.

## Interview Tip:
"Changing keys causes React to unmount and remount â€” state is lost."

---

## Question 81: What happens if two elements have the same key?

## Answer:
React can't distinguish them â€” it may update the wrong element, causing bugs and warnings.

## Key Points:
- React can't distinguish elements.
- May update wrong element.
- Causes bugs and warnings.
- Always use unique keys.

## Interview Tip:
"Duplicate keys cause subtle bugs â€” always use unique keys."

---

## Question 82: Why are random keys a bad idea?

## Answer:
Random keys change every render, causing React to unmount and remount all items every time.

```jsx
// Bad: random key
{items.map(item => <li key={Math.random()}>{item.name}</li>)}
```

## Key Points:
- Keys change every render.
- Unmount/remount all items.
- State loss.
- Terrible performance.
- Use stable IDs.

## Interview Tip:
"Random keys defeat the purpose of keys â€” use stable IDs."

---

## Question 83: Why shouldn't array indexes be used as keys?

## Answer:
When items are reordered, inserted, or deleted, the index changes. This causes:
- **State bugs**: State follows the wrong item.
- **Performance**: Unnecessary re-renders.
- **Animation issues**: Transitions break.

## Key Points:
- Indexes change on list mutations.
- State follows wrong item.
- Use stable, unique IDs.
- Only OK for static lists.

## Interview Tip:
"Indexes as keys cause state bugs when lists change â€” use IDs."

---

## Question 84: What is dynamic rendering?

## Answer:
Dynamic rendering generates UI based on data at runtime.

```jsx
function UserList({ users }) {
  return users.map(user => <UserCard key={user.id} user={user} />);
}
```

## Key Points:
- UI generated from data.
- Data drives the output.
- Common pattern in React.
- List and conditional rendering.

## Interview Tip:
"Dynamic rendering = data drives the UI."

---

## Question 85: What is recursive rendering?

## Answer:
Recursive rendering is when a component renders itself.

```jsx
function TreeNode({ node }) {
  return (
    <div>
      {node.name}
      {node.children?.map(child => (
        <TreeNode key={child.id} node={child} />
      ))}
    </div>
  );
}
```

## Key Points:
- Component renders itself.
- For tree structures.
- Each level renders children.
- Common for comments, folders.

## Interview Tip:
"Recursive rendering is for tree structures â€” comments, folders, categories."

---

## Question 86: What is portal rendering?

## Answer:
Portals render children into a DOM node outside the parent component's DOM hierarchy.

```jsx
ReactDOM.createPortal(children, container);
```

## Key Points:
- Render outside parent DOM.
- Same React tree.
- Different DOM position.
- For modals, tooltips, overlays.

## Interview Tip:
"Portals render in a different DOM node but stay in the React tree."

---

## Question 87: What are React Portals?

## Answer:
Portals provide a way to render children into a DOM node that exists outside the parent component's DOM hierarchy.

```jsx
function Modal({ children }) {
  return ReactDOM.createPortal(
    <div className="modal">{children}</div>,
    document.getElementById("modal-root")
  );
}
```

## Key Points:
- Render outside parent DOM.
- Same React context.
- For modals, tooltips, dropdowns.
- Event bubbling works correctly.

## Interview Tip:
"Portals are for rendering outside the parent DOM â€” modals and tooltips."

---

## Question 88: When should you use React Portals?

## Answer:
- **Modals**: Render outside layout hierarchy.
- **Tooltips**: Position relative to viewport.
- **Dropdowns**: Avoid overflow issues.
- **Notifications**: Toast messages.

## Key Points:
- Modals and dialogs.
- Tooltips and popovers.
- Dropdowns.
- Notifications.
- Anything needing to escape parent CSS.

## Interview Tip:
"Use portals when a component needs to escape its parent's CSS (overflow, z-index)."

---

## Question 89: How do portals differ from normal rendering?

## Answer:
- **DOM position**: Portals render in a different DOM node.
- **React tree**: Same React context and event bubbling.
- **CSS isolation**: Escapes parent CSS constraints.

## Key Points:
- Different DOM position.
- Same React tree.
- Events bubble correctly.
- CSS isolation.

## Interview Tip:
"Portals change DOM position but keep React tree â€” events still bubble correctly."

---

## Question 90: What are common portal use cases?

## Answer:
- **Modals**: Full-screen overlays.
- **Tooltips**: Positioned tooltips.
- **Dropdowns**: Menu dropdowns.
- **Toasts**: Notification messages.
- **Loading overlays**: Full-screen loading.

## Key Points:
- Modals and dialogs.
- Tooltips and popovers.
- Dropdowns and menus.
- Toasts and notifications.
- Loading overlays.

## Interview Tip:
"Modals are the most common portal use case."

---

## Part 4 (91â€“100): Forms

---

## Question 91: What are controlled components?

## Answer:
Controlled components have their value controlled by React state.

```jsx
const [value, setValue] = useState("");
<input value={value} onChange={(e) => setValue(e.target.value)} />
```

## Key Points:
- Value from React state.
- Changes via event handlers.
- React is source of truth.
- Recommended approach.

## Interview Tip:
"Controlled components = React controls the value."

---

## Question 92: What are uncontrolled components?

## Answer:
Uncontrolled components store their value in the DOM, accessed via refs.

```jsx
const inputRef = useRef();
<input ref={inputRef} defaultValue="hello" />
```

## Key Points:
- DOM stores value.
- Refs to access.
- Less control.
- Use for file inputs.

## Interview Tip:
"Uncontrolled components use refs â€” simpler but less control."

---

## Question 93: What is the difference between controlled and uncontrolled components?

## Answer:
| Feature | Controlled | Uncontrolled |
|---------|-----------|--------------|
| Value source | React state | DOM |
| Access | State variable | Ref |
| Validation | On change | On submit |
| Control | Full | Limited |

## Key Points:
- Controlled: React state, full control.
- Uncontrolled: DOM, refs, less control.
- Controlled is recommended.
- Uncontrolled for file inputs.

## Interview Tip:
"Controlled for most forms; uncontrolled for file inputs."

---

## Question 94: Which approach is recommended and why?

## Answer:
Controlled components are recommended because:
- **Single source of truth**: React state.
- **Validation**: Instant feedback.
- **Control**: Full control over input.
- **Predictability**: Declarative approach.

## Key Points:
- Single source of truth.
- Instant validation.
- Full control.
- Predictable behavior.
- Industry standard.

## Interview Tip:
"Controlled components are the standard â€” they give you full control."

---

## Question 95: How do you handle form input in React?

## Answer:
```jsx
function Form() {
  const [formData, setFormData] = useState({ name: "", email: "" });

  const handleChange = (e) => {
    setFormData({ ...formData, [e.target.name]: e.target.value });
  };

  const handleSubmit = (e) => {
    e.preventDefault();
    console.log(formData);
  };

  return (
    <form onSubmit={handleSubmit}>
      <input name="name" value={formData.name} onChange={handleChange} />
      <input name="email" value={formData.email} onChange={handleChange} />
      <button type="submit">Submit</button>
    </form>
  );
}
```

## Key Points:
- State for form data.
- `onChange` handler.
- `onSubmit` handler.
- `e.preventDefault()`.
- Controlled inputs.

## Interview Tip:
"Use state for form data, onChange for updates, onSubmit for submission."

---

## Question 96: How do you handle multiple form fields?

## Answer:
Use a single state object with computed property names:

```jsx
const [form, setForm] = useState({ name: "", email: "" });

const handleChange = (e) => {
  setForm({ ...form, [e.target.name]: e.target.value });
};
```

## Key Points:
- Single state object.
- Computed property names.
- One handler for all fields.
- `name` attribute matches state key.

## Interview Tip:
"One state object, one handler, computed property names â€” clean and scalable."

---

## Question 97: How do you validate forms in React?

## Answer:
```jsx
const [errors, setErrors] = useState({});

const validate = () => {
  const newErrors = {};
  if (!form.name) newErrors.name = "Name is required";
  if (!form.email.includes("@")) newErrors.email = "Invalid email";
  setErrors(newErrors);
  return Object.keys(newErrors).length === 0;
};

const handleSubmit = (e) => {
  e.preventDefault();
  if (validate()) { /* submit */ }
};
```

## Key Points:
- Validate on submit or change.
- Track errors in state.
- Display error messages.
- Use libraries (Zod, Yup) for complex validation.

## Interview Tip:
"Validate on submit, track errors in state, display error messages."

---

## Question 98: What are the most popular React form libraries?

## Answer:
- **React Hook Form**: Performance, minimal re-renders.
- **Formik**: Full-featured, popular.
- **Zod**: Schema validation (with React Hook Form).
- **Yup**: Schema validation (with Formik).

## Key Points:
- React Hook Form: best performance.
- Formik: full-featured.
- Zod/Yup: validation schemas.
- Choose based on needs.

## Interview Tip:
"React Hook Form + Zod is the modern standard for React forms."

---

## Question 99: How do you reset a form in React?

## Answer:
```jsx
const handleSubmit = (e) => {
  e.preventDefault();
  // Submit data
  setForm({ name: "", email: "" }); // Reset state
};
```

## Key Points:
- Reset state to initial values.
- For controlled components.
- `form.reset()` for uncontrolled.
- Clear errors too.

## Interview Tip:
"Reset form by setting state back to initial values."

---

## Question 100: How do you upload files in a React form?

## Answer:
```jsx
const [file, setFile] = useState(null);

const handleFileChange = (e) => {
  setFile(e.target.files[0]);
};

const handleSubmit = (e) => {
  e.preventDefault();
  const formData = new FormData();
  formData.append("file", file);
  // Send formData to server
};

<input type="file" onChange={handleFileChange} />
```

## Key Points:
- Use uncontrolled input for files.
- `e.target.files[0]` for selected file.
- `FormData` for upload.
- Send via `fetch` or Axios.

## Interview Tip:
"File inputs are uncontrolled â€” use `e.target.files` and `FormData`."

---

## Part 5 (101â€“110): useState

---

## Question 101: What is the `useState` Hook?

## Answer:
`useState` adds state to functional components.

```jsx
const [count, setCount] = useState(0);
```

Returns current state and a setter function.

## Key Points:
- State in functional components.
- Returns `[state, setState]`.
- Initial value as argument.
- Triggers re-render on update.
- Most used hook.

## Interview Tip:
"`useState` is the most fundamental hook â€” it adds state to functional components."

---

## Question 102: Why do we use `useState`?

## Answer:
- **State management**: Store mutable data.
- **Re-rendering**: Trigger re-renders on change.
- **Local state**: Component-specific data.
- **Interactive UI**: Handle user input.

## Key Points:
- Store mutable data.
- Trigger re-renders.
- Local component state.
- Handle user interactions.

## Interview Tip:
"`useState` makes components interactive â€” it's how you manage data that changes."

---

## Question 103: How does `useState` work internally?

## Answer:
React stores state in a linked list associated with the component's fiber node. Each `useState` call corresponds to a slot in this list. On re-render, React reads the state in the same order.

## Key Points:
- Linked list on fiber node.
- Order matters.
- Same order on every render.
- Hooks rules ensure consistency.

## Interview Tip:
"React stores hooks in order â€” that's why you can't call them conditionally."

---

## Question 104: What happens when `setState` is called?

## Answer:
1. State is updated.
2. Component is scheduled for re-render.
3. React re-renders the component.
4. New state value is used.

## Key Points:
- State updated.
- Re-render scheduled.
- Component re-renders.
- New value used.

## Interview Tip:
"setState triggers a re-render â€” that's how the UI updates."

---

## Question 105: Is `setState` synchronous or asynchronous?

## Answer:
`setState` is asynchronous â€” React batches state updates for performance. The state isn't updated immediately.

```jsx
setCount(count + 1);
console.log(count); // Still old value!
```

## Key Points:
- Asynchronous.
- Batched for performance.
- State not updated immediately.
- Use callback for latest state.

## Interview Tip:
"setState is asynchronous â€” don't read state immediately after setting it."

---

## Question 106: What is functional state update?

## Answer:
Functional update uses the previous state to compute the new state.

```jsx
setCount(prev => prev + 1);
```

## Key Points:
- Uses previous state.
- Ensures correct value.
- Avoids stale closures.
- Use when new state depends on old.

## Interview Tip:
"Use functional update when new state depends on previous state."

---

## Question 107: When should you use the functional updater form of `setState`?

## Answer:
When the new state depends on the previous state:

```jsx
setCount(prev => prev + 1); // Correct
setCount(count + 1);         // May be stale
```

## Key Points:
- New state depends on previous.
- Avoids stale closures.
- Ensures correct updates.
- Use for counters, toggles.

## Interview Tip:
"Use functional updater when new state depends on old state."

---

## Question 108: Can you store objects in state?

## Answer:
Yes, but you must create a new object (not mutate).

```jsx
const [user, setUser] = useState({ name: "", age: 0 });

// Correct
setUser({ ...user, name: "Alice" });

// Wrong (mutation)
user.name = "Alice";
setUser(user);
```

## Key Points:
- Objects are valid state.
- Create new objects (spread).
- Never mutate state directly.
- React compares by reference.

## Interview Tip:
"Always create new objects â€” React compares by reference, not value."

---

## Question 109: Can you store arrays in state?

## Answer:
Yes, but create a new array (not mutate).

```jsx
const [items, setItems] = useState([]);

// Add
setItems([...items, newItem]);

// Remove
setItems(items.filter(item => item.id !== id));
```

## Key Points:
- Arrays are valid state.
- Create new arrays.
- Spread for adding.
- Filter for removing.
- Never mutate directly.

## Interview Tip:
"Use spread and filter â€” never mutate arrays in state."

---

## Question 110: Why shouldn't you mutate state directly?

## Answer:
- **No re-render**: React doesn't detect mutations.
- **Stale UI**: UI doesn't update.
- **Bugs**: Hard-to-find issues.
- **Reference equality**: React compares by reference.

```jsx
// Wrong
user.name = "Alice";
setUser(user); // React doesn't detect change

// Correct
setUser({ ...user, name: "Alice" }); // New reference
```

## Key Points:
- Mutations don't trigger re-renders.
- React compares by reference.
- Always create new objects/arrays.
- Use spread operator.

## Interview Tip:
"Mutations are invisible to React â€” always create new references."

---

## Part 6 (111â€“120): useEffect

---

## Question 111: What is the `useEffect` Hook?

## Answer:
`useEffect` handles side effects in functional components â€” data fetching, subscriptions, DOM manipulation.

```jsx
useEffect(() => {
  // Side effect
  fetchData();
}, [dependency]);
```

## Key Points:
- Handles side effects.
- Runs after render.
- Dependency array controls when.
- Cleanup function for unmount.
- Replaces lifecycle methods.

## Interview Tip:
"`useEffect` is for side effects â€” data fetching, subscriptions, DOM manipulation."

---

## Question 112: Why do we use `useEffect`?

## Answer:
- **Data fetching**: Fetch data after mount.
- **Subscriptions**: Subscribe to events.
- **DOM manipulation**: Interact with DOM.
- **Timers**: Set up intervals/timeouts.
- **Cleanup**: Clean up on unmount.

## Key Points:
- Data fetching.
- Subscriptions.
- DOM manipulation.
- Timers.
- Cleanup.

## Interview Tip:
"`useEffect` handles anything that happens outside the render cycle."

---

## Question 113: What are the different dependency array options in `useEffect`?

## Answer:
```jsx
// Runs on every render
useEffect(() => {});

// Runs only on mount
useEffect(() => {}, []);

// Runs when dependencies change
useEffect(() => {}, [dep1, dep2]);
```

## Key Points:
- No array: every render.
- Empty array: mount only.
- With dependencies: when deps change.
- Controls when effect runs.

## Interview Tip:
"Empty array = mount only; dependencies = when they change; no array = every render."

---

## Question 114: What happens if the dependency array is omitted?

## Answer:
The effect runs after every render.

```jsx
useEffect(() => {
  console.log("Runs on every render");
});
```

## Key Points:
- Runs after every render.
- Can cause performance issues.
- Usually unintended.
- Add dependency array.

## Interview Tip:
"No dependency array = every render â€” usually a mistake."

---

## Question 115: What happens if the dependency array is empty (`[]`)?

## Answer:
The effect runs only once after the initial render (mount).

```jsx
useEffect(() => {
  console.log("Runs once on mount");
}, []);
```

## Key Points:
- Runs once on mount.
- Equivalent to `componentDidMount`.
- Common for data fetching.
- No re-runs.

## Interview Tip:
"Empty array = mount only â€” use it for initial data fetching."

---

## Question 116: What happens if dependencies change?

## Answer:
The effect runs again when any dependency changes.

```jsx
useEffect(() => {
  fetchUser(userId);
}, [userId]); // Runs when userId changes
```

## Key Points:
- Effect re-runs on dependency change.
- Previous cleanup runs first.
- Common for dependent data fetching.
- Track all dependencies.

## Interview Tip:
"Effect re-runs when dependencies change â€” track all dependencies."

---

## Question 117: What is the cleanup function in `useEffect`?

## Answer:
The cleanup function runs before the effect re-runs and on unmount.

```jsx
useEffect(() => {
  const subscription = subscribe();
  return () => {
    subscription.unsubscribe(); // Cleanup
  };
}, []);
```

## Key Points:
- Runs before re-run and on unmount.
- Clean up subscriptions.
- Clear timers.
- Prevent memory leaks.

## Interview Tip:
"Cleanup prevents memory leaks â€” always clean up subscriptions and timers."

---

## Question 118: When does the cleanup function run?

## Answer:
1. Before the effect re-runs (when dependencies change).
2. When the component unmounts.

## Key Points:
- Before re-run.
- On unmount.
- Cleans up previous effect.
- Prevents side effect accumulation.

## Interview Tip:
"Cleanup runs before re-run and on unmount â€” it prevents side effect accumulation."

---

## Question 119: Why is cleanup important?

## Answer:
- **Memory leaks**: Prevent memory leaks from subscriptions.
- **Stale data**: Avoid updating unmounted components.
- **Resource management**: Clear timers and intervals.
- **Consistency**: Ensure clean state between effect runs.

## Key Points:
- Prevent memory leaks.
- Avoid stale updates.
- Clear resources.
- Maintain consistency.

## Interview Tip:
"Cleanup prevents memory leaks and stale updates â€” always clean up."

---

## Question 120: What are common mistakes when using `useEffect`?

## Answer:
1. **Missing dependencies**: Stale closures.
2. **No cleanup**: Memory leaks.
3. **Infinite loops**: Setting state without conditions.
4. **Wrong dependency type**: Object/array causing re-runs.
5. **Using `useEffect` for derived state**: Use `useMemo` instead.

## Key Points:
- Missing dependencies.
- No cleanup.
- Infinite loops.
- Wrong dependencies.
- Derived state.

## Interview Tip:
"The most common mistake is missing dependencies â€” use the exhaustive-deps ESLint rule."

---

## Part 7 (121â€“130): Dependency Arrays & Effects

---

## Question 121: What causes an infinite loop in `useEffect`?

## Answer:
Setting state inside `useEffect` without proper dependencies:

```jsx
// Bad: infinite loop
useEffect(() => {
  setCount(count + 1); // Sets state â†’ re-render â†’ effect runs again
});
```

## Key Points:
- Setting state triggers re-render.
- Re-render triggers effect.
- Effect sets state again.
- Add proper dependencies.

## Interview Tip:
"Setting state in useEffect without dependencies causes infinite loops."

---

## Question 122: How do you prevent infinite loops?

## Answer:
1. **Add dependencies**: Only run when specific values change.
2. **Use conditions**: Check before setting state.
3. **Empty array**: Run only on mount.

```jsx
useEffect(() => {
  if (data) setProcessed(processData(data));
}, [data]); // Only when data changes
```

## Key Points:
- Add proper dependencies.
- Use conditions.
- Empty array for mount-only effects.
- Don't set state unconditionally.

## Interview Tip:
"Add dependencies and use conditions â€” that prevents infinite loops."

---

## Question 123: Why should all dependencies be included in the dependency array?

## Answer:
Including all dependencies ensures the effect has access to the latest values. Missing dependencies cause stale closures.

```jsx
// Bad: missing dependency
useEffect(() => {
  fetchUser(userId);
}, []); // userId is stale!

// Good: all dependencies
useEffect(() => {
  fetchUser(userId);
}, [userId]);
```

## Key Points:
- Access latest values.
- Prevent stale closures.
- ESLint rule enforces this.
- Include all used values.

## Interview Tip:
"Include all dependencies â€” missing ones cause stale closures."

---

## Question 124: What is the `eslint-plugin-react-hooks` rule?

## Answer:
The `exhaustive-deps` rule warns when dependencies are missing from `useEffect` and other hooks.

```json
{
  "rules": {
    "react-hooks/exhaustive-deps": "warn"
  }
}
```

## Key Points:
- Warns about missing dependencies.
- Prevents stale closures.
- Part of React hooks plugin.
- Follow the warnings.

## Interview Tip:
"Follow the exhaustive-deps rule â€” it prevents stale closure bugs."

---

## Question 125: Can you ignore dependency warnings? When, if ever?

## Answer:
Rarely. Ignoring warnings causes stale closures. Legitimate cases:
- **Mount-only effect**: Use empty array `[]`.
- **Intentional**: When you specifically want old behavior.
- **Stable references**: Functions that don't change.

## Key Points:
- Usually don't ignore.
- Mount-only: empty array.
- Intentional: document why.
- Use `useCallback` for stable references.

## Interview Tip:
"Almost never ignore warnings â€” fix the root cause instead."

---

## Question 126: What is a stale closure in React?

## Answer:
A stale closure captures an old value of a variable instead of the current one.

```jsx
function Counter() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    const timer = setInterval(() => {
      console.log(count); // Always 0!
    }, 1000);
    return () => clearInterval(timer);
  }, []); // Captures initial count
}
```

## Key Points:
- Captures old values.
- Effect has stale reference.
- Common with intervals and callbacks.
- Fix with dependencies or refs.

## Interview Tip:
"Stale closures capture old values â€” add dependencies or use refs."

---

## Question 127: How do stale closures happen?

## Answer:
When an effect or callback captures a variable from a previous render instead of the current one. This happens when:
- Missing dependencies in `useEffect`.
- Callbacks in event handlers capture old state.
- Intervals/timeouts capture old values.

## Key Points:
- Missing dependencies.
- Old state captured.
- Common in callbacks and timers.
- Fix with dependencies or refs.

## Interview Tip:
"Stale closures happen when effects capture old values â€” add dependencies."

---

## Question 128: How do you fix stale closure issues?

## Answer:
1. **Add dependencies**: Effect re-runs with new values.
2. **Use ref**: Refs always have current value.
3. **Functional update**: `setState(prev => prev + 1)`.

```jsx
// Fix with ref
const countRef = useRef(count);
countRef.current = count;

useEffect(() => {
  const timer = setInterval(() => {
    console.log(countRef.current); // Current value
  }, 1000);
}, []);
```

## Key Points:
- Add dependencies.
- Use refs for current values.
- Functional updates for state.
- Choose based on use case.

## Interview Tip:
"Refs always have the current value â€” use them to fix stale closures."

---

## Question 129: Can you make API calls inside `useEffect`?

## Answer:
Yes, but use an async function inside:

```jsx
useEffect(() => {
  async function fetchData() {
    const res = await fetch("/api/data");
    const data = await res.json();
    setData(data);
  }
  fetchData();
}, []);
```

## Key Points:
- Async function inside effect.
- Can't make effect itself async.
- Call async function inside.
- Handle errors.
- Add cleanup for cancellation.

## Interview Tip:
"Wrap async calls in a function inside useEffect â€” don't make the effect itself async."

---

## Question 130: How do you cancel an API request in `useEffect`?

## Answer:
Use `AbortController`:

```jsx
useEffect(() => {
  const controller = new AbortController();

  async function fetchData() {
    try {
      const res = await fetch("/api/data", { signal: controller.signal });
      const data = await res.json();
      setData(data);
    } catch (err) {
      if (err.name !== "AbortError") throw err;
    }
  }
  fetchData();

  return () => controller.abort();
}, []);
```

## Key Points:
- `AbortController` for cancellation.
- Cleanup function aborts request.
- Handle `AbortError`.
- Prevents state updates on unmounted components.

## Interview Tip:
"AbortController prevents stale data and memory leaks from cancelled requests."

---

## Part 8 (131â€“140): useRef

---

## Question 131: What is the `useRef` Hook?

## Answer:
`useRef` creates a mutable ref object that persists across renders without triggering re-renders.

```jsx
const inputRef = useRef(null);
<input ref={inputRef} />
```

## Key Points:
- Mutable ref object.
- Persists across renders.
- No re-render on change.
- `.current` property.
- DOM access and value storage.

## Interview Tip:
"`useRef` is a mutable container that doesn't trigger re-renders."

---

## Question 132: What is the difference between `useRef` and `useState`?

## Answer:
| Feature | useRef | useState |
|---------|--------|----------|
| Re-render | No | Yes |
| Mutability | Mutable | Immutable (new value) |
| Use case | DOM access, values | UI state |

## Key Points:
- `useRef`: no re-render, mutable.
- `useState`: triggers re-render, immutable update.
- `useRef` for values that don't affect UI.
- `useState` for values that do.

## Interview Tip:
"`useRef` for values that don't affect rendering; `useState` for values that do."

---

## Question 133: When should you use `useRef`?

## Answer:
- **DOM access**: Focus, measurements, animations.
- **Timer IDs**: Store interval/timeout IDs.
- **Previous values**: Track previous state.
- **Mutable values**: Values that don't affect rendering.

## Key Points:
- DOM access.
- Timer storage.
- Previous values.
- Non-rendering values.

## Interview Tip:
"Use `useRef` for DOM access and values that don't affect the UI."

---

## Question 134: How do you focus an input using `useRef`?

## Answer:
```jsx
const inputRef = useRef(null);

useEffect(() => {
  inputRef.current.focus();
}, []);

<input ref={inputRef} />
```

## Key Points:
- Create ref with `useRef`.
- Attach to element with `ref` prop.
- Access with `ref.current`.
- Call DOM methods directly.

## Interview Tip:
"`useRef` + `ref.current.focus()` â€” the standard pattern for focus management."

---

## Question 135: Can updating a ref trigger a re-render?

## Answer:
No. Updating a ref does not trigger a re-render.

```jsx
const countRef = useRef(0);
countRef.current = 1; // No re-render
```

## Key Points:
- No re-render on ref update.
- Mutable without re-render.
- Use for values that don't affect UI.
- Use `useState` for UI-affecting values.

## Interview Tip:
"Ref updates don't trigger re-renders â€” that's by design."

---

## Question 136: What is `forwardRef`?

## Answer:
`forwardRef` passes a ref through a component to a child component.

```jsx
const Input = forwardRef((props, ref) => {
  return <input ref={ref} {...props} />;
});

const ref = useRef();
<Input ref={ref} />;
```

## Key Points:
- Passes ref to child component.
- Forwards ref to DOM element.
- Needed for component libraries.
- Use `useRef` in parent.

## Interview Tip:
"`forwardRef` lets parents access child DOM elements â€” use it for component libraries."

---

## Question 137: When should you use `forwardRef`?

## Answer:
- **Component libraries**: Expose DOM access to consumers.
- **Focus management**: Parent needs to focus child input.
- **Animations**: Parent needs child DOM for animations.
- **Third-party integration**: Pass refs to third-party components.

## Key Points:
- Component libraries.
- Focus management.
- Animations.
- Third-party integration.

## Interview Tip:
"Use `forwardRef` when the parent needs to access the child's DOM element."

---

## Question 138: What is `useImperativeHandle`?

## Answer:
`useImperativeHandle` customizes the ref value exposed to parent components.

```jsx
const Input = forwardRef((props, ref) => {
  const inputRef = useRef();

  useImperativeHandle(ref, () => ({
    focus: () => inputRef.current.focus(),
    clear: () => { inputRef.current.value = ""; }
  }));

  return <input ref={inputRef} />;
});
```

## Key Points:
- Customizes exposed ref.
- Limit parent's access.
- Combine with `forwardRef`.
- Expose only needed methods.

## Interview Tip:
"`useImperativeHandle` limits what the parent can do â€” expose only what's needed."

---

## Question 139: When should you use `useImperativeHandle`?

## Answer:
When you want to expose specific methods to the parent without exposing the entire DOM element.

## Key Points:
- Limit exposed API.
- Specific methods only.
- Component library pattern.
- Combine with `forwardRef`.

## Interview Tip:
"Use it to create a clean, limited API for parent components."

---

## Question 140: What are common use cases for refs?

## Answer:
- **Focus management**: Focus inputs programmatically.
- **DOM measurements**: Get element dimensions.
- **Animations**: Integrate with GSAP, Framer Motion.
- **Timer IDs**: Store interval/timeout IDs.
- **Previous values**: Track previous props/state.
- **Third-party integration**: Non-React library integration.

## Key Points:
- Focus, measurements, animations.
- Timer storage.
- Previous values.
- Third-party integration.

## Interview Tip:
"Refs are for imperative actions â€” focus, measurements, and third-party integration."

---

## Part 9 (141â€“150): Memoization Hooks

---

## Question 141: What is the `useMemo` Hook?

## Answer:
`useMemo` memoizes a computed value, recalculating only when dependencies change.

```jsx
const expensiveResult = useMemo(() => {
  return computeExpensiveValue(data);
}, [data]);
```

## Key Points:
- Memoizes computed values.
- Recalculates only when dependencies change.
- Performance optimization.
- Avoids unnecessary recalculations.

## Interview Tip:
"`useMemo` caches computed values â€” use it for expensive calculations."

---

## Question 142: When should you use `useMemo`?

## Answer:
- **Expensive calculations**: Complex computations.
- **Derived data**: Filtering, sorting, transforming.
- **Referential equality**: Stable object/array references.
- **Preventing child re-renders**: Stable props.

## Key Points:
- Expensive calculations.
- Derived data.
- Referential equality.
- Prevent unnecessary re-renders.

## Interview Tip:
"Use `useMemo` for expensive calculations or when you need stable references."

---

## Question 143: What is the `useCallback` Hook?

## Answer:
`useCallback` memoizes a function, returning the same reference between renders.

```jsx
const handleClick = useCallback(() => {
  doSomething(id);
}, [id]);
```

## Key Points:
- Memoizes functions.
- Same reference between renders.
- Prevents child re-renders.
- Dependencies control when it changes.

## Interview Tip:
"`useCallback` stabilizes function references â€” use it when passing callbacks to memoized children."

---

## Question 144: What is the difference between `useMemo` and `useCallback`?

## Answer:
- **`useMemo`**: Memoizes a value (result of a function).
- **`useCallback`**: Memoizes a function itself.

```jsx
const value = useMemo(() => compute(a, b), [a, b]); // Value
const fn = useCallback(() => doSomething(a), [a]);   // Function
```

## Key Points:
- `useMemo`: memoizes value.
- `useCallback`: memoizes function.
- `useCallback(fn, deps)` = `useMemo(() => fn, deps)`.
- Both optimize re-renders.

## Interview Tip:
"`useMemo` for values, `useCallback` for functions â€” they're closely related."

---

## Question 145: When is memoization unnecessary?

## Answer:
- **Cheap calculations**: Simple computations.
- **Primitive values**: Numbers, strings (already stable).
- **Always changing**: Dependencies change every render.
- **Local use**: Value not passed to children.

## Key Points:
- Cheap calculations.
- Primitive values.
- Always-changing dependencies.
- Local-only values.

## Interview Tip:
"Don't memoize everything â€” only expensive calculations or values passed to children."

---

## Question 146: What is `React.memo`?

## Answer:
`React.memo` is a HOC that prevents re-renders if props haven't changed.

```jsx
const MemoizedComponent = React.memo(function MyComponent({ data }) {
  return <div>{data.name}</div>;
});
```

## Key Points:
- Prevents unnecessary re-renders.
- Shallow comparison of props.
- Use for pure components.
- Wrap component with `React.memo`.

## Interview Tip:
"`React.memo` prevents re-renders when props are the same."

---

## Question 147: What is the difference between `React.memo` and `useMemo`?

## Answer:
- **`React.memo`**: Memoizes a component (prevents re-render).
- **`useMemo`**: Memoizes a value (prevents recalculation).

## Key Points:
- `React.memo`: component level.
- `useMemo`: value level.
- Different purposes.
- Both optimize performance.

## Interview Tip:
"`React.memo` for components; `useMemo` for values."

---

## Question 148: How do `React.memo` and `useCallback` work together?

## Answer:
`React.memo` prevents re-renders, but only if props are the same. `useCallback` stabilizes function references so `React.memo` works correctly.

```jsx
const MemoizedChild = React.memo(Child);

function Parent() {
  const handleClick = useCallback(() => {}, []);
  return <MemoizedChild onClick={handleClick} />;
}
```

## Key Points:
- `React.memo` needs stable props.
- `useCallback` stabilizes functions.
- Together they prevent unnecessary re-renders.
- Use when child is expensive to render.

## Interview Tip:
"`React.memo` + `useCallback` = prevent unnecessary child re-renders."

---

## Question 149: What are the performance costs of memoization?

## Answer:
- **Memory**: Memoized values consume memory.
- **Comparison**: Shallow comparison has a cost.
- **Complexity**: Code becomes harder to read.
- **Over-optimization**: Unnecessary memoization wastes resources.

## Key Points:
- Memory overhead.
- Comparison cost.
- Code complexity.
- Don't over-optimize.

## Interview Tip:
"Memoization has costs â€” only use it when the benefit outweighs the cost."

---

## Question 150: How do you decide whether to optimize with memoization?

## Answer:
1. **Profile first**: Use React DevTools Profiler.
2. **Measure**: Is the component actually slow?
3. **Expensive**: Is the calculation expensive?
4. **Frequent re-renders**: Does it re-render often?
5. **Child components**: Are children expensive?

## Key Points:
- Profile before optimizing.
- Measure actual performance.
- Only optimize what's slow.
- Don't over-optimize.

## Interview Tip:
"Don't optimize prematurely â€” profile first, then optimize."

---

## Part 10 (151â€“160): Context API

---

## Question 151: What is the Context API?

## Answer:
The Context API provides a way to share data across the component tree without prop drilling.

```jsx
const ThemeContext = createContext("light");

function App() {
  return (
    <ThemeContext.Provider value="dark">
      <Child />
    </ThemeContext.Provider>
  );
}

function Child() {
  const theme = useContext(ThemeContext);
}
```

## Key Points:
- Share data without prop drilling.
- `createContext` to create.
- `Provider` to supply value.
- `useContext` to consume.
- Built into React.

## Interview Tip:
"Context API solves prop drilling â€” share data across the component tree."

---

## Question 152: Why was Context API introduced?

## Answer:
To solve prop drilling â€” passing data through many intermediate components that don't need it.

## Key Points:
- Solve prop drilling.
- Share global data.
- Avoid unnecessary props.
- Built-in solution.

## Interview Tip:
"Context was introduced to solve prop drilling â€” it's the built-in solution."

---

## Question 153: What problems does Context API solve?

## Answer:
- **Prop drilling**: Passing props through many levels.
- **Global state**: Sharing data across the app.
- **Theme/locale**: Application-wide settings.

## Key Points:
- Prop drilling.
- Global data sharing.
- Theme, locale, auth state.
- Avoids unnecessary props.

## Interview Tip:
"Context solves prop drilling for global data like themes and auth."

---

## Question 154: When should you use Context API?

## Answer:
- **Theme**: Light/dark mode.
- **Locale**: Language settings.
- **Auth**: Current user.
- **Global settings**: Application-wide config.

## Key Points:
- Theme and locale.
- Authentication state.
- Global settings.
- Infrequently changing data.

## Interview Tip:
"Use Context for truly global, infrequently changing data."

---

## Question 155: When should you avoid Context API?

## Answer:
- **Frequently changing data**: Causes too many re-renders.
- **Complex state**: Use Redux or Zustand.
- **Performance-critical**: Context triggers re-renders in all consumers.

## Key Points:
- Frequently changing data.
- Complex state logic.
- Performance-critical paths.
- Use state management instead.

## Interview Tip:
"Avoid Context for frequently changing data â€” it re-renders all consumers."

---

## Question 156: How do you create a Context?

## Answer:
```jsx
const MyContext = createContext(defaultValue);
```

## Key Points:
- `createContext(defaultValue)`.
- Default value for when no Provider.
- Returns Provider and Consumer.
- Usually exported for use.

## Interview Tip:
"`createContext` creates the context â€” export it for use across components."

---

## Question 157: What is a Provider?

## Answer:
The Provider supplies the context value to all consumers below it.

```jsx
<MyContext.Provider value={someValue}>
  <ChildComponent />
</MyContext.Provider>
```

## Key Points:
- Supplies context value.
- Wraps consumer components.
- Value changes trigger re-renders.
- Can be nested.

## Interview Tip:
"Provider supplies the value â€” consumers below it can access it."

---

## Question 158: What is a Consumer?

## Answer:
A Consumer reads the context value (older pattern, `useContext` is preferred).

```jsx
<MyContext.Consumer>
  {value => <div>{value}</div>}
</MyContext.Consumer>
```

## Key Points:
- Reads context value.
- Older pattern.
- `useContext` is preferred.
- Render props pattern.

## Interview Tip:
"Use `useContext` instead of Consumer â€” it's cleaner."

---

## Question 159: What is the `useContext` Hook?

## Answer:
`useContext` reads the context value in functional components.

```jsx
const theme = useContext(ThemeContext);
```

## Key Points:
- Reads context value.
- Re-renders when context changes.
- Cleaner than Consumer.
- Most common way to consume context.

## Interview Tip:
"`useContext` is the modern way to consume context â€” cleaner than Consumer."

---

## Question 160: How does Context trigger re-renders?

## Answer:
When the Provider's value changes, ALL consumers re-render â€” even if they only use part of the value.

```jsx
<Context.Provider value={{ theme, user }}>
  {/* Both re-render if either changes */}
  <ThemeConsumer />
  <UserConsumer />
</Context.Provider>
```

## Key Points:
- All consumers re-render on value change.
- No partial consumption.
- Split contexts for different data.
- Use `useMemo` for value.

## Interview Tip:
"Context re-renders all consumers â€” split contexts for different data."

---

## Part 11 (161â€“170): useReducer

---

## Question 161: What is the `useReducer` Hook?

## Answer:
`useReducer` manages complex state with a reducer function.

```jsx
const [state, dispatch] = useReducer(reducer, initialState);

function reducer(state, action) {
  switch (action.type) {
    case "increment": return { count: state.count + 1 };
    case "decrement": return { count: state.count - 1 };
  }
}
```

## Key Points:
- Complex state management.
- Reducer function for state transitions.
- Dispatch actions to update state.
- Similar to Redux pattern.
- Alternative to `useState`.

## Interview Tip:
"`useReducer` is for complex state â€” it uses the Redux pattern."

---

## Question 162: When should you use `useReducer` instead of `useState`?

## Answer:
- **Complex state**: Multiple related values.
- **Complex transitions**: State depends on previous state.
- **Many actions**: Multiple ways to update state.
- **Predictability**: Clear state transitions.

## Key Points:
- Complex state objects.
- Multiple related updates.
- Clear state transitions.
- When `useState` becomes messy.

## Interview Tip:
"Use `useReducer` when state logic gets complex â€” it's cleaner than multiple `useState` calls."

---

## Question 163: What is a reducer function?

## Answer:
A reducer takes current state and an action, returns new state.

```jsx
function reducer(state, action) {
  switch (action.type) {
    case "increment":
      return { count: state.count + 1 };
    default:
      return state;
  }
}
```

## Key Points:
- Pure function.
- Takes `(state, action)`.
- Returns new state.
- Never mutates state.
- Predictable state transitions.

## Interview Tip:
"Reducers are pure functions â€” same input always produces same output."

---

## Question 164: What are actions in `useReducer`?

## Answer:
Actions are objects describing what happened.

```jsx
dispatch({ type: "increment" });
dispatch({ type: "add", payload: 5 });
```

## Key Points:
- Objects describing state changes.
- `type` property required.
- `payload` for data.
- Dispatched to reducer.

## Interview Tip:
"Actions describe what happened â€” the reducer decides how state changes."

---

## Question 165: How does dispatch work?

## Answer:
`dispatch` sends an action to the reducer, which calculates the new state.

```jsx
dispatch({ type: "increment" });
```

## Key Points:
- Sends action to reducer.
- Triggers re-render.
- Same reference across renders.
- Never changes.

## Interview Tip:
"`dispatch` sends actions â€” the reducer handles the rest."

---

## Question 166: What are the advantages of `useReducer`?

## Answer:
- **Predictable**: Clear state transitions.
- **Testable**: Reducers are pure functions.
- **Organized**: All state logic in one place.
- **Debuggable**: Actions log state changes.

## Key Points:
- Predictable state changes.
- Easy to test.
- Organized state logic.
- Debuggable with action logging.

## Interview Tip:
"`useReducer` makes state logic predictable and testable."

---

## Question 167: Can `useReducer` replace Redux?

## Answer:
For simple apps, yes. `useReducer` + Context can replace Redux for basic state management. But Redux offers:
- **DevTools**: Time-travel debugging.
- **Middleware**: Thunks, sagas.
- **Ecosystem**: Many plugins.

## Key Points:
- Can replace Redux for simple apps.
- Redux has DevTools, middleware.
- Use Redux for complex apps.
- `useReducer` + Context for simple apps.

## Interview Tip:
"`useReducer` + Context can replace Redux for simple apps â€” Redux is better for complex ones."

---

## Question 168: What are common use cases for `useReducer`?

## Answer:
- **Form state**: Complex forms with multiple fields.
- **State machines**: Multi-step workflows.
- **Shopping cart**: Add, remove, update items.
- **Todo list**: CRUD operations.

## Key Points:
- Complex forms.
- State machines.
- Shopping cart.
- CRUD operations.

## Interview Tip:
"`useReducer` is great for complex forms and CRUD operations."

---

## Question 169: Can `useReducer` be combined with Context API?

## Answer:
Yes, this is a common pattern for global state management.

```jsx
const [state, dispatch] = useReducer(reducer, initialState);

return (
  <AppContext.Provider value={{ state, dispatch }}>
    {children}
  </AppContext.Provider>
);
```

## Key Points:
- Combine for global state.
- Context provides state and dispatch.
- Components consume via `useContext`.
- Simple Redux alternative.

## Interview Tip:
"`useReducer` + Context = simple global state management."

---

## Question 170: What are the limitations of `useReducer`?

## Answer:
- **No middleware**: No built-in side effect handling.
- **No DevTools**: No time-travel debugging.
- **Re-renders**: All consumers re-render on state change.
- **Single reducer**: One reducer per context.

## Key Points:
- No middleware.
- No DevTools.
- Re-renders all consumers.
- Single reducer.

## Interview Tip:
"For complex apps, Redux's DevTools and middleware are worth the extra setup."

---

## Part 12 (171â€“180): Custom Hooks

---

## Question 171: What is a custom Hook?

## Answer:
A custom Hook is a function that starts with `use` and can call other hooks. It lets you extract and reuse stateful logic.

```jsx
function useFetch(url) {
  const [data, setData] = useState(null);
  const [loading, setLoading] = useState(true);

  useEffect(() => {
    fetch(url)
      .then(res => res.json())
      .then(data => { setData(data); setLoading(false); });
  }, [url]);

  return { data, loading };
}
```

## Key Points:
- Function starting with `use`.
- Can call other hooks.
- Reuses stateful logic.
- Custom logic extraction.
- Reusable across components.

## Interview Tip:
"Custom hooks extract and reuse stateful logic â€” they're the modern alternative to HOCs."

---

## Question 172: Why do we create custom Hooks?

## Answer:
- **Reuse logic**: Share stateful logic between components.
- **Cleaner components**: Extract complex logic.
- **Testability**: Test logic independently.
- **Organization**: Group related logic.

## Key Points:
- Logic reuse.
- Cleaner components.
- Independent testing.
- Better organization.

## Interview Tip:
"Custom hooks make components cleaner and logic reusable."

---

## Question 173: What naming convention should custom Hooks follow?

## Answer:
Always start with `use` â€” this tells React it's a hook and follows the rules of hooks.

```jsx
function useAuth() { ... }
function useFetch() { ... }
function useLocalStorage() { ... }
```

## Key Points:
- Start with `use`.
- Tells React it's a hook.
- Enables linting rules.
- Convention, not just style.

## Interview Tip:
"Always start custom hooks with `use` â€” it's required for React's rules."

---

## Question 174: Can one custom Hook use another custom Hook?

## Answer:
Yes, custom hooks can call other hooks.

```jsx
function useAuth() {
  const user = useCurrentUser();
  const permissions = usePermissions(user.id);
  return { user, permissions };
}
```

## Key Points:
- Hooks can call hooks.
- Compose complex logic.
- Build on simpler hooks.
- Clean composition.

## Interview Tip:
"Custom hooks compose â€” build complex hooks from simpler ones."

---

## Question 175: What are common real-world custom Hooks?

## Answer:
- `useFetch`: Data fetching with loading/error states.
- `useLocalStorage`: Persist state to localStorage.
- `useDebounce`: Debounce values.
- `useAuth`: Authentication state.
- `useMediaQuery`: Responsive design.
- `useOnClickOutside`: Click outside detection.

## Key Points:
- Data fetching.
- Storage persistence.
- Debouncing.
- Authentication.
- Responsive design.

## Interview Tip:
"`useFetch`, `useLocalStorage`, `useDebounce` â€” the most common custom hooks."

---

## Question 176: How do custom Hooks share logic?

## Answer:
Custom hooks encapsulate stateful logic and return values/components can use.

```jsx
// Shared logic
function useCounter(initial = 0) {
  const [count, setCount] = useState(initial);
  const increment = () => setCount(c => c + 1);
  return { count, increment };
}

// Used by multiple components
function ComponentA() {
  const { count, increment } = useCounter();
}
```

## Key Points:
- Encapsulate stateful logic.
- Return values for components.
- Each component gets its own state.
- Logic is shared, state is not.

## Interview Tip:
"Custom hooks share logic, not state â€” each component gets its own state."

---

## Question 177: Do custom Hooks share state?

## Answer:
No. Each component that uses a custom hook gets its own independent state.

```jsx
function ComponentA() {
  const { count } = useCounter(); // Own state
}

function ComponentB() {
  const { count } = useCounter(); // Different state
}
```

## Key Points:
- Each component gets own state.
- Logic is shared, state is not.
- Use Context for shared state.
- Custom hooks for shared logic.

## Interview Tip:
"Custom hooks share logic, not state â€” use Context for shared state."

---

## Question 178: What are the benefits of custom Hooks over HOCs?

## Answer:
- **No wrapper hell**: Flat structure.
- **No prop collisions**: Clear data flow.
- **Composable**: Hooks can call hooks.
- **Simpler**: Easier to understand.
- **TypeScript**: Better type inference.

## Key Points:
- No wrapper nesting.
- No prop collisions.
- Composable.
- Simpler code.
- Better TypeScript support.

## Interview Tip:
"Custom hooks avoid wrapper hell and prop collisions â€” they're cleaner than HOCs."

---

## Question 179: What are the benefits of custom Hooks over render props?

## Answer:
- **Cleaner syntax**: No nested render functions.
- **Multiple hooks**: Easy to use multiple hooks.
- **TypeScript**: Better type inference.
- **Readability**: Linear code flow.

## Key Points:
- No nested render functions.
- Easy to compose multiple hooks.
- Better TypeScript support.
- More readable.

## Interview Tip:
"Custom hooks are cleaner than render props â€” no nested functions."

---

## Question 180: What are common mistakes when writing custom Hooks?

## Answer:
1. **Not starting with `use`**: Breaks React's rules.
2. **Calling hooks conditionally**: Violates rules of hooks.
3. **Returning too much**: Keep return values minimal.
4. **Not handling cleanup**: Memory leaks.
5. **Over-abstracting**: Too many small hooks.

## Key Points:
- Start with `use`.
- Don't call conditionally.
- Minimal return values.
- Handle cleanup.
- Don't over-abstract.

## Interview Tip:
"Start with `use`, follow the rules, handle cleanup â€” the custom hook essentials."

---

## Part 13 (181â€“190): Advanced React Hooks

---

## Question 181: What is `useLayoutEffect`?

## Answer:
`useLayoutEffect` fires synchronously after DOM mutations but before the browser paints. Use it for DOM measurements.

```jsx
useLayoutEffect(() => {
  const rect = ref.current.getBoundingClientRect();
  setHeight(rect.height);
}, []);
```

## Key Points:
- Fires after DOM mutation, before paint.
- Synchronous.
- For DOM measurements.
- Blocks painting.
- Use `useEffect` unless you need measurements.

## Interview Tip:
"`useLayoutEffect` blocks painting â€” use it only when you need DOM measurements before paint."

---

## Question 182: What is the difference between `useEffect` and `useLayoutEffect`?

## Answer:
| Feature | useEffect | useLayoutEffect |
|---------|----------|-----------------|
| Timing | After paint | Before paint |
| Blocking | No | Yes |
| Use case | Side effects | DOM measurements |

## Key Points:
- `useEffect`: after paint, non-blocking.
- `useLayoutEffect`: before paint, blocking.
- Use `useEffect` by default.
- Use `useLayoutEffect` for measurements.

## Interview Tip:
"Default to `useEffect` â€” use `useLayoutEffect` only for DOM measurements."

---

## Question 183: When should you use `useLayoutEffect`?

## Answer:
- **DOM measurements**: Get element dimensions before paint.
- **DOM mutations**: Mutate DOM before user sees it.
- **Animations**: Set initial animation state.

## Key Points:
- DOM measurements.
- DOM mutations before paint.
- Animation setup.
- Rarely needed.

## Interview Tip:
"`useLayoutEffect` is for DOM measurements that must happen before paint."

---

## Question 184: What is `useTransition`?

## Answer:
`useTransition` marks state updates as non-urgent, keeping the UI responsive during heavy updates.

```jsx
const [isPending, startTransition] = useTransition();

function handleClick() {
  startTransition(() => {
    setHeavyState(newValue);
  });
}
```

## Key Points:
- Marks updates as non-urgent.
- Keeps UI responsive.
- `isPending` for loading state.
- React 18 feature.

## Interview Tip:
"`useTransition` keeps the UI responsive during heavy updates."

---

## Question 185: What problems does `useTransition` solve?

## Answer:
- **Janky UI**: Heavy updates block interactions.
- **Responsiveness**: User input stays responsive.
- **Prioritization**: Urgent updates before non-urgent.

## Key Points:
- Prevents janky UI.
- Keeps input responsive.
- Prioritizes urgent updates.
- React 18 concurrent feature.

## Interview Tip:
"`useTransition` prevents heavy updates from blocking user interactions."

---

## Question 186: What is `useDeferredValue`?

## Answer:
`useDeferredValue` defers updating a value, keeping the UI responsive.

```jsx
const deferredValue = useDeferredValue(value);
```

## Key Points:
- Defers value updates.
- Keeps UI responsive.
- React 18 feature.
- For search inputs, filtering.

## Interview Tip:
"`useDeferredValue` keeps search inputs responsive while filtering large lists."

---

## Question 187: When should you use `useDeferredValue`?

## Answer:
- **Search inputs**: Defer filtering while typing.
- **Large lists**: Defer rendering large lists.
- **Heavy computations**: Defer expensive calculations.

## Key Points:
- Search inputs.
- Large list rendering.
- Heavy computations.
- React 18 concurrent feature.

## Interview Tip:
"`useDeferredValue` for search inputs â€” keep typing responsive while filtering."

---

## Question 188: What is `useId`?

## Answer:
`useId` generates unique IDs that are consistent between server and client.

```jsx
const id = useId();
<input id={id} />
```

## Key Points:
- Generates unique IDs.
- Consistent server/client.
- For accessibility.
- React 18 feature.

## Interview Tip:
"`useId` for accessible IDs that work with SSR."

---

## Question 189: Why is `useId` useful?

## Answer:
- **Accessibility**: Associate labels with inputs.
- **SSR consistency**: Same ID on server and client.
- **Unique IDs**: No collisions.

## Key Points:
- Accessibility (labels, ARIA).
- SSR consistency.
- Unique IDs.
- No manual ID management.

## Interview Tip:
"`useId` solves the SSR ID mismatch problem â€” use it for accessibility."

---

## Question 190: What is `useSyncExternalStore`?

## Answer:
`useSyncExternalStore` subscribes to external stores with consistent snapshots.

```jsx
const value = useSyncExternalStore(subscribe, getSnapshot);
```

## Key Points:
- Subscribe to external stores.
- Consistent snapshots.
- For state management libraries.
- React 18 feature.

## Interview Tip:
"`useSyncExternalStore` is for state management library authors."

---

## Part 14 (191â€“200): Performance & Optimization

---

## Question 191: What causes unnecessary re-renders in React?

## Answer:
1. **Parent re-renders**: Children re-render too.
2. **New objects/arrays**: New references on every render.
3. **Anonymous functions**: New function references.
4. **Context changes**: All consumers re-render.
5. **State updates**: Setting state triggers re-render.

## Key Points:
- Parent re-renders.
- New references.
- Anonymous functions.
- Context changes.
- State updates.

## Interview Tip:
"New references (objects, arrays, functions) cause unnecessary re-renders."

---

## Question 192: How do you identify unnecessary re-renders?

## Answer:
1. **React DevTools Profiler**: Highlight re-renders.
2. **`why-did-you-render`**: Logs re-render reasons.
3. **Console.log**: In render function.
4. **React.StrictMode**: Highlights issues.

## Key Points:
- React DevTools Profiler.
- why-did-you-render library.
- Console.log in render.
- StrictMode for development.

## Interview Tip:
"React DevTools Profiler is the best tool â€” it shows exactly what re-renders and why."

---

## Question 193: How can you optimize React performance?

## Answer:
1. **`React.memo`**: Prevent unnecessary re-renders.
2. **`useMemo`**: Memoize expensive calculations.
3. **`useCallback`**: Stabilize function references.
4. **Code splitting**: `React.lazy()` for lazy loading.
5. **Virtualization**: For large lists.
6. **Avoid inline objects/functions**: Create stable references.

## Key Points:
- Memoization (memo, useMemo, useCallback).
- Code splitting.
- Virtualization.
- Stable references.

## Interview Tip:
"Profile first, then optimize â€” memo, useMemo, useCallback are the tools."

---

## Question 194: What is code splitting in React?

## Answer:
Code splitting loads JavaScript on demand instead of loading everything upfront.

```jsx
const HeavyComponent = React.lazy(() => import("./HeavyComponent"));
```

## Key Points:
- Load JavaScript on demand.
- `React.lazy()` for dynamic imports.
- Smaller initial bundle.
- Faster initial load.

## Interview Tip:
"Code splitting reduces initial bundle size â€” use `React.lazy()`."

---

## Question 195: What is lazy loading?

## Answer:
Lazy loading defers loading of non-critical resources until they're needed.

```jsx
const Dashboard = React.lazy(() => import("./Dashboard"));
```

## Key Points:
- Load on demand.
- Smaller initial bundle.
- Faster initial load.
- Use for routes and heavy components.

## Interview Tip:
"Lazy load routes and heavy components â€” it improves initial load time."

---

## Question 196: What is `React.lazy()`?

## Answer:
`React.lazy()` dynamically imports a component, enabling code splitting.

```jsx
const LazyComponent = React.lazy(() => import("./Component"));
```

## Key Points:
- Dynamic import.
- Code splitting.
- Load on demand.
- Use with `Suspense`.

## Interview Tip:
"`React.lazy()` + `Suspense` = lazy loading with loading states."

---

## Question 197: What is `Suspense`?

## Answer:
`Suspense` shows a fallback while lazy-loaded components are loading.

```jsx
<Suspense fallback={<Loading />}>
  <LazyComponent />
</Suspense>
```

## Key Points:
- Shows fallback during loading.
- Works with `React.lazy()`.
- Also works with data fetching.
- Multiple Suspense boundaries.

## Interview Tip:
"`Suspense` shows a loading state while components or data load."

---

## Question 198: What are Error Boundaries?

## Answer:
Error Boundaries catch JavaScript errors in child components and display fallback UI.

```jsx
class ErrorBoundary extends React.Component {
  state = { hasError: false };

  static getDerivedStateFromError() {
    return { hasError: true };
  }

  render() {
    if (this.state.hasError) return <ErrorFallback />;
    return this.props.children;
  }
}
```

## Key Points:
- Catch rendering errors.
- Display fallback UI.
- Class component only (for now).
- Wrap components that may error.
- Don't catch event handler errors.

## Interview Tip:
"Error Boundaries catch rendering errors â€” they're essential for production apps."

---

## Question 199: What tools do you use to profile React performance?

## Answer:
- **React DevTools Profiler**: Visualize re-renders.
- **Chrome DevTools Performance**: CPU profiling.
- **Lighthouse**: Performance audit.
- **why-did-you-render**: Re-render logging.

## Key Points:
- React DevTools Profiler.
- Chrome DevTools.
- Lighthouse.
- why-did-you-render.

## Interview Tip:
"React DevTools Profiler is the primary tool â€” it shows re-renders and their causes."

---

## Question 200: What performance optimization techniques have you used in production React applications?

## Answer:
1. **`React.memo`**: Prevent unnecessary re-renders.
2. **`useMemo`**: Memoize expensive calculations.
3. **`useCallback`**: Stabilize callbacks.
4. **Code splitting**: Lazy load routes.
5. **Virtualization**: For large lists (react-window).
6. **Image optimization**: Lazy load images.
7. **Bundle analysis**: Find large dependencies.

## Key Points:
- Memoization for re-renders.
- Code splitting for bundle size.
- Virtualization for large lists.
- Image optimization.
- Bundle analysis.

## Interview Tip:
"Profile, identify bottlenecks, apply targeted optimizations."

---

## Part 15 (201â€“210): React Internals

---

## Question 201: What is React Fiber?

## Answer:
React Fiber is the reconciliation engine (React 16+). It enables incremental rendering, priority-based updates, and concurrent features.

## Key Points:
- Reconciliation engine.
- Incremental rendering.
- Priority-based updates.
- Concurrent features.
- Replaces the old stack reconciler.

## Interview Tip:
"Fiber enables concurrent rendering â€” React can pause and resume work."

---

## Question 202: Why was React Fiber introduced?

## Answer:
- **Incremental rendering**: Split work into chunks.
- **Prioritization**: Important updates first.
- **Concurrency**: Pause and resume rendering.
- **Better UX**: Keep UI responsive.

## Key Points:
- Incremental rendering.
- Priority updates.
- Concurrency.
- Better UX.

## Interview Tip:
"Fiber was introduced to enable concurrent rendering and better prioritization."

---

## Question 203: How does the React Fiber architecture work?

## Answer:
Fiber represents each component as a fiber node (a JavaScript object). These nodes form a linked tree. React processes fiber nodes incrementally, pausing and resuming as needed.

## Key Points:
- Fiber nodes represent components.
- Linked tree structure.
- Incremental processing.
- Pause and resume.
- Work-in-progress tree.

## Interview Tip:
"Fiber nodes are the unit of work â€” React processes them incrementally."

---

## Question 204: What is reconciliation in React?

## Answer:
Reconciliation is React's algorithm for comparing Virtual DOM trees and determining what to update.

## Key Points:
- Diffing algorithm.
- Compares old and new Virtual DOM.
- Determines minimal updates.
- O(n) with heuristics.

## Interview Tip:
"Reconciliation is the diffing algorithm â€” it finds what changed."

---

## Question 205: How does React's diffing algorithm work?

## Answer:
1. **Different element types**: Destroy and recreate.
2. **Same type**: Update changed props.
3. **Lists**: Use keys to match elements.
4. **Heuristics**: O(n) instead of O(nÂ³).

## Key Points:
- Type comparison.
- Props diffing.
- Key-based list matching.
- O(n) complexity.

## Interview Tip:
"React's diffing uses heuristics for O(n) complexity â€” it assumes different types mean different trees."

---

## Question 206: Why does React use the Virtual DOM?

## Answer:
- **Performance**: Minimize expensive DOM operations.
- **Batching**: Batch multiple updates.
- **Cross-platform**: Same API for web, native.
- **Declarative**: Describe UI, React handles updates.

## Key Points:
- Minimize DOM operations.
- Batch updates.
- Cross-platform.
- Declarative approach.

## Interview Tip:
"The Virtual DOM minimizes expensive real DOM operations."

---

## Question 207: How does React decide which components to re-render?

## Answer:
1. **State change**: Component with changed state.
2. **Props change**: Parent re-renders with new props.
3. **Context change**: Consumers of changed context.
4. **Force update**: `forceUpdate()` (class components).

## Key Points:
- State, props, context changes.
- Parent re-renders propagate.
- `React.memo` can prevent.
- Shallow comparison by default.

## Interview Tip:
"State, props, or context changes trigger re-renders â€” `React.memo` can prevent them."

---

## Question 208: What is the commit phase in React?

## Answer:
The commit phase applies changes to the real DOM. It's synchronous and cannot be interrupted.

## Key Points:
- Applies changes to real DOM.
- Synchronous.
- Cannot be interrupted.
- Runs after render phase.

## Interview Tip:
"The commit phase is when React actually updates the DOM â€” it's synchronous."

---

## Question 209: What is the render phase in React?

## Answer:
The render phase creates the Virtual DOM and diffs it. It can be interrupted (in concurrent mode).

## Key Points:
- Creates Virtual DOM.
- Diffs old and new.
- Can be interrupted.
- Pure computation.

## Interview Tip:
"The render phase is pure computation â€” it can be interrupted in concurrent mode."

---

## Question 210: What is concurrent rendering?

## Answer:
Concurrent rendering allows React to prepare multiple versions of the UI simultaneously, prioritizing urgent updates.

## Key Points:
- Prepare multiple UI versions.
- Prioritize urgent updates.
- Pause and resume rendering.
- React 18 feature.

## Interview Tip:
"Concurrent rendering keeps the UI responsive by prioritizing urgent updates."

---

## Part 16 (211â€“220): Rendering Strategies

---

## Question 211: What is client-side rendering (CSR)?

## Answer:
CSR renders the application in the browser. The server sends an empty HTML shell with JavaScript.

## Key Points:
- Renders in browser.
- Empty HTML from server.
- JavaScript does the rendering.
- Poor SEO (initially).
- Fast subsequent navigation.

## Interview Tip:
"CSR is the default React behavior â€” everything renders in the browser."

---

## Question 212: What is server-side rendering (SSR)?

## Answer:
SSR renders the application on the server, sending fully rendered HTML to the browser.

## Key Points:
- Renders on server.
- Fully rendered HTML.
- Good for SEO.
- Faster initial load.
- Hydration for interactivity.

## Interview Tip:
"SSR sends fully rendered HTML â€” good for SEO and initial load."

---

## Question 213: What is static site generation (SSG)?

## Answer:
SSG generates HTML at build time. Pages are pre-rendered and served as static files.

## Key Points:
- Build-time rendering.
- Static HTML files.
- Fastest performance.
- No server computation.
- Content updates require rebuild.

## Interview Tip:
"SSG is the fastest â€” pre-rendered static files."

---

## Question 214: What is incremental static regeneration (ISR)?

## Answer:
ISR updates static pages after build time without rebuilding the entire site.

## Key Points:
- Update static pages after build.
- Revalidate on a timer.
- Fresh content without full rebuild.
- Next.js feature.

## Interview Tip:
"ISR combines SSG performance with dynamic content freshness."

---

## Question 215: What are the advantages and disadvantages of CSR?

## Answer:
- **Advantages**: Simple, fast subsequent navigation, rich interactions.
- **Disadvantages**: Poor SEO, slower initial load, blank page initially.

## Key Points:
- Simple setup.
- Fast navigation.
- Poor SEO.
- Slower initial load.

## Interview Tip:
"CSR for apps behind authentication; SSR/SSG for public-facing content."

---

## Question 216: What are the advantages and disadvantages of SSR?

## Answer:
- **Advantages**: Good SEO, fast initial load, social media previews.
- **Disadvantages**: Server load, slower TTFB, complex setup.

## Key Points:
- Good SEO.
- Fast initial load.
- Higher server load.
- Complex setup.

## Interview Tip:
"SSR for SEO-critical content; CSR for authenticated apps."

---

## Question 217: When would you choose CSR over SSR?

## Answer:
- **Admin dashboards**: Behind authentication, no SEO needed.
- **Internal tools**: Not indexed by search engines.
- **Real-time apps**: Heavy client-side interactions.

## Key Points:
- Authenticated apps.
- Internal tools.
- Real-time applications.
- No SEO requirements.

## Interview Tip:
"CSR for authenticated apps; SSR for public content."

---

## Question 218: What causes hydration in React?

## Answer:
Hydration is when React attaches event listeners to server-rendered HTML, making it interactive.

## Key Points:
- Attach event listeners.
- Make HTML interactive.
- Happens after SSR.
- Must match server HTML.

## Interview Tip:
"Hydration makes server-rendered HTML interactive."

---

## Question 219: What is hydration mismatch?

## Answer:
Hydration mismatch occurs when the client-rendered HTML doesn't match the server-rendered HTML.

## Key Points:
- Client HTML â‰  server HTML.
- Causes warnings.
- Common with dates, random values.
- Must match for proper hydration.

## Interview Tip:
"Hydration mismatches happen when server and client HTML differ â€” use `suppressHydrationWarning` for dates."

---

## Question 220: How do you debug hydration issues?

## Answer:
1. **Check console**: React logs hydration mismatches.
2. **Identify differences**: Find what doesn't match.
3. **Common causes**: Dates, random values, browser-only code.
4. **Use `suppressHydrationWarning`**: For intentional differences.

## Key Points:
- Check console for warnings.
- Find what doesn't match.
- Common: dates, random values.
- `suppressHydrationWarning` for intentional differences.

## Interview Tip:
"Hydration mismatches are usually dates or random values â€” use `suppressHydrationWarning`."

---

## Part 17 (221â€“230): React 18 & React 19

---

## Question 221: What are the major features introduced in React 18?

## Answer:
- **Concurrent features**: Automatic batching, transitions.
- **Suspense improvements**: Data fetching support.
- **Server Components**: Render on server.
- **New hooks**: `useTransition`, `useDeferredValue`, `useId`.

## Key Points:
- Concurrent rendering.
- Automatic batching.
- New hooks.
- Server Components.

## Interview Tip:
"React 18 introduced concurrent rendering â€” automatic batching, transitions, and new hooks."

---

## Question 222: What are concurrent features in React?

## Answer:
Concurrent features allow React to prepare multiple UI versions, prioritizing urgent updates.

- **Automatic batching**: Batch state updates.
- **Transitions**: Mark non-urgent updates.
- **Suspense**: Loading states for data.

## Key Points:
- Multiple UI versions.
- Priority-based updates.
- Automatic batching.
- Transitions and Suspense.

## Interview Tip:
"Concurrent features keep the UI responsive by prioritizing urgent updates."

---

## Question 223: What is automatic batching?

## Answer:
Automatic batching groups multiple state updates into a single re-render.

```jsx
function handleClick() {
  setCount(c => c + 1);
  setFlag(f => !f);
  // Only one re-render (React 18)
}
```

## Key Points:
- Groups state updates.
- Single re-render.
- Automatic in React 18.
- Performance optimization.

## Interview Tip:
"Automatic batching reduces re-renders â€” multiple updates become one render."

---

## Question 224: How does automatic batching improve performance?

## Answer:
- **Fewer re-renders**: Multiple updates = one render.
- **Better performance**: Less DOM updates.
- **Automatic**: No code changes needed.

## Key Points:
- Fewer re-renders.
- Less DOM updates.
- Automatic optimization.
- Better performance.

## Interview Tip:
"Automatic batching is free performance â€” no code changes needed."

---

## Question 225: What are React Server Components?

## Answer:
Server Components render on the server and send only the rendered output to the client. They don't send JavaScript.

## Key Points:
- Render on server.
- No JavaScript sent to client.
- Access server resources directly.
- Smaller bundle size.

## Interview Tip:
"Server Components reduce bundle size â€” no JavaScript for server-rendered components."

---

## Question 226: What are Client Components?

## Answer:
Client Components render on both server (for initial HTML) and client (for interactivity). They require `"use client"` directive.

## Key Points:
- Render on server and client.
- `"use client"` directive.
- Can use hooks and event handlers.
- Send JavaScript to client.

## Interview Tip:
"Client Components are traditional React components â€” they need interactivity."

---

## Question 227: What is the difference between Server Components and Client Components?

## Answer:
| Feature | Server Components | Client Components |
|---------|------------------|-------------------|
| Rendering | Server only | Server + Client |
| JavaScript | Not sent | Sent to client |
| Hooks | No | Yes |
| Interactivity | No | Yes |
| Directive | Default | `"use client"` |

## Key Points:
- Server: no JS, no hooks, no events.
- Client: full React features.
- Server is the default.
- Client needs `"use client"`.

## Interview Tip:
"Server Components for data; Client Components for interactivity."

---

## Question 228: When should you use Server Components?

## Answer:
- **Data fetching**: Fetch data directly on server.
- **Large dependencies**: Keep them off the client.
- **Static content**: No interactivity needed.
- **SEO**: Server-rendered content.

## Key Points:
- Data fetching.
- Large dependencies.
- Static content.
- SEO-critical content.

## Interview Tip:
"Server Components for data and static content; Client Components for interactivity."

---

## Question 229: What new features were introduced in React 19?

## Answer:
- **Actions**: Async functions for form submissions.
- **`useActionState`**: Form state management.
- **`useFormStatus`**: Form submission status.
- **`useOptimistic`**: Optimistic updates.
- **ref as prop**: No need for `forwardRef`.

## Key Points:
- Actions for forms.
- New form hooks.
- Optimistic updates.
- ref as prop.

## Interview Tip:
"React 19 focuses on forms â€” Actions, `useActionState`, and `useFormStatus`."

---

## Question 230: How do React 18 and React 19 improve developer experience?

## Answer:
- **React 18**: Concurrent features, automatic batching, new hooks.
- **React 19**: Simplified forms, ref as prop, better error handling.

## Key Points:
- Concurrent rendering.
- Automatic batching.
- Simplified forms.
- Better DX.

## Interview Tip:
"React 18 improved performance; React 19 simplified forms and refs."

---

## Part 18 (231â€“240): Design Patterns

---

## Question 231: What is component composition?

## Answer:
Combining simple components to build complex UIs using `children` and props.

## Key Points:
- Combine simple components.
- Build complex UIs.
- Use `children` and props.
- React's core pattern.

## Interview Tip:
"Composition is React's core pattern â€” build complex UIs from simple pieces."

---

## Question 232: What are compound components?

## Answer:
Components that work together, sharing implicit state.

```jsx
<Select>
  <Select.Option value="1">Option 1</Select.Option>
</Select>
```

## Key Points:
- Work together as a unit.
- Share implicit state.
- Clean API.
- Common in UI libraries.

## Interview Tip:
"Compound components share state implicitly â€” they work as a unit."

---

## Question 233: What is the Higher-Order Component (HOC) pattern?

## Answer:
A function that takes a component and returns an enhanced component.

```jsx
const Enhanced = withAuth(Component);
```

## Key Points:
- Function takes component, returns enhanced.
- Adds functionality.
- Cross-cutting concerns.
- Being replaced by hooks.

## Interview Tip:
"HOCs add functionality â€” but custom hooks are usually better."

---

## Question 234: When should you use HOCs?

## Answer:
- **Authentication**: Protect routes.
- **Data fetching**: Add loading states.
- **Logging**: Track usage.
- **Legacy code**: When hooks aren't available.

## Key Points:
- Cross-cutting concerns.
- Authentication.
- Data fetching.
- Legacy code.

## Interview Tip:
"HOCs for cross-cutting concerns â€” but prefer hooks in modern code."

---

## Question 235: What are the drawbacks of HOCs?

## Answer:
- **Wrapper hell**: Deep nesting.
- **Prop collisions**: Same prop names.
- **No hooks**: Can't use hooks inside.
- **Debugging**: Harder to trace.

## Key Points:
- Wrapper hell.
- Prop collisions.
- No hooks inside.
- Harder debugging.

## Interview Tip:
"Custom hooks avoid HOC drawbacks â€” no wrapper hell, no prop collisions."

---

## Question 236: What is the Render Props pattern?

## Answer:
A component receives a function as a prop and calls it to render.

```jsx
<MouseTracker render={({ x, y }) => <p>{x}, {y}</p>} />
```

## Key Points:
- Function as prop.
- Component calls function.
- Shares data with caller.
- Being replaced by hooks.

## Interview Tip:
"Render props share data via a function â€” hooks are usually cleaner."

---

## Question 237: When should you use Render Props?

## Answer:
- **Dynamic rendering**: Different render logic per use.
- **Shared state**: Share state with flexible rendering.
- **Libraries**: When building component libraries.

## Key Points:
- Dynamic rendering.
- Shared state.
- Library patterns.
- Being replaced by hooks.

## Interview Tip:
"Render props for flexible rendering â€” but hooks are usually better."

---

## Question 238: What are the advantages of custom Hooks over HOCs?

## Answer:
- **No wrapper hell**: Flat structure.
- **No prop collisions**: Clear data flow.
- **Composable**: Hooks can call hooks.
- **Simpler**: Easier to understand.

## Key Points:
- No wrapper nesting.
- No prop collisions.
- Composable.
- Simpler code.

## Interview Tip:
"Custom hooks are cleaner than HOCs â€” no wrapper hell."

---

## Question 239: What are the advantages of custom Hooks over Render Props?

## Answer:
- **Cleaner syntax**: No nested functions.
- **Multiple hooks**: Easy to use many hooks.
- **Better TypeScript**: Better type inference.
- **Linear flow**: Easier to read.

## Key Points:
- No nested functions.
- Easy composition.
- Better TypeScript.
- More readable.

## Interview Tip:
"Custom hooks are cleaner than render props â€” no nested functions."

---

## Question 240: Which React design pattern do you prefer and why?

## Answer:
Custom Hooks. They're:
- **Composable**: Hooks can call hooks.
- **Clean**: No wrapper hell.
- **Type-safe**: Better TypeScript support.
- **Testable**: Easy to test in isolation.

## Key Points:
- Composable.
- Clean syntax.
- Type-safe.
- Testable.

## Interview Tip:
"Custom hooks are the modern standard â€” they're composable, clean, and testable."

---

## Part 19 (241â€“250): Architecture & Best Practices

---

## Question 241: How do you structure a large React application?

## Answer:
```
src/
  components/      # Shared UI components
  features/        # Feature-based modules
  hooks/           # Custom hooks
  utils/           # Utility functions
  services/        # API calls
  context/         # Context providers
  types/           # TypeScript types
```

## Key Points:
- Feature-based organization.
- Shared components separate.
- Custom hooks in hooks/.
- Services for API calls.
- Types for TypeScript.

## Interview Tip:
"Feature-based organization scales better than type-based."

---

## Question 242: How do you organize components in a scalable project?

## Answer:
Feature-based:
```
features/
  auth/
    components/
    hooks/
    services/
  dashboard/
    components/
    hooks/
    services/
```

## Key Points:
- Feature-based folders.
- Each feature is self-contained.
- Shared components in components/.
- Easy to navigate.

## Interview Tip:
"Feature-based organization scales better â€” each feature is self-contained."

---

## Question 243: How do you decide where state should live?

## Answer:
1. **Local state**: Component-specific (useState).
2. **Lifted state**: Shared between siblings.
3. **Context**: Global state (theme, auth).
4. **URL state**: Filters, pagination.
5. **Server state**: TanStack Query.

## Key Points:
- Local for component-specific.
- Lifted for sibling sharing.
- Context for global.
- URL for filters.
- Server state with TanStack Query.

## Interview Tip:
"Start local, lift when needed, use Context for global."

---

## Question 244: How do you avoid prop drilling in large applications?

## Answer:
1. **Context API**: Share data without drilling.
2. **State management**: Redux, Zustand.
3. **Component composition**: Use `children`.
4. **Custom hooks**: Encapsulate shared logic.

## Key Points:
- Context API.
- State management.
- Composition.
- Custom hooks.

## Interview Tip:
"Context API is the built-in solution for prop drilling."

---

## Question 245: How do you manage shared business logic?

## Answer:
Custom hooks:
```jsx
function useAuth() { ... }
function useCart() { ... }
function useNotifications() { ... }
```

## Key Points:
- Custom hooks for shared logic.
- Reusable across components.
- Testable in isolation.
- Clean separation.

## Interview Tip:
"Custom hooks are the standard for shared business logic."

---

## Question 246: What are common React anti-patterns?

## Answer:
1. **Mutating state**: Direct mutation.
2. **Missing keys**: In lists.
3. **Inline functions**: Causing re-renders.
4. **Overusing Context**: For frequently changing data.
5. **Premature optimization**: Memoizing everything.

## Key Points:
- State mutation.
- Missing keys.
- Inline functions.
- Context overuse.
- Premature optimization.

## Interview Tip:
"The biggest anti-pattern is mutating state directly â€” always create new references."

---

## Question 247: How do you write reusable React components?

## Answer:
1. **Single responsibility**: One job per component.
2. **Clear props API**: Well-defined interface.
3. **Composition**: Use `children` and render props.
4. **Defaults**: Sensible default prop values.
5. **Documentation**: Document props and usage.

## Key Points:
- Single responsibility.
- Clear props API.
- Composition.
- Defaults.
- Documentation.

## Interview Tip:
"Reusable components have a single responsibility and a clear props API."

---

## Question 248: How do you debug complex React applications?

## Answer:
1. **React DevTools**: Component tree, props, state.
2. **Console.log**: Strategic logging.
3. **Breakpoints**: In browser DevTools.
4. **Error Boundaries**: Catch errors.
5. **Profiler**: Find performance issues.

## Key Points:
- React DevTools.
- Console.log.
- Breakpoints.
- Error Boundaries.
- Profiler.

## Interview Tip:
"React DevTools + console.log + breakpoints â€” the debugging toolkit."

---

## Question 249: What React best practices do you follow in production?

## Answer:
1. **TypeScript**: Type safety.
2. **Error Boundaries**: Catch errors.
3. **Code splitting**: Lazy load routes.
4. **Performance profiling**: Regular profiling.
5. **Testing**: Unit and integration tests.
6. **Accessibility**: ARIA attributes, keyboard support.

## Key Points:
- TypeScript.
- Error Boundaries.
- Code splitting.
- Performance profiling.
- Testing.
- Accessibility.

## Interview Tip:
"TypeScript, Error Boundaries, code splitting, and testing â€” the production essentials."

---

## Question 250: How would you architect a large enterprise React application?

## Answer:
- **TypeScript**: Type safety everywhere.
- **Feature-based structure**: Self-contained modules.
- **State management**: Redux Toolkit or Zustand.
- **Routing**: React Router with lazy loading.
- **API layer**: TanStack Query or custom hooks.
- **Testing**: Jest + React Testing Library.
- **Error handling**: Error Boundaries + Sentry.
- **Performance**: Profiling + optimization.

## Key Points:
- TypeScript for type safety.
- Feature-based structure.
- State management for complex state.
- Lazy loading for performance.
- Comprehensive testing.

## Interview Tip:
"TypeScript + feature-based structure + state management + testing = enterprise React."

---

## Part 20 (251â€“260): Production & Debugging

---

## Question 251: How do you debug a React application in production?

## Answer:
1. **Error tracking**: Sentry for error monitoring.
2. **Source maps**: Enable for debugging.
3. **Console logs**: Strategic logging.
4. **React DevTools**: Production build profiling.
5. **Network tab**: Check API calls.

## Key Points:
- Sentry for errors.
- Source maps for debugging.
- Console logs.
- React DevTools.
- Network tab.

## Interview Tip:
"Sentry + source maps + React DevTools â€” the production debugging toolkit."

---

## Question 252: A React page is re-rendering continuously. How would you debug it?

## Answer:
1. **React DevTools Profiler**: See what's re-rendering.
2. **Check for state updates in render**: State updates causing loops.
3. **Check useEffect dependencies**: Missing dependencies.
4. **Check Context**: Context value changing every render.
5. **Console.log in render**: Track render count.

## Key Points:
- Profiler to identify.
- State updates in render.
- useEffect dependencies.
- Context value stability.
- Console.log for tracking.

## Interview Tip:
"Use the Profiler to find what's re-rendering, then check for state update loops."

---

## Question 253: A component is rendering too slowly. How do you identify the bottleneck?

## Answer:
1. **React DevTools Profiler**: Find slow components.
2. **Chrome DevTools Performance**: CPU profiling.
3. **Check render count**: How many times it renders.
4. **Check child components**: Are children re-rendering?
5. **Check expensive operations**: In render function.

## Key Points:
- Profiler for component timing.
- Chrome DevTools for CPU.
- Render count.
- Child re-renders.
- Expensive operations.

## Interview Tip:
"Profile with React DevTools â€” find which component is slow and why."

---

## Question 254: How do you debug unnecessary re-renders?

## Answer:
1. **React DevTools**: Highlight re-renders.
2. **why-did-you-render**: Logs re-render reasons.
3. **Console.log in render**: Track when renders happen.
4. **Check props**: Are props changing?
5. **Check Context**: Is context value stable?

## Key Points:
- React DevTools highlight.
- why-did-you-render library.
- Console.log tracking.
- Props stability.
- Context stability.

## Interview Tip:
"why-did-you-render logs exactly why components re-render â€” it's invaluable."

---

## Question 255: How do you profile React performance using React DevTools?

## Answer:
1. **Open Profiler tab** in React DevTools.
2. **Record** interactions.
3. **Analyze** which components render and how long.
4. **Identify** slow components and unnecessary re-renders.

## Key Points:
- Profiler tab.
- Record interactions.
- Analyze render times.
- Identify bottlenecks.

## Interview Tip:
"The Profiler shows exactly which components render and how long they take."

---

## Question 256: How do you debug memory leaks in React?

## Answer:
1. **Chrome DevTools Memory**: Take heap snapshots.
2. **Check useEffect cleanup**: Are subscriptions cleaned up?
3. **Check event listeners**: Are they removed?
4. **Check timers**: Are intervals cleared?
5. **Check closures**: Are large objects captured?

## Key Points:
- Heap snapshots.
- useEffect cleanup.
- Event listener removal.
- Timer cleanup.
- Closure analysis.

## Interview Tip:
"Most memory leaks are from missing useEffect cleanup â€” always clean up subscriptions."

---

## Question 257: What are common causes of memory leaks in React applications?

## Answer:
1. **Missing useEffect cleanup**: Subscriptions not cleaned up.
2. **Event listeners**: Not removed on unmount.
3. **Timers**: Intervals not cleared.
4. **Closures**: Capturing large objects.
5. **Third-party libraries**: Not properly destroyed.

## Key Points:
- Missing cleanup.
- Event listeners.
- Timers.
- Closures.
- Third-party libraries.

## Interview Tip:
"Always return a cleanup function from useEffect when you subscribe to something."

---

## Question 258: How do you debug hydration errors in React?

## Answer:
1. **Check console**: React logs hydration mismatches.
2. **Identify differences**: What doesn't match?
3. **Common causes**: Dates, random values, browser APIs.
4. **Use `suppressHydrationWarning`**: For intentional differences.

## Key Points:
- Console warnings.
- Identify differences.
- Common causes.
- suppressHydrationWarning.

## Interview Tip:
"Hydration mismatches are usually dates or random values â€” use suppressHydrationWarning."

---

## Question 259: How do you debug state synchronization issues?

## Answer:
1. **React DevTools**: Inspect state values.
2. **Console.log**: Log state changes.
3. **Check dependencies**: Are effects correct?
4. **Check race conditions**: Are async operations ordered?
5. **Use functional updates**: `setState(prev => ...)`.

## Key Points:
- DevTools for inspection.
- Console.log for tracking.
- Dependency checking.
- Race condition handling.
- Functional updates.

## Interview Tip:
"Use React DevTools to inspect state â€” check if state matches expectations."

---

## Question 260: How do you debug race conditions caused by asynchronous API calls?

## Answer:
1. **AbortController**: Cancel stale requests.
2. **Cleanup in useEffect**: Cancel on unmount.
3. **Ignore stale responses**: Check if component is mounted.
4. **Use TanStack Query**: Handles race conditions automatically.

## Key Points:
- AbortController for cancellation.
- Cleanup functions.
- Stale response handling.
- TanStack Query.

## Interview Tip:
"AbortController prevents stale responses â€” always cancel requests on cleanup."

---

## Part 21 (261â€“270): State Management Decisions

---

## Question 261: When is local component state enough?

## Answer:
- **Form inputs**: Input values.
- **UI toggles**: Modals, dropdowns.
- **Component-specific data**: Not shared.
- **Temporary data**: Loading states.

## Key Points:
- Form inputs.
- UI toggles.
- Component-specific.
- Temporary data.

## Interview Tip:
"Start with local state â€” only go global when you need to share."

---

## Question 262: When would you choose Context API?

## Answer:
- **Theme**: Light/dark mode.
- **Locale**: Language settings.
- **Auth**: Current user.
- **Infrequently changing data**: Global settings.

## Key Points:
- Theme and locale.
- Authentication.
- Global settings.
- Infrequent changes.

## Interview Tip:
"Context for global, infrequently changing data."

---

## Question 263: When would you choose Redux Toolkit?

## Answer:
- **Complex state**: Many interdependent values.
- **Frequent updates**: Real-time data.
- **DevTools needed**: Time-travel debugging.
- **Large teams**: Clear patterns and conventions.

## Key Points:
- Complex state.
- Frequent updates.
- DevTools.
- Large teams.

## Interview Tip:
"Redux for complex state with many updates â€” DevTools are invaluable."

---

## Question 264: When would you choose Zustand?

## Answer:
- **Simple global state**: Less boilerplate than Redux.
- **Performance**: Minimal re-renders.
- **Small to medium apps**: Simple API.
- **TypeScript**: Great TS support.

## Key Points:
- Simple global state.
- Minimal boilerplate.
- Good performance.
- TypeScript-friendly.

## Interview Tip:
"Zustand for simple global state â€” less boilerplate than Redux."

---

## Question 265: When would you choose React Query or TanStack Query?

## Answer:
- **Server state**: Data from APIs.
- **Caching**: Automatic caching.
- **Refetching**: Background updates.
- **Loading/error states**: Automatic management.

## Key Points:
- Server state management.
- Automatic caching.
- Background refetching.
- Loading/error states.

## Interview Tip:
"TanStack Query for server state â€” it handles caching, loading, and errors automatically."

---

## Question 266: How do you decide whether state should be global or local?

## Answer:
- **Local**: Used by one component.
- **Lifted**: Shared between siblings.
- **Global**: Used across many components.
- **URL**: Filters, pagination.
- **Server**: API data.

## Key Points:
- Local for component-specific.
- Lifted for siblings.
- Global for app-wide.
- URL for filters.
- Server state for API data.

## Interview Tip:
"Start local, lift when needed, go global only when necessary."

---

## Question 267: What data should never be stored in global state?

## Answer:
- **Form inputs**: Use local state.
- **Temporary UI state**: Modals, tooltips.
- **Derived data**: Compute from other state.
- **Server data**: Use TanStack Query.

## Key Points:
- Form inputs.
- Temporary UI.
- Derived data.
- Server data.

## Interview Tip:
"Form inputs, temporary UI, and derived data should stay local."

---

## Question 268: How do you avoid overusing Context API?

## Answer:
- **Split contexts**: Separate concerns.
- **Use state management**: For complex state.
- **Local state**: For component-specific data.
- **URL state**: For filters and pagination.

## Key Points:
- Split contexts.
- State management for complex.
- Local for component-specific.
- URL for filters.

## Interview Tip:
"Split contexts and use local state â€” don't put everything in Context."

---

## Question 269: How do you organize application state in a large React project?

## Answer:
1. **Local state**: Component-specific (useState).
2. **URL state**: Filters, pagination.
3. **Server state**: TanStack Query.
4. **Global state**: Zustand or Redux.
5. **Context**: Theme, auth, locale.

## Key Points:
- Local for component-specific.
- URL for filters.
- Server state with TanStack Query.
- Global for shared state.
- Context for theme/auth.

## Interview Tip:
"Categorize state: local, URL, server, global â€” use the right tool for each."

---

## Question 270: How do you handle shared state across multiple pages?

## Answer:
- **URL state**: Filters, search queries.
- **Global state**: Zustand or Redux.
- **Server state**: TanStack Query with cache.
- **Context**: Theme, auth.

## Key Points:
- URL for shareable state.
- Global for app-wide state.
- Server state with caching.
- Context for theme/auth.

## Interview Tip:
"URL state for shareable filters; global state for app-wide data."

---

## Part 22 (271â€“280): Testing

---

## Question 271: How do you test React components?

## Answer:
```jsx
import { render, screen, fireEvent } from "@testing-library/react";

test("renders button", () => {
  render(<Button label="Click me" />);
  expect(screen.getByText("Click me")).toBeInTheDocument();
});

test("calls onClick", () => {
  const handleClick = jest.fn();
  render(<Button onClick={handleClick} />);
  fireEvent.click(screen.getByRole("button"));
  expect(handleClick).toHaveBeenCalled();
});
```

## Key Points:
- React Testing Library for rendering.
- `screen` for querying.
- `fireEvent` for interactions.
- Jest for assertions.

## Interview Tip:
"React Testing Library tests behavior, not implementation."

---

## Question 272: What is the difference between unit, integration, and end-to-end testing?

## Answer:
- **Unit**: Test individual components/functions.
- **Integration**: Test component interactions.
- **E2E**: Test full user flows (Cypress, Playwright).

## Key Points:
- Unit: individual pieces.
- Integration: component interactions.
- E2E: full user flows.
- Different tools for each.

## Interview Tip:
"Unit for components, integration for features, E2E for user flows."

---

## Question 273: What is React Testing Library?

## Answer:
React Testing Library provides utilities for testing React components by simulating user interactions.

## Key Points:
- Test behavior, not implementation.
- Simulate user interactions.
- Query by role, text, label.
- Industry standard.

## Interview Tip:
"React Testing Library tests what the user sees and does."

---

## Question 274: Why is React Testing Library preferred over Enzyme?

## Answer:
- **Behavior-focused**: Tests what users see.
- **Implementation-agnostic**: Doesn't test internals.
- **Accessible queries**: By role, label, text.
- **Maintained**: Active development.

## Key Points:
- Tests behavior.
- Implementation-agnostic.
- Accessible queries.
- Modern and maintained.

## Interview Tip:
"React Testing Library tests behavior; Enzyme tests implementation. Behavior is more reliable."

---

## Question 275: What is Jest?

## Answer:
Jest is a JavaScript testing framework with built-in assertions, mocking, and code coverage.

## Key Points:
- Testing framework.
- Built-in assertions.
- Mocking support.
- Code coverage.
- Industry standard.

## Interview Tip:
"Jest is the standard JavaScript testing framework."

---

## Question 276: How do you test asynchronous React components?

## Answer:
```jsx
import { render, screen, waitFor } from "@testing-library/react";

test("loads data", async () => {
  render(<UserProfile />);
  await waitFor(() => {
    expect(screen.getByText("Alice")).toBeInTheDocument();
  });
});
```

## Key Points:
- `waitFor` for async operations.
- `findBy` queries for async elements.
- Mock API calls.
- Test loading and error states.

## Interview Tip:
"Use `waitFor` or `findBy` for async operations."

---

## Question 277: How do you mock API requests in tests?

## Answer:
```jsx
// MSW (Mock Service Worker)
import { rest } from "msw";
import { setupServer } from "msw/node";

const server = setupServer(
  rest.get("/api/users", (req, res, ctx) => {
    return res(ctx.json([{ name: "Alice" }]));
  })
);

beforeAll(() => server.listen());
afterAll(() => server.close());
```

## Key Points:
- MSW for API mocking.
- Intercept network requests.
- Return mock data.
- Test different responses.

## Interview Tip:
"MSW is the standard for API mocking â€” it intercepts actual network requests."

---

## Question 278: What should you test in a React component?

## Answer:
- **Rendering**: Does it render correctly?
- **User interactions**: Click, type, submit.
- **State changes**: Does state update correctly?
- **Conditional rendering**: Different states.
- **Error states**: Error handling.

## Key Points:
- Rendering.
- User interactions.
- State changes.
- Conditional rendering.
- Error states.

## Interview Tip:
"Test what the user sees and does â€” not implementation details."

---

## Question 279: What should you avoid testing?

## Answer:
- **Implementation details**: Internal state, methods.
- **Third-party code**: Library internals.
- **Styling**: CSS classes (use visual testing).
- **Trivial code**: Simple getters/setters.

## Key Points:
- Implementation details.
- Third-party code.
- Styling.
- Trivial code.

## Interview Tip:
"Don't test implementation details â€” test behavior."

---

## Question 280: How much test coverage is enough?

## Answer:
Aim for 80%+ coverage, but focus on:
- **Critical paths**: Core features.
- **Complex logic**: Business rules.
- **Edge cases**: Error handling.
- **User flows**: Key interactions.

## Key Points:
- 80%+ as a guideline.
- Focus on critical paths.
- Complex logic and edge cases.
- Quality over quantity.

## Interview Tip:
"Coverage is a metric, not a goal â€” focus on testing critical paths."

---

## Part 23 (281â€“290): Accessibility (A11y)

---

## Question 281: What is accessibility in React?

## Answer:
Accessibility (A11y) ensures applications are usable by everyone, including people with disabilities.

## Key Points:
- Usable by everyone.
- Screen reader support.
- Keyboard navigation.
- ARIA attributes.
- Semantic HTML.

## Interview Tip:
"Accessibility ensures everyone can use your application."

---

## Question 282: Why is accessibility important?

## Answer:
- **Inclusivity**: Everyone deserves access.
- **Legal requirements**: ADA, WCAG compliance.
- **SEO**: Semantic HTML improves SEO.
- **Better UX**: Accessibility improves UX for everyone.

## Key Points:
- Inclusivity.
- Legal compliance.
- SEO benefits.
- Better UX.

## Interview Tip:
"Accessibility is the right thing to do and it's often legally required."

---

## Question 283: How do you make React applications accessible?

## Answer:
1. **Semantic HTML**: Use proper elements.
2. **ARIA attributes**: For custom components.
3. **Keyboard support**: Tab, Enter, Escape.
4. **Focus management**: Visible focus indicators.
5. **Alt text**: For images.

## Key Points:
- Semantic HTML.
- ARIA attributes.
- Keyboard support.
- Focus management.
- Alt text.

## Interview Tip:
"Semantic HTML is the foundation â€” use proper elements before adding ARIA."

---

## Question 284: What are ARIA attributes?

## Answer:
ARIA (Accessible Rich Internet Applications) attributes provide accessibility information for custom components.

```jsx
<div role="button" aria-label="Close" onClick={close}>Ã—</div>
```

## Key Points:
- Accessibility attributes.
- For custom components.
- `role`, `aria-label`, `aria-describedby`.
- Use when semantic HTML isn't enough.

## Interview Tip:
"ARIA attributes are for custom components â€” prefer semantic HTML first."

---

## Question 285: How do you build accessible forms?

## Answer:
1. **Labels**: Associate labels with inputs.
2. **Error messages**: Announce errors.
3. **Required fields**: Indicate required fields.
4. **Keyboard support**: Tab through fields.
5. **Focus management**: Focus first error.

## Key Points:
- Proper labels.
- Error announcements.
- Required indicators.
- Keyboard navigation.
- Focus management.

## Interview Tip:
"Labels are the foundation of accessible forms â€” always associate them."

---

## Question 286: How do you ensure keyboard accessibility?

## Answer:
1. **Tab order**: Logical tab sequence.
2. **Focus indicators**: Visible focus styles.
3. **Keyboard handlers**: Enter, Escape, Arrow keys.
4. **Skip links**: Skip to main content.
5. **Focus trapping**: In modals.

## Key Points:
- Logical tab order.
- Visible focus.
- Keyboard handlers.
- Skip links.
- Focus trapping.

## Interview Tip:
"Test with only the keyboard â€” if you can't use it, it's not accessible."

---

## Question 287: How do you test accessibility?

## Answer:
1. **Manual testing**: Keyboard navigation, screen reader.
2. **Automated tools**: axe, Lighthouse.
3. **React Testing Library**: Accessible queries.
4. **Screen readers**: NVDA, VoiceOver.

## Key Points:
- Manual testing.
- Automated tools.
- Testing Library queries.
- Screen reader testing.

## Interview Tip:
"Automated tools catch 30% of issues â€” manual testing catches the rest."

---

## Question 288: What tools do you use to check accessibility?

## Answer:
- **axe-core**: Automated accessibility testing.
- **Lighthouse**: Performance and accessibility audit.
- **eslint-plugin-jsx-a11y**: Linting for accessibility.
- **Screen readers**: NVDA, VoiceOver.

## Key Points:
- axe-core for automated testing.
- Lighthouse for audits.
- ESLint plugin for linting.
- Screen readers for manual testing.

## Interview Tip:
"axe-core + Lighthouse + manual testing â€” the accessibility toolkit."

---

## Question 289: What are common accessibility mistakes in React applications?

## Answer:
1. **Missing labels**: Inputs without labels.
2. **No alt text**: Images without alt.
3. **Poor focus management**: No visible focus.
4. **Non-semantic HTML**: Using divs for everything.
5. **Missing keyboard support**: No keyboard handlers.

## Key Points:
- Missing labels.
- No alt text.
- Poor focus.
- Non-semantic HTML.
- Missing keyboard support.

## Interview Tip:
"Missing labels and alt text are the most common accessibility mistakes."

---

## Question 290: How does semantic HTML improve accessibility in React?

## Answer:
Semantic HTML (`<nav>`, `<main>`, `<button>`) provides built-in accessibility. Screen readers understand these elements without ARIA attributes.

## Key Points:
- Built-in accessibility.
- Screen reader support.
- Keyboard support.
- Better than ARIA.

## Interview Tip:
"Use semantic HTML â€” it's accessible by default."

---

## Part 24 (291â€“300): Real Senior Interview Questions

---

## Question 291: What are the biggest mistakes developers make in React?

## Answer:
1. **Mutating state**: Direct mutation.
2. **Missing keys**: In lists.
3. **Prop drilling**: Instead of Context.
4. **Overusing state**: Everything in global state.
5. **No error handling**: Missing Error Boundaries.
6. **Premature optimization**: Memoizing everything.

## Key Points:
- State mutation.
- Missing keys.
- Prop drilling.
- State overuse.
- No error handling.
- Premature optimization.

## Interview Tip:
"The biggest mistake is mutating state â€” it causes subtle bugs."

---

## Question 292: What React features do you use most frequently in production?

## Answer:
- **useState**: State management.
- **useEffect**: Side effects.
- **useContext**: Global data.
- **useCallback/useMemo**: Performance.
- **React.lazy**: Code splitting.
- **Error Boundaries**: Error handling.

## Key Points:
- useState and useEffect.
- useContext for global data.
- Performance hooks.
- Code splitting.
- Error handling.

## Interview Tip:
"useState, useEffect, useContext, and custom hooks â€” the production essentials."

---

## Question 293: What is the most challenging React bug you've fixed?

## Answer:
Choose a real bug and describe:
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
"Interviewers want to see your debugging process."

---

## Question 294: How do you review React code during a pull request?

## Answer:
Check for:
1. **State management**: Proper state handling.
2. **Performance**: Unnecessary re-renders.
3. **Accessibility**: ARIA attributes, keyboard support.
4. **Error handling**: Error Boundaries.
5. **Testing**: Adequate test coverage.
6. **TypeScript**: Proper typing.

## Key Points:
- State management.
- Performance.
- Accessibility.
- Error handling.
- Testing.
- TypeScript.

## Interview Tip:
"Accessibility and error handling are the most important things to check."

---

## Question 295: What React best practices do you enforce in your team?

## Answer:
1. **TypeScript**: Type safety.
2. **ESLint**: Code quality.
3. **Testing**: Required for new features.
4. **Accessibility**: ARIA attributes, keyboard support.
5. **Error Boundaries**: For all routes.
6. **Code review**: All PRs reviewed.

## Key Points:
- TypeScript.
- ESLint.
- Testing.
- Accessibility.
- Error Boundaries.
- Code review.

## Interview Tip:
"TypeScript, ESLint, testing, and accessibility â€” the team standards."

---

## Question 296: How do you onboard a new developer to a large React codebase?

## Answer:
1. **Documentation**: README, architecture docs.
2. **Walkthrough**: Codebase tour.
3. **Small tasks**: Start with simple bugs.
4. **Pair programming**: Work together on features.
5. **Code review**: Detailed feedback.

## Key Points:
- Documentation.
- Codebase tour.
- Small tasks.
- Pair programming.
- Code review.

## Interview Tip:
"Start with small tasks and pair programming â€” build confidence gradually."

---

## Question 297: If React didn't exist, what alternative would you choose and why?

## Answer:
- **Vue**: Similar component model, easier learning curve.
- **Svelte**: Compiles away, no runtime overhead.
- **Solid**: Fine-grained reactivity, fast.

## Key Points:
- Vue for similarity.
- Svelte for simplicity.
- Solid for performance.
- Choose based on needs.

## Interview Tip:
"Vue for a similar experience; Svelte for simplicity; Solid for performance."

---

## Question 298: What React features are you most excited about in the future?

## Answer:
- **Server Components**: Better performance.
- **React Compiler**: Automatic optimization.
- **Actions**: Simplified forms.
- **Concurrent features**: Better UX.

## Key Points:
- Server Components.
- React Compiler.
- Actions.
- Concurrent features.

## Interview Tip:
"Server Components and the React Compiler â€” they'll change how we write React."

---

## Question 299: How would you explain React to a junior developer?

## Answer:
"React is a JavaScript library for building user interfaces. You create small, reusable pieces called components, and React handles updating the DOM efficiently when your data changes. It uses a Virtual DOM to minimize expensive browser operations."

## Key Points:
- Library for UIs.
- Component-based.
- Virtual DOM.
- Declarative.

## Interview Tip:
"Keep it simple: React is a library for building UIs with components."

---

## Question 300: If you were building a production React application today, what architecture, tools, and best practices would you choose, and why?

## Answer:
- **Next.js**: Full-stack React framework.
- **TypeScript**: Type safety.
- **Tailwind CSS**: Utility-first styling.
- **TanStack Query**: Server state management.
- **Zustand**: Client state management.
- **Zod**: Validation.
- **Jest + React Testing Library**: Testing.
- **Sentry**: Error tracking.

## Key Points:
- Next.js for framework.
- TypeScript for type safety.
- Tailwind for styling.
- TanStack Query for server state.
- Zustand for client state.
- Zod for validation.

## Interview Tip:
"Next.js + TypeScript + TanStack Query + Zustand â€” the modern React stack."

---

# End of React Interview Questions & Answers
