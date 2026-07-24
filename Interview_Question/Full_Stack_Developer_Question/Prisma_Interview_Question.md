# Prisma ORM Interview Questions

---

## Introduction

1. What is Prisma ORM?
2. Why was Prisma created?
3. What problems does Prisma solve?
4. What are the advantages of Prisma over traditional ORMs?
5. What are the disadvantages of Prisma?
6. How does Prisma differ from TypeORM?
7. How does Prisma differ from Sequelize?
8. How does Prisma differ from Mongoose?
9. What are the main components of Prisma?
10. What is Prisma Client?

---

## Prisma Schema

11. What is the Prisma Schema?
12. What is the purpose of `schema.prisma`?
13. What are datasource blocks?
14. What are generator blocks?
15. How do you configure PostgreSQL in Prisma?
16. How do you configure MySQL in Prisma?
17. How do you configure MongoDB in Prisma?
18. What are models in Prisma?
19. What are scalar types in Prisma?
20. What are enums in Prisma?

---

## Fields & Relations

21. What is the `@id` attribute?
22. What is `@default()`?
23. What is `@unique`?
24. What is `@updatedAt`?
25. What is `@map`?
26. What is `@@map`?
27. What is `@@index`?
28. What is `@@unique`?
29. What is a one-to-one relationship?
30. What is a one-to-many relationship?

---

## Relationships

31. What is a many-to-many relationship?
32. How do you define relationships in Prisma?
33. What is the `@relation` attribute?
34. How do implicit many-to-many relations work?
35. How do explicit many-to-many relations work?
36. What are relation fields?
37. What are foreign keys?
38. How does referential integrity work?
39. What happens when related records are deleted?
40. What are referential actions (`Cascade`, `Restrict`, `SetNull`, etc.)?

---

## Migrations

41. What are Prisma Migrations?
42. Why are migrations important?
43. What is `prisma migrate dev`?
44. What is `prisma migrate deploy`?
45. What is `prisma db push`?
46. What is the difference between `migrate` and `db push`?
47. What is Prisma Introspection?
48. What is `prisma db pull`?
49. What is Prisma Studio?
50. How do you seed a database using Prisma?

---

# CRUD Operations

51. How do you create a record using Prisma Client?
52. What is the difference between `create()` and `createMany()`?
53. How do you retrieve a single record?
54. What is the difference between `findUnique()` and `findFirst()`?
55. How do you retrieve multiple records?
56. What is `findMany()`?
57. How do you update a record?
58. What is the difference between `update()` and `updateMany()`?
59. How do you delete a record?
60. What is the difference between `delete()` and `deleteMany()`?

---

# Filtering & Sorting

61. How do you filter records using `where`?
62. How do you combine multiple filter conditions?
63. How do you use logical operators (`AND`, `OR`, `NOT`)?
64. How do you perform case-insensitive searches?
65. How do you search for partial matches?
66. How do you filter by date ranges?
67. How do you filter related records?
68. How do you sort results using `orderBy`?
69. How do you sort by multiple fields?
70. How do you sort by related model fields?

---

# Pagination

71. How do you implement pagination in Prisma?
72. What is offset pagination?
73. What is cursor-based pagination?
74. What are the advantages of cursor pagination?
75. When should you use offset pagination?
76. How do `skip` and `take` work?
77. How does the `cursor` option work?
78. How do you implement infinite scrolling with Prisma?
79. How do you count the total number of records?
80. What pagination strategy do you use in production?

---

# Relations & Nested Queries

81. How do you query related records?
82. What is the `include` option?
83. What is the `select` option?
84. What is the difference between `include` and `select`?
85. How do you create related records in a single query?
86. What are nested writes?
87. How do you update related records?
88. How do you delete related records?
89. How do you connect existing related records?
90. What is the difference between `connect`, `disconnect`, `set`, and `connectOrCreate`?

---

# Transactions & Advanced Queries

91. What are database transactions?
92. How do you use `$transaction()` in Prisma?
93. When should you use transactions?
94. How do interactive transactions work?
95. What are aggregations in Prisma?
96. How do you use `count()`?
97. How do you use `aggregate()`?
98. How do you use `groupBy()`?
99. When would you use raw SQL with Prisma?
100. What are `$queryRaw()` and `$executeRaw()`?

---

# Performance Optimization

101. How do you optimize Prisma queries?
102. What is the N+1 query problem?
103. How do you avoid N+1 queries in Prisma?
104. How do `select` and `include` affect performance?
105. When should you use `select` instead of `include`?
106. How do you reduce over-fetching of data?
107. How do you optimize queries that return large datasets?
108. How do you monitor slow Prisma queries?
109. How do you enable Prisma query logging?
110. What Prisma best practices improve application performance?

---

# Database Design & Indexing

111. What is database indexing?
112. When should you create an index?
113. How do you define indexes in Prisma?
114. What is the difference between `@unique` and `@@index`?
115. What is a composite index?
116. When should you use a composite unique constraint?
117. How do foreign keys affect performance?
118. How do you optimize relational database schemas?
119. How do you design efficient Prisma models?
120. What database design mistakes should you avoid?

---

# Transactions & Concurrency

121. What is database concurrency?
122. What problems can occur with concurrent updates?
123. How do Prisma transactions help maintain data consistency?
124. When should you use interactive transactions?
125. How do you ensure atomic operations?
126. What is optimistic concurrency control?
127. What is pessimistic locking?
128. How do you prevent race conditions in Prisma?
129. What are idempotent operations?
130. What transaction best practices do you follow?

---

# Production Best Practices

131. How do you manage Prisma in production?
132. How do you handle database connection pooling?
133. What is Prisma Accelerate?
134. What is Prisma Data Proxy?
135. How do you manage environment variables securely?
136. How do you deploy Prisma migrations in production?
137. How do you seed production and development databases safely?
138. How do you handle Prisma errors gracefully?
139. How do you test Prisma-based applications?
140. What logging and monitoring practices do you use with Prisma?

---

# Senior Real-World Interview Questions

141. Describe the largest Prisma project you've worked on.
142. What was the most challenging Prisma issue you've solved?
143. How do you debug slow Prisma queries?
144. How do you review Prisma schema changes during a pull request?
145. What naming conventions do you follow in Prisma schemas?
146. How would you migrate a legacy SQL project to Prisma?
147. How would you design a multi-tenant SaaS database using Prisma?
148. What Prisma features do you use most frequently in production?
149. If you were starting a new production project today, how would you structure Prisma, migrations, and database access?
150. In your opinion, what separates a junior, mid-level, and senior Prisma developer?

---
