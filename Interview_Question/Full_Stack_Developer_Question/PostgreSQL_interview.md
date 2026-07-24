# PostgreSQL Interview Questions (250 Total)

---

## PostgreSQL Fundamentals

1. What is PostgreSQL?
2. Why is PostgreSQL popular?
3. What are the advantages of PostgreSQL?
4. What are the disadvantages of PostgreSQL?
5. How does PostgreSQL differ from MySQL?
6. How does PostgreSQL differ from MongoDB?
7. What types of applications are best suited for PostgreSQL?
8. What is ACID in PostgreSQL?
9. What is MVCC (Multi-Version Concurrency Control)?
10. Why does PostgreSQL use MVCC?

---

## Database Basics

11. What is a database?
12. What is a schema in PostgreSQL?
13. What is a table?
14. What is a row (record)?
15. What is a column?
16. What is a primary key?
17. What is a foreign key?
18. What is a unique constraint?
19. What is a check constraint?
20. What is a default constraint?

---

## Data Types

21. What are PostgreSQL data types?
22. What is the difference between `CHAR`, `VARCHAR`, and `TEXT`?
23. What is the `UUID` data type?
24. When should you use `UUID` instead of `SERIAL`?
25. What numeric data types are available?
26. What date and time data types does PostgreSQL support?
27. What is the `BOOLEAN` type?
28. What is the `JSON` data type?
29. What is the `JSONB` data type?
30. What is the difference between `JSON` and `JSONB`?

---

## Basic SQL

31. What is SQL?
32. What is the `SELECT` statement?
33. What is the `INSERT` statement?
34. What is the `UPDATE` statement?
35. What is the `DELETE` statement?
36. What is the `TRUNCATE` statement?
37. What is the difference between `DELETE`, `TRUNCATE`, and `DROP`?
38. What is the `WHERE` clause?
39. What is the `ORDER BY` clause?
40. What is the `LIMIT` clause?

---

## Filtering & Operators

41. What is the `LIKE` operator?
42. What is `ILIKE`?
43. What is the `IN` operator?
44. What is the `BETWEEN` operator?
45. What is the `IS NULL` operator?
46. What is the `DISTINCT` keyword?
47. What is the `CASE` expression?
48. What are aggregate functions?
49. What is the difference between `COUNT(*)` and `COUNT(column)`?
50. What SQL best practices do you follow?

---

# SQL Joins

51. What is an INNER JOIN?
52. What is a LEFT JOIN?
53. What is a RIGHT JOIN?
54. What is a FULL OUTER JOIN?
55. What is a CROSS JOIN?
56. What is a SELF JOIN?
57. What is the difference between INNER JOIN and LEFT JOIN?
58. When would you use a FULL OUTER JOIN?
59. How do you join more than two tables?
60. What are common mistakes when writing JOIN queries?

---

# GROUP BY & Aggregation

61. What is the `GROUP BY` clause?
62. Why do we use `GROUP BY`?
63. What is the `HAVING` clause?
64. What is the difference between `WHERE` and `HAVING`?
65. What aggregate functions are available in PostgreSQL?
66. What is `COUNT()`?
67. What is `SUM()`?
68. What is `AVG()`?
69. What are `MIN()` and `MAX()`?
70. How do you group data by multiple columns?

---

# Subqueries

71. What is a subquery?
72. What is the difference between a correlated and a non-correlated subquery?
73. When should you use a subquery?
74. What are the advantages of subqueries?
75. What are the disadvantages of subqueries?
76. What is the `EXISTS` operator?
77. What is the `NOT EXISTS` operator?
78. What is the difference between `EXISTS` and `IN`?
79. When is `EXISTS` more efficient than `IN`?
80. What are common subquery optimization techniques?

---

# Common Table Expressions (CTEs)

81. What is a Common Table Expression (CTE)?
82. Why use a CTE instead of a subquery?
83. What is the `WITH` clause?
84. What are recursive CTEs?
85. When would you use a recursive CTE?
86. What are the advantages of CTEs?
87. What are the disadvantages of CTEs?
88. How do CTEs improve query readability?
89. What performance considerations exist when using CTEs?
90. What are common real-world use cases for CTEs?

---

# Window Functions

91. What are window functions?
92. How do window functions differ from aggregate functions?
93. What is the `OVER()` clause?
94. What is `ROW_NUMBER()`?
95. What is `RANK()`?
96. What is `DENSE_RANK()`?
97. What is `LEAD()`?
98. What is `LAG()`?
99. What are partitioning and ordering in window functions?
100. When would you use window functions in real-world applications?

---

# Indexing

101. What is an index in PostgreSQL?
102. Why are indexes important?
103. How does a B-Tree index work?
104. What is a Hash index?
105. What is a GIN (Generalized Inverted Index)?
106. What is a GiST (Generalized Search Tree) index?
107. When should you use a BRIN index?
108. What is a composite index?
109. What is a partial index?
110. What is a covering index?

---

# Index Optimization

111. How do you decide which columns should be indexed?
112. What are the disadvantages of adding too many indexes?
113. How do indexes affect INSERT, UPDATE, and DELETE operations?
114. What is index selectivity?
115. How do you identify unused indexes?
116. How do you remove unnecessary indexes?
117. What is index fragmentation?
118. How do you rebuild an index?
119. How do you monitor index performance?
120. What indexing best practices do you follow?

---

# Query Optimization

121. What is the `EXPLAIN` command?
122. What is `EXPLAIN ANALYZE`?
123. How do you read an execution plan?
124. What is a sequential scan?
125. What is an index scan?
126. What is a bitmap index scan?
127. What is a nested loop join?
128. What is a hash join?
129. What is a merge join?
130. How do you optimize slow SQL queries?

---

# Transactions & Concurrency

131. What is a database transaction?
132. What are the ACID properties?
133. What are transaction isolation levels?
134. What is the Read Committed isolation level?
135. What is Repeatable Read?
136. What is Serializable isolation?
137. What is MVCC (Multi-Version Concurrency Control)?
138. How does MVCC improve concurrency?
139. What are row-level locks?
140. What is the difference between optimistic and pessimistic locking?

---

# Deadlocks & Performance

141. What is a deadlock?
142. How does PostgreSQL detect deadlocks?
143. How do you prevent deadlocks?
144. What is table partitioning?
145. When should you partition a table?
146. What is connection pooling?
147. What is the purpose of PgBouncer?
148. How do you monitor PostgreSQL performance?
149. What are common PostgreSQL performance bottlenecks?
150. What performance tuning best practices do you follow for production databases?

---

# Database Design

151. What is database normalization?
152. What are the different normal forms (1NF, 2NF, 3NF, BCNF)?
153. Why is normalization important?
154. What is denormalization?
155. When should you denormalize a database?
156. What are the trade-offs between normalization and denormalization?
157. How do you design a scalable relational database?
158. What is database schema design?
159. How do you model one-to-one relationships?
160. How do you model one-to-many and many-to-many relationships?

---

# Constraints & Keys

161. What types of constraints does PostgreSQL support?
162. What is a PRIMARY KEY?
163. What is a FOREIGN KEY?
164. What is a UNIQUE constraint?
165. What is a CHECK constraint?
166. What is a NOT NULL constraint?
167. What is a DEFAULT constraint?
168. What are composite keys?
169. When should you use natural keys vs surrogate keys?
170. What are cascading actions (`CASCADE`, `RESTRICT`, `SET NULL`, `NO ACTION`)?

---

# Views, Functions & Triggers

171. What is a View?
172. What is a Materialized View?
173. What is the difference between a View and a Materialized View?
174. When should you use a Materialized View?
175. What is a stored procedure?
176. What is the difference between a stored procedure and a function?
177. What are PostgreSQL functions?
178. What are triggers?
179. When should you use triggers?
180. What are the drawbacks of triggers?

---

# Security

181. How does PostgreSQL handle authentication?
182. What are PostgreSQL roles?
183. What is the difference between users and roles?
184. How do you grant permissions?
185. How do you revoke permissions?
186. What is the principle of least privilege?
187. How do you secure sensitive data in PostgreSQL?
188. How do you encrypt data at rest and in transit?
189. How do you protect against SQL Injection?
190. What PostgreSQL security best practices do you follow?

---

# Backup, Recovery & Administration

191. How do you back up a PostgreSQL database?
192. What is `pg_dump`?
193. What is `pg_restore`?
194. What is point-in-time recovery (PITR)?
195. What is Write-Ahead Logging (WAL)?
196. What is replication in PostgreSQL?
197. What is the difference between streaming replication and logical replication?
198. What is high availability (HA)?
199. How do you monitor PostgreSQL in production?
200. What administrative best practices do you follow for PostgreSQL?

---

# Database Architecture

201. How do you structure a PostgreSQL database for a large application?
202. What database design principles do you follow?
203. How do you design a scalable relational database?
204. How do you model complex relationships?
205. How do you design an audit logging system?
206. How do you implement soft deletes?
207. How do you implement multi-tenancy?
208. What is the difference between shared-database and separate-database multi-tenancy?
209. How do you manage schema changes in production?
210. What database architecture patterns have you used?

---

# Scaling PostgreSQL

211. How do you scale PostgreSQL?
212. What are read replicas?
213. When should you use read replicas?
214. What is database sharding?
215. When should you shard a database?
216. What are the advantages and disadvantages of sharding?
217. What is horizontal scaling?
218. What is vertical scaling?
219. How do you handle millions of rows efficiently?
220. What are common scalability bottlenecks in PostgreSQL?

---

# Production Optimization

221. How do you troubleshoot slow SQL queries?
222. How do you identify blocking queries?
223. How do you monitor database performance?
224. Which PostgreSQL metrics do you monitor?
225. How do you optimize connection pooling?
226. How do you optimize disk usage?
227. How do you optimize memory settings?
228. How do you optimize PostgreSQL for high write throughput?
229. What maintenance tasks should be scheduled regularly?
230. What production best practices do you always follow?

---

# Real-World Database Design

231. How would you design the database for an e-commerce platform?
232. How would you design the database for a CRM system?
233. How would you design the database for an ERP system?
234. How would you design the database for a social media application?
235. How would you design the database for a school management system?
236. How would you design the database for a booking system?
237. How would you handle concurrent seat booking without double-booking?
238. How would you design an inventory management database?
239. How would you design an order and payment system?
240. How would you migrate a large production database with minimal downtime?

---

# Senior Real-World Interview Questions

241. Describe the largest PostgreSQL database you've worked with.
242. What was the most difficult database issue you've solved?
243. How do you debug production database performance issues?
244. How do you review SQL queries during a pull request?
245. What SQL coding standards do you enforce?
246. How do you mentor junior developers on database design?
247. What PostgreSQL features do you use most often in production?
248. If you were building a production SaaS today, how would you design the database?
249. What PostgreSQL best practices do you always follow?
250. In your opinion, what separates a junior, mid-level, and senior PostgreSQL developer?

---

