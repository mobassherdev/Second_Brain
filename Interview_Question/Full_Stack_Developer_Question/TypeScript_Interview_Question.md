# TypeScript Interview Questions (1–200)

---

## Part 1 (1–25): Fundamentals

1. What is TypeScript?
2. Why should you use TypeScript instead of JavaScript?
3. What are the advantages of TypeScript?
4. What are the disadvantages of TypeScript?
5. What is static typing?
6. What is dynamic typing?
7. What is a superset language?
8. How does TypeScript work?
9. Can browsers execute TypeScript directly?
10. How do you compile TypeScript?
11. What is the TypeScript compiler (`tsc`)?
12. What is `tsconfig.json`?
13. What is the purpose of `strict` mode?
14. What are primitive types in TypeScript?
15. What is type inference?
16. What is type annotation?
17. What is the `any` type?
18. Why is `any` considered dangerous?
19. What is the `unknown` type?
20. What is the difference between `any` and `unknown`?
21. What is the `never` type?
22. What is the `void` type?
23. What is the difference between `null` and `undefined`?
24. What is the `object` type?
25. What is the difference between `Object`, `object`, and `{}`?

---

## Part 2 (26–50): Types

26. What are union types?
27. What are intersection types?
28. What are literal types?
29. What are tuple types?
30. What is a readonly tuple?
31. What are enum types?
32. What is the difference between numeric and string enums?
33. Why do many developers avoid enums?
34. What is a const enum?
35. What are type aliases?
36. What is the difference between `type` and `interface`?
37. When should you use `type`?
38. When should you use `interface`?
39. Can interfaces extend interfaces?
40. Can types extend interfaces?
41. What are declaration merging and interface merging?
42. What is optional chaining (`?.`)?
43. What is nullish coalescing (`??`)?
44. What is optional property (`?`)?
45. What is optional parameter?
46. What are default parameters?
47. What are rest parameters?
48. What are spread operators?
49. What are index signatures?
50. What are template literal types?

---

## Part 3 (51–75): Advanced TypeScript

51. What are generics?
52. Why do we use generics?
53. What are generic constraints?
54. What is the `keyof` operator?
55. What is the `typeof` operator?
56. What is indexed access type?
57. What are mapped types?
58. What are conditional types?
59. What is the `infer` keyword?
60. What are utility types?
61. What is `Partial<T>`?
62. What is `Required<T>`?
63. What is `Readonly<T>`?
64. What is `Pick<T>`?
65. What is `Omit<T>`?
66. What is `Exclude<T>`?
67. What is `Extract<T>`?
68. What is `Record<K, T>`?
69. What is `ReturnType<T>`?
70. What is `Parameters<T>`?
71. What is `Awaited<T>`?
72. What is `NonNullable<T>`?
73. What is `InstanceType<T>`?
74. What is a discriminated union?
75. What is type narrowing?

---

## Part 4 (76–100): Real-World & Interview Questions

76. What are type guards?
77. How do you create a custom type guard?
78. What is type assertion?
79. What is the difference between type assertion and type casting?
80. What is declaration file (`.d.ts`)?
81. What is module augmentation?
82. What is namespace in TypeScript?
83. Why are ES Modules preferred over namespaces?
84. What are decorators?
85. What are mixins?
86. How do you organize types in a large project?
87. How do you share types between frontend and backend?
88. How does TypeScript help in React projects?
89. How does TypeScript help in Node.js projects?
90. What are common TypeScript mistakes?
91. How do you migrate a JavaScript project to TypeScript?
92. What TypeScript features do you use most often?
93. How do you debug TypeScript errors?
94. How do you improve TypeScript performance in large projects?
95. What TypeScript compiler options do you commonly use?
96. What are the best practices for writing TypeScript?
97. What TypeScript interview questions have you been asked before?
98. What is your favorite TypeScript feature and why?
99. What are the biggest challenges you've faced with TypeScript?
100. If you were starting a new project today, how would you configure TypeScript and why?


---

## Part 5 — Functions & Advanced Types (101–120)

101. What are function overloads?
102. How do function overloads work?
103. When should you use overloads instead of union types?
104. What are generic functions?
105. What are generic interfaces?
106. What are generic classes?
107. What are generic type aliases?
108. What are generic constraints?
109. What is the `extends` keyword in generics?
110. What is a default generic type?
111. What is covariance?
112. What is contravariance?
113. What is bivariance?
114. What is type variance?
115. What is structural typing?
116. What is nominal typing?
117. Why does TypeScript use structural typing?
118. What is duck typing?
119. What is type compatibility?
120. How does TypeScript determine assignability?

---

## Part 6 — Advanced Type System (121–140)

121. What are recursive types?
122. What are recursive conditional types?
123. What is distributive conditional typing?
124. What is the `infer` keyword used for?
125. How does type inference work?
126. What is contextual typing?
127. What is control flow analysis?
128. What is exhaustive type checking?
129. What is the `satisfies` operator?
130. What is declaration merging?
131. What are ambient declarations?
132. What is `declare`?
133. What is a declaration file (`.d.ts`)?
134. How do you write custom declaration files?
135. How do third-party libraries provide types?
136. What is DefinitelyTyped?
137. What is module augmentation?
138. What is global augmentation?
139. What is interface merging?
140. What is namespace merging?

---

## Part 7 — Classes & OOP (141–160)

141. How are classes implemented in TypeScript?
142. What are access modifiers?
143. What is `public`?
144. What is `private`?
145. What is `protected`?
146. What are readonly properties?
147. What are parameter properties?
148. What are abstract classes?
149. What are abstract methods?
150. What are interfaces with classes?
151. What is `implements`?
152. What is `extends` in classes?
153. What are static members?
154. What are getters?
155. What are setters?
156. What are decorators?
157. What are property decorators?
158. What are method decorators?
159. What are class decorators?
160. When should you use classes instead of interfaces?

---

## Part 8 — Modules & Configuration (161–180)

161. What are ES Modules in TypeScript?
162. What is CommonJS?
163. What is the difference between ES Modules and CommonJS?
164. What is `moduleResolution`?
165. What is `baseUrl`?
166. What are path aliases?
167. What is `paths` in tsconfig?
168. What is `target` in tsconfig?
169. What is `lib` in tsconfig?
170. What is `module` in tsconfig?
171. What is `strictNullChecks`?
172. What is `noImplicitAny`?
173. What is `noUnusedLocals`?
174. What is `noUnusedParameters`?
175. What is `skipLibCheck`?
176. What is `incremental` compilation?
177. What is source mapping?
178. What is declaration generation?
179. How do you organize a large TypeScript project?
180. What is project references?

---

## Part 9 — React & Node.js with TypeScript (181–190)

181. How do you type React props?
182. How do you type React state?
183. How do you type event handlers in React?
184. How do you type refs?
185. How do you type custom hooks?
186. How do you type Context API?
187. How do you type Redux Toolkit?
188. How do you type API responses?
189. How do you share types between frontend and backend?
190. How do you use TypeScript with Express.js?

---

## Part 10 — Senior Interview Questions (191–200)

191. How would you migrate a large JavaScript project to TypeScript?
192. What are the biggest advantages of strict mode?
193. How do you reduce TypeScript compile time?
194. What TypeScript mistakes do developers commonly make?
195. What TypeScript features do you use most in production?
196. How do you design reusable types?
197. How do you avoid overly complex generic types?
198. What are TypeScript best practices for enterprise applications?
199. How has TypeScript improved your real-world projects?
200. If you were starting a new React/Next.js project today, how would you configure TypeScript and why?

---
