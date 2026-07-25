# Redux Toolkit Interview Questions (150 Total)

---

# Redux Fundamentals

1. What is Redux?
2. Why was Redux created?
3. What problems does Redux solve?
4. What are the advantages of Redux?
5. What are the disadvantages of Redux?
6. What is Redux Toolkit?
7. Why was Redux Toolkit introduced?
8. How does Redux Toolkit differ from Redux?
9. When should you use Redux Toolkit?
10. When should you avoid Redux?

---

# Core Concepts

11. What is a Store?
12. What is the global state?
13. What is an Action?
14. What is a Reducer?
15. What is a Slice?
16. What is `createSlice()`?
17. What is `configureStore()`?
18. What is `createAction()`?
19. What is `PayloadAction`?
20. What is the Redux data flow?

---

# Store Configuration

21. How do you create a Redux Toolkit store?
22. How do you add multiple reducers?
23. What is the root reducer?
24. How do you organize slices in a large project?
25. How do you configure middleware?
26. What middleware is included by default?
27. What is the Redux DevTools Extension?
28. How do you enable Redux DevTools?
29. How do you configure Redux Toolkit for production?
30. What store configuration best practices do you follow?

---

# React Integration

31. What is the React-Redux library?
32. What is the `Provider` component?
33. Why is `Provider` required?
34. What is `useSelector()`?
35. What is `useDispatch()`?
36. How does `useSelector()` work?
37. How do you prevent unnecessary re-renders with `useSelector()`?
38. What is `shallowEqual`?
39. What are typed Redux hooks?
40. How do you create custom typed hooks in TypeScript?

---

# State Management

41. What data should be stored in Redux?
42. What data should remain in local component state?
43. What is normalized state?
44. Why is normalized state important?
45. What is immutable state?
46. How does Redux Toolkit handle immutable updates?
47. What is Immer?
48. How does Immer simplify reducer logic?
49. What common Redux mistakes should be avoided?
50. What Redux Toolkit best practices do you follow?

---

# Async Logic

51. What is asynchronous logic in Redux?
52. Why can't reducers contain asynchronous code?
53. What is `createAsyncThunk()`?
54. How does `createAsyncThunk()` work?
55. What arguments does `createAsyncThunk()` receive?
56. What are the `pending`, `fulfilled`, and `rejected` action states?
57. How do you handle loading states?
58. How do you handle error states?
59. How do you cancel an async thunk?
60. What are common mistakes when using async thunks?

---

# Extra Reducers

61. What are `extraReducers`?
62. How do `reducers` differ from `extraReducers`?
63. When should you use `extraReducers`?
64. How do you handle async thunk actions in `extraReducers`?
65. What is the builder callback syntax?
66. Why is the builder pattern preferred?
67. How do you share actions between slices?
68. How do you reset state from another slice?
69. How do you handle global logout actions?
70. What are common `extraReducers` best practices?

---

# RTK Query

71. What is RTK Query?
72. Why was RTK Query introduced?
73. How does RTK Query differ from `createAsyncThunk()`?
74. When should you use RTK Query?
75. What is `createApi()`?
76. What is `fetchBaseQuery()`?
77. How do you define endpoints?
78. What is the difference between `query` and `mutation`?
79. How do generated hooks work?
80. What are tags in RTK Query?

---

# Caching & Data Fetching

81. How does RTK Query cache data?
82. What is cache invalidation?
83. How do you invalidate cached data?
84. What are `providesTags`?
85. What are `invalidatesTags`?
86. How do you refetch cached data?
87. How do polling and automatic refetching work?
88. How do you perform optimistic updates?
89. How do you prefetch data?
90. What RTK Query best practices do you follow?

---

# Middleware & Persistence

91. What is middleware in Redux Toolkit?
92. What middleware is included by default?
93. What is Redux Thunk middleware?
94. How do you create custom middleware?
95. What is `redux-persist`?
96. How do you persist Redux state?
97. What state should not be persisted?
98. How do you clear persisted state on logout?
99. How do you debug Redux state changes?
100. What Redux Toolkit middleware and persistence best practices do you follow?

---

# Performance Optimization

101. How do you optimize Redux Toolkit performance?
102. What causes unnecessary re-renders in Redux applications?
103. How does `useSelector()` trigger re-renders?
104. What is `shallowEqual`?
105. When should you use memoized selectors?
106. What is `createSelector()`?
107. How does `createSelector()` improve performance?
108. What are derived selectors?
109. What is state normalization?
110. How does normalized state improve performance?

---

# Entity Adapter

111. What is `createEntityAdapter()`?
112. Why should you use `createEntityAdapter()`?
113. What problems does it solve?
114. How does `createEntityAdapter()` normalize state?
115. What methods does Entity Adapter provide?
116. How do you sort entities using Entity Adapter?
117. How do you update entities efficiently?
118. When should you avoid using Entity Adapter?
119. How does Entity Adapter compare to manually normalized state?
120. What Entity Adapter best practices do you follow?

---

# Large-Scale Architecture

121. How do you organize Redux Toolkit in a large project?
122. How do you organize slices by feature?
123. How do you avoid deeply nested Redux state?
124. What is code splitting in Redux?
125. What are dynamic reducers?
126. How do you lazy-load Redux slices?
127. How do you share state across multiple features?
128. How do you handle global state versus feature state?
129. What Redux architecture patterns have you used?
130. What project structure do you recommend for large Redux applications?

---

# Testing

131. How do you test Redux reducers?
132. How do you test Redux slices?
133. How do you test async thunks?
134. How do you mock API calls in Redux tests?
135. How do you test RTK Query endpoints?
136. How do you test selectors?
137. How do you test custom middleware?
138. How do you test Redux-connected React components?
139. What testing libraries do you use for Redux applications?
140. What Redux testing best practices do you follow?

---

# Senior Real-World Interview Questions

141. Describe the largest Redux Toolkit project you've worked on.
142. What was the most difficult Redux state management problem you've solved?
143. How do you debug Redux applications in production?
144. How do you review Redux-related pull requests?
145. What Redux coding standards do you enforce?
146. How would you migrate a legacy Redux application to Redux Toolkit?
147. How would you design state management for a large SaaS application?
148. What Redux Toolkit features do you use most frequently in production?
149. If you were starting a new React project today, how would you structure Redux Toolkit and RTK Query?
150. In your opinion, what separates a junior, mid-level, and senior Redux Toolkit developer?

---

# ANSWERS


---

## Part 1 (1â€“10): Redux Fundamentals

---

## Question 1: What is Redux?

## Answer:
Redux is a predictable state management library for JavaScript applications. It stores the entire application state in a single centralized store, making state changes predictable and debuggable.

```javascript
const store = createStore(reducer);
store.dispatch({ type: "INCREMENT" });
console.log(store.getState()); // { count: 1 }
```

## Key Points:
- Predictable state management.
- Single centralized store.
- Unidirectional data flow.
- Time-travel debugging.
- Works with any JavaScript framework.

## Interview Tip:
"Redux is predictable â€” every state change goes through a reducer, making changes traceable."

---

## Question 2: Why was Redux created?

## Answer:
Redux was created by Dan Abramov in 2015 to solve the challenges of managing state in large React applications. It was inspired by Flux and Elm, providing a predictable state container.

## Key Points:
- Created by Dan Abramov in 2015.
- Inspired by Flux and Elm.
- Solve complex state management.
- Predictable state changes.
- Time-travel debugging.

## Interview Tip:
"Redux was created because managing state in large React apps was chaotic â€” Redux makes it predictable."

---

## Question 3: What problems does Redux solve?

## Answer:
1. **Prop drilling**: Passing data through many components.
2. **State synchronization**: Keeping state consistent across components.
3. **Debugging**: Hard to trace state changes.
4. **Predictability**: Unpredictable state mutations.
5. **Shared state**: Multiple components need the same data.

## Key Points:
- Prop drilling.
- State synchronization.
- Debugging difficulty.
- Unpredictable mutations.
- Shared state management.

## Interview Tip:
"Redux solves the chaos of managing shared state across a large application."

---

## Question 4: What are the advantages of Redux?

## Answer:
- **Predictable**: State changes are traceable.
- **Centralized**: Single source of truth.
- **Debuggable**: Time-travel debugging with DevTools.
- **Maintainable**: Clear patterns for state changes.
- **Testable**: Pure functions (reducers) are easy to test.
- **Middleware**: Extensible with middleware.

## Key Points:
- Predictable state changes.
- Single source of truth.
- Time-travel debugging.
- Clear patterns.
- Easy to test.

## Interview Tip:
"Redux's biggest advantage is predictability â€” every state change is traceable."

---

## Question 5: What are the disadvantages of Redux?

## Answer:
- **Boilerplate**: Many files, actions, reducers.
- **Learning curve**: Concepts like reducers, actions, middleware.
- **Verbosity**: Simple operations require multiple steps.
- **Overkill**: Too much for simple applications.
- **Performance**: Can cause unnecessary re-renders.

## Key Points:
- Boilerplate code.
- Learning curve.
- Verbosity.
- Overkill for simple apps.
- Performance considerations.

## Interview Tip:
"Redux Toolkit was created to solve the boilerplate problem â€” it's much simpler."

---

## Question 6: What is Redux Toolkit?

## Answer:
Redux Toolkit (RTK) is the official, recommended way to write Redux logic. It simplifies store setup, reduces boilerplate, and includes best practices by default.

```javascript
import { createSlice, configureStore } from "@reduxjs/toolkit";

const counterSlice = createSlice({
  name: "counter",
  initialState: { value: 0 },
  reducers: {
    increment: (state) => { state.value += 1; }
  }
});

const store = configureStore({ reducer: { counter: counterSlice.reducer } });
```

## Key Points:
- Official Redux library.
- Simplified store setup.
- Reduced boilerplate.
- Includes best practices.
- Recommended for all Redux projects.

## Interview Tip:
"Redux Toolkit is the modern way to write Redux â€” it's simpler and includes best practices."

---

## Question 7: Why was Redux Toolkit introduced?

## Answer:
To solve Redux's main complaints:
- **Too much boilerplate**: Actions, reducers, constants.
- **Complex setup**: Store configuration.
- **Immutability by hand**: Spread operators everywhere.
- **Best practices**: Too many decisions to make.

RTK provides sensible defaults and simplifies everything.

## Key Points:
- Reduce boilerplate.
- Simplify setup.
- Handle immutability automatically.
- Include best practices.
- Make Redux easier.

## Interview Tip:
"Redux Toolkit was introduced because Redux had too much boilerplate â€” RTK simplifies everything."

---

## Question 8: How does Redux Toolkit differ from Redux?

## Answer:
| Feature | Redux | Redux Toolkit |
|---------|-------|---------------|
| Boilerplate | High | Low |
| Store setup | Manual | `configureStore()` |
| Reducers | Manual switch/case | `createSlice()` |
| Immutability | Manual spread | Immer built-in |
| Async | Manual thunks | `createAsyncThunk()` |

## Key Points:
- Less boilerplate.
- Simpler store setup.
- Automatic immutability (Immer).
- Built-in async handling.
- Official recommendation.

## Interview Tip:
"Redux Toolkit is Redux with batteries included â€” less boilerplate, more features."

---

## Question 9: When should you use Redux Toolkit?

## Answer:
- **Complex state**: Many interdependent values.
- **Shared state**: Multiple components need the same data.
- **Frequent updates**: Real-time data.
- **Large teams**: Need clear patterns.
- **Debugging**: Time-travel debugging needed.

## Key Points:
- Complex state management.
- Shared state across components.
- Frequent state updates.
- Large team collaboration.
- Debugging requirements.

## Interview Tip:
"Use Redux Toolkit when state is complex, shared, and frequently updated."

---

## Question 10: When should you avoid Redux?

## Answer:
- **Simple state**: useState is enough.
- **Local state**: Component-specific data.
- **Server state**: Use TanStack Query instead.
- **Small apps**: Context API is sufficient.
- **Infrequent updates**: No need for Redux overhead.

## Key Points:
- Simple state â†’ useState.
- Local state â†’ useState.
- Server state â†’ TanStack Query.
- Small apps â†’ Context API.
- Infrequent updates â†’ Context API.

## Interview Tip:
"Don't use Redux for everything â€” useState for local, Context for global, TanStack Query for server state."

---

## Part 2 (11â€“20): Core Concepts

---

## Question 11: What is a Store?

## Answer:
The store is the single centralized object that holds the entire application state. It's the single source of truth.

```javascript
const store = configureStore({
  reducer: {
    counter: counterReducer,
    users: usersReducer
  }
});
```

## Key Points:
- Single source of truth.
- Holds entire application state.
- Created with `configureStore()`.
- Provides `getState()`, `dispatch()`, `subscribe()`.
- One store per application.

## Interview Tip:
"The store is the single source of truth â€” one store holds all state."

---

## Question 12: What is the global state?

## Answer:
Global state is the application-wide state stored in the Redux store. It's accessible from any component connected to the store.

## Key Points:
- Application-wide state.
- Accessible from any component.
- Stored in Redux store.
- Managed by reducers.
- Single source of truth.

## Interview Tip:
"Global state is data shared across the entire application."

---

## Question 13: What is an Action?

## Answer:
An action is a plain JavaScript object that describes what happened. It must have a `type` property and optionally a `payload`.

```javascript
{ type: "counter/increment" }
{ type: "users/addUser", payload: { name: "Alice" } }
```

## Key Points:
- Plain JavaScript object.
- Must have `type` property.
- Optional `payload` for data.
- Describes what happened.
- Dispatched to trigger state changes.

## Interview Tip:
"Actions describe what happened â€” the reducer decides how state changes."

---

## Question 14: What is a Reducer?

## Answer:
A reducer is a pure function that takes current state and an action, returns new state.

```javascript
function counterReducer(state = { value: 0 }, action) {
  switch (action.type) {
    case "increment":
      return { value: state.value + 1 };
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

## Question 15: What is a Slice?

## Answer:
A slice is a collection of reducer logic and actions for a single feature. Created with `createSlice()`.

```javascript
const counterSlice = createSlice({
  name: "counter",
  initialState: { value: 0 },
  reducers: {
    increment: (state) => { state.value += 1; },
    decrement: (state) => { state.value -= 1; }
  }
});
```

## Key Points:
- Collection of reducer logic and actions.
- Created with `createSlice()`.
- Auto-generates actions.
- Uses Immer for immutability.
- One slice per feature.

## Interview Tip:
"Slices organize Redux logic by feature â€” one slice per feature."

---

## Question 16: What is `createSlice()`?

## Answer:
`createSlice()` creates a slice of Redux state with reducers and auto-generated actions.

```javascript
const usersSlice = createSlice({
  name: "users",
  initialState: [],
  reducers: {
    addUser: (state, action) => { state.push(action.payload); },
    removeUser: (state, action) => state.filter(u => u.id !== action.payload)
  }
});
```

## Key Points:
- Creates slice with reducers and actions.
- Auto-generates action creators.
- Uses Immer for immutability.
- Reducers can "mutate" state (Immer handles it).
- Returns `{ actions, reducer }`.

## Interview Tip:
"`createSlice()` auto-generates actions â€” no need to write action creators manually."

---

## Question 17: What is `configureStore()`?

## Answer:
`configureStore()` creates the Redux store with sensible defaults.

```javascript
const store = configureStore({
  reducer: {
    counter: counterSlice.reducer,
    users: usersSlice.reducer
  }
});
```

## Key Points:
- Creates Redux store.
- Includes Redux DevTools.
- Includes thunk middleware.
- Combines reducers automatically.
- Sensible defaults.

## Interview Tip:
"`configureStore()` is the modern way to create a store â€” it includes DevTools and middleware by default."

---

## Question 18: What is `createAction()`?

## Answer:
`createAction()` creates an action creator function.

```javascript
const increment = createAction("counter/increment");
increment(); // { type: "counter/increment" }
increment(5); // { type: "counter/increment", payload: 5 }
```

## Key Points:
- Creates action creator.
- Auto-generates type.
- Payload as argument.
- Used with `createReducer()`.
- `createSlice()` generates actions automatically.

## Interview Tip:
"`createSlice()` generates actions automatically â€” you rarely need `createAction()` directly."

---

## Question 19: What is `PayloadAction`?

## Answer:
`PayloadAction` is a TypeScript type for actions with a payload.

```typescript
reducers: {
  setUser: (state, action: PayloadAction<User>) => {
    state.user = action.payload;
  }
}
```

## Key Points:
- TypeScript type for actions.
- Includes `type` and `payload`.
- Generic type for payload.
- Used in `createSlice()` reducers.
- Type-safe actions.

## Interview Tip:
"`PayloadAction<User>` types the payload â€” it's essential for TypeScript Redux."

---

## Question 20: What is the Redux data flow?

## Answer:
1. **UI dispatches action**: `dispatch({ type: "increment" })`.
2. **Store calls reducer**: Reducer computes new state.
3. **Store updates state**: New state is saved.
4. **UI re-renders**: Components read new state.

```
UI â†’ dispatch(action) â†’ reducer(state, action) â†’ newState â†’ UI
```

## Key Points:
- Unidirectional data flow.
- UI dispatches actions.
- Reducers compute new state.
- Store saves new state.
- UI re-renders.

## Interview Tip:
"Redux data flow is unidirectional: dispatch â†’ reducer â†’ state â†’ UI."

---

## Part 3 (21â€“30): Store Configuration

---

## Question 21: How do you create a Redux Toolkit store?

## Answer:
```javascript
import { configureStore } from "@reduxjs/toolkit";
import counterReducer from "./counterSlice";
import usersReducer from "./usersSlice";

const store = configureStore({
  reducer: {
    counter: counterReducer,
    users: usersReducer
  }
});

export default store;
```

## Key Points:
- `configureStore()` from Redux Toolkit.
- Combine reducers in `reducer` object.
- Includes DevTools and middleware by default.
- Export the store.

## Interview Tip:
"`configureStore()` is the standard â€” it includes DevTools and middleware."

---

## Question 22: How do you add multiple reducers?

## Answer:
```javascript
const store = configureStore({
  reducer: {
    counter: counterSlice.reducer,
    users: usersSlice.reducer,
    auth: authSlice.reducer
  }
});
```

Each key in the `reducer` object becomes a slice of state.

## Key Points:
- Object of reducers.
- Each key = state slice.
- `combineReducers` is automatic.
- One reducer per feature.

## Interview Tip:
"Each key in the reducer object becomes a state slice â€” `state.counter`, `state.users`."

---

## Question 23: What is the root reducer?

## Answer:
The root reducer combines all slice reducers into a single reducer. Redux Toolkit does this automatically with `configureStore()`.

## Key Points:
- Combines all slice reducers.
- Created automatically by `configureStore()`.
- Single reducer for the store.
- Each slice handles its own state.

## Interview Tip:
"`configureStore()` combines reducers automatically â€” no need for `combineReducers`."

---

## Question 24: How do you organize slices in a large project?

## Answer:
Feature-based organization:
```
src/
  features/
    auth/
      authSlice.ts
    users/
      usersSlice.ts
    posts/
      postsSlice.ts
  store.ts
```

## Key Points:
- Feature-based organization.
- One slice per feature.
- Co-locate related logic.
- Central store configuration.
- Easy to navigate.

## Interview Tip:
"One slice per feature â€” co-locate related logic."

---

## Question 25: How do you configure middleware?

## Answer:
```javascript
const store = configureStore({
  reducer: rootReducer,
  middleware: (getDefaultMiddleware) =>
    getDefaultMiddleware().concat(customMiddleware)
});
```

## Key Points:
- `middleware` option in `configureStore()`.
- `getDefaultMiddleware()` for defaults.
- `.concat()` to add custom middleware.
- `.prepend()` to add before defaults.

## Interview Tip:
"Use `getDefaultMiddleware().concat()` to add custom middleware."

---

## Question 26: What middleware is included by default?

## Answer:
- **Redux Thunk**: For async logic.
- **Serializable Check**: Ensures state is serializable.
- **Immutable Check**: Ensures state isn't mutated.

## Key Points:
- Thunk for async logic.
- Serializable check for safety.
- Immutable check for correctness.
- Included by default in Redux Toolkit.

## Interview Tip:
"Redux Toolkit includes thunk, serializable check, and immutable check by default."

---

## Question 27: What is the Redux DevTools Extension?

## Answer:
Redux DevTools is a browser extension that provides:
- **State inspection**: View current state.
- **Action logging**: See all dispatched actions.
- **Time-travel debugging**: Go back to previous states.
- **Action replay**: Replay actions.

## Key Points:
- Browser extension.
- State inspection.
- Action logging.
- Time-travel debugging.
- Essential for Redux development.

## Interview Tip:
"Redux DevTools is essential â€” time-travel debugging is invaluable."

---

## Question 28: How do you enable Redux DevTools?

## Answer:
Redux Toolkit enables DevTools automatically in development:

```javascript
const store = configureStore({
  reducer: rootReducer
  // DevTools enabled by default in development
});
```

Disabled automatically in production.

## Key Points:
- Enabled by default in development.
- Disabled in production automatically.
- No configuration needed.
- Redux Toolkit handles it.

## Interview Tip:
"DevTools is enabled by default â€” no configuration needed."

---

## Question 29: How do you configure Redux Toolkit for production?

## Answer:
```javascript
const store = configureStore({
  reducer: rootReducer,
  middleware: (getDefaultMiddleware) =>
    getDefaultMiddleware({
      serializableCheck: false // If needed
    }),
  devTools: process.env.NODE_ENV !== "production"
});
```

## Key Points:
- Disable DevTools in production.
- Configure middleware as needed.
- Optimize for performance.
- Remove development-only checks.

## Interview Tip:
"Redux Toolkit handles production configuration automatically â€” DevTools are disabled."

---

## Question 30: What store configuration best practices do you follow?

## Answer:
1. **One store**: Single store per application.
2. **Feature-based slices**: One slice per feature.
3. **TypeScript**: Type the store and slices.
4. **DevTools**: Keep enabled in development.
5. **Middleware**: Use defaults unless needed.

## Key Points:
- Single store.
- Feature-based slices.
- TypeScript types.
- DevTools in development.
- Default middleware.

## Interview Tip:
"One store, feature-based slices, TypeScript â€” the Redux Toolkit essentials."

---

## Part 4 (31â€“40): React Integration

---

## Question 31: What is the React-Redux library?

## Answer:
React-Redux is the official library for connecting React components to the Redux store. It provides hooks like `useSelector` and `useDispatch`.

## Key Points:
- Official React-Redux binding.
- Hooks for store access.
- `useSelector` for reading state.
- `useDispatch` for dispatching actions.
- `Provider` for store injection.

## Interview Tip:
"React-Redux connects React components to the Redux store."

---

## Question 32: What is the `Provider` component?

## Answer:
`Provider` makes the Redux store available to all components in the tree.

```jsx
import { Provider } from "react-redux";
import store from "./store";

function App() {
  return (
    <Provider store={store}>
      <MyApp />
    </Provider>
  );
}
```

## Key Points:
- Makes store available to components.
- Wraps the application.
- Passes store as prop.
- Required for Redux hooks.
- One Provider per app.

## Interview Tip:
"Wrap your app with `Provider` to make the Redux store available."

---

## Question 33: Why is `Provider` required?

## Answer:
`Provider` uses React Context to make the store available to all components. Without it, `useSelector` and `useDispatch` can't access the store.

## Key Points:
- Uses React Context.
- Makes store accessible.
- Required for Redux hooks.
- Wraps the application.

## Interview Tip:
"Without `Provider`, Redux hooks can't access the store."

---

## Question 34: What is `useSelector()`?

## Answer:
`useSelector` reads data from the Redux store.

```jsx
import { useSelector } from "react-redux";

function Counter() {
  const count = useSelector((state) => state.counter.value);
  return <div>{count}</div>;
}
```

## Key Points:
- Reads data from store.
- Selector function as argument.
- Re-renders when selected data changes.
- Replaces `mapStateToProps`.

## Interview Tip:
"`useSelector` reads state â€” it re-renders when the selected data changes."

---

## Question 35: What is `useDispatch()`?

## Answer:
`useDispatch` returns the dispatch function for dispatching actions.

```jsx
import { useDispatch } from "react-redux";
import { increment } from "./counterSlice";

function Counter() {
  const dispatch = useDispatch();
  return <button onClick={() => dispatch(increment())}>+</button>;
}
```

## Key Points:
- Returns dispatch function.
- Dispatches actions.
- Replaces `mapDispatchToProps`.
- Use in components.

## Interview Tip:
"`useDispatch` returns the dispatch function â€” use it to dispatch actions."

---

## Question 36: How does `useSelector()` work?

## Answer:
`useSelector` subscribes to the store and re-renders the component when the selected value changes. It uses strict equality (`===`) by default.

## Key Points:
- Subscribes to store.
- Re-renders on selected value change.
- Strict equality by default.
- Selector function runs on every state change.

## Interview Tip:
"`useSelector` re-renders when the selected value changes â€” use specific selectors."

---

## Question 37: How do you prevent unnecessary re-renders with `useSelector()`?

## Answer:
1. **Select specific values**: Don't select entire objects.
2. **Use `shallowEqual`**: For object comparisons.
3. **Use memoized selectors**: `createSelector()`.
4. **Select primitives**: Numbers, strings, booleans.

```jsx
// Bad: selects entire object
const user = useSelector((state) => state.user);

// Good: selects specific value
const userName = useSelector((state) => state.user.name);
```

## Key Points:
- Select specific values.
- Use `shallowEqual` for objects.
- Memoized selectors.
- Prefer primitives.

## Interview Tip:
"Select specific values, not entire objects â€” it prevents unnecessary re-renders."

---

## Question 38: What is `shallowEqual`?

## Answer:
`shallowEqual` compares objects by their properties (shallow comparison) instead of reference equality.

```jsx
import { shallowEqual } from "react-redux";

const user = useSelector(
  (state) => ({ name: state.user.name, email: state.user.email }),
  shallowEqual
);
```

## Key Points:
- Shallow comparison of objects.
- Prevents re-renders when properties are same.
- Use when selecting objects.
- Import from `react-redux`.

## Interview Tip:
"Use `shallowEqual` when selecting objects â€” it prevents re-renders when properties don't change."

---

## Question 39: What are typed Redux hooks?

## Answer:
Typed hooks are pre-configured `useSelector` and `useDispatch` with TypeScript types.

```typescript
// store.ts
export type RootState = ReturnType<typeof store.getState>;
export type AppDispatch = typeof store.dispatch;

// hooks.ts
export const useAppSelector = useSelector.withTypes<RootState>();
export const useAppDispatch = useDispatch.withTypes<AppDispatch>();
```

## Key Points:
- Pre-configured with types.
- Type-safe state access.
- Type-safe dispatch.
- Use throughout the app.

## Interview Tip:
"Typed hooks provide type safety â€” use them throughout your app."

---

## Question 40: How do you create custom typed hooks in TypeScript?

## Answer:
```typescript
// hooks.ts
import { useSelector, useDispatch } from "react-redux";
import type { RootState, AppDispatch } from "./store";

export const useAppSelector = useSelector.withTypes<RootState>();
export const useAppDispatch = useDispatch.withTypes<AppDispatch>();
```

## Key Points:
- Create typed versions of hooks.
- Export for use throughout app.
- Type-safe state and dispatch.
- Centralized hook definitions.

## Interview Tip:
"Create typed hooks once, use them everywhere â€” it's the TypeScript Redux pattern."

---

## Part 5 (41â€“50): State Management

---

## Question 41: What data should be stored in Redux?

## Answer:
- **Shared state**: Data used by multiple components.
- **Global state**: Application-wide data.
- **Complex state**: Many interdependent values.
- **Persistent state**: Data that survives navigation.

## Key Points:
- Shared across components.
- Application-wide data.
- Complex state logic.
- Persistent data.

## Interview Tip:
"Redux is for shared, global, complex state â€” not for component-local data."

---

## Question 42: What data should remain in local component state?

## Answer:
- **Form inputs**: Input values.
- **UI toggles**: Modals, dropdowns.
- **Component-specific**: Data only this component uses.
- **Temporary data**: Loading states, errors.

## Key Points:
- Form inputs.
- UI toggles.
- Component-specific data.
- Temporary data.

## Interview Tip:
"If only one component uses the data, keep it local with useState."

---

## Question 43: What is normalized state?

## Answer:
Normalized state stores entities by ID in a flat structure, like a database table.

```javascript
// Normalized
{
  users: {
    byId: {
      1: { id: 1, name: "Alice" },
      2: { id: 2, name: "Bob" }
    },
    allIds: [1, 2]
  }
}
```

## Key Points:
- Flat structure.
- Entities by ID.
- No duplication.
- Easy to update.
- Like a database table.

## Interview Tip:
"Normalized state is like a database â€” entities by ID, no duplication."

---

## Question 44: Why is normalized state important?

## Answer:
- **No duplication**: Single source per entity.
- **Easy updates**: Update one place.
- **Performance**: Efficient lookups.
- **Consistency**: No stale data.

## Key Points:
- No data duplication.
- Easy to update.
- Fast lookups.
- Consistent data.

## Interview Tip:
"Normalized state prevents duplication â€” update once, reflect everywhere."

---

## Question 45: What is immutable state?

## Answer:
Immutable state means state is never mutated directly. Instead, new state objects are created with the changes.

```javascript
// Wrong: mutation
state.value = 5;

// Correct: new object
return { ...state, value: 5 };
```

## Key Points:
- Never mutate state directly.
- Create new objects.
- Redux requires immutability.
- Immer handles this in Redux Toolkit.

## Interview Tip:
"Redux requires immutable updates â€” Redux Toolkit's Immer handles this automatically."

---

## Question 46: How does Redux Toolkit handle immutable updates?

## Answer:
Redux Toolkit uses Immer internally, allowing you to write "mutating" code that actually creates immutable updates.

```javascript
reducers: {
  increment: (state) => {
    state.value += 1; // Looks like mutation, but Immer makes it immutable
  }
}
```

## Key Points:
- Uses Immer internally.
- Write "mutating" code.
- Immer creates immutable updates.
- Simpler than spread operators.
- Safe by default.

## Interview Tip:
"Redux Toolkit uses Immer â€” you can write `state.value += 1` and it's immutable."

---

## Question 47: What is Immer?

## Answer:
Immer is a library that simplifies immutable state updates. It lets you write code that appears to mutate state, but actually creates a new immutable copy.

## Key Points:
- Simplifies immutable updates.
- "Mutating" syntax.
- Creates immutable copies.
- Built into Redux Toolkit.
- Proxy-based.

## Interview Tip:
"Immer lets you write `state.value = 5` instead of `return { ...state, value: 5 }`."

---

## Question 48: How does Immer simplify reducer logic?

## Answer:
```javascript
// Without Immer (verbose)
reducers: {
  addUser: (state, action) => {
    return [...state, action.payload];
  }
}

// With Immer (simpler)
reducers: {
  addUser: (state, action) => {
    state.push(action.payload); // Looks like mutation
  }
}
```

## Key Points:
- Write "mutating" code.
- Immer handles immutability.
- Simpler reducer logic.
- Less boilerplate.
- Built into Redux Toolkit.

## Interview Tip:
"Immer makes reducers much simpler â€” write `state.push()` instead of spread operators."

---

## Question 49: What common Redux mistakes should be avoided?

## Answer:
1. **Mutating state directly**: Outside of Immer.
2. **Storing non-serializable data**: Functions, class instances.
3. **Overusing Redux**: For simple state.
4. **Selecting entire objects**: Causes unnecessary re-renders.
5. **No TypeScript**: Missing type safety.

## Key Points:
- Don't mutate outside reducers.
- Keep state serializable.
- Use local state for simple data.
- Select specific values.
- Use TypeScript.

## Interview Tip:
"The biggest mistake is overusing Redux â€” use local state for component-specific data."

---

## Question 50: What Redux Toolkit best practices do you follow?

## Answer:
1. **One slice per feature**: Organize by feature.
2. **TypeScript**: Type everything.
3. **Normalized state**: For collections.
4. **Memoized selectors**: For derived data.
5. **RTK Query**: For server state.
6. **Local state**: For component-specific data.

## Key Points:
- Feature-based slices.
- TypeScript types.
- Normalized state.
- Memoized selectors.
- RTK Query for server state.

## Interview Tip:
"One slice per feature, TypeScript, normalized state â€” the Redux Toolkit best practices."

---

## Part 6 (51â€“60): Async Logic

---

## Question 51: What is asynchronous logic in Redux?

## Answer:
Async logic includes API calls, timers, and other operations that don't complete immediately. Redux handles this with middleware like thunks.

## Key Points:
- API calls.
- Timers.
- Non-immediate operations.
- Handled by middleware.
- Thunks are the standard.

## Interview Tip:
"Async logic in Redux is handled by middleware â€” thunks are the standard."

---

## Question 52: Why can't reducers contain asynchronous code?

## Answer:
Reducers must be pure functions â€” same input always produces same output. Async operations are non-deterministic (network delays, failures), making reducers impure.

## Key Points:
- Reducers must be pure.
- Async is non-deterministic.
- Side effects belong in middleware.
- Thunks handle async logic.

## Interview Tip:
"Reducers are pure functions â€” async logic belongs in thunks."

---

## Question 53: What is `createAsyncThunk()`?

## Answer:
`createAsyncThunk()` creates async action creators for API calls and other async operations.

```javascript
const fetchUsers = createAsyncThunk("users/fetch", async () => {
  const response = await fetch("/api/users");
  return response.json();
});
```

## Key Points:
- Creates async action creators.
- Handles pending, fulfilled, rejected states.
- Auto-generates action types.
- Returns a promise.
- Built into Redux Toolkit.

## Interview Tip:
"`createAsyncThunk()` handles the entire async lifecycle â€” pending, fulfilled, rejected."

---

## Question 54: How does `createAsyncThunk()` work?

## Answer:
1. **Dispatch pending**: When async operation starts.
2. **Execute payload creator**: The async function.
3. **Dispatch fulfilled**: When operation succeeds.
4. **Dispatch rejected**: When operation fails.

## Key Points:
- Dispatches pending action.
- Executes async function.
- Dispatches fulfilled on success.
- Dispatches rejected on failure.
- Auto-generates action types.

## Interview Tip:
"`createAsyncThunk()` handles the full lifecycle â€” pending â†’ fulfilled/rejected."

---

## Question 55: What arguments does `createAsyncThunk()` receive?

## Answer:
```javascript
const fetchUser = createAsyncThunk(
  "users/fetch",           // Action type prefix
  async (userId, thunkAPI) => { // Payload creator
    const response = await fetch(`/api/users/${userId}`);
    return response.json();
  }
);
```

First argument: action type prefix. Second: async payload creator.

## Key Points:
- Action type prefix.
- Async payload creator.
- `thunkAPI` for extra utilities.
- Returns the result.

## Interview Tip:
"`thunkAPI` provides `rejectWithValue`, `dispatch`, `getState` â€” useful for error handling."

---

## Question 56: What are the `pending`, `fulfilled`, and `rejected` action states?

## Answer:
- **Pending**: Async operation started.
- **Fulfilled**: Operation succeeded.
- **Rejected**: Operation failed.

```javascript
extraReducers: (builder) => {
  builder
    .addCase(fetchUsers.pending, (state) => { state.loading = true; })
    .addCase(fetchUsers.fulfilled, (state, action) => { state.users = action.payload; })
    .addCase(fetchUsers.rejected, (state, action) => { state.error = action.error.message; })
}
```

## Key Points:
- Pending: loading state.
- Fulfilled: success with data.
- Rejected: error state.
- Handle all three in extraReducers.

## Interview Tip:
"Handle all three states â€” pending for loading, fulfilled for data, rejected for errors."

---

## Question 57: How do you handle loading states?

## Answer:
```javascript
const usersSlice = createSlice({
  name: "users",
  initialState: { users: [], loading: false, error: null },
  extraReducers: (builder) => {
    builder
      .addCase(fetchUsers.pending, (state) => {
        state.loading = true;
        state.error = null;
      })
      .addCase(fetchUsers.fulfilled, (state, action) => {
        state.loading = false;
        state.users = action.payload;
      })
      .addCase(fetchUsers.rejected, (state, action) => {
        state.loading = false;
        state.error = action.error.message;
      });
  }
});
```

## Key Points:
- `loading: true` on pending.
- `loading: false` on fulfilled/rejected.
- Display loading indicator in UI.
- Clear errors on new request.

## Interview Tip:
"Set loading on pending, clear on fulfilled/rejected â€” the standard loading pattern."

---

## Question 58: How do you handle error states?

## Answer:
```javascript
.addCase(fetchUsers.rejected, (state, action) => {
  state.loading = false;
  state.error = action.error.message;
})
```

Use `rejectWithValue` for custom error messages:
```javascript
const fetchUsers = createAsyncThunk(
  "users/fetch",
  async (_, thunkAPI) => {
    try {
      const response = await fetch("/api/users");
      if (!response.ok) throw new Error("Failed");
      return response.json();
    } catch (err) {
      return thunkAPI.rejectWithValue(err.message);
    }
  }
);
```

## Key Points:
- Handle rejected state.
- `action.error.message` for errors.
- `rejectWithValue` for custom errors.
- Display errors in UI.

## Interview Tip:
"Use `rejectWithValue` for custom error messages â€” it's cleaner than `action.error.message`."

---

## Question 59: How do you cancel an async thunk?

## Answer:
```javascript
const fetchUsers = createAsyncThunk(
  "users/fetch",
  async (_, { signal }) => {
    const response = await fetch("/api/users", { signal });
    return response.json();
  }
);

// Cancel
dispatch(fetchUsers()).abort();
```

## Key Points:
- `signal` from thunkAPI.
- Pass to fetch `signal` option.
- `.abort()` to cancel.
- Handle AbortError.

## Interview Tip:
"Use `signal` from thunkAPI to cancel async thunks â€” pass it to fetch."

---

## Question 60: What are common mistakes when using async thunks?

## Answer:
1. **Not handling all states**: Missing pending/rejected.
2. **Not using `rejectWithValue`**: Generic errors.
3. **Mutating state outside reducers**: In payload creators.
4. **Not canceling on unmount**: Memory leaks.
5. **Storing non-serializable data**: Functions in state.

## Key Points:
- Handle all three states.
- Use `rejectWithValue`.
- Don't mutate in payload creators.
- Cancel on unmount.
- Keep state serializable.

## Interview Tip:
"Handle all three states â€” pending, fulfilled, rejected â€” don't skip any."

---

## Part 7 (61â€“70): Extra Reducers

---

## Question 61: What are `extraReducers`?

## Answer:
`extraReducers` handle actions defined outside the slice (like async thunks or actions from other slices).

```javascript
const usersSlice = createSlice({
  name: "users",
  initialState: [],
  reducers: {},
  extraReducers: (builder) => {
    builder.addCase(fetchUsers.fulfilled, (state, action) => {
      return action.payload;
    });
  }
});
```

## Key Points:
- Handle external actions.
- Async thunk actions.
- Actions from other slices.
- Builder callback syntax.
- Don't generate action creators.

## Interview Tip:
"`extraReducers` handle actions from outside the slice â€” async thunks and cross-slice actions."

---

## Question 62: How do `reducers` differ from `extraReducers`?

## Answer:
| Feature | reducers | extraReducers |
|---------|----------|---------------|
| Actions | Generated by slice | External actions |
| Action creators | Auto-generated | Not generated |
| Use case | Slice-specific | Cross-slice, async |

## Key Points:
- `reducers`: slice-specific, auto-generates actions.
- `extraReducers`: external actions, no auto-generation.
- Use `reducers` for synchronous slice logic.
- Use `extraReducers` for async and cross-slice.

## Interview Tip:
"`reducers` for slice actions; `extraReducers` for external actions."

---

## Question 63: When should you use `extraReducers`?

## Answer:
- **Async thunks**: Handle pending/fulfilled/rejected.
- **Cross-slice actions**: Respond to other slices' actions.
- **External actions**: Actions from outside the app.

## Key Points:
- Async thunk states.
- Cross-slice communication.
- External action handling.

## Interview Tip:
"Use `extraReducers` for async thunks and cross-slice actions."

---

## Question 64: How do you handle async thunk actions in `extraReducers`?

## Answer:
```javascript
extraReducers: (builder) => {
  builder
    .addCase(fetchUsers.pending, (state) => {
      state.loading = true;
    })
    .addCase(fetchUsers.fulfilled, (state, action) => {
      state.loading = false;
      state.users = action.payload;
    })
    .addCase(fetchUsers.rejected, (state, action) => {
      state.loading = false;
      state.error = action.error.message;
    });
}
```

## Key Points:
- `addCase` for each state.
- Pending, fulfilled, rejected.
- Update state accordingly.
- Builder callback syntax.

## Interview Tip:
"Handle all three states in `extraReducers` â€” pending, fulfilled, rejected."

---

## Question 65: What is the builder callback syntax?

## Answer:
```javascript
extraReducers: (builder) => {
  builder
    .addCase(actionCreator, (state, action) => { /* ... */ })
    .addCase(anotherAction, (state, action) => { /* ... */ });
}
```

## Key Points:
- Type-safe syntax.
- Chain `addCase` calls.
- Recommended by Redux Toolkit.
- Better than object notation.

## Interview Tip:
"Builder callback syntax is type-safe and recommended â€” use it always."

---

## Question 66: Why is the builder pattern preferred?

## Answer:
- **Type-safe**: TypeScript inference works correctly.
- **Explicit**: Clear which actions are handled.
- **Chainable**: Clean syntax.
- **Recommended**: Official Redux Toolkit recommendation.

## Key Points:
- Type-safe.
- Explicit and clear.
- Chainable syntax.
- Official recommendation.

## Interview Tip:
"Builder pattern is type-safe â€” always use it with TypeScript."

---

## Question 67: How do you share actions between slices?

## Answer:
Export the action creator and use it in another slice's `extraReducers`:

```javascript
// authSlice.js
export const logout = createAction("auth/logout");

// usersSlice.js
import { logout } from "./authSlice";

extraReducers: (builder) => {
  builder.addCase(logout, (state) => {
    return initialState; // Reset state
  });
}
```

## Key Points:
- Export action creators.
- Import in other slices.
- Use in `extraReducers`.
- Cross-slice communication.

## Interview Tip:
"Export actions and import them in other slices for cross-slice communication."

---

## Question 68: How do you reset state from another slice?

## Answer:
```javascript
// Listen for logout action
extraReducers: (builder) => {
  builder.addCase(logout, () => {
    return initialState; // Reset to initial state
  });
}
```

## Key Points:
- Listen for global actions.
- Return `initialState` to reset.
- Handle in each slice that needs resetting.
- Common for logout.

## Interview Tip:
"Return `initialState` to reset a slice â€” listen for logout in all relevant slices."

---

## Question 69: How do you handle global logout actions?

## Answer:
1. **Create a global logout action**: `createAction("auth/logout")`.
2. **Dispatch on logout**: Clear auth state.
3. **Listen in all slices**: Reset state in each slice.

```javascript
// Each slice listens for logout
extraReducers: (builder) => {
  builder.addCase(logout, () => initialState);
}
```

## Key Points:
- Global logout action.
- Each slice resets on logout.
- Clear all sensitive data.
- Return initial state.

## Interview Tip:
"Every slice with sensitive data should listen for logout and reset."

---

## Question 70: What are common `extraReducers` best practices?

## Answer:
1. **Builder syntax**: Always use builder callback.
2. **Handle all states**: Pending, fulfilled, rejected.
3. **Type actions**: Use TypeScript for type safety.
4. **Reset on logout**: Listen for global actions.
5. **Keep reducers pure**: No side effects.

## Key Points:
- Builder syntax.
- All states handled.
- TypeScript types.
- Reset on logout.
- Pure reducers.

## Interview Tip:
"Builder syntax, handle all states, type everything â€” the `extraReducers` best practices."

---

## Part 8 (71â€“80): RTK Query

---

## Question 71: What is RTK Query?

## Answer:
RTK Query is a data fetching and caching solution built into Redux Toolkit. It eliminates the need to write data fetching logic manually.

```javascript
import { createApi, fetchBaseQuery } from "@reduxjs/toolkit/query/react";

const apiSlice = createApi({
  reducerPath: "api",
  baseQuery: fetchBaseQuery({ baseUrl: "/api" }),
  endpoints: (builder) => ({
    getUsers: builder.query({ query: () => "/users" })
  })
});
```

## Key Points:
- Data fetching and caching.
- Built into Redux Toolkit.
- Auto-generated hooks.
- Automatic caching.
- Eliminates manual fetching logic.

## Interview Tip:
"RTK Query eliminates manual data fetching â€” it handles caching, loading, and errors automatically."

---

## Question 72: Why was RTK Query introduced?

## Answer:
To eliminate the need for:
- **Manual async thunks**: For every API call.
- **Loading states**: Manual loading/error management.
- **Caching**: Manual cache logic.
- **Data synchronization**: Keeping data fresh.

RTK Query automates all of this.

## Key Points:
- Eliminate manual thunks.
- Automatic loading states.
- Built-in caching.
- Data synchronization.
- Less boilerplate.

## Interview Tip:
"RTK Query eliminates the boilerplate of manual data fetching."

---

## Question 73: How does RTK Query differ from `createAsyncThunk()`?

## Answer:
| Feature | createAsyncThunk | RTK Query |
|---------|-----------------|-----------|
| Caching | Manual | Automatic |
| Loading states | Manual | Automatic |
| Refetching | Manual | Automatic |
| Code | More boilerplate | Less boilerplate |
| Use case | Custom async logic | Data fetching |

## Key Points:
- RTK Query: automatic caching and loading.
- createAsyncThunk: manual everything.
- RTK Query for data fetching.
- createAsyncThunk for custom async logic.

## Interview Tip:
"RTK Query for data fetching; createAsyncThunk for custom async logic."

---

## Question 74: When should you use RTK Query?

## Answer:
- **API data fetching**: Standard CRUD operations.
- **Caching needed**: Automatic cache management.
- **Loading states**: Automatic loading/error handling.
- **Data synchronization**: Keep data fresh.

## Key Points:
- Standard API fetching.
- Automatic caching.
- Loading states.
- Data synchronization.

## Interview Tip:
"Use RTK Query for all API data fetching â€” it handles everything automatically."

---

## Question 75: What is `createApi()`?

## Answer:
`createApi()` defines an API slice with endpoints and configuration.

```javascript
const apiSlice = createApi({
  reducerPath: "api",
  baseQuery: fetchBaseQuery({ baseUrl: "/api" }),
  endpoints: (builder) => ({
    getUsers: builder.query({ query: () => "/users" }),
    addUser: builder.mutation({ query: (user) => ({ url: "/users", method: "POST", body: user }) })
  })
});
```

## Key Points:
- Defines API slice.
- Configures base URL.
- Defines endpoints.
- Returns hooks.
- Auto-generates reducer.

## Interview Tip:
"`createApi()` is the entry point â€” define your API, endpoints, and configuration."

---

## Question 76: What is `fetchBaseQuery()`?

## Answer:
`fetchBaseQuery()` is a wrapper around `fetch` that simplifies API calls.

```javascript
const baseQuery = fetchBaseQuery({
  baseUrl: "/api",
  prepareHeaders: (headers) => {
    headers.set("Authorization", `Bearer ${token}`);
    return headers;
  }
});
```

## Key Points:
- Wrapper around `fetch`.
- Configures base URL.
- Add headers (auth).
- Returns a base query function.
- Used in `createApi()`.

## Interview Tip:
"`fetchBaseQuery()` configures the base URL and headers â€” use it for all API calls."

---

## Question 77: How do you define endpoints?

## Answer:
```javascript
endpoints: (builder) => ({
  // Query (read)
  getUsers: builder.query({ query: () => "/users" }),
  getUser: builder.query({ query: (id) => `/users/${id}` }),
  
  // Mutation (write)
  addUser: builder.mutation({
    query: (user) => ({ url: "/users", method: "POST", body: user })
  })
})
```

## Key Points:
- `builder.query` for reads.
- `builder.mutation` for writes.
- `query` function returns URL or config.
- Auto-generates hooks.

## Interview Tip:
"`query` for reads, `mutation` for writes â€” RTK Query generates hooks for both."

---

## Question 78: What is the difference between `query` and `mutation`?

## Answer:
- **Query**: Read data (GET). Cached automatically.
- **Mutation**: Write data (POST, PUT, DELETE). Not cached.

## Key Points:
- Query: read, cached.
- Mutation: write, not cached.
- Queries have auto-generated hooks.
- Mutations can invalidate cache.

## Interview Tip:
"Queries read and cache; mutations write and invalidate."

---

## Question 79: How do generated hooks work?

## Answer:
RTK Query auto-generates hooks for each endpoint:

```javascript
// Auto-generated hooks
const { data, error, isLoading } = useGetUsersQuery();
const [addUser] = useAddUserMutation();
```

## Key Points:
- Auto-generated from endpoints.
- `useQuery` hooks for queries.
- `useMutation` hooks for mutations.
- Return data, loading, error.
- Type-safe.

## Interview Tip:
"RTK Query generates hooks automatically â€” `useGetUsersQuery()`, `useAddUserMutation()`."

---

## Question 80: What are tags in RTK Query?

## Answer:
Tags are cache labels used for cache invalidation.

```javascript
endpoints: (builder) => ({
  getUsers: builder.query({
    query: () => "/users",
    providesTags: ["Users"]
  }),
  addUser: builder.mutation({
    query: (user) => ({ url: "/users", method: "POST", body: user }),
    invalidatesTags: ["Users"]
  })
})
```

## Key Points:
- Cache labels.
- `providesTags`: endpoint provides tags.
- `invalidatesTags`: mutation invalidates tags.
- Auto-refetch on invalidation.
- Keep data fresh.

## Interview Tip:
"Tags connect queries and mutations â€” when a mutation invalidates a tag, related queries refetch."

---

## Part 9 (81â€“90): Caching & Data Fetching

---

## Question 81: How does RTK Query cache data?

## Answer:
RTK Query caches query results automatically. When the same query is made again, it returns cached data instead of fetching.

## Key Points:
- Automatic caching.
- Cache by query arguments.
- Returns cached data on repeat queries.
- Configurable cache duration.
- Shared across components.

## Interview Tip:
"RTK Query caches automatically â€” no manual cache management needed."

---

## Question 82: What is cache invalidation?

## Answer:
Cache invalidation marks cached data as stale, triggering a refetch when the data is needed again.

## Key Points:
- Mark data as stale.
- Trigger refetch.
- Keep data fresh.
- Based on tags.

## Interview Tip:
"Cache invalidation keeps data fresh â€” when data changes, invalidate the cache."

---

## Question 83: How do you invalidate cached data?

## Answer:
Use `invalidatesTags` in mutations:

```javascript
addUser: builder.mutation({
  query: (user) => ({ url: "/users", method: "POST", body: user }),
  invalidatesTags: ["Users"] // Invalidates all "Users" queries
})
```

## Key Points:
- `invalidatesTags` in mutations.
- Specify tags to invalidate.
- Triggers refetch of related queries.
- Keep data fresh.

## Interview Tip:
"When a mutation changes data, invalidate the related tags â€” queries refetch automatically."

---

## Question 84: What are `providesTags`?

## Answer:
`providesTags` labels a query's cached data with tags. Other endpoints can invalidate these tags.

```javascript
getUsers: builder.query({
  query: () => "/users",
  providesTags: ["Users"]
})
```

## Key Points:
- Labels cached data.
- Used for invalidation.
- Connects queries to mutations.
- Can be dynamic.

## Interview Tip:
"`providesTags` labels the cache; `invalidatesTags` clears it."

---

## Question 85: What are `invalidatesTags`?

## Answer:
`invalidatesTags` specifies which tags a mutation invalidates, triggering refetches.

```javascript
deleteUser: builder.mutation({
  query: (id) => ({ url: `/users/${id}`, method: "DELETE" }),
  invalidatesTags: ["Users"]
})
```

## Key Points:
- Specifies tags to invalidate.
- Triggers refetch of related queries.
- Used in mutations.
- Keeps data fresh.

## Interview Tip:
"`invalidatesTags` in mutations triggers refetches of related queries."

---

## Question 86: How do you refetch cached data?

## Answer:
```javascript
const { data, refetch } = useGetUsersQuery();

// Manual refetch
<button onClick={refetch}>Refresh</button>
```

## Key Points:
- `refetch` function from query hook.
- Manual refetch on demand.
- Automatic refetch via tag invalidation.
- Polling for automatic updates.

## Interview Tip:
"`refetch()` for manual refresh; tag invalidation for automatic refresh."

---

## Question 87: How do polling and automatic refetching work?

## Answer:
```javascript
const { data } = useGetUsersQuery(undefined, {
  pollingInterval: 30000 // Refetch every 30 seconds
});
```

## Key Points:
- `pollingInterval` option.
- Refetch at regular intervals.
- Keep data fresh automatically.
- Configurable interval.

## Interview Tip:
"Polling for real-time-ish data â€” `pollingInterval: 30000` for every 30 seconds."

---

## Question 88: How do you perform optimistic updates?

## Answer:
```javascript
addUser: builder.mutation({
  query: (user) => ({ url: "/users", method: "POST", body: user }),
  onQueryStarted: async (user, { dispatch, queryFulfilled }) => {
    // Optimistically update cache
    const patchResult = dispatch(
      apiSlice.util.updateQueryData("getUsers", undefined, (draft) => {
        draft.push(user);
      })
    );
    try {
      await queryFulfilled;
    } catch {
      patchResult.undo(); // Rollback on error
    }
  }
})
```

## Key Points:
- Update cache before server responds.
- Rollback on error.
- `updateQueryData` for cache manipulation.
- Better UX.

## Interview Tip:
"Optimistic updates improve UX â€” update cache immediately, rollback on error."

---

## Question 89: How do you prefetch data?

## Answer:
```javascript
const prefetchUsers = apiSlice.usePrefetch("getUsers");

<Link onMouseEnter={() => prefetchUsers()}>Users</Link>
```

## Key Points:
- `usePrefetch` hook.
- Prefetch on hover or interaction.
- Cache data before needed.
- Better perceived performance.

## Interview Tip:
"Prefetch on hover â€” data is ready before the user clicks."

---

## Question 90: What RTK Query best practices do you follow?

## Answer:
1. **Tags for invalidation**: Use tags for cache management.
2. **Polling for real-time**: Use pollingInterval for live data.
3. **Optimistic updates**: For better UX.
4. **Prefetching**: Prefetch on hover.
5. **Error handling**: Handle errors in components.

## Key Points:
- Tags for invalidation.
- Polling for live data.
- Optimistic updates.
- Prefetching.
- Error handling.

## Interview Tip:
"Tags, polling, optimistic updates, prefetching â€” the RTK Query essentials."

---

## Part 10 (91â€“100): Middleware & Persistence

---

## Question 91: What is middleware in Redux Toolkit?

## Answer:
Middleware intercepts actions before they reach the reducer, enabling side effects like logging, async operations, and analytics.

## Key Points:
- Intercepts actions.
- Before reducer.
- Side effects.
- Logging, async, analytics.
- Extensible.

## Interview Tip:
"Middleware intercepts actions â€” it's where side effects happen."

---

## Question 92: What middleware is included by default?

## Answer:
- **Redux Thunk**: Async logic.
- **Serializable Check**: Ensures state is serializable.
- **Immutable Check**: Ensures state isn't mutated.

## Key Points:
- Thunk for async.
- Serializable check.
- Immutable check.
- Included by default.

## Interview Tip:
"Redux Toolkit includes thunk, serializable check, and immutable check by default."

---

## Question 93: What is Redux Thunk middleware?

## Answer:
Thunk middleware lets you write action creators that return functions instead of plain objects. These functions can perform async operations.

```javascript
const fetchUsers = () => async (dispatch) => {
  dispatch({ type: "users/loading" });
  const users = await fetch("/api/users");
  dispatch({ type: "users/loaded", payload: users });
};
```

## Key Points:
- Action creators return functions.
- Functions can be async.
- Access to dispatch and getState.
- Standard for async logic.
- Included in Redux Toolkit.

## Interview Tip:
"Thunks are functions that return functions â€” they handle async logic."

---

## Question 94: How do you create custom middleware?

## Answer:
```javascript
const loggerMiddleware = (store) => (next) => (action) => {
  console.log("Dispatching:", action);
  const result = next(action);
  console.log("Next state:", store.getState());
  return result;
};

const store = configureStore({
  reducer: rootReducer,
  middleware: (getDefaultMiddleware) =>
    getDefaultMiddleware().concat(loggerMiddleware)
});
```

## Key Points:
- Three-level function: store â†’ next â†’ action.
- Call `next(action)` to proceed.
- Access store with `store.getState()`.
- Add to middleware array.

## Interview Tip:
"Custom middleware: store â†’ next â†’ action. Call `next(action)` to proceed."

---

## Question 91: What is middleware in Redux Toolkit?

## Answer:
Middleware intercepts actions between dispatch and reducer. It's used for side effects like logging, async operations, and analytics.

## Key Points:
- Intercepts actions.
- Between dispatch and reducer.
- For side effects.
- Logging, async, analytics.

## Interview Tip:
"Middleware intercepts actions â€” use it for logging, async, and analytics."

---

## Question 92: What middleware is included by default?

## Answer:
- **Thunk**: Async logic.
- **Serializable check**: Ensures state is serializable.
- **Immutable check**: Ensures state isn't mutated.

## Key Points:
- Thunk for async.
- Serializable check.
- Immutable check.
- Included by default.

## Interview Tip:
"Redux Toolkit includes thunk, serializable check, and immutable check by default."

---

## Question 93: What is Redux Thunk middleware?

## Answer:
Thunk middleware allows you to write action creators that return functions instead of plain objects. These functions can perform async operations.

```javascript
const fetchUsers = () => async (dispatch) => {
  dispatch({ type: "users/loading" });
  const users = await fetch("/api/users").then(r => r.json());
  dispatch({ type: "users/loaded", payload: users });
};
```

## Key Points:
- Action creators return functions.
- Functions can be async.
- Access to dispatch and getState.
- Handles side effects.
- Built into Redux Toolkit.

## Interview Tip:
"Thunks let you write async action creators â€” they're the standard for async Redux."

---

## Question 94: How do you create custom middleware?

## Answer:
```javascript
const analyticsMiddleware = (store) => (next) => (action) => {
  if (action.type.includes("fulfilled")) {
    trackEvent(action.type);
  }
  return next(action);
};
```

## Key Points:
- Three-level function.
- Track actions.
- Access store state.
- Call `next(action)`.
- Add to middleware array.

## Interview Tip:
"Custom middleware for logging, analytics, or error tracking."

---

## Question 95: What is `redux-persist`?

## Answer:
`redux-persist` persists Redux state to storage (localStorage, sessionStorage) so it survives page refreshes.

```javascript
import { persistStore, persistReducer } from "redux-persist";
import storage from "redux-persist/lib/storage";

const persistConfig = { key: "root", storage };
const persistedReducer = persistReducer(persistConfig, rootReducer);
```

## Key Points:
- Persists Redux state.
- Survives page refresh.
- Configurable storage.
- Whitelist/blacklist options.

## Interview Tip:
"`redux-persist` keeps state across page refreshes â€” use it for user preferences."

---

## Question 96: How do you persist Redux state?

## Answer:
```javascript
import { persistStore, persistReducer } from "redux-persist";
import storage from "redux-persist/lib/storage";

const persistConfig = {
  key: "root",
  storage,
  whitelist: ["auth", "preferences"] // Only persist these
};

const persistedReducer = persistReducer(persistConfig, rootReducer);
const store = configureStore({ reducer: persistedReducer });
const persistor = persistStore(store);
```

## Key Points:
- `persistReducer` wraps the root reducer.
- `persistStore` creates the persistor.
- `whitelist`/`blacklist` for selective persistence.
- Use with `PersistGate` in React.

## Interview Tip:
"Use `whitelist` to persist only what's needed â€” don't persist everything."

---

## Question 97: What state should not be persisted?

## Answer:
- **Loading states**: Temporary.
- **Error states**: Temporary.
- **UI state**: Modals, dropdowns.
- **Server state**: Use RTK Query caching instead.
- **Large data**: Performance impact.

## Key Points:
- Loading and error states.
- UI state.
- Server state (use RTK Query).
- Large data.
- Only persist what's needed.

## Interview Tip:
"Don't persist loading, errors, or UI state â€” only persist user preferences and auth."

---

## Question 98: How do you clear persisted state on logout?

## Answer:
```javascript
import { persistor } from "./store";

async function logout() {
  dispatch(logoutAction());
  await persistor.purge(); // Clear persisted state
}
```

## Key Points:
- `persistor.purge()` clears persisted state.
- Call on logout.
- Clear sensitive data.
- Reset to initial state.

## Interview Tip:
"Call `persistor.purge()` on logout to clear persisted sensitive data."

---

## Question 99: How do you debug Redux state changes?

## Answer:
1. **Redux DevTools**: Inspect state, actions, diffs.
2. **Console.log**: In middleware.
3. **Action logging**: Log all dispatched actions.
4. **Time-travel**: Go back to previous states.

## Key Points:
- Redux DevTools for inspection.
- Console.log in middleware.
- Action logging.
- Time-travel debugging.

## Interview Tip:
"Redux DevTools is the primary tool â€” time-travel debugging is invaluable."

---

## Question 100: What Redux Toolkit middleware and persistence best practices do you follow?

## Answer:
1. **Default middleware**: Use unless you need custom.
2. **Selective persistence**: Only persist necessary state.
3. **Clear on logout**: Purge persisted state.
4. **DevTools**: Keep enabled in development.
5. **Custom middleware**: For logging, analytics.

## Key Points:
- Default middleware.
- Selective persistence.
- Clear on logout.
- DevTools in development.
- Custom middleware for specific needs.

## Interview Tip:
"Default middleware, selective persistence, clear on logout â€” the persistence best practices."

---

## Part 10 (101â€“110): Performance Optimization

---

## Question 101: How do you optimize Redux Toolkit performance?

## Answer:
1. **Memoized selectors**: `createSelector()`.
2. **Specific selectors**: Don't select entire objects.
3. **Normalized state**: Flat state structure.
4. **`shallowEqual`**: For object comparisons.
5. **RTK Query**: Automatic caching.

## Key Points:
- Memoized selectors.
- Specific value selection.
- Normalized state.
- shallowEqual.
- RTK Query caching.

## Interview Tip:
"Memoized selectors and normalized state are the performance foundations."

---

## Question 102: What causes unnecessary re-renders in Redux applications?

## Answer:
1. **Selecting entire objects**: New reference every render.
2. **New function references**: Inline functions in selectors.
3. **Context changes**: All consumers re-render.
4. **Frequent updates**: State changes often.

## Key Points:
- Selecting entire objects.
- New function references.
- Context changes.
- Frequent updates.

## Interview Tip:
"Selecting entire objects is the #1 cause of unnecessary re-renders."

---

## Question 103: How does `useSelector()` trigger re-renders?

## Answer:
`useSelector()` subscribes to the store and re-renders when the selected value changes (by reference equality).

## Key Points:
- Subscribes to store.
- Re-renders on value change.
- Reference equality by default.
- Use `shallowEqual` for objects.

## Interview Tip:
"`useSelector` uses reference equality â€” select specific values, not objects."

---

## Question 104: What is `shallowEqual`?

## Answer:
`shallowEqual` compares objects by their properties (shallow) instead of reference.

```jsx
const user = useSelector(
  (state) => ({ name: state.user.name, email: state.user.email }),
  shallowEqual
);
```

## Key Points:
- Shallow comparison of objects.
- Prevents re-renders when properties are same.
- Import from `react-redux`.
- Use when selecting objects.

## Interview Tip:
"Use `shallowEqual` when selecting objects â€” it prevents unnecessary re-renders."

---

## Question 105: When should you use memoized selectors?

## Answer:
- **Derived data**: Computed from state.
- **Expensive calculations**: Filtering, sorting.
- **Referential equality**: Need stable references.
- **Performance**: Components re-render often.

## Key Points:
- Derived data.
- Expensive calculations.
- Referential equality.
- Performance optimization.

## Interview Tip:
"Memoize selectors that compute derived data or do expensive operations."

---

## Question 106: What is `createSelector()`?

## Answer:
`createSelector()` creates memoized selectors that only recompute when inputs change.

```javascript
import { createSelector } from "@reduxjs/toolkit";

const selectUsers = (state) => state.users;
const selectActiveUsers = createSelector(
  [selectUsers],
  (users) => users.filter(u => u.isActive)
);
```

## Key Points:
- Memoized selectors.
- Only recomputes when inputs change.
- From `reselect` library (included in RTK).
- Performance optimization.

## Interview Tip:
"`createSelector()` memoizes derived data â€” it only recomputes when inputs change."

---

## Question 107: How does `createSelector()` improve performance?

## Answer:
- **Memoization**: Caches results.
- **Input-based**: Only recomputes when inputs change.
- **Referential equality**: Same output = same reference.
- **Prevents re-renders**: Stable references.

## Key Points:
- Caches results.
- Input-based recomputation.
- Stable references.
- Prevents re-renders.

## Interview Tip:
"`createSelector()` prevents unnecessary re-renders by memoizing derived data."

---

## Question 108: What are derived selectors?

## Answer:
Derived selectors compute values from state, like filtering or aggregating.

```javascript
const selectTotalPrice = createSelector(
  [(state) => state.cart.items],
  (items) => items.reduce((sum, item) => sum + item.price * item.quantity, 0)
);
```

## Key Points:
- Compute from state.
- Filtering, aggregating, transforming.
- Memoized with `createSelector`.
- Performance optimization.

## Interview Tip:
"Derived selectors compute values from state â€” memoize them with `createSelector`."

---

## Question 109: What is state normalization?

## Answer:
State normalization stores data in a flat structure with entities by ID.

```javascript
{
  users: {
    byId: { 1: { id: 1, name: "Alice" }, 2: { id: 2, name: "Bob" } },
    allIds: [1, 2]
  }
}
```

## Key Points:
- Flat structure.
- Entities by ID.
- No duplication.
- Easy updates.
- Entity Adapter automates this.

## Interview Tip:
"Normalized state prevents duplication â€” use Entity Adapter to automate it."

---

## Question 110: How does normalized state improve performance?

## Answer:
- **Fast lookups**: O(1) by ID.
- **No duplication**: Single source per entity.
- **Easy updates**: Update one place.
- **Consistent data**: No stale references.

## Key Points:
- O(1) lookups.
- No duplication.
- Easy updates.
- Consistent data.

## Interview Tip:
"Normalized state = fast lookups + no duplication + easy updates."

---

## Part 11 (111â€“120): Entity Adapter

---

## Question 111: What is `createEntityAdapter()`?

## Answer:
`createEntityAdapter()` provides utilities for managing normalized entity state.

```javascript
const usersAdapter = createEntityAdapter();
const usersSlice = createSlice({
  name: "users",
  initialState: usersAdapter.getInitialState(),
  reducers: {
    addUser: usersAdapter.addOne,
    updateUser: usersAdapter.updateOne,
    removeUser: usersAdapter.removeOne
  }
});
```

## Key Points:
- Manages normalized entity state.
- CRUD utilities.
- Auto-generates selectors.
- Sorting support.
- Built into Redux Toolkit.

## Interview Tip:
"Entity Adapter automates normalized state management â€” CRUD operations are built-in."

---

## Question 112: Why should you use `createEntityAdapter()`?

## Answer:
- **Normalized state**: Automatic normalization.
- **CRUD utilities**: addOne, updateOne, removeOne.
- **Selectors**: Auto-generated selectors.
- **Sorting**: Built-in sorting.
- **Performance**: Optimized updates.

## Key Points:
- Automatic normalization.
- CRUD utilities.
- Auto-generated selectors.
- Sorting support.
- Performance optimization.

## Interview Tip:
"Entity Adapter automates everything about normalized state â€” use it for collections."

---

## Question 113: What problems does it solve?

## Answer:
- **Manual normalization**: Automates flat state structure.
- **CRUD operations**: Standardized add/update/remove.
- **Selector creation**: Auto-generated selectors.
- **Sorting**: Built-in sorting.

## Key Points:
- Automates normalization.
- Standardized CRUD.
- Auto-generated selectors.
- Built-in sorting.

## Interview Tip:
"Entity Adapter eliminates the boilerplate of normalized state management."

---

## Question 114: How does `createEntityAdapter()` normalize state?

## Answer:
```javascript
{
  ids: [1, 2, 3],
  entities: {
    1: { id: 1, name: "Alice" },
    2: { id: 2, name: "Bob" },
    3: { id: 3, name: "Charlie" }
  }
}
```

## Key Points:
- `ids` array for ordering.
- `entities` object by ID.
- Flat structure.
- No duplication.

## Interview Tip:
"Entity Adapter stores `ids` for ordering and `entities` by ID â€” the standard normalized structure."

---

## Question 115: What methods does Entity Adapter provide?

## Answer:
- **addOne**: Add single entity.
- **addMany**: Add multiple entities.
- **setOne**: Upsert single entity.
- **setMany**: Upsert multiple entities.
- **updateOne**: Update single entity.
- **updateMany**: Update multiple entities.
- **removeOne**: Remove single entity.
- **removeMany**: Remove multiple entities.
- **setAll**: Replace all entities.
- **removeAll**: Remove all entities.

## Key Points:
- Full CRUD operations.
- Upsert support.
- Batch operations.
- Replace all.

## Interview Tip:
"Entity Adapter provides all CRUD operations â€” addOne, updateOne, removeOne, setAll."

---

## Question 116: How do you sort entities using Entity Adapter?

## Answer:
```javascript
const usersAdapter = createEntityAdapter({
  sortComparer: (a, b) => a.name.localeCompare(b.name)
});
```

## Key Points:
- `sortComparer` option.
- Automatic sorting.
- Sorted by specified field.
- Maintains order.

## Interview Tip:
"Entity Adapter sorts automatically â€” just provide a `sortComparer`."

---

## Question 117: How do you update entities efficiently?

## Answer:
```javascript
// Update single
usersAdapter.updateOne(state, {
  id: 1,
  changes: { name: "Alice Updated" }
});

// Update multiple
usersAdapter.updateMany(state, [
  { id: 1, changes: { name: "Alice" } },
  { id: 2, changes: { name: "Bob" } }
]);
```

## Key Points:
- `updateOne` for single update.
- `updateMany` for batch updates.
- Only specify changed fields.
- Efficient partial updates.

## Interview Tip:
"`updateOne` with `changes` for partial updates â€” only specify what changed."

---

## Question 118: When should you avoid using Entity Adapter?

## Answer:
- **Simple state**: Single values, not collections.
- **Nested data**: Deeply nested structures.
- **Non-entity data**: Settings, UI state.
- **Small collections**: Few items, no performance issues.

## Key Points:
- Simple state doesn't need it.
- Nested data is complex.
- Non-entity data.
- Small collections.

## Interview Tip:
"Entity Adapter is for collections â€” don't use it for simple state."

---

## Question 119: How does Entity Adapter compare to manually normalized state?

## Answer:
| Feature | Entity Adapter | Manual |
|---------|---------------|--------|
| Boilerplate | Low | High |
| CRUD | Built-in | Manual |
| Selectors | Auto-generated | Manual |
| Sorting | Built-in | Manual |
| Updates | Efficient | Manual |

## Key Points:
- Entity Adapter: less boilerplate, more features.
- Manual: full control, more code.
- Entity Adapter is recommended.

## Interview Tip:
"Entity Adapter eliminates boilerplate â€” use it unless you need full control."

---

## Question 120: What Entity Adapter best practices do you follow?

## Answer:
1. **One adapter per entity type**: Users, posts, etc.
2. **Use selectors**: Auto-generated selectors.
3. **Sort with sortComparer**: Automatic sorting.
4. **Use updateOne**: For partial updates.
5. **Combine with createSlice**: Clean integration.

## Key Points:
- One adapter per entity.
- Use auto-generated selectors.
- Automatic sorting.
- Partial updates.
- Combine with createSlice.

## Interview Tip:
"One adapter per entity, use selectors, automatic sorting â€” the Entity Adapter best practices."

---

## Part 12 (121â€“130): Large-Scale Architecture

---

## Question 121: How do you organize Redux Toolkit in a large project?

## Answer:
Feature-based:
```
src/
  features/
    auth/
      authSlice.ts
      authAPI.ts
    users/
      usersSlice.ts
      usersAPI.ts
  store.ts
  hooks.ts
```

## Key Points:
- Feature-based organization.
- Co-locate related logic.
- Central store configuration.
- Shared hooks file.

## Interview Tip:
"Feature-based organization scales â€” co-locate slices, APIs, and components."

---

## Question 122: How do you organize slices by feature?

## Answer:
```
features/
  auth/
    authSlice.ts     # Auth state
    authAPI.ts       # Auth API calls
    authSelectors.ts # Auth selectors
  users/
    usersSlice.ts
    usersAPI.ts
    usersSelectors.ts
```

## Key Points:
- One slice per feature.
- Co-locate API, selectors.
- Easy to find and maintain.
- Self-contained features.

## Interview Tip:
"Each feature has its own slice, API, and selectors â€” self-contained."

---

## Question 123: How do you avoid deeply nested Redux state?

## Answer:
1. **Normalize data**: Flat structure.
2. **Entity Adapter**: For collections.
3. **Separate slices**: Different concerns.
4. **Selectors**: Compute derived data.

## Key Points:
- Normalize data.
- Entity Adapter for collections.
- Separate slices.
- Selectors for derived data.

## Interview Tip:
"Normalize data and use Entity Adapter â€” flat state is easier to manage."

---

## Question 124: What is code splitting in Redux?

## Answer:
Code splitting loads Redux slices only when needed, reducing initial bundle size.

## Key Points:
- Load slices on demand.
- Reduce initial bundle.
- Dynamic imports.
- Feature-based loading.

## Interview Tip:
"Code split Redux slices for large apps â€” load features on demand."

---

## Question 125: What are dynamic reducers?

## Answer:
Dynamic reducers are reducers added to the store at runtime, not at initialization.

## Key Points:
- Add reducers at runtime.
- Reduce initial bundle.
- Feature-based loading.
- Advanced pattern.

## Interview Tip:
"Dynamic reducers for large apps â€” add features on demand."

---

## Question 126: How do you lazy-load Redux slices?

## Answer:
```javascript
// Dynamic import
const usersSlice = await import("./features/users/usersSlice");
store.injectReducer("users", usersSlice.default);
```

## Key Points:
- Dynamic imports.
- `injectReducer` for adding slices.
- Reduce initial bundle.
- Load on demand.

## Interview Tip:
"Lazy-load slices for large apps â€” reduces initial bundle size."

---

## Question 127: How do you share state across multiple features?

## Answer:
1. **Global slice**: Shared state in its own slice.
2. **Cross-slice actions**: Listen for actions from other slices.
3. **Selectors**: Compute from shared state.

## Key Points:
- Global slice for shared state.
- Cross-slice actions.
- Selectors for derived data.
- Keep shared state minimal.

## Interview Tip:
"Global slices for truly shared state; cross-slice actions for communication."

---

## Question 128: How do you handle global state versus feature state?

## Answer:
- **Global state**: Auth, theme, locale.
- **Feature state**: Feature-specific data.

## Key Points:
- Global for app-wide concerns.
- Feature for specific concerns.
- Keep global state minimal.
- Feature slices for most data.

## Interview Tip:
"Global state for auth, theme, locale â€” everything else in feature slices."

---

## Question 129: What Redux architecture patterns have you used?

## Answer:
- **Feature-based slices**: One slice per feature.
- **Normalized state**: For collections.
- **Entity Adapter**: For CRUD operations.
- **RTK Query**: For data fetching.
- **Selectors**: For derived data.

## Key Points:
- Feature-based organization.
- Normalized state.
- Entity Adapter.
- RTK Query.
- Memoized selectors.

## Interview Tip:
"Feature slices + normalized state + Entity Adapter + RTK Query â€” the modern Redux pattern."

---

## Question 130: What project structure do you recommend for large Redux applications?

## Answer:
```
src/
  features/
    auth/
    users/
    posts/
  shared/
    components/
    hooks/
    utils/
  store.ts
  hooks.ts
  types.ts
```

## Key Points:
- Feature-based organization.
- Shared code in `shared/`.
- Central store configuration.
- Shared hooks and types.
- Easy to navigate.

## Interview Tip:
"Feature-based + shared directory â€” the scalable Redux structure."

---

## Part 13 (131â€“140): Testing

---

## Question 131: How do you test Redux reducers?

## Answer:
```javascript
test("increments counter", () => {
  const state = counterReducer({ value: 0 }, increment());
  expect(state.value).toBe(1);
});
```

Reducers are pure functions â€” easy to test.

## Key Points:
- Test pure functions.
- Pass state and action.
- Assert new state.
- Simple and fast.

## Interview Tip:
"Reducers are pure functions â€” they're the easiest thing to test."

---

## Question 132: How do you test Redux slices?

## Answer:
```javascript
test("addUser adds a user", () => {
  const state = usersSlice.reducer([], addUser({ id: 1, name: "Alice" }));
  expect(state).toHaveLength(1);
  expect(state[0].name).toBe("Alice");
});
```

## Key Points:
- Test slice reducers.
- Import actions from slice.
- Assert state changes.
- Test all actions.

## Interview Tip:
"Test slice reducers by dispatching actions and asserting state."

---

## Question 133: How do you test async thunks?

## Answer:
```javascript
test("fetchUsers fetches users", async () => {
  const dispatch = jest.fn();
  const getState = jest.fn();
  
  await fetchUsers()(dispatch, getState, undefined);
  
  expect(dispatch).toHaveBeenCalledWith(
    expect.objectContaining({ type: fetchUsers.pending.type })
  );
});
```

## Key Points:
- Mock dispatch and getState.
- Call thunk directly.
- Assert dispatched actions.
- Test pending, fulfilled, rejected.

## Interview Tip:
"Test async thunks by calling them directly with mock dispatch."

---

## Question 134: How do you mock API calls in Redux tests?

## Answer:
```javascript
// MSW
import { rest } from "msw";
import { setupServer } from "msw/node";

const server = setupServer(
  rest.get("/api/users", (req, res, ctx) => {
    return res(ctx.json([{ id: 1, name: "Alice" }]));
  })
);
```

## Key Points:
- MSW for API mocking.
- Intercept requests.
- Return mock data.
- Test different responses.

## Interview Tip:
"MSW is the standard for API mocking â€” it intercepts actual network requests."

---

## Question 135: How do you test RTK Query endpoints?

## Answer:
```javascript
test("getUsers returns users", async () => {
  const { data } = await store.dispatch(
    apiSlice.endpoints.getUsers.initiate()
  );
  expect(data).toEqual([{ id: 1, name: "Alice" }]);
});
```

## Key Points:
- Dispatch endpoint directly.
- Assert returned data.
- Mock API responses.
- Test caching behavior.

## Interview Tip:
"Test RTK Query by dispatching endpoints directly."

---

## Question 136: How do you test selectors?

## Answer:
```javascript
test("selectActiveUsers returns active users", () => {
  const state = { users: [{ id: 1, isActive: true }, { id: 2, isActive: false }] };
  const result = selectActiveUsers(state);
  expect(result).toEqual([{ id: 1, isActive: true }]);
});
```

## Key Points:
- Test with mock state.
- Assert returned value.
- Test memoization.
- Simple and fast.

## Interview Tip:
"Test selectors with mock state â€” they're pure functions."

---

## Question 137: How do you test custom middleware?

## Answer:
```javascript
test("middleware logs actions", () => {
  const store = { getState: jest.fn(), dispatch: jest.fn() };
  const next = jest.fn();
  const action = { type: "TEST" };
  
  middleware(store)(next)(action);
  expect(next).toHaveBeenCalledWith(action);
});
```

## Key Points:
- Mock store, next, action.
- Call middleware directly.
- Assert next was called.
- Test side effects.

## Interview Tip:
"Test middleware by calling it directly with mock store and next."

---

## Question 138: How do you test Redux-connected React components?

## Answer:
```jsx
function renderWithProviders(ui, { preloadedState } = {}) {
  const store = configureStore({
    reducer: rootReducer,
    preloadedState
  });
  return render(<Provider store={store}>{ui}</Provider>);
}

test("renders user name", () => {
  renderWithProviders(<UserProfile />, {
    preloadedState: { user: { name: "Alice" } }
  });
  expect(screen.getByText("Alice")).toBeInTheDocument();
});
```

## Key Points:
- Create test store with preloaded state.
- Wrap with Provider.
- Test with preloaded state.
- Test user interactions.

## Interview Tip:
"Create a test store with preloaded state â€” it's the standard testing pattern."

---

## Question 139: What testing libraries do you use for Redux applications?

## Answer:
- **Jest**: Test runner.
- **React Testing Library**: Component testing.
- **MSW**: API mocking.
- **Redux Mock Store**: Store mocking.

## Key Points:
- Jest for test runner.
- React Testing Library for components.
- MSW for API mocking.
- Standard testing stack.

## Interview Tip:
"Jest + React Testing Library + MSW â€” the Redux testing stack."

---

## Question 140: What Redux testing best practices do you follow?

## Answer:
1. **Test reducers**: Pure functions, easy to test.
2. **Test selectors**: With mock state.
3. **Test thunks**: With mock dispatch.
4. **Test components**: With preloaded state.
5. **Mock APIs**: Use MSW.

## Key Points:
- Test reducers, selectors, thunks.
- Components with preloaded state.
- MSW for API mocking.
- Focus on behavior.

## Interview Tip:
"Test reducers first â€” they're the foundation. Then selectors, thunks, and components."

---

## Part 14 (141â€“150): Senior Real-World Interview Questions

---

## Question 141: Describe the largest Redux Toolkit project you've worked on.

## Answer:
Pick a real project and describe:
- **Scale**: Number of slices, actions, components.
- **Architecture**: How you organized the store.
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

## Question 142: What was the most difficult Redux state management problem you've solved?

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
"Interviewers want to see your debugging process."

---

## Question 143: How do you debug Redux applications in production?

## Answer:
1. **Redux DevTools**: Inspect state and actions.
2. **Console.log**: In middleware.
3. **Error tracking**: Sentry for errors.
4. **State snapshots**: Log state at key points.

## Key Points:
- Redux DevTools.
- Console.log in middleware.
- Error tracking.
- State snapshots.

## Interview Tip:
"Redux DevTools for state inspection; Sentry for error tracking."

---

## Question 144: How do you review Redux-related pull requests?

## Answer:
Check for:
1. **State structure**: Normalized, flat.
2. **Immutability**: No direct mutations.
3. **Selectors**: Memoized selectors.
4. **TypeScript**: Proper typing.
5. **Testing**: Adequate coverage.

## Key Points:
- State structure.
- Immutability.
- Memoized selectors.
- TypeScript.
- Testing.

## Interview Tip:
"Check state structure, immutability, and TypeScript typing."

---

## Question 145: What Redux coding standards do you enforce?

## Answer:
1. **One slice per feature**: Organize by feature.
2. **TypeScript**: Type everything.
3. **Normalized state**: For collections.
4. **Memoized selectors**: For derived data.
5. **RTK Query**: For data fetching.

## Key Points:
- Feature-based slices.
- TypeScript types.
- Normalized state.
- Memoized selectors.
- RTK Query.

## Interview Tip:
"One slice per feature, TypeScript, normalized state â€” the Redux Toolkit standards."

---

## Question 146: How would you migrate a legacy Redux application to Redux Toolkit?

## Answer:
1. **Install Redux Toolkit**: `npm install @reduxjs/toolkit`.
2. **Replace createStore**: Use `configureStore()`.
3. **Convert reducers**: Use `createSlice()`.
4. **Convert thunks**: Use `createAsyncThunk()`.
5. **Add Entity Adapter**: For normalized state.
6. **Test**: Verify everything works.

## Key Points:
- Install Redux Toolkit.
- Replace store creation.
- Convert reducers to slices.
- Convert thunks.
- Test thoroughly.

## Interview Tip:
"Migrate incrementally â€” convert one slice at a time."

---

## Question 147: How would you design state management for a large SaaS application?

## Answer:
- **Redux Toolkit**: For complex client state.
- **RTK Query**: For server state.
- **Feature-based slices**: One per feature.
- **Normalized state**: For collections.
- **Entity Adapter**: For CRUD operations.
- **Memoized selectors**: For derived data.

## Key Points:
- Redux Toolkit for client state.
- RTK Query for server state.
- Feature-based organization.
- Normalized state.
- Memoized selectors.

## Interview Tip:
"Redux Toolkit + RTK Query + feature-based slices â€” the SaaS state management pattern."

---

## Question 148: What Redux Toolkit features do you use most frequently in production?

## Answer:
- **createSlice**: For all state logic.
- **configureStore**: For store setup.
- **createAsyncThunk**: For async operations.
- **RTK Query**: For data fetching.
- **createEntityAdapter**: For normalized state.
- **createSelector**: For derived data.

## Key Points:
- createSlice and configureStore.
- createAsyncThunk for async.
- RTK Query for data fetching.
- Entity Adapter for collections.
- createSelector for derived data.

## Interview Tip:
"createSlice, RTK Query, Entity Adapter, createSelector â€” the Redux Toolkit essentials."

---

## Question 149: If you were starting a new React project today, how would you structure Redux Toolkit and RTK Query?

## Answer:
```
src/
  features/
    auth/
      authSlice.ts
    users/
      usersSlice.ts
  services/
    api.ts           # RTK Query API
  store.ts
  hooks.ts
  types.ts
```

- One slice per feature.
- RTK Query for all API calls.
- Entity Adapter for collections.
- Typed hooks throughout.

## Key Points:
- Feature-based slices.
- RTK Query for APIs.
- Entity Adapter for collections.
- Typed hooks.
- Clean structure.

## Interview Tip:
"Feature slices + RTK Query + Entity Adapter + typed hooks â€” the modern Redux structure."

---

## Question 150: In your opinion, what separates a junior, mid-level, and senior Redux Toolkit developer?

## Answer:
- **Junior**: Knows createSlice, useSelector, useDispatch. Can manage simple state.
- **Mid-level**: Understands normalized state, Entity Adapter, RTK Query. Can design state architecture.
- **Senior**: Designs scalable state management, handles complex async flows, optimizes performance, mentors others.

The biggest differentiator: a senior understands when NOT to use Redux.

## Key Points:
- Junior: basic slices and hooks.
- Mid-level: normalized state, RTK Query.
- Senior: architecture, optimization, mentoring.
- Senior knows when Redux is overkill.

## Interview Tip:
"The best answer shows self-awareness. Pick your level and explain what you're doing to grow."

---

# End of Redux Toolkit Interview Questions & Answers
