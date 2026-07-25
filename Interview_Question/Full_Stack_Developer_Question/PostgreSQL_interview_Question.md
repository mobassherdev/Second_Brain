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

# ANSWERS


---

## Part 1 (1â€“10): PostgreSQL Fundamentals

---

## Question 1: What is PostgreSQL?

## Answer:
PostgreSQL is an open-source, object-relational database management system (ORDBMS) known for its reliability, feature set, and standards compliance. It's been in active development since 1996 and supports both SQL (relational) and JSON (non-relational) querying.

I use it for almost every project that needs a relational database â€” it handles everything from simple CRUD apps to complex analytical workloads with millions of rows.

## Key Points:
- Open-source ORDBMS, actively developed since 1996.
- Supports SQL and JSON querying.
- ACID compliant with MVCC for concurrency.
- Extensible with custom types, functions, and extensions.
- Used by Apple, Instagram, Spotify, and thousands of companies.

## Interview Tip:
Don't just say "it's a relational database." Mention MVCC, extensibility, and JSON support â€” that's what makes PostgreSQL special.

---

## Question 2: Why is PostgreSQL popular?

## Answer:
- **Standards compliance**: Most SQL-standard compliant database.
- **Extensibility**: Custom types, functions, operators, and extensions.
- **JSON support**: First-class JSON/JSONB for hybrid relational-document needs.
- **Concurrency**: MVCC allows readers and writers to work simultaneously.
- **Community**: Active open-source community and ecosystem.
- **Reliability**: Battle-tested for 25+ years.
- **Licensing**: PostgreSQL License (very permissive, not copyleft).

## Key Points:
- Most SQL-standard compliant database.
- Extensible with custom types and extensions.
- Excellent JSON support alongside relational data.
- MVCC for high concurrency.
- Active community and permissive license.

## Interview Tip:
"PostgreSQL is the Swiss Army knife of databases â€” it does relational, document, and everything in between."

---

## Question 3: What are the advantages of PostgreSQL?

## Answer:
- **ACID compliance**: Reliable transactions.
- **MVCC**: High concurrency without locking.
- **Extensibility**: Custom types, functions, indexes.
- **JSON/JSONB**: Document storage alongside relational data.
- **Full-text search**: Built-in text search capabilities.
- **Extensions**: PostGIS (geospatial), pg_trgm (fuzzy search), TimescaleDB (time series).
- **Standards compliance**: Most complete SQL implementation.
- **Replication**: Streaming and logical replication.

## Key Points:
- ACID and MVCC for reliability and concurrency.
- JSONB for document-style storage.
- Powerful extensions ecosystem.
- Full-text search built-in.
- Streaming and logical replication.

## Interview Tip:
Mention extensions â€” "PostGIS for geospatial, TimescaleDB for time series, pgvector for AI embeddings."

---

## Question 4: What are the disadvantages of PostgreSQL?

## Answer:
- **Complexity**: More complex to set up and tune than MySQL.
- **Memory usage**: Higher memory consumption for similar workloads.
- **Write performance**: Slightly slower writes than MySQL for simple workloads.
- **Replication complexity**: Logical replication setup is more involved.
- **Learning curve**: Advanced features (CTEs, window functions) take time.
- **No built-in clustering**: Requires external tools (Patroni, pgBouncer).

## Key Points:
- More complex setup than MySQL.
- Higher memory usage.
- Write performance slightly slower for simple workloads.
- Advanced features have a learning curve.
- Clustering requires external tools.

## Interview Tip:
Be honest about trade-offs. "PostgreSQL trades simplicity for features â€” it's more powerful but requires more knowledge."

---

## Question 5: How does PostgreSQL differ from MySQL?

## Answer:
| Feature | PostgreSQL | MySQL |
|---------|-----------|-------|
| Standards compliance | Full SQL standard | Partial |
| JSON support | JSONB (indexed, queryable) | JSON (basic) |
| Concurrency | MVCC | MVCC (InnoDB) |
| Extensibility | Custom types, functions | Limited |
| Data types | Rich (arrays, hstore, UUID) | Basic |
| ACID | Full | Full (InnoDB) |
| Licensing | PostgreSQL License | GPL |

PostgreSQL is more feature-rich; MySQL is simpler and faster for basic workloads.

## Key Points:
- PostgreSQL: more features, extensibility, standards compliance.
- MySQL: simpler, faster for basic CRUD, larger ecosystem for CMS.
- Both support ACID and MVCC (InnoDB).
- PostgreSQL has better JSON and extension support.
- Choose PostgreSQL for complex queries; MySQL for simple apps.

## Interview Tip:
"PostgreSQL for complex applications, MySQL for simple CMS-style apps. Both are excellent."

---

## Question 6: How does PostgreSQL differ from MongoDB?

## Answer:
| Feature | PostgreSQL | MongoDB |
|---------|-----------|---------|
| Model | Relational (tables) | Document (collections) |
| Schema | Fixed schema | Schema-flexible |
| Query language | SQL | MQL (MongoDB Query Language) |
| Transactions | ACID (multi-row) | ACID (multi-document, 4.0+) |
| Joins | Native JOINs | `$lookup` (aggregation) |
| Indexing | B-Tree, GIN, GiST | B-Tree, text, geospatial |
| Consistency | Strong | Eventual (tunable) |

PostgreSQL with JSONB gives you the best of both worlds.

## Key Points:
- PostgreSQL: relational with optional JSON.
- MongoDB: document-native, schema-flexible.
- PostgreSQL has stronger consistency guarantees.
- MongoDB is simpler for document-heavy workloads.
- PostgreSQL with JSONB often replaces MongoDB.

## Interview Tip:
"PostgreSQL with JSONB is often a better choice than MongoDB â€” you get relational AND document capabilities."

---

## Question 7: What types of applications are best suited for PostgreSQL?

## Answer:
- **Complex queries**: Applications with JOINs, aggregations, and analytics.
- **Data integrity**: Financial, healthcare, and e-commerce systems.
- **Geospatial**: Location-based apps (with PostGIS).
- **Full-text search**: Content management and search engines.
- **Hybrid workloads**: Relational + document data (JSONB).
- **Time-series**: IoT and monitoring (with TimescaleDB).
- **Scientific data**: Complex data types and arrays.

Not ideal for: simple key-value stores, caching (use Redis), or real-time messaging (use Kafka).

## Key Points:
- Best for complex queries and data integrity.
- Excellent for geospatial, full-text search, and hybrid data.
- Extensions expand use cases (PostGIS, TimescaleDB, pgvector).
- Not ideal for simple key-value or caching.

## Interview Tip:
"If the application needs complex queries, data integrity, and joins, PostgreSQL is the right choice."

---

## Question 8: What is ACID in PostgreSQL?

## Answer:
ACID stands for Atomicity, Consistency, Isolation, Durability â€” the four properties that guarantee database transactions are processed reliably.

- **Atomicity**: All operations in a transaction succeed or none do.
- **Consistency**: The database moves from one valid state to another.
- **Isolation**: Concurrent transactions don't interfere with each other.
- **Durability**: Committed data persists even after crashes.

```sql
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT; -- Both succeed or both fail
```

## Key Points:
- Atomicity: all-or-nothing transactions.
- Consistency: data integrity rules always enforced.
- Isolation: concurrent transactions don't interfere.
- Durability: committed data survives crashes.
- PostgreSQL fully implements all four properties.

## Interview Tip:
"The bank transfer example is perfect â€” both debits and credits must succeed or both must fail."

---

## Question 9: What is MVCC (Multi-Version Concurrency Control)?

## Answer:
MVCC allows multiple transactions to access the same data simultaneously without blocking each other. Instead of locking rows for reading, PostgreSQL creates a new version of the row when it's modified. Readers see the old version; writers create new versions.

This means readers never block writers, and writers never block readers.

## Key Points:
- Multiple versions of each row exist simultaneously.
- Readers see a consistent snapshot without blocking.
- Writers create new row versions instead of overwriting.
- Readers don't block writers; writers don't block readers.
- Old versions are cleaned up by VACUUM.

## Interview Tip:
"MVCC is why PostgreSQL can handle high concurrency â€” readers and writers work simultaneously without conflicts."

---

## Question 10: Why does PostgreSQL use MVCC?

## Answer:
Without MVCC, reads would block writes and writes would block reads â€” causing performance bottlenecks in concurrent applications. MVCC eliminates this by:
- Showing each transaction a snapshot of the database at the time it started.
- Allowing concurrent reads and writes.
- Providing consistent views without locks.

The trade-off: old row versions accumulate and must be cleaned up by VACUUM.

## Key Points:
- Eliminates read-write blocking.
- Each transaction sees a consistent snapshot.
- Enables high concurrency.
- Trade-off: requires VACUUM to clean up old versions.
- Essential for OLTP workloads with many concurrent users.

## Interview Tip:
"MVCC trades storage for concurrency â€” old versions are cleaned up by VACUUM."

---

## Part 2 (11â€“20): Database Basics

---

## Question 11: What is a database?

## Answer:
A database is an organized collection of structured data stored electronically. In PostgreSQL, a database is a container for schemas, tables, views, functions, and other objects. Each database is isolated â€” you connect to a specific database to work with its data.

```sql
CREATE DATABASE myapp;
\c myapp  -- Connect to the database
```

## Key Points:
- Organized collection of structured data.
- In PostgreSQL, a database contains schemas and objects.
- Each database is isolated from others.
- Created with `CREATE DATABASE`.
- You connect to a specific database for operations.

## Interview Tip:
"A PostgreSQL server can host multiple databases â€” each one is isolated."

---

## Question 12: What is a schema in PostgreSQL?

## Answer:
A schema is a logical container for database objects (tables, views, functions, indexes). It organizes objects within a database and controls access.

```sql
CREATE SCHEMA app;
CREATE TABLE app.users (id SERIAL PRIMARY KEY, name TEXT);
CREATE TABLE app.posts (id SERIAL PRIMARY KEY, title TEXT);

-- Search path
SET search_path TO app, public;
```

Schemas allow multiple teams or applications to share a database without conflicts.

## Key Points:
- Logical container for database objects.
- Organizes tables, views, functions, and indexes.
- Controls access and namespaces.
- Multiple schemas per database.
- `public` is the default schema.

## Interview Tip:
"Schemas are like namespaces in programming â€” they prevent naming conflicts between different parts of the application."

---

## Question 13: What is a table?

## Answer:
A table is a structured collection of data organized into rows and columns. It's the primary way to store data in a relational database.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  email VARCHAR(255) UNIQUE NOT NULL,
  created_at TIMESTAMP DEFAULT NOW()
);
```

Each table has a defined structure (schema) that governs what data can be stored.

## Key Points:
- Structured collection of rows and columns.
- Defined by columns with specific data types.
- Primary way to store data in relational databases.
- Created with `CREATE TABLE`.
- Enforces data integrity through constraints.

## Interview Tip:
"Tables are the foundation of relational databases â€” everything else builds on them."

---

## Question 14: What is a row (record)?

## Answer:
A row (also called a record or tuple) is a single entry in a table. It represents one instance of the entity the table models.

```sql
INSERT INTO users (name, email) VALUES ('Alice', 'alice@example.com');
-- This creates one row in the users table
```

Each row contains values for each column in the table.

## Key Points:
- A single entry in a table.
- Also called a record or tuple.
- Contains values for all columns.
- Created with `INSERT`.
- Each row is uniquely identified by its primary key.

## Interview Tip:
"Row = record = tuple â€” they all mean the same thing. Use whichever term the interviewer uses."

---

## Question 15: What is a column?

## Answer:
A column defines a specific attribute of the data stored in a table. Each column has a name, data type, and optional constraints.

```sql
CREATE TABLE products (
  id SERIAL PRIMARY KEY,    -- Column: id, type: integer
  name VARCHAR(100) NOT NULL, -- Column: name, type: varchar
  price DECIMAL(10,2),       -- Column: price, type: decimal
  in_stock BOOLEAN DEFAULT true -- Column: in_stock, type: boolean
);
```

## Key Points:
- Defines an attribute of the table.
- Has a name, data type, and constraints.
- Each row has a value for each column.
- Constraints enforce data integrity.
- Types determine what data can be stored.

## Interview Tip:
"Columns define the structure; rows contain the data. Together they form the table."

---

## Question 16: What is a primary key?

## Answer:
A primary key uniquely identifies each row in a table. It must be unique and cannot be NULL.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL
);
```

A table can have only one primary key. The primary key automatically creates a unique index.

## Key Points:
- Uniquely identifies each row.
- Must be unique and NOT NULL.
- Only one primary key per table.
- Automatically creates a unique index.
- Can be a single column or multiple columns (composite).

## Interview Tip:
"The primary key is the identity of each row â€” it must be unique and never null."

---

## Question 17: What is a foreign key?

## Answer:
A foreign key links one table to another by referencing the primary key of the referenced table. It enforces referential integrity â€” you can't insert a row that references a non-existent row.

```sql
CREATE TABLE posts (
  id SERIAL PRIMARY KEY,
  title TEXT NOT NULL,
  user_id INTEGER REFERENCES users(id)
);
```

Foreign keys can also cascade actions (DELETE CASCADE, UPDATE CASCADE).

## Key Points:
- References the primary key of another table.
- Enforces referential integrity.
- Prevents orphaned rows.
- Can cascade actions on delete/update.
- Creates an implicit index (sometimes).

## Interview Tip:
"Foreign keys enforce relationships between tables â€” without them, you can have orphaned data."

---

## Question 18: What is a unique constraint?

## Answer:
A unique constraint ensures all values in a column (or combination of columns) are unique across the table.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email VARCHAR(255) UNIQUE NOT NULL
);
```

Unlike primary keys, unique constraints allow NULL values (unless combined with NOT NULL).

## Key Points:
- Ensures all values in a column are unique.
- Allows NULL values (unless combined with NOT NULL).
- Creates a unique index automatically.
- Multiple unique constraints per table.
- Different from primary key (only one PK, multiple UNIQUE).

## Interview Tip:
"Unique constraints prevent duplicate values â€” emails, usernames, or any identifier that must be unique."

---

## Question 19: What is a check constraint?

## Answer:
A check constraint validates that values in a column satisfy a specific condition.

```sql
CREATE TABLE products (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL,
  price DECIMAL(10,2) CHECK (price >= 0),
  quantity INTEGER CHECK (quantity >= 0)
);
```

PostgreSQL evaluates the condition for every INSERT and UPDATE.

## Key Points:
- Validates data against a condition.
- Prevents invalid data from being inserted.
- Applied on INSERT and UPDATE.
- Can reference multiple columns.
- Named constraints for better error messages.

## Interview Tip:
"Check constraints prevent invalid data at the database level â€” don't rely solely on application validation."

---

## Question 20: What is a default constraint?

## Answer:
A default constraint provides a default value for a column when no value is specified during INSERT.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL,
  role TEXT DEFAULT 'user',
  created_at TIMESTAMP DEFAULT NOW()
);
```

The default can be a constant, function call, or expression.

## Key Points:
- Provides a default value when none is specified.
- Can be a constant or function call (e.g., `NOW()`).
- Applied automatically during INSERT.
- Doesn't affect UPDATE unless explicitly set.
- Useful for timestamps, status fields, and common values.

## Interview Tip:
"`DEFAULT NOW()` is the most common default â€” it auto-sets timestamps on insert."

---

## Part 3 (21â€“30): Data Types

---

## Question 21: What are PostgreSQL data types?

## Answer:
PostgreSQL supports a rich set of data types:
- **Numeric**: `INTEGER`, `BIGINT`, `DECIMAL`, `NUMERIC`, `REAL`, `DOUBLE PRECISION`
- **Text**: `CHAR`, `VARCHAR`, `TEXT`
- **Date/Time**: `DATE`, `TIME`, `TIMESTAMP`, `TIMESTAMPTZ`, `INTERVAL`
- **Boolean**: `BOOLEAN`
- **JSON**: `JSON`, `JSONB`
- **Arrays**: `INTEGER[]`, `TEXT[]`
- **UUID**: `UUID`
- **Network**: `INET`, `CIDR`, `MACADDR`
- **Geometric**: `POINT`, `LINE`, `POLYGON`

PostgreSQL's type system is extensible â€” you can create custom types.

## Key Points:
- Rich set of built-in types.
- JSON and JSONB for document storage.
- Arrays, UUID, network, and geometric types.
- Extensible â€” create custom types.
- Type-safe with strict type checking.

## Interview Tip:
"PostgreSQL's type system is one of its strengths â€” arrays, JSONB, UUID, and custom types set it apart."

---

## Question 22: What is the difference between `CHAR`, `VARCHAR`, and `TEXT`?

## Answer:
- **`CHAR(n)`**: Fixed-length, padded with spaces. Always stores n characters.
- **`VARCHAR(n)`**: Variable-length, up to n characters. No padding.
- **`TEXT`**: Variable-length, unlimited size. No padding.

```sql
CREATE TABLE example (
  code CHAR(5),       -- Always 5 characters
  name VARCHAR(100),  -- Up to 100 characters
  description TEXT    -- Unlimited
);
```

In practice, `TEXT` and `VARCHAR(n)` perform identically in PostgreSQL.

## Key Points:
- `CHAR(n)`: fixed-length, padded.
- `VARCHAR(n)`: variable-length with limit.
- `TEXT`: variable-length, unlimited.
- `TEXT` and `VARCHAR` have identical performance.
- Use `TEXT` unless you need a length constraint.

## Interview Tip:
"Just use `TEXT` in PostgreSQL â€” it's simpler and performs the same as `VARCHAR`."

---

## Question 23: What is the `UUID` data type?

## Answer:
UUID (Universally Unique Identifier) is a 128-bit value that's globally unique. It's generated without a database sequence, making it ideal for distributed systems.

```sql
CREATE EXTENSION IF NOT EXISTS "uuid-ossp";
CREATE TABLE users (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  name TEXT NOT NULL
);
```

Format: `550e8400-e29b-41d4-a716-446655440000`

## Key Points:
- 128-bit globally unique identifier.
- No central authority needed (distributed generation).
- Default format: `uuid_generate_v4()` (random).
- Larger than SERIAL (16 bytes vs 4 bytes).
- Great for distributed systems and APIs.

## Interview Tip:
"UUIDs are perfect for distributed systems â€” no sequence conflicts across multiple databases."

---

## Question 24: When should you use `UUID` instead of `SERIAL`?

## Answer:
Use UUID when:
- **Distributed systems**: Multiple databases generating IDs.
- **API exposure**: IDs visible to users (UUIDs aren't sequential).
- **Merging data**: Combining data from multiple sources.
- **Microservices**: Each service generates its own IDs.

Use SERIAL when:
- **Single database**: No distributed generation needed.
- **Performance**: UUIDs are larger and slower for indexing.
- **Simplicity**: Auto-incrementing integers are simpler.

## Key Points:
- UUID: distributed, non-sequential, larger.
- SERIAL: single database, sequential, smaller.
- UUID for distributed systems and API exposure.
- SERIAL for performance-critical, single-database apps.
- Consider UUID v7 (time-ordered) for better index performance.

## Interview Tip:
"UUID v7 is the modern choice â€” time-ordered like SERIAL but globally unique."

---

## Question 25: What numeric data types are available?

## Answer:
- **`SMALLINT`**: 2-byte integer (-32,768 to 32,767).
- **`INTEGER`**: 4-byte integer (-2B to 2B).
- **`BIGINT`**: 8-byte integer (very large range).
- **`DECIMAL(p,s)`**: Exact precision (financial data).
- **`NUMERIC(p,s)`**: Same as DECIMAL.
- **`REAL`**: 4-byte floating point.
- **`DOUBLE PRECISION`**: 8-byte floating point.

```sql
CREATE TABLE products (
  quantity INTEGER,
  price DECIMAL(10,2),
  weight REAL
);
```

## Key Points:
- `INTEGER` for most whole numbers.
- `BIGINT` for very large numbers.
- `DECIMAL` for exact precision (money).
- `REAL`/`DOUBLE PRECISION` for floating point.
- Avoid floating point for financial data.

## Interview Tip:
"Use DECIMAL for money â€” floating point has rounding errors."

---

## Question 26: What date and time data types does PostgreSQL support?

## Answer:
- **`DATE`**: Date only (no time).
- **`TIME`**: Time only (no date).
- **`TIMESTAMP`**: Date and time (no timezone).
- **`TIMESTAMPTZ`**: Date and time with timezone.
- **`INTERVAL`**: Duration (e.g., 2 hours, 3 days).

```sql
CREATE TABLE events (
  event_date DATE,
  start_time TIME,
  created_at TIMESTAMPTZ DEFAULT NOW(),
  duration INTERVAL
);
```

Use `TIMESTAMPTZ` for most cases â€” it handles timezone conversions automatically.

## Key Points:
- `DATE`: date only.
- `TIME`: time only.
- `TIMESTAMP`: date + time (no timezone).
- `TIMESTAMPTZ`: date + time + timezone (recommended).
- `INTERVAL`: duration for calculations.

## Interview Tip:
"Always use `TIMESTAMPTZ` â€” it handles timezone conversions correctly."

---

## Question 27: What is the `BOOLEAN` type?

## Answer:
The `BOOLEAN` type stores `true`, `false`, or `NULL`. It's a single byte of storage.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL,
  is_active BOOLEAN DEFAULT true,
  email_verified BOOLEAN DEFAULT false
);

SELECT * FROM users WHERE is_active = true;
```

PostgreSQL accepts `TRUE`, `FALSE`, `t`, `f`, `yes`, `no`, `1`, `0` as boolean values.

## Key Points:
- Stores `true`, `false`, or `NULL`.
- Single byte of storage.
- Accepts multiple input formats.
- Useful for flags and status fields.
- `IS TRUE`, `IS FALSE`, `IS NULL` for proper checks.

## Interview Tip:
"Use `IS TRUE` and `IS FALSE` instead of `= true` â€” they handle NULL correctly."

---

## Question 28: What is the `JSON` data type?

## Answer:
The `JSON` data type stores JSON text exactly asè¾“å…¥. It validates that the input is valid JSON but stores it as a text string â€” it doesn't support indexing or efficient querying.

```sql
CREATE TABLE events (
  id SERIAL PRIMARY KEY,
  data JSON
);

INSERT INTO events (data) VALUES ('{"type": "click", "page": "/home"}');
```

Use `JSONB` instead for most cases â€” it's more efficient.

## Key Points:
- Stores JSON as text (validates format).
- No indexing or efficient querying.
- Preserves formatting and duplicate keys.
- Readable but slower to query.
- Use JSONB instead for most cases.

## Interview Tip:
"There's rarely a reason to use JSON over JSONB â€” JSONB is better in almost every way."

---

## Question 29: What is the `JSONB` data type?

## Answer:
JSONB stores JSON in a decomposed binary format. It supports indexing, efficient querying, and operators for extracting and filtering data.

```sql
CREATE TABLE events (
  id SERIAL PRIMARY KEY,
  data JSONB
);

-- Query with operators
SELECT * FROM events WHERE data @> '{"type": "click"}';
SELECT * FROM events WHERE data->>'page' = '/home';

-- Index it
CREATE INDEX idx_events_data ON events USING GIN (data);
```

## Key Points:
- Binary JSON format â€” efficient storage and querying.
- Supports GIN indexing for fast lookups.
- Operators: `@>`, `->`, `->>`, `#>`, `#>>`, `?`, `@?`, `@@`.
- Doesn't preserve duplicate keys or formatting.
- Use for document storage and flexible schemas.

## Interview Tip:
"JSONB with GIN index gives you MongoDB-like document querying inside PostgreSQL."

---

## Question 30: What is the difference between `JSON` and `JSONB`?

## Answer:
| Feature | JSON | JSONB |
|---------|------|-------|
| Storage | Text (verbatim) | Binary (decomposed) |
| Indexing | No | Yes (GIN) |
| Querying | Slow (text scan) | Fast (binary scan) |
| Duplicate keys | Preserved | Removed |
| Formatting | Preserved | Not preserved |
| Performance | Slower | Faster |

Always use JSONB unless you need to preserve exact formatting or duplicate keys.

## Key Points:
- JSONB is faster for querying and indexing.
- JSON preserves formatting and duplicate keys.
- JSONB uses GIN indexes for efficient lookups.
- JSONB removes duplicate keys.
- JSONB is the default choice for most applications.

## Interview Tip:
"There's almost never a reason to use JSON over JSONB. JSONB is better in every way that matters."

---

## Part 4 (31â€“40): Basic SQL

---

## Question 31: What is SQL?

## Answer:
SQL (Structured Query Language) is the standard language for managing and querying relational databases. It's used to create, read, update, and delete data (CRUD), as well as define database structures and control access.

PostgreSQL implements the SQL standard with many extensions (JSONB, arrays, CTEs, window functions).

## Key Points:
- Standard language for relational databases.
- CRUD operations: SELECT, INSERT, UPDATE, DELETE.
- DDL: CREATE, ALTER, DROP for structures.
- DCL: GRANT, REVOKE for permissions.
- PostgreSQL extends SQL with many features.

## Interview Tip:
"SQL is the universal language of relational databases â€” knowing it well is essential."

---

## Question 32: What is the `SELECT` statement?

## Answer:
The `SELECT` statement retrieves data from one or more tables.

```sql
-- Select all columns
SELECT * FROM users;

-- Select specific columns
SELECT name, email FROM users;

-- With conditions
SELECT name FROM users WHERE is_active = true;

-- With ordering and limits
SELECT name, created_at FROM users ORDER BY created_at DESC LIMIT 10;
```

## Key Points:
- Retrieves data from tables.
- `*` selects all columns.
- `WHERE` filters rows.
- `ORDER BY` sorts results.
- `LIMIT` restricts the number of rows.

## Interview Tip:
"SELECT is the most commonly used SQL statement â€” master WHERE, ORDER BY, and LIMIT."

---

## Question 33: What is the `INSERT` statement?

## Answer:
The `INSERT` statement adds new rows to a table.

```sql
-- Single row
INSERT INTO users (name, email) VALUES ('Alice', 'alice@example.com');

-- Multiple rows
INSERT INTO users (name, email) VALUES
  ('Bob', 'bob@example.com'),
  ('Charlie', 'charlie@example.com');

-- From another table
INSERT INTO users_backup (name, email)
SELECT name, email FROM users WHERE created_at < '2024-01-01';
```

## Key Points:
- Adds new rows to a table.
- Specify columns and values.
- Can insert multiple rows at once.
- Can insert from another table's query result.
- `RETURNING` clause returns inserted data.

## Interview Tip:
"Use `RETURNING *` to get the inserted row back â€” useful for getting auto-generated IDs."

---

## Question 34: What is the `UPDATE` statement?

## Answer:
The `UPDATE` statement modifies existing rows.

```sql
-- Update specific rows
UPDATE users SET is_active = false WHERE last_login < '2024-01-01';

-- Update multiple columns
UPDATE users SET name = 'Alice Smith', role = 'admin' WHERE id = 1;

-- Update with subquery
UPDATE users SET role = 'premium'
WHERE id IN (SELECT user_id FROM subscriptions WHERE active = true);

-- Return updated rows
UPDATE users SET score = score + 10 RETURNING id, score;
```

## Key Points:
- Modifies existing rows.
- `SET` specifies columns and new values.
- `WHERE` filters which rows to update.
- Without `WHERE`, updates ALL rows.
- `RETURNING` returns affected rows.

## Interview Tip:
"Always use a WHERE clause unless you intentionally want to update every row."

---

## Question 35: What is the `DELETE` statement?

## Answer:
The `DELETE` statement removes rows from a table.

```sql
-- Delete specific rows
DELETE FROM users WHERE is_active = false;

-- Delete all rows
DELETE FROM users;

-- Delete with subquery
DELETE FROM posts WHERE user_id IN (SELECT id FROM users WHERE banned = true);

-- Return deleted rows
DELETE FROM users WHERE created_at < '2020-01-01' RETURNING *;
```

## Key Points:
- Removes rows from a table.
- `WHERE` filters which rows to delete.
- Without `WHERE`, deletes ALL rows.
- Triggers fire on DELETE.
- `RETURNING` returns deleted rows.

## Interview Tip:
"`DELETE` is logged and fires triggers. `TRUNCATE` is faster for deleting all rows."

---

## Question 36: What is the `TRUNCATE` statement?

## Answer:
`TRUNCATE` removes all rows from a table quickly. It doesn't fire row-level triggers and uses minimal logging.

```sql
TRUNCATE TABLE logs;
TRUNCATE TABLE sessions RESTART IDENTITY;
```

`RESTART IDENTITY` resets the sequence (like SERIAL) back to its initial value.

## Key Points:
- Removes all rows quickly.
- Doesn't fire row-level triggers.
- Resets sequences with `RESTART IDENTITY`.
- Faster than `DELETE` for full table clears.
- Cannot be rolled back in some configurations.

## Interview Tip:
"TRUNCATE is faster than DELETE for clearing tables â€” but DELETE is more flexible and loggable."

---

## Question 37: What is the difference between `DELETE`, `TRUNCATE`, and `DROP`?

## Answer:
| Feature | DELETE | TRUNCATE | DROP |
|---------|--------|----------|------|
| Removes | Specific rows | All rows | Entire table |
| WHERE clause | Yes | No | N/A |
| Triggers | Fires | Doesn't fire | Doesn't fire |
| Speed | Slower | Faster | Fastest |
| Rollback | Yes | Yes* | Yes* |
| Resets sequence | No | Yes (with option) | N/A |
| Structure | Keeps table | Keeps table | Removes table |

*Depends on transaction configuration.

## Key Points:
- DELETE: removes specific rows, fires triggers.
- TRUNCATE: removes all rows, faster, resets sequences.
- DROP: removes the entire table structure.
- DELETE is most flexible; TRUNCATE is fastest for full clears.
- DROP is destructive â€” the table no longer exists.

## Interview Tip:
"DELETE for specific rows, TRUNCATE for all rows, DROP to remove the table entirely."

---

## Question 38: What is the `WHERE` clause?

## Answer:
The `WHERE` clause filters rows based on conditions. It's used with SELECT, UPDATE, and DELETE.

```sql
-- Comparison operators
SELECT * FROM users WHERE age > 18;
SELECT * FROM users WHERE status = 'active';

-- Logical operators
SELECT * FROM users WHERE age > 18 AND status = 'active';
SELECT * FROM users WHERE role = 'admin' OR role = 'moderator';

-- IN, BETWEEN, LIKE
SELECT * FROM users WHERE id IN (1, 2, 3);
SELECT * FROM users WHERE age BETWEEN 18 AND 30;
SELECT * FROM users WHERE name LIKE 'A%';
```

## Key Points:
- Filters rows based on conditions.
- Comparison: `=`, `!=`, `>`, `<`, `>=`, `<=`.
- Logical: `AND`, `OR`, `NOT`.
- Special: `IN`, `BETWEEN`, `LIKE`, `IS NULL`.
- Without WHERE, operations affect all rows.

## Interview Tip:
"WHERE is the most important clause for filtering â€” master all the operators."

---

## Question 39: What is the `ORDER BY` clause?

## Answer:
`ORDER BY` sorts query results by one or more columns.

```sql
-- Ascending (default)
SELECT * FROM users ORDER BY name;

-- Descending
SELECT * FROM users ORDER BY created_at DESC;

-- Multiple columns
SELECT * FROM users ORDER BY role, name ASC;

-- Sort by expression
SELECT * FROM users ORDER BY LENGTH(name) DESC;

-- Sort by column position
SELECT name, email FROM users ORDER BY 2; -- Sorts by email
```

## Key Points:
- Sorts results by column(s).
- `ASC` for ascending (default).
- `DESC` for descending.
- Can sort by expression or column position.
- NULLS FIRST / NULLS LAST controls null placement.

## Interview Tip:
"Use column position for simple sorts: `ORDER BY 1` sorts by the first selected column."

---

## Question 40: What is the `LIMIT` clause?

## Answer:
`LIMIT` restricts the number of rows returned by a query. `OFFSET` skips a specified number of rows.

```sql
-- First 10 users
SELECT * FROM users ORDER BY id LIMIT 10;

-- Pagination: page 2 (rows 11-20)
SELECT * FROM users ORDER BY id LIMIT 10 OFFSET 10;

-- Or using FETCH (SQL standard)
SELECT * FROM users ORDER BY id
FETCH FIRST 10 ROWS ONLY
OFFSET 10 ROWS;
```

## Key Points:
- `LIMIT` restricts the number of rows returned.
- `OFFSET` skips rows before returning.
- Essential for pagination.
- `FETCH FIRST n ROWS ONLY` is the SQL standard alternative.
- Always use `ORDER BY` with `LIMIT` for consistent results.

## Interview Tip:
"LIMIT + OFFSET is the simplest pagination, but cursor-based pagination is better for large datasets."

---

## Part 5 (41â€“50): Filtering & Operators

---

## Question 41: What is the `LIKE` operator?

## Answer:
`LIKE` performs pattern matching on text values using wildcards:
- `%` matches any sequence of characters.
- `_` matches a single character.

```sql
-- Names starting with 'A'
SELECT * FROM users WHERE name LIKE 'A%';

-- Names ending with 'son'
SELECT * FROM users WHERE name LIKE '%son';

-- Names with exactly 5 characters
SELECT * FROM users WHERE name LIKE '_____';

-- Contains 'test'
SELECT * FROM users WHERE email LIKE '%test%';
```

## Key Points:
- `%` matches any characters (including none).
- `_` matches exactly one character.
- Case-sensitive by default in PostgreSQL.
- Use `ILIKE` for case-insensitive matching.
- Combine with `NOT LIKE` for exclusion.

## Interview Tip:
"`LIKE` is case-sensitive in PostgreSQL. Use `ILIKE` for case-insensitive matching."

---

## Question 42: What is `ILIKE`?

## Answer:
`ILIKE` is PostgreSQL's case-insensitive version of `LIKE`. It matches patterns regardless of case.

```sql
-- Same result in PostgreSQL
SELECT * FROM users WHERE name LIKE '%alice%';
SELECT * FROM users WHERE name ILIKE '%alice%';

-- Matches 'Alice', 'ALICE', 'alice', etc.
SELECT * FROM users WHERE name ILIKE 'alice';
```

`ILIKE` is PostgreSQL-specific â€” not portable to other databases.

## Key Points:
- Case-insensitive LIKE.
- PostgreSQL-specific (not in SQL standard).
- Matches regardless of case.
- Use for case-insensitive searches.
- For portable code, use `LOWER()` with `LIKE`.

## Interview Tip:
"`ILIKE` is convenient but PostgreSQL-specific. For portability, use `LOWER(column) LIKE '%alice%'`."

---

## Question 43: What is the `IN` operator?

## Answer:
`IN` checks if a value matches any value in a list or subquery.

```sql
-- List of values
SELECT * FROM users WHERE role IN ('admin', 'moderator', 'editor');

-- Subquery
SELECT * FROM posts WHERE user_id IN (SELECT id FROM users WHERE banned = true);

-- NOT IN for exclusion
SELECT * FROM users WHERE id NOT IN (1, 2, 3);
```

`IN` is equivalent to multiple `OR` conditions but cleaner.

## Key Points:
- Matches a value against a list or subquery.
- Cleaner than multiple `OR` conditions.
- `NOT IN` for exclusion.
- Can use subqueries for dynamic lists.
- Be careful with NULL values in `NOT IN`.

## Interview Tip:
"Watch out for NULL in `NOT IN` â€” if the list contains NULL, no rows are returned."

---

## Question 44: What is the `BETWEEN` operator?

## Answer:
`BETWEEN` checks if a value falls within an inclusive range.

```sql
-- Date range
SELECT * FROM orders WHERE created_at BETWEEN '2024-01-01' AND '2024-12-31';

-- Numeric range
SELECT * FROM products WHERE price BETWEEN 10 AND 50;

-- NOT BETWEEN for exclusion
SELECT * FROM products WHERE price NOT BETWEEN 100 AND 200;
```

`BETWEEN` is inclusive â€” both endpoints are included.

## Key Points:
- Checks if value is within an inclusive range.
- Both endpoints are included.
- Works with numbers, dates, and text.
- `NOT BETWEEN` for exclusion.
- Equivalent to `>= AND <=`.

## Interview Tip:
"`BETWEEN` is inclusive â€” `BETWEEN 1 AND 10` includes both 1 and 10."

---

## Question 45: What is the `IS NULL` operator?

## Answer:
`IS NULL` checks if a value is NULL. You can't use `= NULL` â€” NULL represents an unknown value and doesn't equal anything, including itself.

```sql
-- Check for NULL
SELECT * FROM users WHERE email IS NULL;

-- Check for NOT NULL
SELECT * FROM users WHERE email IS NOT NULL;

-- NULL-safe equality (PostgreSQL-specific)
SELECT * FROM users WHERE email IS NOT DISTINCT FROM NULL;
```

## Key Points:
- `IS NULL` checks for NULL values.
- `IS NOT NULL` checks for non-NULL.
- Never use `= NULL` â€” it doesn't work.
- NULL is not equal to anything, including itself.
- `IS NOT DISTINCT FROM` for NULL-safe comparison.

## Interview Tip:
"`= NULL` never works. Always use `IS NULL` or `IS NOT NULL`."

---

## Question 46: What is the `DISTINCT` keyword?

## Answer:
`DISTINCT` removes duplicate rows from query results.

```sql
-- Unique values
SELECT DISTINCT role FROM users;

-- Unique combinations
SELECT DISTINCT department, role FROM employees;

-- Count unique values
SELECT COUNT(DISTINCT user_id) FROM orders;
```

## Key Points:
- Removes duplicate rows from results.
- `DISTINCT ON` (PostgreSQL) for unique per group.
- `COUNT(DISTINCT column)` counts unique values.
- Applies to all selected columns.
- Can impact performance on large datasets.

## Interview Tip:
"`DISTINCT ON` is a PostgreSQL extension â€” it's great for getting one row per group."

---

## Question 47: What is the `CASE` expression?

## Answer:
`CASE` provides conditional logic in SQL â€” like if/else in programming.

```sql
SELECT name,
  CASE
    WHEN age < 18 THEN 'Minor'
    WHEN age BETWEEN 18 AND 65 THEN 'Adult'
    ELSE 'Senior'
  END AS age_group
FROM users;

-- Simple CASE
SELECT name,
  CASE role
    WHEN 'admin' THEN 'Administrator'
    WHEN 'user' THEN 'Regular User'
    ELSE 'Unknown'
  END AS role_label
FROM users;
```

## Key Points:
- Conditional logic in SQL.
- `WHEN ... THEN ... ELSE ... END` syntax.
- Can be used in SELECT, WHERE, ORDER BY.
- Useful for categorization and labeling.
- Equivalent to switch/case in programming.

## Interview Tip:
"CASE is SQL's version of if/else â€” use it for categorization and conditional logic."

---

## Question 48: What are aggregate functions?

## Answer:
Aggregate functions perform calculations across multiple rows and return a single result.

```sql
SELECT
  COUNT(*) AS total_users,
  COUNT(email) AS users_with_email,
  SUM(balance) AS total_balance,
  AVG(balance) AS avg_balance,
  MIN(created_at) AS first_user,
  MAX(created_at) AS latest_user
FROM users;
```

Common aggregates: `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`.

## Key Points:
- Perform calculations across rows.
- Return a single result.
- `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`.
- Used with `GROUP BY` for per-group aggregates.
- Ignore NULL values (except `COUNT(*)`).

## Interview Tip:
"Aggregate functions are the foundation of data analysis in SQL."

---

## Question 49: What is the difference between `COUNT(*)` and `COUNT(column)`?

## Answer:
- **`COUNT(*)`**: Counts all rows, including those with NULL values.
- **`COUNT(column)`**: Counts only non-NULL values in that column.

```sql
SELECT
  COUNT(*) AS total_rows,        -- All rows
  COUNT(email) AS emails,        -- Only non-NULL emails
  COUNT(*) - COUNT(email) AS missing_emails
FROM users;
```

`COUNT(*)` is slightly faster because it doesn't need to check for NULLs.

## Key Points:
- `COUNT(*)`: counts all rows.
- `COUNT(column)`: counts non-NULL values.
- `COUNT(*)` is faster â€” doesn't check NULLs.
- Use `COUNT(*)` for total row count.
- Use `COUNT(column)` for non-NULL count.

## Interview Tip:
"`COUNT(*)` is not slower than `COUNT(column)` â€” it's actually faster because it doesn't check for NULLs."

---

## Question 50: What SQL best practices do you follow?

## Answer:
1. **Use meaningful names**: `users` not `tbl1`, `created_at` not `col2`.
2. **Always use WHERE**: Unless you intentionally want all rows.
3. **Use parameterized queries**: Prevent SQL injection.
4. **Index frequently queried columns**: Speed up WHERE and JOIN.
5. **Avoid SELECT ***: Select only needed columns.
6. **Use aliases**: For readability in complex queries.
7. **Comment complex logic**: Explain why, not what.
8. **Test with EXPLAIN**: Check query performance.

## Key Points:
- Meaningful table and column names.
- Always filter with WHERE.
- Parameterized queries for security.
- Index for performance.
- Avoid SELECT * in production code.

## Interview Tip:
"SELECT * is convenient but wasteful â€” select only the columns you need."

---

## Part 6 (51â€“60): SQL Joins

---

## Question 51: What is an INNER JOIN?

## Answer:
`INNER JOIN` returns only rows that have matching values in both tables.

```sql
SELECT users.name, posts.title
FROM users
INNER JOIN posts ON users.id = posts.user_id;
```

Users without posts and posts without users are excluded.

## Key Points:
- Returns rows with matches in both tables.
- Excludes non-matching rows from both sides.
- Most common type of join.
- `INNER JOIN` and `JOIN` are the same.
- Use when you need related data from both tables.

## Interview Tip:
"INNER JOIN is the default â€” it only returns rows where both tables have matching data."

---

## Question 52: What is a LEFT JOIN?

## Answer:
`LEFT JOIN` returns all rows from the left table and matching rows from the right table. Non-matching rows from the right table return NULL.

```sql
SELECT users.name, posts.title
FROM users
LEFT JOIN posts ON users.id = posts.user_id;
-- Returns ALL users, even those without posts
```

## Key Points:
- Returns all rows from the left table.
- Matching rows from the right table.
- NULL for non-matching right table rows.
- Useful for finding missing relationships.
- Most commonly used join type.

## Interview Tip:
"LEFT JOIN is the most common join â€” it shows all records from the left table with matching data from the right."

---

## Question 53: What is a RIGHT JOIN?

## Answer:
`RIGHT JOIN` returns all rows from the right table and matching rows from the left table. It's the mirror of LEFT JOIN.

```sql
SELECT users.name, posts.title
FROM users
RIGHT JOIN posts ON users.id = posts.user_id;
-- Returns ALL posts, even those without users
```

You can always rewrite a RIGHT JOIN as a LEFT JOIN by swapping the table order.

## Key Points:
- Returns all rows from the right table.
- Matching rows from the left table.
- Mirror of LEFT JOIN.
- Can always be rewritten as LEFT JOIN.
- Less commonly used than LEFT JOIN.

## Interview Tip:
"RIGHT JOIN is just LEFT JOIN in reverse â€” you can always rewrite it."

---

## Question 54: What is a FULL OUTER JOIN?

## Answer:
`FULL OUTER JOIN` returns all rows from both tables. Non-matching rows from either side return NULL.

```sql
SELECT users.name, posts.title
FROM users
FULL OUTER JOIN posts ON users.id = posts.user_id;
-- Returns ALL users and ALL posts
```

Useful for finding all records in both tables, including orphans on both sides.

## Key Points:
- Returns all rows from both tables.
- NULL for non-matching rows from either side.
- Useful for finding all data and orphans.
- Can be expensive on large tables.
- PostgreSQL-specific: FULL JOIN is supported.

## Interview Tip:
"FULL OUTER JOIN shows everything â€” matching and non-matching from both sides."

---

## Question 55: What is a CROSS JOIN?

## Answer:
`CROSS JOIN` returns the Cartesian product â€” every row from the first table combined with every row from the second table.

```sql
SELECT users.name, colors.name
FROM users
CROSS JOIN colors;
-- If 3 users and 4 colors: 12 rows
```

Useful for generating combinations (e.g., all size/color options for products).

## Key Points:
- Returns the Cartesian product (all combinations).
- No ON clause needed.
- Can produce very large result sets.
- Useful for generating combinations.
- Be careful â€” 1000 x 1000 = 1,000,000 rows.

## Interview Tip:
"CROSS JOIN produces all combinations â€” use it carefully, the result set can be huge."

---

## Question 56: What is a SELF JOIN?

## Answer:
A SELF JOIN joins a table with itself â€” useful for hierarchical data like finding managers and employees.

```sql
SELECT
  e.name AS employee,
  m.name AS manager
FROM employees e
LEFT JOIN employees m ON e.manager_id = m.id;
```

Alias the table differently for each reference.

## Key Points:
- Joins a table with itself.
- Requires table aliases.
- Useful for hierarchical and recursive data.
- Same as any other join â€” just different table references.
- Used for comparing rows within the same table.

## Interview Tip:
"SELF JOIN is just joining a table to itself â€” use aliases to distinguish the two references."

---

## Question 57: What is the difference between INNER JOIN and LEFT JOIN?

## Answer:
| Feature | INNER JOIN | LEFT JOIN |
|---------|-----------|-----------|
| Left table rows | Only matching | All rows |
| Right table rows | Only matching | Matching or NULL |
| Non-matching | Excluded | Included with NULL |
| Use case | Only related data | All data + related data |

INNER JOIN is more restrictive; LEFT JOIN includes everything from the left table.

## Key Points:
- INNER JOIN: only matching rows.
- LEFT JOIN: all left rows + matching right rows.
- LEFT JOIN includes NULLs for non-matching right rows.
- Use LEFT JOIN when you need all records from the left table.
- INNER JOIN is the default join type.

## Interview Tip:
"INNER JOIN = intersection. LEFT JOIN = all left + matching right."

---

## Question 58: When would you use a FULL OUTER JOIN?

## Answer:
- **Data reconciliation**: Finding mismatches between two datasets.
- **Reporting**: Showing all records from both sides.
- **Orphan detection**: Finding records in either table without matches.
- **Merging datasets**: Combining data from two sources.

```sql
-- Find users with and without orders, and orders without users
SELECT users.name, orders.id
FROM users
FULL OUTER JOIN orders ON users.id = orders.user_id;
```

## Key Points:
- Finding mismatches between datasets.
- Showing all records from both tables.
- Detecting orphaned records.
- Merging data from different sources.
- Be careful with performance on large tables.

## Interview Tip:
"FULL OUTER JOIN is great for data reconciliation â€” it shows everything in both datasets."

---

## Question 59: How do you join more than two tables?

## Answer:
Chain multiple JOINs:

```sql
SELECT
  users.name,
  posts.title,
  comments.body
FROM users
INNER JOIN posts ON users.id = posts.user_id
INNER JOIN comments ON posts.id = comments.post_id;
```

Each JOIN adds a new table. The ON clause specifies the relationship.

## Key Points:
- Chain multiple JOINs in sequence.
- Each JOIN adds one table.
- ON clause defines the relationship.
- ORDER of joins matters for performance.
- Use table aliases for clarity.

## Interview Tip:
"When joining many tables, make sure you have indexes on the join columns."

---

## Question 60: What are common mistakes when writing JOIN queries?

## Answer:
1. **Missing ON clause**: Cross join instead of intended join.
2. **Wrong join type**: Using INNER instead of LEFT (missing rows).
3. **Missing indexes on join columns**: Slow queries.
4. **Joining too many tables**: Performance degrades.
5. **Ambiguous column names**: Column exists in multiple tables.
6. **Forgetting table aliases**: Confusing when joining same table.

## Key Points:
- Always specify the ON clause.
- Choose the right join type for your needs.
- Index join columns.
- Use table aliases when joining multiple tables.
- Be mindful of join order for performance.

## Interview Tip:
"The most common mistake is using the wrong join type â€” always think about what data you need."

---

## Part 7 (61â€“70): GROUP BY & Aggregation

---

## Question 61: What is the `GROUP BY` clause?

## Answer:
`GROUP BY` groups rows with the same values in specified columns, allowing aggregate functions to work per group.

```sql
SELECT role, COUNT(*) AS user_count
FROM users
GROUP BY role;
-- Returns one row per role with count
```

## Key Points:
- Groups rows by column values.
- Aggregate functions work per group.
- Each group returns one row.
- Non-aggregated columns must be in GROUP BY.
- Essential for summaries and reports.

## Interview Tip:
"GROUP BY turns many rows into summary rows â€” one row per group."

---

## Question 62: Why do we use `GROUP BY`?

## Answer:
To aggregate data per category â€” counts per role, totals per user, averages per department, etc.

```sql
-- Users per role
SELECT role, COUNT(*) FROM users GROUP BY role;

-- Revenue per month
SELECT DATE_TRUNC('month', created_at), SUM(amount)
FROM orders
GROUP BY DATE_TRUNC('month', created_at)
ORDER BY 1;
```

Without GROUP BY, aggregate functions work on the entire table.

## Key Points:
- Aggregate data per category.
- Create summaries and reports.
- Count, sum, average per group.
- Essential for data analysis.
- Combine with HAVING for filtered groups.

## Interview Tip:
"GROUP BY is the foundation of data analysis â€” it lets you summarize data by category."

---

## Question 63: What is the `HAVING` clause?

## Answer:
`HAVING` filters groups after aggregation â€” unlike WHERE which filters before aggregation.

```sql
-- Roles with more than 10 users
SELECT role, COUNT(*) AS user_count
FROM users
GROUP BY role
HAVING COUNT(*) > 10;
```

`HAVING` can use aggregate functions; `WHERE` cannot.

## Key Points:
- Filters groups after aggregation.
- Can use aggregate functions (COUNT, SUM, etc.).
- WHERE filters before aggregation.
- HAVING filters after aggregation.
- Often used with GROUP BY.

## Interview Tip:
"WHERE filters rows; HAVING filters groups. Use HAVING when filtering on aggregate results."

---

## Question 64: What is the difference between `WHERE` and `HAVING`?

## Answer:
| Feature | WHERE | HAVING |
|---------|-------|--------|
| Filters | Individual rows | Groups |
| Timing | Before aggregation | After aggregation |
| Aggregate functions | Cannot use | Can use |
| Without GROUP BY | Works | N/A |

```sql
-- WHERE: filter before grouping
SELECT role, COUNT(*) FROM users WHERE is_active = true GROUP BY role;

-- HAVING: filter after grouping
SELECT role, COUNT(*) FROM users GROUP BY role HAVING COUNT(*) > 10;
```

## Key Points:
- WHERE: row-level filtering before GROUP BY.
- HAVING: group-level filtering after GROUP BY.
- WHERE cannot use aggregate functions.
- HAVING can use aggregate functions.
- Use both when needed.

## Interview Tip:
"WHERE first, then GROUP BY, then HAVING â€” that's the order of operations."

---

## Question 65: What aggregate functions are available in PostgreSQL?

## Answer:
- **`COUNT()`**: Number of rows or non-NULL values.
- **`SUM()`**: Total of numeric values.
- **`AVG()`**: Average of numeric values.
- **`MIN()`**: Smallest value.
- **`MAX()`**: Largest value.
- **`ARRAY_AGG()`**: Aggregate into an array.
- **`STRING_AGG()`**: Concatenate strings.
- **`JSON_AGG()`**: Aggregate into JSON array.
- **`MODE()`**: Most frequent value.
- **`PERCENTILE_CONT()`**: Percentile calculation.

## Key Points:
- COUNT, SUM, AVG, MIN, MAX are the basics.
- ARRAY_AGG and STRING_AGG for aggregation.
- JSON_AGG for JSON aggregation.
- MODE and PERCENTILE for statistical analysis.
- PostgreSQL has rich aggregate support.

## Interview Tip:
"PostgreSQL has more aggregate functions than most databases â€” ARRAY_AGG, STRING_AGG, and JSON_AGG are particularly useful."

---

## Question 66: What is `COUNT()`?

## Answer:
`COUNT()` returns the number of rows or non-NULL values.

```sql
SELECT COUNT(*) FROM users;                    -- All rows
SELECT COUNT(email) FROM users;                -- Non-NULL emails
SELECT COUNT(DISTINCT role) FROM users;         -- Unique roles
SELECT role, COUNT(*) FROM users GROUP BY role; -- Per role
```

`COUNT(*)` is the fastest and most common variant.

## Key Points:
- `COUNT(*)`: all rows (fastest).
- `COUNT(column)`: non-NULL values.
- `COUNT(DISTINCT column)`: unique non-NULL values.
- Most commonly used aggregate function.
- Returns a BIGINT.

## Interview Tip:
"`COUNT(*)` is not slower than `COUNT(column)` â€” it's actually faster."

---

## Question 67: What is `SUM()`?

## Answer:
`SUM()` calculates the total of numeric values.

```sql
SELECT SUM(amount) FROM orders;                         -- Total revenue
SELECT user_id, SUM(amount) FROM orders GROUP BY user_id; -- Per user
SELECT SUM(amount) FROM orders WHERE status = 'completed'; -- Filtered
```

NULL values are ignored.

## Key Points:
- Calculates total of numeric values.
- Ignores NULL values.
- Works with integer, decimal, and floating-point types.
- Use with GROUP BY for per-category totals.
- Returns NULL if no rows match.

## Interview Tip:
"SUM is essential for financial reporting â€” total revenue, total costs, etc."

---

## Question 68: What is `AVG()`?

## Answer:
`AVG()` calculates the average of numeric values.

```sql
SELECT AVG(balance) FROM accounts;                         -- Overall average
SELECT role, AVG(balance) FROM accounts GROUP BY role;    -- Per role
SELECT AVG(balance) FROM accounts WHERE is_active = true; -- Filtered
```

NULL values are ignored.

## Key Points:
- Calculates average of numeric values.
- Ignores NULL values.
- Returns numeric type (may need casting).
- Use with GROUP BY for per-category averages.
- Combine with ROUND for formatting.

## Interview Tip:
"Use `ROUND(AVG(value), 2)` to format averages to 2 decimal places."

---

## Question 69: What are `MIN()` and `MAX()`?

## Answer:
`MIN()` returns the smallest value; `MAX()` returns the largest.

```sql
SELECT MIN(created_at) AS first_user, MAX(created_at) AS latest_user FROM users;
SELECT MIN(price) AS cheapest, MAX(price) AS most_expensive FROM products;
SELECT role, MIN(created_at), MAX(created_at) FROM users GROUP BY role;
```

Works with numbers, dates, and text (alphabetical order).

## Key Points:
- MIN: smallest value; MAX: largest value.
- Works with numbers, dates, and text.
- Ignores NULL values.
- Useful for finding boundaries and ranges.
- Can be used with GROUP BY.

## Interview Tip:
"MIN and MAX are great for finding the first and last records, or the cheapest and most expensive items."

---

## Question 70: How do you group data by multiple columns?

## Answer:
```sql
-- Group by department and role
SELECT department, role, COUNT(*)
FROM employees
GROUP BY department, role
ORDER BY department, role;

-- Multiple aggregations
SELECT
  department,
  role,
  COUNT(*) AS headcount,
  AVG(salary) AS avg_salary,
  MAX(salary) AS max_salary
FROM employees
GROUP BY department, role;
```

## Key Points:
- List all non-aggregated columns in GROUP BY.
- Each unique combination becomes a group.
- ORDER BY for sorted results.
- Multiple aggregations per group.
- GROUP BY order matters for readability.

## Interview Tip:
"When grouping by multiple columns, each unique combination becomes its own group."

---

## Part 8 (71â€“80): Subqueries

---

## Question 71: What is a subquery?

## Answer:
A subquery is a query nested inside another query. It's evaluated first, and its result is used by the outer query.

```sql
-- Subquery in WHERE
SELECT * FROM users
WHERE id IN (SELECT user_id FROM orders WHERE amount > 100);

-- Subquery in FROM
SELECT avg_balance FROM (
  SELECT AVG(balance) AS avg_balance FROM accounts
) AS stats;

-- Subquery in SELECT
SELECT name, (SELECT COUNT(*) FROM posts WHERE posts.user_id = users.id) AS post_count
FROM users;
```

## Key Points:
- Query inside another query.
- Evaluated first, result used by outer query.
- Can appear in WHERE, FROM, or SELECT.
- Correlated subqueries reference outer query.
- Can be replaced by JOINs in many cases.

## Interview Tip:
"Subqueries are useful but can often be rewritten as JOINs for better performance."

---

## Question 72: What is the difference between a correlated and a non-correlated subquery?

## Answer:
- **Non-correlated**: Independent of the outer query. Evaluated once.
- **Correlated**: References the outer query. Evaluated for each row.

```sql
-- Non-correlated: evaluated once
SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);

-- Correlated: evaluated for each user
SELECT * FROM users u WHERE EXISTS (
  SELECT 1 FROM orders o WHERE o.user_id = u.id
);
```

Non-correlated subqueries are generally faster.

## Key Points:
- Non-correlated: independent, evaluated once.
- Correlated: references outer query, evaluated per row.
- Correlated subqueries can be slower.
- EXISTS with correlated subquery is common.
- Most correlated subqueries can be rewritten as JOINs.

## Interview Tip:
"Correlated subqueries are like nested loops â€” the inner query runs for each outer row."

---

## Question 73: When should you use a subquery?

## Answer:
- **Filtering**: `WHERE id IN (SELECT ...)`
- **Existence check**: `WHERE EXISTS (SELECT ...)`
- **Derived tables**: `FROM (SELECT ...) AS alias`
- **Calculated columns**: `SELECT (SELECT COUNT(*) ...)`
- **Temporary results**: Complex intermediate results

For performance, consider JOINs or CTEs instead.

## Key Points:
- Filtering with IN or EXISTS.
- Derived tables for complex calculations.
- Calculated columns in SELECT.
- EXISTS for existence checks.
- Consider JOINs for better performance.

## Interview Tip:
"Use subqueries for clarity; use JOINs for performance. Know both approaches."

---

## Question 74: What are the advantages of subqueries?

## Answer:
- **Readability**: Can be clearer than complex JOINs.
- **Modularity**: Each subquery handles one piece.
- **Independence**: Can be developed and tested separately.
- **Flexibility**: Can appear in WHERE, FROM, and SELECT.
- **Logical**: Matches how we think about problems.

## Key Points:
- More readable than complex JOINs for some queries.
- Modular approach to complex logic.
- Independent of the outer query (non-correlated).
- Flexible placement in queries.
- Good for step-by-step logic.

## Interview Tip:
"Subqueries are great for readability when the logic is step-by-step."

---

## Question 75: What are the disadvantages of subqueries?

## Answer:
- **Performance**: Correlated subqueries can be slow.
- **Readability**: Deeply nested subqueries are hard to follow.
- **Optimization**: PostgreSQL may not optimize all subqueries well.
- **Alternatives**: JOINs and CTEs are often better.

## Key Points:
- Correlated subqueries execute per row (slow).
- Deep nesting reduces readability.
- Not always optimized by the planner.
- JOINs and CTEs are often better alternatives.
- Use subqueries only when they're the clearest approach.

## Interview Tip:
"If a subquery is slow, try rewriting it as a JOIN or CTE."

---

## Question 76: What is the `EXISTS` operator?

## Answer:
`EXISTS` checks if a subquery returns any rows. It's faster than `IN` for large datasets because it stops at the first match.

```sql
SELECT * FROM users u
WHERE EXISTS (
  SELECT 1 FROM orders o WHERE o.user_id = u.id
);
```

`EXISTS` returns TRUE if the subquery returns at least one row.

## Key Points:
- Returns TRUE if subquery returns any rows.
- Stops at first match (short-circuits).
- Faster than IN for large datasets.
- Often used with correlated subqueries.
- `SELECT 1` is conventional inside EXISTS.

## Interview Tip:
"`EXISTS` is usually faster than `IN` â€” it stops at the first match instead of scanning all results."

---

## Question 77: What is the `NOT EXISTS` operator?

## Answer:
`NOT EXISTS` checks that a subquery returns no rows â€” the opposite of EXISTS.

```sql
-- Users who have never placed an order
SELECT * FROM users u
WHERE NOT EXISTS (
  SELECT 1 FROM orders o WHERE o.user_id = u.id
);
```

Very useful for finding "leftovers" â€” records in one table without matches in another.

## Key Points:
- Returns TRUE if subquery returns no rows.
- Useful for finding records without matches.
- Often used with correlated subqueries.
- Performance is similar to EXISTS.
- Alternative to LEFT JOIN ... IS NULL.

## Interview Tip:
"`NOT EXISTS` and `LEFT JOIN ... IS NULL` achieve the same thing â€” choose based on readability."

---

## Question 78: What is the difference between `EXISTS` and `IN`?

## Answer:
| Feature | EXISTS | IN |
|---------|--------|-----|
| Logic | Checks existence | Checks membership |
| Performance | Stops at first match | Scans all values |
| NULL handling | Works correctly | Can have issues |
| Large datasets | Faster | Slower |
| Index usage | Good | Good |

`EXISTS` is generally preferred for large datasets and subqueries.

## Key Points:
- EXISTS stops at first match; IN scans all.
- EXISTS is usually faster for large datasets.
- IN has issues with NULL values.
- Both can use indexes.
- EXISTS with correlated subquery is common.

## Interview Tip:
"`EXISTS` is usually better than `IN` â€” it short-circuits and handles NULLs correctly."

---

## Question 79: When is `EXISTS` more efficient than `IN`?

## Answer:
- When the subquery returns many rows.
- When the outer table is large.
- When you only need to check existence, not values.
- When the subquery is correlated and can use an index.

```sql
-- EXISTS: stops at first match
SELECT * FROM users u
WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);

-- IN: scans all matching orders
SELECT * FROM users u
WHERE u.id IN (SELECT user_id FROM orders);
```

## Key Points:
- EXISTS is faster when subquery returns many rows.
- EXISTS short-circuits on first match.
- IN scans all values from subquery.
- Both benefit from indexes on join columns.
- EXISTS is preferred for existence checks.

## Interview Tip:
"If you're just checking 'does this exist?', use EXISTS â€” it's faster."

---

## Question 80: What are common subquery optimization techniques?

## Answer:
1. **Use EXISTS instead of IN**: Short-circuits on first match.
2. **Add indexes on subquery columns**: Speed up joins.
3. **Rewrite as JOIN**: Often faster than correlated subqueries.
4. **Use CTEs**: Better readability and sometimes better performance.
5. **Avoid correlated subqueries when possible**: They execute per row.

## Key Points:
- EXISTS over IN for large datasets.
- Index subquery join columns.
- Rewrite correlated subqueries as JOINs.
- CTEs for readability and potential optimization.
- Test with EXPLAIN ANALYZE.

## Interview Tip:
"EXPLAIN ANALYZE is your best friend â€” measure, don't guess."

---

## Part 9 (81â€“90): Common Table Expressions (CTEs)

---

## Question 81: What is a Common Table Expression (CTE)?

## Answer:
A CTE is a named temporary result set defined with the `WITH` clause. It exists for the duration of a single query and can be referenced multiple times.

```sql
WITH active_users AS (
  SELECT id, name, email
  FROM users
  WHERE is_active = true
)
SELECT * FROM active_users WHERE name LIKE 'A%';
```

CTEs make complex queries more readable by breaking them into named steps.

## Key Points:
- Named temporary result set.
- Defined with `WITH` clause.
- Exists for one query.
- Can be referenced multiple times.
- Improves readability of complex queries.

## Interview Tip:
"CTEs are like variables for queries â€” name a result and reuse it."

---

## Question 82: Why use a CTE instead of a subquery?

## Answer:
- **Readability**: Named steps are easier to follow.
- **Reusability**: Reference the CTE multiple times in the same query.
- **Modularity**: Break complex logic into understandable pieces.
- **Recursion**: CTEs support recursive queries.
- **Debugging**: Test each CTE independently.

```sql
-- Hard to read with subqueries
SELECT * FROM (
  SELECT user_id, COUNT(*) as order_count FROM orders GROUP BY user_id
) oc
JOIN users u ON oc.user_id = u.id
WHERE oc.order_count > 5;

-- Clear with CTE
WITH order_counts AS (
  SELECT user_id, COUNT(*) as order_count
  FROM orders GROUP BY user_id
)
SELECT u.name, oc.order_count
FROM users u
JOIN order_counts oc ON u.id = oc.user_id
WHERE oc.order_count > 5;
```

## Key Points:
- More readable than nested subqueries.
- Reusable within the same query.
- Supports recursive queries.
- Easier to debug and test.
- Cleaner step-by-step logic.

## Interview Tip:
"CTEs turn complex queries into readable, step-by-step logic."

---

## Question 83: What is the `WITH` clause?

## Answer:
The `WITH` clause defines CTEs at the beginning of a query. Multiple CTEs can be defined, separated by commas.

```sql
WITH
  active_users AS (
    SELECT * FROM users WHERE is_active = true
  ),
  recent_orders AS (
    SELECT * FROM orders WHERE created_at > NOW() - INTERVAL '7 days'
  )
SELECT u.name, COUNT(o.id) AS order_count
FROM active_users u
JOIN recent_orders o ON u.id = o.user_id
GROUP BY u.name;
```

## Key Points:
- Defines CTEs at query start.
- Multiple CTEs separated by commas.
- Each CTE can reference previous CTEs.
- CTEs are available to the main query.
- Can be chained for complex logic.

## Interview Tip:
"WITH is the entry point for CTEs â€” define them first, then use them in the main query."

---

## Question 84: What are recursive CTEs?

## Answer:
Recursive CTEs reference themselves, allowing traversal of hierarchical data (org charts, tree structures, graphs).

```sql
WITH RECURSIVE org_chart AS (
  -- Base case: top-level manager
  SELECT id, name, manager_id, 1 AS level
  FROM employees WHERE manager_id IS NULL

  UNION ALL

  -- Recursive case: employees under managers
  SELECT e.id, e.name, e.manager_id, oc.level + 1
  FROM employees e
  JOIN org_chart oc ON e.manager_id = oc.id
)
SELECT * FROM org_chart ORDER BY level, name;
```

## Key Points:
- CTE that references itself.
- Base case + recursive case pattern.
- Uses `UNION ALL` to combine results.
- Essential for hierarchical data traversal.
- `SEARCH` and `CYCLE` clauses for ordering and loop detection.

## Interview Tip:
"Recursive CTEs are the SQL way to traverse trees â€” org charts, categories, threads."

---

## Question 85: When would you use a recursive CTE?

## Answer:
- **Org charts**: Finding all employees under a manager.
- **Category trees**: Traversing parent-child categories.
- **Threaded comments**: Finding all replies to a comment.
- **Graph traversal**: Finding paths between nodes.
- **Bill of materials**: Finding all components in a product.
- **Date series**: Generating a series of dates.

## Key Points:
- Hierarchical data traversal.
- Tree and graph structures.
- Threaded data (comments, forums).
- Generating sequences.
- Finding paths in networks.

## Interview Tip:
"If the data has a parent-child relationship, a recursive CTE is probably the answer."

---

## Question 86: What are the advantages of CTEs?

## Answer:
- **Readability**: Named steps make complex queries clear.
- **Reusability**: Reference multiple times in the same query.
- **Modularity**: Break logic into testable pieces.
- **Recursion**: Handle hierarchical data.
- **Maintainability**: Easier to modify and debug.
- **Optimization**: PostgreSQL can optimize CTEs (since v12).

## Key Points:
- Named, readable, reusable query blocks.
- Recursive CTEs for hierarchical data.
- Modular approach to complex queries.
- PostgreSQL 12+ inlines CTEs for better performance.
- Easier to maintain than nested subqueries.

## Interview Tip:
"CTEs are the modern approach to complex SQL â€” use them instead of deeply nested subqueries."

---

## Question 87: What are the disadvantages of CTEs?

## Answer:
- **Performance (pre-v12)**: CTEs were optimization fences.
- **Overuse**: Simple queries don't need CTEs.
- **Materialization**: Some CTEs materialize unnecessarily.
- **Recursion limits**: Recursive CTEs have depth limits.

Since PostgreSQL 12, CTEs are inlined by default (like views), improving performance.

## Key Points:
- Pre-v12: CTEs were materialized (slower).
- v12+: CTEs are inlined (faster).
- Overuse adds unnecessary complexity.
- Recursive CTEs have depth limits.
- Use CTEs when they improve clarity.

## Interview Tip:
"PostgreSQL 12+ inlines CTEs by default â€” the old performance concern is mostly gone."

---

## Question 88: How do CTEs improve query readability?

## Answer:
CTEs break complex queries into named, logical steps:

```sql
-- Hard to read
SELECT u.name, COUNT(o.id) FROM users u JOIN orders o ON u.id = o.user_id WHERE o.created_at > NOW() - INTERVAL '30 days' GROUP BY u.name HAVING COUNT(o.id) > 5;

-- Readable with CTEs
WITH recent_orders AS (
  SELECT * FROM orders WHERE created_at > NOW() - INTERVAL '30 days'
),
active_buyers AS (
  SELECT user_id, COUNT(*) AS order_count
  FROM recent_orders GROUP BY user_id HAVING COUNT(*) > 5
)
SELECT u.name, ab.order_count
FROM users u JOIN active_buyers ab ON u.id = ab.user_id;
```

## Key Points:
- Each CTE has a clear, descriptive name.
- Complex logic broken into steps.
- Easy to understand the flow.
- Each step can be tested independently.
- Comments can be added per CTE.

## Interview Tip:
"CTEs turn a wall of SQL into readable, named steps."

---

## Question 89: What performance considerations exist when using CTEs?

## Answer:
- **PostgreSQL 12+**: CTEs are inlined by default (fast).
- **Recursive CTEs**: Can be slow for deep hierarchies.
- **Multiple references**: Pre-12 materialized; 12+ may inline.
- **`MATERIALIZED` hint**: Force materialization when needed.

```sql
-- Force materialization (PostgreSQL 12+)
WITH my_cte AS MATERIALIZED (
  SELECT * FROM large_table WHERE ...
)
SELECT * FROM my_cte;
```

## Key Points:
- v12+ inlines CTEs by default.
- Use MATERIALIZED to force materialization.
- Recursive CTEs can be slow for deep data.
- Test with EXPLAIN ANALYZE.
- CTEs are generally well-optimized.

## Interview Tip:
"Use EXPLAIN ANALYZE to check if your CTE is being inlined or materialized."

---

## Question 90: What are common real-world use cases for CTEs?

## Answer:
- **Hierarchical data**: Org charts, category trees.
- **Aggregation**: Pre-aggregate data before joining.
- **Data transformation**: Step-by-step data cleaning.
- **Running totals**: Cumulative calculations.
- **Ranking**: Top N per group.
- **Recursive traversal**: Finding paths and relationships.

## Key Points:
- Hierarchical traversal with recursive CTEs.
- Pre-aggregation before joins.
- Data transformation pipelines.
- Running totals and rankings.
- Complex reporting queries.

## Interview Tip:
"CTEs are everywhere in production SQL â€” aggregation, hierarchy, ranking, and transformation."

---

## Part 10 (91â€“100): Window Functions

---

## Question 91: What are window functions?

## Answer:
Window functions perform calculations across a set of rows related to the current row, without collapsing them (unlike GROUP BY).

```sql
SELECT
  name,
  department,
  salary,
  AVG(salary) OVER (PARTITION BY department) AS dept_avg,
  ROW_NUMBER() OVER (ORDER BY salary DESC) AS rank
FROM employees;
```

Each row keeps its identity while also showing the window calculation.

## Key Points:
- Calculate across related rows without collapsing.
- `OVER()` clause defines the window.
- `PARTITION BY` groups the window.
- `ORDER BY` orders within the window.
- Rows keep their identity (unlike GROUP BY).

## Interview Tip:
"Window functions are like GROUP BY without losing individual rows â€” incredibly powerful for analytics."

---

## Question 92: How do window functions differ from aggregate functions?

## Answer:
| Feature | Aggregate Functions | Window Functions |
|---------|-------------------|-----------------|
| Result rows | One per group | One per input row |
| GROUP BY | Required | Not required |
| Row identity | Lost | Preserved |
| Use case | Summary reports | Analytics with detail |

```sql
-- Aggregate: one row per department
SELECT department, AVG(salary) FROM employees GROUP BY department;

-- Window: every row keeps its identity
SELECT name, department, salary, AVG(salary) OVER (PARTITION BY department) FROM employees;
```

## Key Points:
- Aggregate collapses rows; window preserves them.
- Window functions don't need GROUP BY.
- Each row keeps its original data.
- Window functions are for analytics.
- Use aggregate for summaries; window for rankings and running totals.

## Interview Tip:
"Aggregate = summary. Window = analytics with detail. Know when to use each."

---

## Question 93: What is the `OVER()` clause?

## Answer:
The `OVER()` clause defines the window for window functions. It can include `PARTITION BY` and `ORDER BY`.

```sql
-- No partition: entire result set
ROW_NUMBER() OVER (ORDER BY salary DESC)

-- Partition: per department
AVG(salary) OVER (PARTITION BY department)

-- Partition + order: per department, ordered by salary
RANK() OVER (PARTITION BY department ORDER BY salary DESC)
```

## Key Points:
- Defines the window for calculation.
- `PARTITION BY`: groups the window.
- `ORDER BY`: orders within the window.
- Can be empty: entire result set.
- Required for all window functions.

## Interview Tip:
"`OVER()` is what makes it a window function â€” without it, it's just a regular function."

---

## Question 94: What is `ROW_NUMBER()`?

## Answer:
`ROW_NUMBER()` assigns a unique sequential number to each row within the partition.

```sql
SELECT
  name,
  department,
  salary,
  ROW_NUMBER() OVER (PARTITION BY department ORDER BY salary DESC) AS rn
FROM employees;
-- Each department: 1, 2, 3, ... (no ties)
```

Ties get arbitrary but unique numbers.

## Key Points:
- Assigns unique sequential numbers.
- No ties â€” each row gets a distinct number.
- Order determined by ORDER BY in OVER().
- Great for pagination and deduplication.
- Always returns unique numbers.

## Interview Tip:
"`ROW_NUMBER()` is perfect for pagination and removing duplicates â€” it always gives unique numbers."

---

## Question 95: What is `RANK()`?

## Answer:
`RANK()` assigns a rank to each row, with ties getting the same rank. The next rank skips numbers.

```sql
SELECT
  name,
  salary,
  RANK() OVER (ORDER BY salary DESC) AS rank
FROM employees;
-- Salaries: 100, 90, 90, 80 â†’ Ranks: 1, 2, 2, 4 (skips 3)
```

## Key Points:
- Assigns rank with ties getting same rank.
- Next rank skips numbers after ties.
- `1, 2, 2, 4` (not `1, 2, 2, 3`).
- Good for "top N" queries where ties matter.
- Ties get identical ranks.

## Interview Tip:
"`RANK()` skips numbers after ties â€” `1, 2, 2, 4` not `1, 2, 2, 3`."

---

## Question 96: What is `DENSE_RANK()`?

## Answer:
`DENSE_RANK()` assigns a rank to each row, with ties getting the same rank. Unlike RANK, it doesn't skip numbers.

```sql
SELECT
  name,
  salary,
  DENSE_RANK() OVER (ORDER BY salary DESC) AS dense_rank
FROM employees;
-- Salaries: 100, 90, 90, 80 â†’ DENSE_RANK: 1, 2, 2, 3
```

## Key Points:
- Assigns rank with ties getting same rank.
- Does NOT skip numbers after ties.
- `1, 2, 2, 3` (not `1, 2, 2, 4`).
- Better for "top N" where you don't want gaps.
- Continuous ranking without gaps.

## Interview Tip:
"`DENSE_RANK()` doesn't skip numbers â€” `1, 2, 2, 3` not `1, 2, 2, 4`."

---

## Question 97: What is `LEAD()`?

## Answer:
`LEAD()` accesses the next row's value within the partition.

```sql
SELECT
  name,
  salary,
  LEAD(salary) OVER (ORDER BY salary DESC) AS next_salary
FROM employees;
-- Shows the salary of the next higher-paid employee
```

Useful for comparing consecutive rows (e.g., time series).

## Key Points:
- Accesses the next row's value.
- Default: NULL if no next row.
- Custom default: `LEAD(salary, 1, 0)`.
- Great for time series analysis.
- Compare consecutive values.

## Interview Tip:
"`LEAD` looks forward; `LAG` looks backward. Both are essential for time series analysis."

---

## Question 98: What is `LAG()`?

## Answer:
`LAG()` accesses the previous row's value within the partition.

```sql
SELECT
  date,
  revenue,
  LAG(revenue) OVER (ORDER BY date) AS prev_revenue,
  revenue - LAG(revenue) OVER (ORDER BY date) AS daily_change
FROM daily_revenue;
-- Compare each day's revenue to the previous day
```

## Key Points:
- Accesses the previous row's value.
- Default: NULL if no previous row.
- Custom default: `LAG(salary, 1, 0)`.
- Great for comparing to previous periods.
- Calculate changes, growth, differences.

## Interview Tip:
"`LAG` looks backward â€” perfect for comparing to the previous period."

---

## Question 99: What are partitioning and ordering in window functions?

## Answer:
- **`PARTITION BY`**: Divides the window into groups (like GROUP BY for windows).
- **`ORDER BY`**: Orders rows within the window.

```sql
-- Per department, ordered by salary
RANK() OVER (PARTITION BY department ORDER BY salary DESC)

-- Entire result set, ordered by date
SUM(amount) OVER (ORDER BY date)
```

PARTITION BY resets the calculation for each group.

## Key Points:
- `PARTITION BY`: groups the window.
- `ORDER BY`: orders within the window.
- PARTITION BY resets the calculation per group.
- ORDER BY is required for ranking and running totals.
- Both are optional in `OVER()`.

## Interview Tip:
"`PARTITION BY` is like GROUP BY for window functions â€” it divides the calculation into groups."

---

## Question 100: When would you use window functions in real-world applications?

## Answer:
- **Ranking**: Top N per category (best-selling products per category).
- **Running totals**: Cumulative revenue over time.
- **Moving averages**: 7-day average sales.
- **Year-over-year growth**: Comparing current period to previous.
- **Deduplication**: Keep first/last record per group.
- **Pagination**: Row numbers for offset-based pagination.
- **Gap detection**: Find missing dates or sequences.

## Key Points:
- Ranking: top N per group.
- Running totals and moving averages.
- Period-over-period comparisons.
- Deduplication and pagination.
- Gap detection in sequences.

## Interview Tip:
"Window functions are the Swiss Army knife of SQL analytics â€” ranking, totals, growth, and comparisons."

---

## Part 11 (101â€“110): Indexing

---

## Question 101: What is an index in PostgreSQL?

## Answer:
An index is a data structure that speeds up data retrieval by allowing the database to find rows without scanning the entire table. Think of it like an index in a book â€” it tells you where to find specific content.

```sql
CREATE INDEX idx_users_email ON users (email);
```

Without an index, PostgreSQL must scan every row (sequential scan). With an index, it can jump directly to matching rows.

## Key Points:
- Data structure for fast lookups.
- Speeds up WHERE, JOIN, and ORDER BY.
- Costs storage and write performance.
- Created with `CREATE INDEX`.
- Essential for query performance.

## Interview Tip:
"Indexes are the single most important optimization â€” most slow queries are missing an index."

---

## Question 102: Why are indexes important?

## Answer:
Without indexes, PostgreSQL scans every row for every query (sequential scan). On a table with 1 million rows, that's 1 million row reads per query. With an index, PostgreSQL can find matching rows in logarithmic time.

Indexes are the difference between millisecond and second response times.

## Key Points:
- Without indexes: sequential scan (slow on large tables).
- With indexes: index scan (fast).
- Essential for WHERE, JOIN, ORDER BY performance.
- The most common cause of slow queries is missing indexes.
- Trade-off: indexes slow down writes.

## Interview Tip:
"If a query is slow, the first thing to check is whether the right index exists."

---

## Question 103: How does a B-Tree index work?

## Answer:
A B-Tree (balanced tree) index organizes data in a tree structure. Each node contains keys and pointers. The tree is balanced â€” all leaf nodes are at the same depth, ensuring consistent lookup time.

```
         [50]
        /    \
    [20, 30]  [60, 80]
    / | \      / | \
  [10] [25] [35] [55] [70] [90]
```

B-Tree is the default index type in PostgreSQL and works for equality and range queries.

## Key Points:
- Default index type in PostgreSQL.
- Balanced tree structure.
- O(log n) lookup time.
- Supports equality (`=`, `IN`) and range (`<`, `>`, `BETWEEN`) queries.
- Works with most data types.

## Interview Tip:
"B-Tree is the default â€” it handles equality and range queries efficiently."

---

## Question 104: What is a Hash index?

## Answer:
A Hash index uses a hash function to map keys to index entries. It's fast for equality lookups but doesn't support range queries.

```sql
CREATE INDEX idx_users_email_hash ON users USING HASH (email);
```

Hash indexes were improved in PostgreSQL 10+ and are now WAL-logged (crash-safe). Use B-Tree unless you specifically need hash performance.

## Key Points:
- Hash function maps keys to entries.
- Fast for equality (`=`) only.
- No range query support.
- Crash-safe since PostgreSQL 10.
- Use B-Tree unless hash is specifically needed.

## Interview Tip:
"Hash indexes are faster for equality but don't support ranges â€” B-Tree is usually better."

---

## Question 105: What is a GIN (Generalized Inverted Index)?

## Answer:
A GIN index indexes composite values â€” arrays, JSONB, full-text search, and hstore. It maps each element to the rows that contain it.

```sql
-- JSONB index
CREATE INDEX idx_events_data ON events USING GIN (data);

-- Full-text search index
CREATE INDEX idx_posts_search ON posts USING GIN (to_tsvector('english', content));

-- Array index
CREATE INDEX idx_products_tags ON products USING GIN (tags);
```

## Key Points:
- Indexes composite values (arrays, JSONB, full-text).
- Maps each element to containing rows.
- Essential for JSONB queries.
- Essential for full-text search.
- Slower to build but fast for queries.

## Interview Tip:
"If you're querying JSONB or arrays, you need a GIN index."

---

## Question 106: What is a GiST (Generalized Search Tree) index?

## Answer:
A GiST index supports complex data types and queries â€” geometric data, full-text search, ranges, and proximity searches.

```sql
-- Geospatial index (PostGIS)
CREATE INDEX idx_locations_geom ON locations USING GIST (geom);

-- Range index
CREATE INDEX idx_events_daterange ON events USING GIST (daterange);
```

GiST is the foundation for PostGIS and range type indexing.

## Key Points:
- Supports complex data types.
- Geospatial, range, and full-text queries.
- Foundation for PostGIS.
- More flexible than B-Tree.
- Used for proximity and containment queries.

## Interview Tip:
"If you're using PostGIS or range types, you need a GiST index."

---

## Question 107: When should you use a BRIN index?

## Answer:
BRIN (Block Range INdex) stores the minimum and maximum values for each block of the table. It's great for large tables where data is naturally ordered (timestamps, auto-increment IDs).

```sql
CREATE INDEX idx_logs_created ON logs USING BRIN (created_at);
```

BRIN is tiny compared to B-Tree â€” perfect for append-only tables like logs.

## Key Points:
- Stores min/max per block.
- Tiny index size (kilobytes vs megabytes).
- Great for naturally ordered data (timestamps).
- Perfect for append-only tables (logs, events).
- Much smaller than B-Tree for large tables.

## Interview Tip:
"BRIN is perfect for log tables â€” tiny index, fast scans on timestamp queries."

---

## Question 108: What is a composite index?

## Answer:
A composite index covers multiple columns in one index.

```sql
CREATE INDEX idx_users_role_active ON users (role, is_active);
```

The column order matters â€” the index can be used for queries that filter on the leading columns.

```sql
-- Uses the index
SELECT * FROM users WHERE role = 'admin';
SELECT * FROM users WHERE role = 'admin' AND is_active = true;

-- May NOT use the index (skips leading column)
SELECT * FROM users WHERE is_active = true;
```

## Key Points:
- Index on multiple columns.
- Column order matters (leftmost prefix rule).
- Query must include leading columns to use index.
- More efficient than multiple single-column indexes.
- Reduces index count and storage.

## Interview Tip:
"Put the most selective column first in a composite index."

---

## Question 109: What is a partial index?

## Answer:
A partial index indexes only rows that match a condition â€” smaller and faster than a full index.

```sql
-- Only index active users
CREATE INDEX idx_active_users ON users (email) WHERE is_active = true;

-- Only index unpaid orders
CREATE INDEX idx_unpaid_orders ON orders (user_id) WHERE status = 'pending';
```

Perfect for queries that always filter on a specific condition.

## Key Points:
- Indexes only matching rows.
- Smaller than full indexes.
- Faster to build and maintain.
- Perfect for filtered queries.
- Reduces index storage and write overhead.

## Interview Tip:
"If you always query `WHERE status = 'pending'`, use a partial index â€” it's smaller and faster."

---

## Question 110: What is a covering index?

## Answer:
A covering index includes all columns needed by a query, allowing PostgreSQL to answer the query from the index alone (index-only scan).

```sql
-- Covering index for a common query
CREATE INDEX idx_users_email_name ON users (email) INCLUDE (name);

-- Query served entirely from index
SELECT name FROM users WHERE email = 'alice@example.com';
```

PostgreSQL 11+ supports `INCLUDE` for covering columns.

## Key Points:
- Includes all columns needed by a query.
- Enables index-only scans.
- `INCLUDE` clause for extra columns (v11+).
- Eliminates table access.
- Dramatically faster for read-heavy queries.

## Interview Tip:
"Covering indexes eliminate table access â€” the query is answered entirely from the index."

---

## Part 12 (111â€“120): Index Optimization

---

## Question 111: How do you decide which columns should be indexed?

## Answer:
Index columns that:
1. **Appear in WHERE clauses**: Frequent filtering.
2. **Appear in JOIN conditions**: Foreign keys.
3. **Appear in ORDER BY**: Sorting.
4. **Appear in GROUP BY**: Aggregation.
5. **Have high cardinality**: Many distinct values.

Don't index:
- Small tables (sequential scan is fast).
- Columns rarely queried.
- Columns with low cardinality (boolean, status with few values).

## Key Points:
- WHERE, JOIN, ORDER BY, GROUP BY columns.
- High cardinality columns (many distinct values).
- Foreign keys (often used in JOINs).
- Avoid indexing small tables.
- Avoid low-cardinality columns.

## Interview Tip:
"Index columns that appear in WHERE, JOIN, and ORDER BY â€” they're the most common performance bottlenecks."

---

## Question 112: What are the disadvantages of adding too many indexes?

## Answer:
- **Write performance**: Each index must be updated on INSERT, UPDATE, DELETE.
- **Storage**: Indexes consume disk space.
- **Maintenance**: VACUUM and REINDEX take longer.
- **Planner overhead**: Too many indexes confuse the query planner.
- **Memory**: Indexes consume shared_buffers.

Balance read performance with write overhead.

## Key Points:
- Slows down INSERT, UPDATE, DELETE.
- Consumes disk space.
- Increases maintenance time.
- Can confuse the query planner.
- Balances read performance with write overhead.

## Interview Tip:
"Every index speeds up reads but slows down writes â€” find the right balance."

---

## Question 113: How do indexes affect INSERT, UPDATE, and DELETE operations?

## Answer:
Every index must be updated when data changes:
- **INSERT**: New entry added to every index.
- **UPDATE**: Old entry removed, new entry added (if indexed column changes).
- **DELETE**: Entry removed from every index.

More indexes = slower writes. This is why you shouldn't index every column.

## Key Points:
- Each index is updated on data changes.
- INSERT: add to all indexes.
- UPDATE: remove and add if indexed column changes.
- DELETE: remove from all indexes.
- More indexes = slower writes.

## Interview Tip:
"Indexes are a trade-off â€” they speed up reads but slow down writes."

---

## Question 114: What is index selectivity?

## Answer:
Selectivity measures how many distinct values an index has relative to the total number of rows. High selectivity = many distinct values = index is effective. Low selectivity = few distinct values = index is less useful.

```sql
-- High selectivity: email (mostly unique)
CREATE INDEX idx_users_email ON users (email);

-- Low selectivity: is_active (only 2 values)
-- Index won't help much
```

A common rule: index columns with >10% distinct values.

## Key Points:
- Measures distinct values vs total rows.
- High selectivity: effective index.
- Low selectivity: less effective index.
- Boolean columns: low selectivity (2 values).
- Unique columns: highest selectivity.

## Interview Tip:
"Highly selective indexes (unique or near-unique) are the most effective."

---

## Question 115: How do you identify unused indexes?

## Answer:
Query `pg_stat_user_indexes`:

```sql
SELECT
  schemaname, relname, indexrelname,
  idx_scan AS times_used,
  pg_size_pretty(pg_relation_size(indexrelid)) AS size
FROM pg_stat_user_indexes
WHERE idx_scan = 0
ORDER BY pg_relation_size(indexrelid) DESC;
```

Indexes with 0 scans are unused â€” consider removing them.

## Key Points:
- `pg_stat_user_indexes` tracks usage.
- `idx_scan = 0` means never used.
- Remove unused indexes to improve write performance.
- Monitor regularly in production.
- Some indexes are used rarely but are critical when needed.

## Interview Tip:
"Unused indexes are dead weight â€” they slow down writes without helping reads."

---

## Question 116: How do you remove unnecessary indexes?

## Answer:
```sql
-- Check before dropping
SELECT * FROM pg_stat_user_indexes WHERE idx_scan = 0;

-- Drop the index
DROP INDEX idx_unused_index;

-- Or drop concurrently (no lock)
DROP INDEX CONCURRENTLY idx_unused_index;
```

Always verify an index is truly unused before dropping it.

## Key Points:
- `DROP INDEX` to remove an index.
- `DROP INDEX CONCURRENTLY` to avoid locking.
- Verify usage before dropping.
- Monitor after dropping to confirm no impact.
- Some indexes are rarely used but critical when needed.

## Interview Tip:
"Use `DROP INDEX CONCURRENTLY` in production â€” it doesn't lock the table."

---

## Question 117: What is index fragmentation?

## Answer:
Over time, as rows are inserted, updated, and deleted, indexes become fragmented â€” pages are partially filled or out of order. This increases I/O and slows down queries.

PostgreSQL's VACUUM helps, but eventually you need `REINDEX`.

## Key Points:
- Indexes become fragmented over time.
- Pages partially filled or out of order.
- Increases I/O and slows queries.
- VACUUM helps but doesn't fully fix it.
- `REINDEX` rebuilds the index.

## Interview Tip:
"Monitor index bloat with `pgstatindex()` â€” high bloat means it's time to REINDEX."

---

## Question 118: How do you rebuild an index?

## Answer:
```sql
-- Rebuild (locks the index)
REINDEX INDEX idx_users_email;

-- Rebuild concurrently (no lock, PostgreSQL 12+)
REINDEX INDEX CONCURRENTLY idx_users_email;

-- Rebuild all indexes on a table
REINDEX TABLE users;
```

`REINDEX CONCURRENTLY` is preferred in production â€” it doesn't block queries.

## Key Points:
- `REINDEX` rebuilds an index.
- `REINDEX CONCURRENTLY` doesn't lock (v12+).
- Rebuild when fragmentation is high.
- Can also be done with `CREATE INDEX CONCURRENTLY` + `DROP INDEX`.
- Schedule during low-traffic periods.

## Interview Tip:
"Use `REINDEX CONCURRENTLY` in production â€” it rebuilds without blocking queries."

---

## Question 119: How do you monitor index performance?

## Answer:
```sql
-- Index usage stats
SELECT * FROM pg_stat_user_indexes;

-- Index size
SELECT
  indexrelname,
  pg_size_pretty(pg_relation_size(indexrelid)) AS size
FROM pg_stat_user_indexes;

-- Index bloat
SELECT * FROM pgstatindex('idx_users_email');
```

Monitor regularly to catch unused, bloated, or missing indexes.

## Key Points:
- `pg_stat_user_indexes` for usage stats.
- `pg_relation_size` for index size.
- `pgstatindex()` for detailed bloat info.
- Monitor in production regularly.
- Set up alerts for unusual patterns.

## Interview Tip:
"Monitor index usage weekly â€” catch unused indexes and missing indexes early."

---

## Question 120: What indexing best practices do you follow?

## Answer:
1. **Index foreign keys**: Always â€” they're used in JOINs.
2. **Index WHERE columns**: Frequently filtered columns.
3. **Use composite indexes**: For multi-column queries.
4. **Use partial indexes**: For filtered queries.
5. **Monitor usage**: Remove unused indexes.
6. **Use covering indexes**: For read-heavy queries.
7. **Avoid over-indexing**: Balance read/write performance.
8. **Use BRIN for append-only tables**: Tiny and efficient.

## Key Points:
- Always index foreign keys.
- Index frequently queried columns.
- Composite indexes for multi-column queries.
- Partial indexes for filtered queries.
- Monitor and remove unused indexes.

## Interview Tip:
"Index foreign keys, index WHERE columns, monitor usage â€” that's the indexing trifecta."

---

## Part 13 (121â€“130): Query Optimization

---

## Question 121: What is the `EXPLAIN` command?

## Answer:
`EXPLAIN` shows the execution plan PostgreSQL would use for a query â€” without actually running it.

```sql
EXPLAIN SELECT * FROM users WHERE email = 'alice@example.com';
-- Seq Scan on users  (cost=0.00..1234.00 rows=1 width=100)
--   Filter: (email = 'alice@example.com')
```

It shows which indexes are used, how tables are joined, and estimated costs.

## Key Points:
- Shows the execution plan without running the query.
- Displays estimated costs, rows, and width.
- Shows which indexes are used.
- Shows join strategies.
- Essential for query optimization.

## Interview Tip:
"EXPLAIN is the first tool for understanding why a query is slow."

---

## Question 122: What is `EXPLAIN ANALYZE`?

## Answer:
`EXPLAIN ANALYZE` actually runs the query and shows the actual execution plan with real timings.

```sql
EXPLAIN ANALYZE SELECT * FROM users WHERE email = 'alice@example.com';
-- Seq Scan on users  (cost=0.00..1234.00 rows=1 width=100) (actual time=0.01..12.34 rows=1 loops=1)
-- Planning Time: 0.1 ms
-- Execution Time: 12.45 ms
```

This shows actual time, rows returned, and loops â€” more accurate than EXPLAIN alone.

## Key Points:
- Actually runs the query.
- Shows actual timings and rows.
- More accurate than EXPLAIN alone.
- Planning time vs execution time.
- Use for real performance analysis.

## Interview Tip:
"EXPLAIN ANALYZE gives you real numbers â€” use it for actual performance optimization."

---

## Question 123: How do you read an execution plan?

## Answer:
Key things to look for:
1. **Seq Scan**: Full table scan (bad for large tables).
2. **Index Scan**: Using an index (good).
3. **cost**: Estimated cost (lower is better).
4. **actual time**: Real execution time.
5. **rows**: Estimated vs actual rows (big difference = bad estimate).
6. **loops**: How many times the node executed.

```sql
-- Good: Index Scan
Index Scan using idx_users_email on users (cost=0.28..8.30 rows=1 width=100)

-- Bad: Seq Scan on large table
Seq Scan on users (cost=0.00..123456.00 rows=1000000 width=100)
```

## Key Points:
- Seq Scan on large tables = missing index.
- Index Scan = index is being used.
- Large cost difference between estimated and actual = bad estimates.
- Look for sequential scans on large tables.
- Compare estimated vs actual rows.

## Interview Tip:
"Seq Scan on a large table is almost always a sign of a missing index."

---

## Question 124: What is a sequential scan?

## Answer:
A sequential scan reads every row in the table â€” from start to finish. It's the fallback when no index can be used.

On small tables, it's fine. On large tables, it's slow because it reads every page.

```sql
EXPLAIN SELECT * FROM users WHERE name = 'Alice';
-- Seq Scan on users  (cost=0.00..1234.00 rows=1 width=100)
```

## Key Points:
- Reads every row in the table.
- No index is used.
- Fine for small tables.
- Slow for large tables.
- Usually indicates a missing index.

## Interview Tip:
"Sequential scan on a large table is almost always a problem â€” add an index."

---

## Question 125: What is an index scan?

## Answer:
An index scan uses an index to find matching rows, then accesses the table to retrieve full rows. Much faster than sequential scan for selective queries.

```sql
EXPLAIN SELECT * FROM users WHERE email = 'alice@example.com';
-- Index Scan using idx_users_email on users (cost=0.28..8.30 rows=1 width=100)
```

## Key Points:
- Uses an index to find rows.
- Much faster than sequential scan.
- Two steps: index lookup + table access.
- Shows which index is used.
- Preferred for selective queries.

## Interview Tip:
"Index Scan means the index is working â€” that's what you want to see."

---

## Question 126: What is a bitmap index scan?

## Answer:
A bitmap index scan combines multiple indexes or handles moderate selectivity. It builds a bitmap of matching row locations, then fetches the rows.

```sql
EXPLAIN SELECT * FROM users WHERE role = 'admin' AND is_active = true;
-- Bitmap Heap Scan on users
--   Recheck Cond: (role = 'admin') AND (is_active = true)
--   -> Bitmap Index Scan on idx_users_role_active
```

## Key Points:
- Combines results from multiple indexes.
- Builds a bitmap of matching rows.
- Good for moderate selectivity.
- Falls back to sequential scan for high selectivity.
- More efficient than multiple index scans.

## Interview Tip:
"Bitmap scans are the middle ground between index scans and sequential scans."

---

## Question 127: What is a nested loop join?

## Answer:
A nested loop join iterates over each row in one table and looks up matching rows in the other table using an index. Efficient for small result sets.

```
For each row in outer table:
  Look up matching rows in inner table using index
```

Best when the outer table is small and the inner table has an index.

## Key Points:
- Iterates over outer table, looks up in inner table.
- Uses index on inner table.
- Efficient for small outer tables.
- Bad for large outer tables (quadratic).
- Default for small result sets.

## Interview Tip:
"Nested loops are fast for small datasets â€” they use indexes on the inner table."

---

## Question 128: What is a hash join?

## Answer:
A hash join builds a hash table from one table, then probes it with rows from the other table. Efficient for large, unsorted tables.

```
Build hash table from smaller table
For each row in larger table:
  Look up in hash table
```

Best when both tables are large and unsorted.

## Key Points:
- Builds hash table from smaller table.
- Probes with larger table.
- Efficient for large, unsorted tables.
- Memory-intensive (hash table in memory).
- Good for equi-joins (`=`).

## Interview Tip:
"Hash joins are great for large equi-joins â€” they avoid sorting both tables."

---

## Question 129: What is a merge join?

## Answer:
A merge join sorts both tables by the join key, then merges them. Efficient when both tables are already sorted or indexed.

```
Sort both tables by join key
Merge sorted tables
```

Best when both tables are large and have indexes on the join key.

## Key Points:
- Sorts both tables, then merges.
- Efficient when tables are pre-sorted.
- Good for large tables with indexes.
- Requires sort or index on join key.
- Less common than hash and nested loop.

## Interview Tip:
"Merge joins are efficient when both tables are sorted â€” indexes on join keys help."

---

## Question 130: How do you optimize slow SQL queries?

## Answer:
1. **Run EXPLAIN ANALYZE**: Identify the bottleneck.
2. **Add missing indexes**: On WHERE, JOIN, ORDER BY columns.
3. **Rewrite the query**: Avoid subqueries, use JOINs.
4. **Reduce data**: SELECT only needed columns.
5. **Check statistics**: ANALYZE to update planner stats.
6. **Tune configuration**: shared_buffers, work_mem.
7. **Partition large tables**: Divide data into smaller chunks.
8. **Consider materialized views**: For complex aggregations.

## Key Points:
- EXPLAIN ANALYZE first.
- Add indexes on frequently queried columns.
- Rewrite for efficiency.
- Select only needed columns.
- Update statistics with ANALYZE.

## Interview Tip:
"Always start with EXPLAIN ANALYZE â€” it tells you exactly what's slow."

---

## Part 14 (131â€“140): Transactions & Concurrency

---

## Question 131: What is a database transaction?

## Answer:
A transaction is a sequence of operations performed as a single logical unit. All operations succeed (COMMIT) or none do (ROLLBACK).

```sql
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT;
```

If anything fails, ROLLBACK undoes all changes.

## Key Points:
- Atomic unit of work.
- All operations succeed or all fail.
- COMMIT saves changes.
- ROLLBACK undoes changes.
- Essential for data consistency.

## Interview Tip:
"Transactions ensure that a series of operations either all happen or none happen â€” like a bank transfer."

---

## Question 132: What are the ACID properties?

## Answer:
- **Atomicity**: All operations in a transaction succeed or none do.
- **Consistency**: Database moves from one valid state to another.
- **Isolation**: Concurrent transactions don't interfere.
- **Durability**: Committed data survives crashes.

PostgreSQL fully implements all four properties.

## Key Points:
- Atomicity: all-or-nothing.
- Consistency: valid states only.
- Isolation: concurrent safety.
- Durability: committed data persists.
- PostgreSQL implements all four.

## Interview Tip:
"ACID is the foundation of reliable databases â€” PostgreSQL implements all four properties."

---

## Question 133: What are transaction isolation levels?

## Answer:
Isolation levels control how transactions see each other's changes:
- **Read Uncommitted**: Can see uncommitted changes (dirty reads).
- **Read Committed**: Only sees committed data (default in PostgreSQL).
- **Repeatable Read**: Consistent snapshot for the transaction.
- **Serializable**: Fully isolated, as if transactions ran one after another.

PostgreSQL defaults to Read Committed.

## Key Points:
- Read Uncommitted: dirty reads possible.
- Read Committed: only committed data (PostgreSQL default).
- Repeatable Read: consistent snapshot.
- Serializable: full isolation.
- Higher isolation = more safety but less concurrency.

## Interview Tip:
"PostgreSQL defaults to Read Committed â€” it's a good balance of safety and performance."

---

## Question 134: What is the Read Committed isolation level?

## Answer:
Read Committed is PostgreSQL's default. Each statement within a transaction sees only data committed before the statement started.

```sql
-- Transaction 1
BEGIN;
UPDATE accounts SET balance = 100 WHERE id = 1;
-- Not yet committed

-- Transaction 2
BEGIN;
SELECT balance FROM accounts WHERE id = 1;
-- Sees the OLD value (before Transaction 1's update)
COMMIT;
```

No dirty reads, but non-repeatable reads are possible.

## Key Points:
- Default in PostgreSQL.
- Each statement sees committed data at statement start.
- No dirty reads.
- Non-repeatable reads possible.
- Good balance of safety and performance.

## Interview Tip:
"Read Committed prevents dirty reads but allows non-repeatable reads â€” good for most applications."

---

## Question 135: What is Repeatable Read?

## Answer:
Repeatable Read gives each transaction a consistent snapshot that doesn't change for the entire transaction duration.

```sql
SET TRANSACTION ISOLATION LEVEL REPEATABLE READ;
BEGIN;
SELECT balance FROM accounts WHERE id = 1; -- See value X
-- ... other transactions modify data ...
SELECT balance FROM accounts WHERE id = 1; -- Still see value X
COMMIT;
```

The snapshot is taken at the first query and doesn't change.

## Key Points:
- Consistent snapshot for the entire transaction.
- No dirty reads or non-repeatable reads.
- Phantom reads possible (in standard SQL).
- PostgreSQL prevents phantoms too (MVCC).
- More isolation but less concurrency.

## Interview Tip:
"Repeatable Read gives you a consistent view â€” what you see doesn't change during the transaction."

---

## Question 136: What is Serializable isolation?

## Answer:
Serializable is the highest isolation level â€” transactions appear to execute one after another, as if there were no concurrency.

```sql
SET TRANSACTION ISOLATION LEVEL SERIALIZABLE;
BEGIN;
-- All reads see a consistent snapshot.
-- All writes are serialized.
COMMIT;
```

Most restrictive but guarantees complete isolation.

## Key Points:
- Highest isolation level.
- Transactions appear serial (one after another).
- No dirty reads, non-repeatable reads, or phantoms.
- Most restrictive â€” least concurrent.
- Use when correctness is critical.

## Interview Tip:
"Serializable is the safest but slowest â€” use it only when correctness absolutely requires it."

---

## Question 137: What is MVCC (Multi-Version Concurrency Control)?

## Answer:
MVCC allows multiple transactions to access the same data simultaneously by keeping multiple versions of each row. Each transaction sees a snapshot of the data at the time it started.

Writers create new versions; readers see old versions. No blocking.

## Key Points:
- Multiple versions of each row.
- Each transaction sees a consistent snapshot.
- Readers don't block writers.
- Writers don't block readers.
- Old versions cleaned up by VACUUM.

## Interview Tip:
"MVCC is why PostgreSQL can handle high concurrency â€” readers and writers work simultaneously."

---

## Question 138: How does MVCC improve concurrency?

## Answer:
Without MVCC, reads would block writes and writes would block reads. MVCC eliminates this by:
- Showing each transaction a snapshot.
- Creating new row versions for writes.
- Readers never wait for writers.
- Writers never wait for readers.

The trade-off: old versions accumulate and must be cleaned up by VACUUM.

## Key Points:
- Eliminates read-write blocking.
- Readers see snapshots, not current data.
- Writers create new versions.
- High concurrency for OLTP workloads.
- VACUUM cleans up old versions.

## Interview Tip:
"MVCC trades storage for concurrency â€” old versions are cleaned up by VACUUM."

---

## Question 139: What are row-level locks?

## Answer:
Row-level locks lock individual rows, allowing other rows to be accessed concurrently. PostgreSQL uses MVCC for most operations, but explicit locking is sometimes needed.

```sql
-- Explicit row lock
SELECT * FROM accounts WHERE id = 1 FOR UPDATE;

-- Lock with skip locked (for job queues)
SELECT * FROM jobs WHERE status = 'pending' LIMIT 1 FOR UPDATE SKIP LOCKED;
```

## Key Points:
- Lock individual rows, not the entire table.
- `FOR UPDATE` locks rows for modification.
- `FOR SHARE` locks rows for reading.
- `SKIP LOCKED` skips already-locked rows (job queues).
- Most operations use MVCC, not locks.

## Interview Tip:
"`FOR UPDATE SKIP LOCKED` is perfect for job queues â€” it prevents multiple workers from picking the same job."

---

## Question 140: What is the difference between optimistic and pessimistic locking?

## Answer:
- **Pessimistic**: Lock rows before modifying, hold until transaction ends.
- **Optimistic**: Don't lock, check for conflicts at commit time.

```sql
-- Pessimistic
SELECT * FROM accounts WHERE id = 1 FOR UPDATE;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;

-- Optimistic (using version column)
UPDATE accounts SET balance = balance - 100, version = version + 1
WHERE id = 1 AND version = 5;
-- If rows affected = 0, conflict occurred â€” retry
```

## Key Points:
- Pessimistic: lock first, modify later.
- Optimistic: modify first, check for conflicts at commit.
- Pessimistic: safer but less concurrent.
- Optimistic: more concurrent but needs retry logic.
- Use pessimistic for high contention; optimistic for low contention.

## Interview Tip:
"Optimistic locking is better for most web apps â€” check the version column and retry on conflict."

---

## Part 15 (141â€“150): Deadlocks & Performance

---

## Question 141: What is a deadlock?

## Answer:
A deadlock occurs when two transactions wait for each other's locks indefinitely.

```
Transaction A: locks row 1, waits for row 2
Transaction B: locks row 2, waits for row 1
â†’ Neither can proceed
```

PostgreSQL detects deadlocks and rolls back one transaction.

## Key Points:
- Two transactions waiting for each other.
- Neither can proceed.
- PostgreSQL detects and resolves deadlocks.
- One transaction is rolled back.
- Applications must handle deadlock errors.

## Interview Tip:
"PostgreSQL automatically detects and resolves deadlocks â€” your app just needs to retry."

---

## Question 142: How does PostgreSQL detect deadlocks?

## Answer:
PostgreSQL runs a deadlock detector process that periodically checks for deadlocks. When detected, it rolls back the transaction that's cheapest to undo.

The deadlock timeout is configurable (default: 1 second).

## Key Points:
- Automatic deadlock detection.
- Deadlock detector process runs periodically.
- Rolls back the cheapest transaction.
- Configurable deadlock timeout.
- Deadlock info logged in server logs.

## Interview Tip:
"PostgreSQL detects deadlocks automatically â€” check the logs for deadlock details."

---

## Question 143: How do you prevent deadlocks?

## Answer:
1. **Consistent lock order**: Always lock tables/rows in the same order.
2. **Short transactions**: Hold locks for the shortest time possible.
3. **Use lower isolation**: Read Committed has fewer deadlock risks.
4. **Avoid user input in locks**: Don't lock based on user-provided values.
5. **Use SELECT FOR UPDATE NOWAIT**: Fail immediately if locked.

## Key Points:
- Lock in consistent order.
- Keep transactions short.
- Lower isolation levels reduce deadlock risk.
- NOWAIT fails immediately on lock conflict.
- Retry logic handles deadlocks gracefully.

## Interview Tip:
"Consistent lock order is the golden rule â€” if everyone locks in the same order, deadlocks can't happen."

---

## Question 144: What is table partitioning?

## Answer:
Table partitioning divides a large table into smaller, more manageable pieces (partitions). Each partition is a separate table but appears as one to queries.

```sql
CREATE TABLE orders (
  id SERIAL,
  created_at TIMESTAMPTZ,
  amount DECIMAL
) PARTITION BY RANGE (created_at);

CREATE TABLE orders_2024 PARTITION OF orders
  FOR VALUES FROM ('2024-01-01') TO ('2025-01-01');
```

## Key Points:
- Divides large tables into smaller pieces.
- Each partition is a separate table.
- Transparent to queries.
- Improves query performance and maintenance.
- Range, list, and hash partitioning.

## Interview Tip:
"Partitioning is essential for large tables â€” it improves query performance and maintenance."

---

## Question 145: When should you partition a table?

## Answer:
- **Very large tables**: >100GB or millions of rows.
- **Time-series data**: Partition by date range.
- **Data lifecycle**: Easy to drop old partitions.
- **Query performance**: Queries that filter by partition key.
- **Maintenance**: VACUUM, REINDEX on smaller pieces.

Don't partition small tables â€” the overhead isn't worth it.

## Key Points:
- Large tables (>100GB or millions of rows).
- Time-series data (partition by date).
- Data lifecycle management (drop old partitions).
- Queries that consistently filter by partition key.
- Small tables don't benefit from partitioning.

## Interview Tip:
"Partition by the column you most frequently filter on â€” usually a date for time-series data."

---

## Question 146: What is connection pooling?

## Answer:
Connection pooling maintains a pool of reusable database connections instead of creating a new connection per request. It reduces connection overhead and prevents connection exhaustion.

```javascript
// Node.js with pg-pool
const { Pool } = require("pg");
const pool = new Pool({ max: 20, idleTimeoutMillis: 30000 });

const client = await pool.connect();
try {
  await client.query("SELECT * FROM users");
} finally {
  client.release(); // Return to pool
}
```

## Key Points:
- Reuse connections instead of creating new ones.
- Reduces connection overhead.
- Prevents connection exhaustion.
- Configurable pool size.
- Most ORMs handle this automatically.

## Interview Tip:
"Connection pooling is essential for production â€” don't create a new connection per request."

---

## Question 147: What is the purpose of PgBouncer?

## Answer:
PgBouncer is a lightweight connection pooler for PostgreSQL. It sits between your application and PostgreSQL, managing a pool of connections.

- Reduces PostgreSQL connection overhead.
- Supports transaction, session, and statement pooling modes.
- Handles thousands of connections with few database connections.

## Key Points:
- Lightweight connection pooler.
- Sits between app and database.
- Three pooling modes: session, transaction, statement.
- Handles many app connections with few DB connections.
- Essential for high-traffic applications.

## Interview Tip:
"PgBouncer is the standard connection pooler for PostgreSQL â€” it's lightweight and efficient."

---

## Question 148: How do you monitor PostgreSQL performance?

## Answer:
1. **pg_stat_statements**: Track query performance.
2. **pg_stat_activity**: Monitor active connections.
3. **pg_stat_user_indexes**: Index usage stats.
4. **EXPLAIN ANALYZE**: Individual query performance.
5. **pgBadger**: Log analysis tool.
6. **pgAdmin**: GUI monitoring.
7. **Datadog/New Relic**: APM integration.

## Key Points:
- `pg_stat_statements` for query performance.
- `pg_stat_activity` for connections.
- `pg_stat_user_indexes` for index usage.
- `EXPLAIN ANALYZE` for individual queries.
- External tools for comprehensive monitoring.

## Interview Tip:
"`pg_stat_statements` is essential â€” it shows you the slowest queries."

---

## Question 149: What are common PostgreSQL performance bottlenecks?

## Answer:
1. **Missing indexes**: Sequential scans on large tables.
2. **Slow queries**: N+1 queries, full table scans.
3. **Connection exhaustion**: Too many connections.
4. **Lock contention**: Deadlocks and blocking.
5. **Insufficient memory**: Too little shared_buffers or work_mem.
6. **Write overhead**: Too many indexes.
7. **VACUUM issues**: Table bloat from missed VACUUMs.

## Key Points:
- Missing indexes are the most common bottleneck.
- Slow queries from poor query design.
- Connection exhaustion under load.
- Lock contention from concurrent writes.
- Memory settings affect query performance.

## Interview Tip:
"90% of PostgreSQL performance issues are missing indexes or slow queries."

---

## Question 150: What performance tuning best practices do you follow for production databases?

## Answer:
1. **Index appropriately**: Foreign keys, WHERE columns, JOIN columns.
2. **Tune memory**: shared_buffers (25% of RAM), work_mem.
3. **Connection pooling**: PgBouncer or application-level pooling.
4. **Regular VACUUM**: Prevent table bloat.
5. **Monitor slow queries**: pg_stat_statements.
6. **Partition large tables**: For time-series and large datasets.
7. **Use EXPLAIN ANALYZE**: For every slow query.
8. **Keep statistics updated**: ANALYZE regularly.

## Key Points:
- Index the right columns.
- Tune memory settings.
- Use connection pooling.
- Regular VACUUM and ANALYZE.
- Monitor with pg_stat_statements.

## Interview Tip:
"Start with indexing, then tune memory, then add connection pooling â€” that covers 80% of performance issues."

---

## Part 16 (151â€“160): Database Design

---

## Question 151: What is database normalization?

## Answer:
Normalization is the process of organizing data to reduce redundancy and improve integrity. It involves splitting tables and defining relationships between them.

Benefits:
- Reduces data duplication.
- Prevents update anomalies.
- Improves data integrity.

The goal: each piece of data is stored in one place.

## Key Points:
- Organizes data to reduce redundancy.
- Prevents update, insert, and delete anomalies.
- Improves data integrity.
- Involves splitting tables and defining relationships.
- Multiple normal forms (1NF, 2NF, 3NF, BCNF).

## Interview Tip:
"Normalization is about putting each piece of data in one place â€” no duplication."

---

## Question 152: What are the different normal forms (1NF, 2NF, 3NF, BCNF)?

## Answer:
- **1NF**: Each column contains atomic (single) values.
- **2NF**: No partial dependencies (all non-key columns depend on the whole primary key).
- **3NF**: No transitive dependencies (non-key columns don't depend on other non-key columns).
- **BCNF**: Every determinant is a candidate key (stricter 3NF).

Most applications aim for 3NF.

## Key Points:
- 1NF: atomic values, no repeating groups.
- 2NF: no partial dependencies.
- 3NF: no transitive dependencies.
- BCNF: every determinant is a candidate key.
- 3NF is the practical target for most apps.

## Interview Tip:
"3NF is the sweet spot â€” enough normalization for integrity without over-engineering."

---

## Question 153: Why is normalization important?

## Answer:
- **Reduces redundancy**: Data stored once, not multiple times.
- **Prevents anomalies**: Update, insert, and delete anomalies.
- **Improves integrity**: Changes propagate correctly.
- **Saves storage**: Less duplicate data.
- **Easier maintenance**: Changes in one place affect all references.

## Key Points:
- Reduces data duplication.
- Prevents anomalies.
- Improves data integrity.
- Saves storage space.
- Easier to maintain and update.

## Interview Tip:
"Normalization prevents the classic problem: update a name in one place but forget another."

---

## Question 154: What is denormalization?

## Answer:
Denormalization intentionally adds redundancy to improve read performance. Instead of joining tables, you store derived or duplicate data.

```sql
-- Normalized: join needed
SELECT u.name, COUNT(o.id) FROM users u JOIN orders o ON u.id = o.user_id GROUP BY u.name;

-- Denormalized: pre-computed
SELECT name, order_count FROM users; -- order_count stored directly
```

## Key Points:
- Intentional redundancy for performance.
- Reduces JOINs for faster reads.
- Increases storage and write overhead.
- Trade-off: read speed vs write complexity.
- Common in analytics and reporting.

## Interview Tip:
"Denormalize when reads are slow and writes are infrequent â€” analytics and reporting."

---

## Question 155: When should you denormalize a database?

## Answer:
- **Read-heavy workloads**: Reporting, analytics, dashboards.
- **Complex joins are slow**: Pre-compute expensive aggregations.
- **Caching layer**: Materialized views for frequent queries.
- **Write-light applications**: Reads far outnumber writes.
- **Real-time analytics**: Pre-aggregated data for speed.

Don't denormalize for write-heavy applications.

## Key Points:
- Read-heavy workloads.
- Slow complex joins.
- Materialized views for caching.
- Write-light applications.
- Real-time analytics.

## Interview Tip:
"Denormalize when reads are slow and you can't optimize with indexes."

---

## Question 156: What are the trade-offs between normalization and denormalization?

## Answer:
| Aspect | Normalized | Denormalized |
|--------|-----------|-------------|
| Redundancy | Low | High |
| Write performance | Better | Slower |
| Read performance | May need JOINs | Faster |
| Storage | Less | More |
| Integrity | Enforced | Application-managed |
| Maintenance | Easier | Harder |

Most applications: normalize first, denormalize specific bottlenecks.

## Key Points:
- Normalized: less redundancy, better writes, more JOINs.
- Denormalized: more redundancy, faster reads, more storage.
- Normalize first, denormalize specific bottlenecks.
- Use materialized views as a middle ground.

## Interview Tip:
"Normalize by default â€” denormalize only when you have a specific performance problem."

---

## Question 157: How do you design a scalable relational database?

## Answer:
1. **Normalize**: Start with 3NF.
2. **Index appropriately**: Foreign keys, WHERE columns.
3. **Partition large tables**: By date or key range.
4. **Read replicas**: Distribute read load.
5. **Connection pooling**: Manage connections efficiently.
6. **Cache frequently accessed data**: Redis or materialized views.
7. **Plan for growth**: Choose data types that scale.

## Key Points:
- Normalize first.
- Index for performance.
- Partition large tables.
- Read replicas for scaling.
- Connection pooling for efficiency.

## Interview Tip:
"Scalable design starts with normalization and indexing â€” add partitioning and replicas as needed."

---

## Question 158: What is database schema design?

## Answer:
Schema design is the process of defining tables, columns, relationships, and constraints. A good schema:
- Models the domain accurately.
- Enforces data integrity.
- Supports required queries efficiently.
- Scales with the application.

```sql
CREATE TABLE users (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  name TEXT NOT NULL,
  email TEXT UNIQUE NOT NULL,
  created_at TIMESTAMPTZ DEFAULT NOW()
);
```

## Key Points:
- Defines tables, columns, relationships, constraints.
- Models the domain accurately.
- Enforces data integrity.
- Supports efficient queries.
- Scales with the application.

## Interview Tip:
"Schema design is the foundation of your application â€” get it right and everything else is easier."

---

## Question 159: How do you model one-to-one relationships?

## Answer:
Use a foreign key on one table referencing the other's primary key, with a UNIQUE constraint.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL
);

CREATE TABLE user_profiles (
  user_id INTEGER PRIMARY KEY REFERENCES users(id),
  bio TEXT,
  avatar_url TEXT
);
```

`user_id` is both the primary key and a foreign key.

## Key Points:
- Foreign key on one table.
- UNIQUE constraint ensures one-to-one.
- Primary key of the dependent references the parent.
- One table is the "owner," the other is the "dependent."
- Can also use shared primary key.

## Interview Tip:
"Use a shared primary key â€” the dependent's PK is also its FK to the parent."

---

## Question 160: How do you model one-to-many and many-to-many relationships?

## Answer:
**One-to-many**: Foreign key on the "many" side.
```sql
CREATE TABLE users (id SERIAL PRIMARY KEY, name TEXT);
CREATE TABLE posts (id SERIAL PRIMARY KEY, user_id INTEGER REFERENCES users(id));
```

**Many-to-many**: Junction table.
```sql
CREATE TABLE users (id SERIAL PRIMARY KEY, name TEXT);
CREATE TABLE posts (id SERIAL PRIMARY KEY, title TEXT);
CREATE TABLE post_tags (
  post_id INTEGER REFERENCES posts(id),
  tag_id INTEGER REFERENCES tags(id),
  PRIMARY KEY (post_id, tag_id)
);
```

## Key Points:
- One-to-many: foreign key on the many side.
- Many-to-many: junction/bridge table.
- Junction table has foreign keys to both tables.
- Composite primary key on junction table.
- Most relationships are one-to-many or many-to-many.

## Interview Tip:
"Foreign key for one-to-many, junction table for many-to-many â€” that covers 95% of relationships."

---

## Part 17 (161â€“170): Constraints & Keys

---

## Question 161: What types of constraints does PostgreSQL support?

## Answer:
- **PRIMARY KEY**: Unique identifier for each row.
- **FOREIGN KEY**: References another table's primary key.
- **UNIQUE**: All values in column(s) must be unique.
- **CHECK**: Values must satisfy a condition.
- **NOT NULL**: Column cannot be NULL.
- **DEFAULT**: Provides a default value when none is specified.
- **EXCLUSION**: Prevents conflicting values (e.g., overlapping time ranges).

## Key Points:
- PRIMARY KEY: unique, not null.
- FOREIGN KEY: referential integrity.
- UNIQUE: no duplicate values.
- CHECK: condition validation.
- NOT NULL: required values.
- DEFAULT: automatic values.
- EXCLUSION: prevents conflicts.

## Interview Tip:
"PostgreSQL has seven constraint types â€” EXCLUSION is unique and powerful for time-range conflicts."

---

## Question 162: What is a PRIMARY KEY?

## Answer:
A primary key uniquely identifies each row. It must be unique and NOT NULL. Only one primary key per table.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL
);
```

The primary key automatically creates a unique index.

## Key Points:
- Uniquely identifies each row.
- Must be unique and NOT NULL.
- Only one per table.
- Automatically creates a unique index.
- Can be single or composite.

## Interview Tip:
"Primary key = identity of each row. It must be unique and never null."

---

## Question 163: What is a FOREIGN KEY?

## Answer:
A foreign key references the primary key of another table, enforcing referential integrity.

```sql
CREATE TABLE posts (
  id SERIAL PRIMARY KEY,
  user_id INTEGER REFERENCES users(id) ON DELETE CASCADE
);
```

Foreign keys prevent orphaned rows and can cascade actions.

## Key Points:
- References another table's primary key.
- Enforces referential integrity.
- Prevents orphaned rows.
- Can cascade actions (DELETE CASCADE, etc.).
- Creates an implicit index.

## Interview Tip:
"Foreign keys enforce relationships â€” without them, you can have orphaned data."

---

## Question 164: What is a UNIQUE constraint?

## Answer:
A unique constraint ensures all values in a column (or combination) are unique.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email TEXT UNIQUE NOT NULL
);
```

Unlike primary keys, unique constraints allow NULLs (unless combined with NOT NULL).

## Key Points:
- Ensures unique values.
- Allows NULLs (unless NOT NULL).
- Multiple unique constraints per table.
- Creates a unique index.
- Different from primary key (only one PK).

## Interview Tip:
"Unique constraints prevent duplicates â€” emails, usernames, or any identifier."

---

## Question 165: What is a CHECK constraint?

## Answer:
A check constraint validates that values satisfy a condition.

```sql
CREATE TABLE products (
  price DECIMAL(10,2) CHECK (price >= 0),
  quantity INTEGER CHECK (quantity >= 0)
);
```

Applied on INSERT and UPDATE.

## Key Points:
- Validates data against a condition.
- Prevents invalid data.
- Applied on INSERT and UPDATE.
- Can reference multiple columns.
- Named constraints for better error messages.

## Interview Tip:
"Check constraints prevent invalid data at the database level â€” don't rely solely on app validation."

---

## Question 166: What is a NOT NULL constraint?

## Answer:
A NOT NULL constraint ensures a column cannot contain NULL values.

```sql
CREATE TABLE users (
  name TEXT NOT NULL,
  email TEXT NOT NULL
);
```

NULL represents an unknown or missing value. NOT NULL enforces that a value is required.

## Key Points:
- Column cannot be NULL.
- Enforces required values.
- Applied on INSERT and UPDATE.
- Fundamental for data integrity.
- Combined with other constraints.

## Interview Tip:
"NOT NULL is the simplest and most fundamental constraint â€” use it for required fields."

---

## Question 167: What is a DEFAULT constraint?

## Answer:
A default constraint provides a value when none is specified.

```sql
CREATE TABLE users (
  role TEXT DEFAULT 'user',
  is_active BOOLEAN DEFAULT true,
  created_at TIMESTAMPTZ DEFAULT NOW()
);
```

The default can be a constant, function, or expression.

## Key Points:
- Provides default value.
- Applied on INSERT when column is omitted.
- Can be constant or function call.
- Useful for timestamps, status, and common values.
- Doesn't affect UPDATE unless explicitly set.

## Interview Tip:
"`DEFAULT NOW()` auto-sets timestamps â€” the most common default in PostgreSQL."

---

## Question 168: What are composite keys?

## Answer:
A composite key is a primary key made up of multiple columns.

```sql
CREATE TABLE post_tags (
  post_id INTEGER,
  tag_id INTEGER,
  PRIMARY KEY (post_id, tag_id)
);
```

Used for junction tables in many-to-many relationships.

## Key Points:
- Primary key with multiple columns.
- All columns together form the unique identifier.
- Common in junction tables.
- Composite indexes follow the leftmost rule.
- Order of columns matters.

## Interview Tip:
"Composite keys are common in junction tables â€” the combination of foreign keys is the primary key."

---

## Question 169: When should you use natural keys vs surrogate keys?

## Answer:
- **Natural keys**: Real-world identifiers (email, ISBN, SSN). Meaningful but may change.
- **Surrogate keys**: Generated identifiers (SERIAL, UUID). No meaning but stable.

```sql
-- Natural key
CREATE TABLE users (email TEXT PRIMARY KEY);

-- Surrogate key
CREATE TABLE users (id SERIAL PRIMARY KEY, email TEXT UNIQUE NOT NULL);
```

Surrogate keys are generally preferred for most applications.

## Key Points:
- Natural keys: meaningful, may change.
- Surrogate keys: generated, stable, no meaning.
- Surrogate keys are generally preferred.
- Natural keys for reference data (countries, currencies).
- Surrogate keys for entity tables (users, orders).

## Interview Tip:
"Surrogate keys (SERIAL, UUID) are generally preferred â€” they're stable and simple."

---

## Question 170: What are cascading actions (`CASCADE`, `RESTRICT`, `SET NULL`, `NO ACTION`)?

## Answer:
Cascading actions define what happens when a referenced row is deleted or updated.

- **CASCADE**: Delete/update referencing rows.
- **RESTRICT**: Prevent delete/update if references exist.
- **SET NULL**: Set foreign key to NULL.
- **SET DEFAULT**: Set foreign key to default value.
- **NO ACTION**: Similar to RESTRICT (default).

```sql
CREATE TABLE posts (
  user_id INTEGER REFERENCES users(id) ON DELETE CASCADE
);
-- Deleting a user deletes their posts
```

## Key Points:
- CASCADE: delete/update references.
- RESTRICT: prevent if references exist.
- SET NULL: set FK to NULL.
- SET DEFAULT: set FK to default.
- NO ACTION: same as RESTRICT (default).

## Interview Tip:
"CASCADE is useful but dangerous â€” make sure you really want to delete related data."

---

## Part 18 (171â€“180): Views, Functions & Triggers

---

## Question 171: What is a View?

## Answer:
A view is a named query that behaves like a table. It doesn't store data â€” it runs the query every time it's accessed.

```sql
CREATE VIEW active_users AS
SELECT id, name, email FROM users WHERE is_active = true;

SELECT * FROM active_users;
```

Views simplify complex queries and provide a layer of abstraction.

## Key Points:
- Named query that behaves like a table.
- No data stored â€” query runs on access.
- Simplifies complex queries.
- Provides abstraction layer.
- Can be updated (with restrictions).

## Interview Tip:
"Views are named queries â€” they simplify complex logic and provide security by hiding tables."

---

## Question 172: What is a Materialized View?

## Answer:
A materialized view stores the result of a query physically. It doesn't update automatically â€” you must refresh it.

```sql
CREATE MATERIALIZED VIEW monthly_sales AS
SELECT DATE_TRUNC('month', created_at), SUM(amount)
FROM orders GROUP BY 1;

-- Refresh when data changes
REFRESH MATERIALIZED VIEW monthly_sales;
```

Perfect for expensive aggregations that don't need real-time updates.

## Key Points:
- Stores query results physically.
- Doesn't update automatically.
- Must be refreshed manually or on schedule.
- Much faster than regular views for complex queries.
- Can be indexed.

## Interview Tip:
"Materialized views are cached query results â€” perfect for expensive aggregations."

---

## Question 173: What is the difference between a View and a Materialized View?

## Answer:
| Feature | View | Materialized View |
|---------|------|-------------------|
| Data storage | None (runs query) | Stores results |
| Updates | Always current | Must refresh |
| Performance | Depends on query | Fast (pre-computed) |
| Indexing | No | Yes |
| Use case | Simple abstraction | Expensive aggregations |

## Key Points:
- View: no storage, always current.
- Materialized View: stored, must refresh.
- Materialized views are faster for complex queries.
- Materialized views can be indexed.
- Use views for simplicity; materialized views for performance.

## Interview Tip:
"Views are always current; materialized views are fast but must be refreshed."

---

## Question 174: When should you use a Materialized View?

## Answer:
- **Expensive aggregations**: Complex GROUP BY across large tables.
- **Reporting dashboards**: Pre-computed metrics.
- **Data warehousing**: Pre-aggregated fact tables.
- **Read-heavy analytics**: Fast reads without recomputing.
- **Periodic refresh**: Data that doesn't change in real-time.

Not for: real-time data, frequently changing data, or simple queries.

## Key Points:
- Expensive aggregations.
- Reporting and dashboards.
- Read-heavy analytics.
- Periodic refresh is acceptable.
- Not for real-time data.

## Interview Tip:
"Materialized views are great for dashboards â€” pre-compute expensive queries and refresh periodically."

---

## Question 175: What is a stored procedure?

## Answer:
A stored procedure is a named block of SQL that can be called with parameters. Procedures can perform operations (INSERT, UPDATE, DELETE) and don't return values directly.

```sql
CREATE PROCEDURE deactivate_users(days_old INTEGER)
LANGUAGE plpgsql
AS $$
BEGIN
  UPDATE users SET is_active = false
  WHERE last_login < NOW() - days_old * INTERVAL '1 day';
END;
$$;

CALL deactivate_users(90);
```

## Key Points:
- Named block of SQL.
- Called with CALL.
- Can perform operations.
- Don't return values directly.
- Support transactions.

## Interview Tip:
"Procedures are for actions; functions are for calculations. Know when to use each."

---

## Question 176: What is the difference between a stored procedure and a function?

## Answer:
| Feature | Procedure | Function |
|---------|-----------|----------|
| Call | `CALL proc()` | `SELECT func()` |
| Returns | No direct return | Returns a value |
| Transaction | Can manage transactions | Cannot manage transactions |
| Use case | Actions (INSERT, UPDATE) | Calculations, expressions |

## Key Points:
- Procedures: called with CALL, no return.
- Functions: called with SELECT, return a value.
- Procedures can manage transactions.
- Functions can be used in queries (WHERE, SELECT).
- Choose based on what you need.

## Interview Tip:
"Functions return values and can be used in queries; procedures perform actions."

---

## Question 177: What are PostgreSQL functions?

## Answer:
Functions are named blocks of SQL (or PL/pgSQL) that return a value and can be used in queries.

```sql
CREATE FUNCTION get_user_order_count(user_id INTEGER)
RETURNS INTEGER
LANGUAGE sql
AS $$
  SELECT COUNT(*)::INTEGER FROM orders WHERE orders.user_id = $1;
$$;

SELECT name, get_user_order_count(id) FROM users;
```

## Key Points:
- Named blocks that return a value.
- Can be used in SELECT, WHERE, etc.
- Support multiple languages (SQL, PL/pgSQL).
- Accept parameters.
- Useful for calculations and business logic.

## Interview Tip:
"Functions are reusable SQL â€” they encapsulate logic and can be used anywhere in a query."

---

## Question 178: What are triggers?

## Answer:
Triggers automatically execute a function when a specific event occurs on a table (INSERT, UPDATE, DELETE).

```sql
CREATE FUNCTION update_timestamp()
RETURNS TRIGGER
LANGUAGE plpgsql
AS $$
BEGIN
  NEW.updated_at = NOW();
  RETURN NEW;
END;
$$;

CREATE TRIGGER set_updated_at
  BEFORE UPDATE ON users
  FOR EACH ROW
  EXECUTE FUNCTION update_timestamp();
```

## Key Points:
- Automatically execute on table events.
- BEFORE or AFTER triggers.
- FOR EACH ROW or FOR EACH STATEMENT.
- Can modify data (BEFORE triggers).
- Useful for auditing and validation.

## Interview Tip:
"Triggers are great for auditing and auto-updating timestamps â€” but use them sparingly."

---

## Question 179: When should you use triggers?

## Answer:
- **Audit logging**: Track changes to data.
- **Auto-timestamps**: Set updated_at on every update.
- **Data validation**: Complex validation logic.
- **Cascading changes**: Update related data automatically.
- **Data transformation**: Clean or transform data on insert.

Don't use triggers for complex business logic â€” keep that in the application.

## Key Points:
- Audit logging.
- Auto-timestamps.
- Complex validation.
- Cascading changes.
- Keep complex logic in the application.

## Interview Tip:
"Triggers are for database-level automation â€” keep complex business logic in the application."

---

## Question 180: What are the drawbacks of triggers?

## Answer:
- **Hidden logic**: Trigger behavior isn't visible in application code.
- **Performance overhead**: Triggers add processing to every operation.
- **Debugging difficulty**: Hard to trace trigger behavior.
- **Cascading triggers**: One trigger can fire another.
- **Maintenance**: Changes require database migrations.
- **Testing complexity**: Harder to test application behavior.

## Key Points:
- Hidden from application code.
- Performance overhead on every operation.
- Hard to debug and trace.
- Can cascade unexpectedly.
- Maintenance overhead.

## Interview Tip:
"Triggers are powerful but hidden â€” use them sparingly and document them well."

---

## Part 19 (181â€“190): Security

---

## Question 181: How does PostgreSQL handle authentication?

## Answer:
PostgreSQL supports multiple authentication methods:
- **Trust**: No authentication (development only).
- **Password**: MD5 or SCRAM-SHA-256 password authentication.
- **Peer**: Unix socket authentication (local connections).
- **LDAP**: LDAP directory authentication.
- **Certificate**: SSL client certificate authentication.
- **PAM**: Pluggable Authentication Modules.

Configured in `pg_hba.conf`.

## Key Points:
- Multiple authentication methods.
- Configured in `pg_hba.conf`.
- Password (MD5, SCRAM-SHA-256) for most apps.
- Certificate for high security.
- Trust for development only.

## Interview Tip:
"SCRAM-SHA-256 is the modern password authentication method â€” use it over MD5."

---

## Question 182: What are PostgreSQL roles?

## Answer:
Roles are database users with privileges. A role can have login permission, database access, and object-level privileges.

```sql
CREATE ROLE app_user LOGIN PASSWORD 'secure_password';
GRANT CONNECT ON DATABASE mydb TO app_user;
GRANT USAGE ON SCHEMA public TO app_user;
GRANT SELECT, INSERT, UPDATE, DELETE ON ALL TABLES IN SCHEMA public TO app_user;
```

Roles can be grouped and inherited.

## Key Points:
- Roles combine users and groups.
- Can have login, database, and object privileges.
- GRANT to give permissions.
- REVOKE to remove permissions.
- Roles can inherit from other roles.

## Interview Tip:
"Roles are PostgreSQL's way of managing users and permissions â€” they combine users and groups."

---

## Question 183: What is the difference between users and roles?

## Answer:
In PostgreSQL, users and roles are the same thing. A role with LOGIN privilege is effectively a user. Historically, "users" could login and "roles" couldn't, but now they're unified.

```sql
-- These are equivalent
CREATE USER app_user PASSWORD 'secret';
CREATE ROLE app_user LOGIN PASSWORD 'secret';
```

## Key Points:
- Users and roles are the same in PostgreSQL.
- A role with LOGIN = a user.
- Historically different, now unified.
- Use CREATE ROLE for new setups.
- Use CREATE USER for compatibility.

## Interview Tip:
"In modern PostgreSQL, users and roles are the same â€” a role with LOGIN is a user."

---

## Question 184: How do you grant permissions?

## Answer:
```sql
-- Grant database access
GRANT CONNECT ON DATABASE mydb TO app_user;

-- Grant schema usage
GRANT USAGE ON SCHEMA public TO app_user;

-- Grant table permissions
GRANT SELECT, INSERT, UPDATE, DELETE ON ALL TABLES IN SCHEMA public TO app_user;

-- Grant sequence permissions (for SERIAL)
GRANT USAGE, SELECT ON ALL SEQUENCES IN SCHEMA public TO app_user;

-- Grant for future tables
ALTER DEFAULT PRIVILEGES IN SCHEMA public
  GRANT SELECT, INSERT, UPDATE, DELETE ON TABLES TO app_user;
```

## Key Points:
- GRANT gives permissions.
- Levels: database, schema, table, column.
- ALTER DEFAULT PRIVILEGES for future objects.
- GRANT with ALL for full access.
- Always follow least privilege.

## Interview Tip:
"GRANT the minimum permissions needed â€” don't give ALL unless necessary."

---

## Question 185: How do you revoke permissions?

## Answer:
```sql
-- Revoke specific permissions
REVOKE INSERT, UPDATE, DELETE ON users FROM app_user;

-- Revoke all permissions
REVOKE ALL ON users FROM app_user;

-- Revoke database access
REVOKE CONNECT ON DATABASE mydb FROM app_user;
```

REVOKE is the opposite of GRANT.

## Key Points:
- REVOKE removes permissions.
- Can revoke specific or all permissions.
- Levels: database, schema, table, column.
- REVOKE ALL for complete removal.
- Check permissions with `\dp` in psql.

## Interview Tip:
"REVOKE is the opposite of GRANT â€” use it to remove unnecessary permissions."

---

## Question 186: What is the principle of least privilege?

## Answer:
Give each user/role only the minimum permissions needed for their job. Don't give ALL if they only need SELECT.

```sql
-- Bad: gives everything
GRANT ALL ON ALL TABLES IN SCHEMA public TO app_user;

-- Good: gives only what's needed
GRANT SELECT, INSERT, UPDATE ON orders TO app_user;
```

## Key Points:
- Minimum necessary permissions.
- No unnecessary access.
- Reduces attack surface.
- Prevents accidental data damage.
- Standard security practice.

## Interview Tip:
"Least privilege means: give only what's needed, nothing more."

---

## Question 187: How do you secure sensitive data in PostgreSQL?

## Answer:
1. **Encryption at rest**: pgcrypto or disk-level encryption.
2. **Encryption in transit**: SSL/TLS connections.
3. **Column-level encryption**: Encrypt specific columns.
4. **Row-level security**: Restrict rows per user.
5. **Least privilege**: Minimal permissions.
6. **Audit logging**: Track access to sensitive data.

```sql
-- Column-level encryption
CREATE EXTENSION pgcrypto;
INSERT INTO users (name, ssn) VALUES ('Alice', pgp_sym_encrypt('123-45-6789', 'secret'));
```

## Key Points:
- Encryption at rest and in transit.
- Column-level encryption with pgcrypto.
- Row-level security for multi-tenant apps.
- Least privilege permissions.
- Audit logging for compliance.

## Interview Tip:
"Encrypt sensitive data at rest and in transit â€” use pgcrypto for column-level encryption."

---

## Question 188: How do you encrypt data at rest and in transit?

## Answer:
**At rest**:
- Disk-level encryption (LUKS, BitLocker, AWS EBS encryption).
- Column-level encryption with pgcrypto.
- Transparent Data Encryption (TDE) extensions.

**In transit**:
- SSL/TLS connections.
- Configure `ssl = on` in postgresql.conf.
- Client certificates for mutual TLS.

```sql
-- Force SSL connections
ALTER SYSTEM SET ssl = on;
-- In pg_hba.conf: hostssl all all 0.0.0.0/0 scram-sha-256
```

## Key Points:
- At rest: disk encryption, column encryption.
- In transit: SSL/TLS.
- pgcrypto for column-level encryption.
- SSL certificates for mutual authentication.
- Force SSL in pg_hba.conf.

## Interview Tip:
"Always use SSL for database connections â€” configure pg_hba.conf to require it."

---

## Question 189: How do you protect against SQL Injection?

## Answer:
1. **Parameterized queries**: Never concatenate user input into SQL.
2. **Use an ORM**: Prisma, TypeORM handle this automatically.
3. **Input validation**: Validate and sanitize all input.
4. **Least privilege**: DB user should have minimal permissions.

```sql
-- BAD: SQL injection vulnerability
SELECT * FROM users WHERE name = '" + userInput + "';

-- GOOD: parameterized query
SELECT * FROM users WHERE name = $1;
```

## Key Points:
- Parameterized queries prevent injection.
- ORMs handle this automatically.
- Validate all input server-side.
- Least privilege limits damage.
- Never concatenate user input into SQL.

## Interview Tip:
"Parameterized queries prevent SQL injection â€” never concatenate user input into SQL."

---

## Question 190: What PostgreSQL security best practices do you follow?

## Answer:
1. **SSL/TLS**: Encrypt connections.
2. **Least privilege**: Minimal permissions per role.
3. **Parameterized queries**: Prevent SQL injection.
4. **Encryption at rest**: pgcrypto or disk encryption.
5. **Audit logging**: Track access and changes.
6. **Strong passwords**: SCRAM-SHA-256 authentication.
7. **Regular updates**: Keep PostgreSQL patched.
8. **Network security**: Restrict access with firewall/pg_hba.conf.

## Key Points:
- SSL for connections.
- Least privilege for permissions.
- Parameterized queries for injection prevention.
- Encryption for sensitive data.
- Audit logging for compliance.

## Interview Tip:
"Security is defense in depth â€” SSL, least privilege, parameterized queries, and encryption."

---

## Part 20 (191â€“200): Backup, Recovery & Administration

---

## Question 191: How do you back up a PostgreSQL database?

## Answer:
```bash
# Full backup
pg_dump -U username -d dbname -F c -f backup.dump

# Backup all databases
pg_dumpall -U username > all_databases.sql

# Backup as SQL text
pg_dump -U username -d dbname -f backup.sql
```

`pg_dump` is the standard backup tool. `-F c` creates a custom format (compressed, restorable).

## Key Points:
- `pg_dump` for single database backup.
- `pg_dumpall` for all databases.
- Custom format (-F c) is compressed and efficient.
- Schedule regular backups.
- Test restores regularly.

## Interview Tip:
"Always test your backups â€” a backup you can't restore is useless."

---

## Question 192: What is `pg_dump`?

## Answer:
`pg_dump` creates a logical backup of a PostgreSQL database. It exports the database as SQL or custom-format archive.

```bash
# Custom format (compressed, recommended)
pg_dump -U username -d dbname -F c -f backup.dump

# Parallel backup (faster for large databases)
pg_dump -U username -d dbname -F d -j 4 -f backup_dir/

# Schema only
pg_dump -U username -d dbname --schema-only -f schema.sql
```

## Key Points:
- Logical backup tool.
- Custom format (-F c) recommended.
- Parallel backup with -j flag.
- Schema-only or data-only options.
- Doesn't require stopping the server.

## Interview Tip:
"`pg_dump -F c` creates compressed, restorable backups â€” it's the standard."

---

## Question 193: What is `pg_restore`?

## Answer:
`pg_restore` restores a database from a `pg_dump` backup (custom or directory format).

```bash
# Restore from backup
pg_restore -U username -d dbname -c backup.dump

# Restore to a new database
pg_restore -U username -d new_dbname backup.dump

# List contents
pg_restore -l backup.dump
```

`-c` drops existing objects before restoring.

## Key Points:
- Restores from pg_dump backups.
- Custom or directory format.
- `-c` drops existing objects.
- `-l` lists backup contents.
- Can restore to a different database.

## Interview Tip:
"`pg_restore` is the partner to `pg_dump` â€” always test your restore process."

---

## Question 194: What is point-in-time recovery (PITR)?

## Answer:
PITR restores a database to a specific point in time using WAL (Write-Ahead Log) archiving.

1. Start with a base backup.
2. Archive WAL files continuously.
3. Restore to any point by replaying WAL files.

```bash
# Restore to specific time
recovery_target_time = '2024-01-15 14:30:00'
```

## Key Points:
- Restore to any point in time.
- Uses base backup + WAL archiving.
- Essential for disaster recovery.
- Can recover from accidental data loss.
- Requires WAL archiving setup.

## Interview Tip:
"PITR lets you restore to the exact moment before disaster struck â€” it's essential for production."

---

## Question 195: What is Write-Ahead Logging (WAL)?

## Answer:
WAL records all changes before they're applied to the database. It ensures durability â€” if the server crashes, changes can be replayed from the WAL.

WAL is also used for replication and PITR.

## Key Points:
- Records changes before applying them.
- Ensures durability (crash recovery).
- Used for replication.
- Used for PITR.
- WAL files are archived for backup.

## Interview Tip:
"WAL is the foundation of PostgreSQL's durability, replication, and backup features."

---

## Question 196: What is replication in PostgreSQL?

## Answer:
Replication copies data from one database (primary) to another (replica). It improves availability and read performance.

- **Streaming replication**: Physical copy of the primary (WAL-based).
- **Logical replication**: Selective table/data replication.

```sql
-- Logical replication
CREATE PUBLICATION my_pub FOR TABLE users, posts;
CREATE SUBSCRIPTION my_sub CONNECTION 'dbname=mydb' PUBLICATION my_pub;
```

## Key Points:
- Copies data from primary to replica.
- Streaming: full physical copy.
- Logical: selective table/data copy.
- Improves availability and read performance.
- Replica can serve read queries.

## Interview Tip:
"Streaming replication for high availability; logical replication for selective data sync."

---

## Question 197: What is the difference between streaming replication and logical replication?

## Answer:
| Feature | Streaming Replication | Logical Replication |
|---------|---------------------|---------------------|
| Level | Entire database cluster | Selected tables |
| Type | Physical (byte-level) | Logical (row-level) |
| Version | Same version required | Cross-version possible |
| Write | Read-only replica | Can write to replica |
| Use case | HA, read scaling | Data sync, migration |

## Key Points:
- Streaming: entire cluster, physical, same version.
- Logical: selected tables, logical, cross-version.
- Streaming replicas are read-only.
- Logical replicas can have different schemas.
- Logical is more flexible but more complex.

## Interview Tip:
"Streaming for HA and read scaling; logical for selective replication and migrations."

---

## Question 198: What is high availability (HA)?

## Answer:
High availability means the database is always accessible, even if components fail. HA strategies include:
- **Replication**: Primary + replicas.
- **Automatic failover**: Switch to replica if primary fails.
- **Load balancing**: Distribute read queries.
- **Monitoring**: Detect failures quickly.
- **Tools**: Patroni, repmgr for automated failover.

## Key Points:
- Database always accessible.
- Replication + automatic failover.
- Monitoring and alerting.
- Patroni and repmgr for automation.
- Trade-off: cost vs availability.

## Interview Tip:
"HA = replication + automatic failover + monitoring. Patroni is the standard for PostgreSQL HA."

---

## Question 199: How do you monitor PostgreSQL in production?

## Answer:
1. **pg_stat_statements**: Query performance.
2. **pg_stat_activity**: Active connections.
3. **pg_stat_user_indexes**: Index usage.
4. **System metrics**: CPU, memory, disk, network.
5. **Logs**: Error logs, slow query logs.
6. **Tools**: Datadog, New Relic, pgWatch2, Prometheus + Grafana.

## Key Points:
- pg_stat_statements for queries.
- pg_stat_activity for connections.
- System metrics for infrastructure.
- Logs for errors and slow queries.
- External tools for comprehensive monitoring.

## Interview Tip:
"Set up alerts for: connection count, query latency, disk usage, and replication lag."

---

## Question 200: What administrative best practices do you follow for PostgreSQL?

## Answer:
1. **Regular backups**: Daily pg_dump + WAL archiving.
2. **Test restores**: Verify backups work.
3. **Monitor performance**: pg_stat_statements, system metrics.
4. **Regular VACUUM**: Prevent table bloat.
5. **Update statistics**: ANALYZE after large changes.
6. **Security updates**: Keep PostgreSQL patched.
7. **Document procedures**: Backup, restore, failover.
8. **Capacity planning**: Monitor growth and plan ahead.

## Key Points:
- Regular backups and tested restores.
- Performance monitoring.
- Regular VACUUM and ANALYZE.
- Security updates.
- Documentation and capacity planning.

## Interview Tip:
"A good DBA prevents problems â€” regular backups, monitoring, and maintenance."

---

## Part 21 (201â€“210): Database Architecture

---

## Question 201: How do you structure a PostgreSQL database for a large application?

## Answer:
```
Database
â”œâ”€â”€ Schema: public (default)
â”œâ”€â”€ Schema: app (application tables)
â”œâ”€â”€ Schema: audit (audit logs)
â”œâ”€â”€ Schema: reporting (materialized views)
```

Use schemas to organize by domain. Keep application tables, audit logs, and reporting data separate.

## Key Points:
- Use schemas for organization.
- Separate concerns: app, audit, reporting.
- Named schemas for different domains.
- Search path for convenience.
- Extensions in separate schemas.

## Interview Tip:
"Schemas are like namespaces â€” they organize objects and control access."

---

## Question 202: What database design principles do you follow?

## Answer:
1. **Normalize first**: 3NF for most tables.
2. **Meaningful names**: `users` not `tbl1`.
3. **Consistent naming**: `created_at`, `updated_at` everywhere.
4. **Primary keys**: SERIAL or UUID for every table.
5. **Foreign keys**: Enforce relationships.
6. **Indexes**: On foreign keys and frequent queries.
7. **Constraints**: NOT NULL, CHECK, UNIQUE where appropriate.
8. **Documentation**: Schema comments.

## Key Points:
- Normalize first.
- Consistent, meaningful naming.
- Primary keys on every table.
- Foreign keys for relationships.
- Indexes for performance.
- Constraints for integrity.

## Interview Tip:
"Consistent naming and constraints make the schema self-documenting."

---

## Question 203: How do you design a scalable relational database?

## Answer:
1. **Normalize**: Start with 3NF.
2. **Index appropriately**: Foreign keys, WHERE columns.
3. **Partition large tables**: By date or key.
4. **Read replicas**: Distribute read load.
5. **Connection pooling**: PgBouncer or app-level.
6. **Cache**: Redis for frequently accessed data.
7. **Monitor**: Track performance and growth.

## Key Points:
- Normalize for integrity.
- Index for performance.
- Partition for large tables.
- Replicas for read scaling.
- Connection pooling for efficiency.

## Interview Tip:
"Scalable design starts with normalization and indexing â€” add partitioning and replicas as needed."

---

## Question 204: How do you model complex relationships?

## Answer:
- **One-to-one**: Shared primary key.
- **One-to-many**: Foreign key on the many side.
- **Many-to-many**: Junction table.
- **Self-referential**: Foreign key to same table (hierarchy).
- **Polymorphic**: Foreign key + type column (use cautiously).

```sql
-- Self-referential (org chart)
CREATE TABLE employees (
  id SERIAL PRIMARY KEY,
  name TEXT,
  manager_id INTEGER REFERENCES employees(id)
);
```

## Key Points:
- Foreign key for one-to-many.
- Junction table for many-to-many.
- Self-referential for hierarchies.
- Polymorphic is an anti-pattern â€” use separate tables.
- Document complex relationships.

## Interview Tip:
"Self-referential relationships model hierarchies â€” org charts, categories, threads."

---

## Question 205: How do you design an audit logging system?

## Answer:
```sql
CREATE TABLE audit_log (
  id SERIAL PRIMARY KEY,
  table_name TEXT NOT NULL,
  record_id INTEGER NOT NULL,
  action TEXT NOT NULL, -- INSERT, UPDATE, DELETE
  old_data JSONB,
  new_data JSONB,
  changed_by TEXT,
  changed_at TIMESTAMPTZ DEFAULT NOW()
);

-- Trigger to capture changes
CREATE FUNCTION audit_trigger_func()
RETURNS TRIGGER AS $$
BEGIN
  INSERT INTO audit_log (table_name, record_id, action, old_data, new_data, changed_by)
  VALUES (TG_TABLE_NAME, NEW.id, TG_OP, to_jsonb(OLD), to_jsonb(NEW), current_user);
  RETURN NEW;
END;
$$ LANGUAGE plpgsql;
```

## Key Points:
- Log all data changes.
- Store old and new values.
- Trigger-based for automatic capture.
- Include timestamp and user.
- Partition audit logs by date for performance.

## Interview Tip:
"Audit logs track who changed what and when â€” essential for compliance and debugging."

---

## Question 206: How do you implement soft deletes?

## Answer:
Add a `deleted_at` column instead of actually deleting rows.

```sql
ALTER TABLE users ADD COLUMN deleted_at TIMESTAMPTZ;

-- Soft delete
UPDATE users SET deleted_at = NOW() WHERE id = 1;

-- Query active records
SELECT * FROM users WHERE deleted_at IS NULL;

-- Partial index for performance
CREATE INDEX idx_users_active ON users (id) WHERE deleted_at IS NULL;
```

## Key Points:
- `deleted_at` TIMESTAMP column.
- NULL = active, non-NULL = deleted.
- Partial index for performance.
- Data is preserved for recovery.
- Filter with `WHERE deleted_at IS NULL`.

## Interview Tip:
"Soft deletes preserve data for recovery â€” use a partial index to keep queries fast."

---

## Question 207: How do you implement multi-tenancy?

## Answer:
Three approaches:
1. **Shared database, shared schema**: Tenant ID column.
2. **Shared database, separate schemas**: Each tenant has own schema.
3. **Separate databases**: Each tenant has own database.

```sql
-- Approach 1: Tenant ID column
CREATE TABLE orders (
  id SERIAL PRIMARY KEY,
  tenant_id INTEGER NOT NULL,
  amount DECIMAL,
  FOREIGN KEY (tenant_id) REFERENCES tenants(id)
);

-- Row-level security
CREATE POLICY tenant_isolation ON orders
  USING (tenant_id = current_setting('app.current_tenant')::INTEGER);
```

## Key Points:
- Shared schema: tenant_id column (simplest).
- Separate schemas: per-tenant schema.
- Separate databases: per-tenant database (most isolated).
- Row-level security for shared schema.
- Trade-off: cost vs isolation.

## Interview Tip:
"Row-level security with shared schema is the most common multi-tenancy approach."

---

## Question 208: What is the difference between shared-database and separate-database multi-tenancy?

## Answer:
| Aspect | Shared Database | Separate Database |
|--------|----------------|-------------------|
| Isolation | Row-level (RLS) | Full database |
| Cost | Lower | Higher |
| Maintenance | One database | Many databases |
| Backup | Single backup | Per-tenant backups |
| Scalability | Limited | Independent |
| Complexity | Simpler | More complex |

## Key Points:
- Shared: lower cost, simpler, less isolated.
- Separate: higher cost, more isolated, independent scaling.
- Shared with RLS for most SaaS apps.
- Separate for high-security or compliance needs.

## Interview Tip:
"Shared database with RLS is the most common â€” it's cost-effective and secure enough for most SaaS."

---

## Question 209: How do you manage schema changes in production?

## Answer:
1. **Migration tools**: Alembic, Flyway, Prisma Migrate.
2. **Zero-downtime migrations**: Online schema changes.
3. **Backward compatibility**: New columns with defaults.
4. **Version control**: Migrations in git.
5. **Test migrations**: Run in staging first.

```sql
-- Safe: add column with default
ALTER TABLE users ADD COLUMN role TEXT DEFAULT 'user';

-- Unsafe: rename column (breaks existing queries)
ALTER TABLE users RENAME COLUMN name TO full_name;
```

## Key Points:
- Use migration tools.
- Zero-downtime changes.
- Backward compatible changes.
- Version control migrations.
- Test in staging first.

## Interview Tip:
"Schema changes should be backward compatible â€” add new columns, don't rename old ones."

---

## Question 210: What database architecture patterns have you used?

## Answer:
- **Monolithic database**: Single database for all features.
- **Database per service**: Microservices with own databases.
- **CQRS**: Separate read and write databases.
- **Event sourcing**: Store events, not state.
- **Shared database**: Multiple services share one database.
- **Data warehouse**: Separate analytics database.

Most applications start with a monolithic database and evolve as needed.

## Key Points:
- Monolithic: simple, single database.
- Per-service: microservices pattern.
- CQRS: separate read/write.
- Event sourcing: store events.
- Start simple, evolve as needed.

## Interview Tip:
"Start with a monolithic database â€” don't over-architect from day one."

---

## Part 22 (211â€“220): Scaling PostgreSQL

---

## Question 211: How do you scale PostgreSQL?

## Answer:
1. **Vertical scaling**: More CPU, RAM, storage on one server.
2. **Read replicas**: Distribute read queries.
3. **Connection pooling**: PgBouncer for efficient connections.
4. **Partitioning**: Divide large tables.
5. **Caching**: Redis for frequently accessed data.
6. **Sharding**: Split data across multiple servers.
7. **Optimization**: Indexes, query tuning.

## Key Points:
- Vertical: bigger server.
- Horizontal reads: read replicas.
- Connection pooling: PgBouncer.
- Partitioning: divide large tables.
- Caching: Redis.
- Sharding: split across servers.

## Interview Tip:
"Start with vertical scaling and read replicas â€” shard only when you have no other option."

---

## Question 212: What are read replicas?

## Answer:
Read replicas are copies of the primary database that serve read queries. They reduce load on the primary and improve read performance.

```sql
-- On primary
CREATE PUBLICATION my_pub FOR ALL TABLES;

-- On replica
CREATE SUBSCRIPTION my_sub CONNECTION 'host=primary dbname=mydb' PUBLICATION my_pub;
```

Replicas can be streaming (physical) or logical.

## Key Points:
- Copies of primary for read queries.
- Reduce primary load.
- Improve read performance.
- Streaming or logical replication.
- Can be in different regions.

## Interview Tip:
"Read replicas are the easiest way to scale reads â€” they reduce load on the primary."

---

## Question 213: When should you use read replicas?

## Answer:
- **Read-heavy workloads**: 80%+ reads, 20% writes.
- **Geographic distribution**: Replicas in different regions.
- **Reporting queries**: Run analytics on replicas, not primary.
- **High availability**: Failover to replica if primary fails.
- **Load reduction**: Offload reads from primary.

## Key Points:
- Read-heavy workloads.
- Geographic distribution.
- Reporting and analytics.
- High availability.
- Load reduction.

## Interview Tip:
"Use read replicas for reporting and analytics â€” don't run heavy queries on the primary."

---

## Question 214: What is database sharding?

## Answer:
Sharding splits a database into smaller pieces (shards) across multiple servers. Each shard contains a subset of the data.

```
Shard 1: users 1-1000
Shard 2: users 1001-2000
Shard 3: users 2001-3000
```

Sharding enables horizontal scaling but adds complexity.

## Key Points:
- Splits data across multiple servers.
- Each shard is an independent database.
- Enables horizontal scaling.
- Adds significant complexity.
- Requires shard key and routing logic.

## Interview Tip:
"Sharding is the nuclear option â€” it solves scaling but adds massive complexity."

---

## Question 215: When should you shard a database?

## Answer:
- **Data exceeds single server capacity**: >10TB or >100K QPS.
- **Write scaling**: Multiple primaries for writes.
- **Geographic distribution**: Data close to users.
- **Before sharding, try**: Vertical scaling, read replicas, partitioning.

Most applications never need sharding.

## Key Points:
- Data exceeds single server capacity.
- Write scaling beyond one server.
- Geographic distribution.
- Last resort after other options.
- Most apps never need sharding.

## Interview Tip:
"Shard only when you've exhausted all other options â€” it's the last resort for scaling."

---

## Question 216: What are the advantages and disadvantages of sharding?

## Answer:
| Aspect | Advantages | Disadvantages |
|--------|-----------|--------------|
| Scaling | Horizontal write scaling | Cross-shard queries are complex |
| Performance | Parallel processing | Distributed transactions |
| Availability | Independent shards | Shard failure affects subset |
| Complexity | None (simple shards) | Significant (routing, joins) |

## Key Points:
- Advantages: horizontal scaling, parallel processing.
- Disadvantages: cross-shard queries, distributed transactions.
- Significant complexity increase.
- Most apps don't need sharding.
- Consider before sharding.

## Interview Tip:
"Sharding solves scaling but creates new problems â€” cross-shard queries are especially painful."

---

## Question 217: What is horizontal scaling?

## Answer:
Horizontal scaling (scaling out) adds more servers to handle increased load. Each server handles a portion of the workload.

In PostgreSQL: read replicas, sharding, connection pooling.

## Key Points:
- Add more servers.
- Each handles a portion of load.
- Read replicas for read scaling.
- Sharding for write scaling.
- More resilient than vertical scaling.

## Interview Tip:
"Horizontal scaling = more servers. Vertical scaling = bigger server."

---

## Question 218: What is vertical scaling?

## Answer:
Vertical scaling (scaling up) adds more CPU, RAM, or storage to a single server. It's simpler but has hardware limits.

## Key Points:
- More resources per server.
- Simpler than horizontal scaling.
- Limited by hardware maximums.
- No architectural changes needed.
- Good for initial scaling.

## Interview Tip:
"Vertical scaling is the simplest approach â€” just add more resources to the existing server."

---

## Question 219: How do you handle millions of rows efficiently?

## Answer:
1. **Indexing**: Proper indexes on queried columns.
2. **Partitioning**: Divide by date or key range.
3. **Pagination**: Use cursor-based pagination.
4. **Select only needed columns**: Avoid SELECT *.
5. **Batch operations**: Process in chunks.
6. **Connection pooling**: Efficient connection management.
7. **Read replicas**: Distribute read load.

## Key Points:
- Indexes for fast lookups.
- Partitioning for large tables.
- Cursor-based pagination.
- Select only needed columns.
- Batch operations for bulk processing.

## Interview Tip:
"Partitioning + indexing + cursor-based pagination handles millions of rows efficiently."

---

## Question 220: What are common scalability bottlenecks in PostgreSQL?

## Answer:
1. **Single primary**: Write scaling limited.
2. **Connection exhaustion**: Too many connections.
3. **Slow queries**: Missing indexes, bad query plans.
4. **Lock contention**: Deadlocks and blocking.
5. **Disk I/O**: Insufficient IOPS.
6. **Memory**: Too little shared_buffers or work_mem.
7. **Write amplification**: Too many indexes.

## Key Points:
- Single primary limits write scaling.
- Connection exhaustion under load.
- Slow queries from missing indexes.
- Lock contention from concurrent writes.
- Disk I/O and memory limitations.

## Interview Tip:
"Connection pooling and proper indexing solve most scalability bottlenecks."

---

## Part 23 (221â€“230): Production Optimization

---

## Question 221: How do you troubleshoot slow SQL queries?

## Answer:
1. **EXPLAIN ANALYZE**: See the execution plan.
2. **Check for sequential scans**: Missing indexes.
3. **Check statistics**: ANALYZE to update.
4. **Check locks**: Blocked queries.
5. **Check connections**: Too many connections.
6. **Check memory**: work_mem too low.
7. **Rewrite query**: Use JOINs instead of subqueries.

## Key Points:
- EXPLAIN ANALYZE first.
- Look for sequential scans.
- Update statistics with ANALYZE.
- Check for blocking queries.
- Verify connection count and memory settings.

## Interview Tip:
"EXPLAIN ANALYZE is the first tool â€” it tells you exactly what's slow and why."

---

## Question 222: How do you identify blocking queries?

## Answer:
```sql
-- Find blocking queries
SELECT
  blocked.pid AS blocked_pid,
  blocked.query AS blocked_query,
  blocking.pid AS blocking_pid,
  blocking.query AS blocking_query
FROM pg_stat_activity blocked
JOIN pg_locks blocked_locks ON blocked.pid = blocked_locks.pid
JOIN pg_locks blocking_locks ON blocked_locks.locktype = blocking_locks.locktype
  AND blocking_locks.relation = blocked_locks.relation
  AND blocking_locks.pid != blocked.pid
JOIN pg_stat_activity blocking ON blocking_locks.pid = blocking.pid
WHERE NOT blocked_locks.granted;
```

## Key Points:
- Query pg_stat_activity and pg_locks.
- Find waiting and blocking processes.
- Check query text for both.
- Kill blocking query if needed.
- Prevent with shorter transactions.

## Interview Tip:
"The pg_locks + pg_stat_activity join shows you exactly who's blocking whom."

---

## Question 223: How do you monitor database performance?

## Answer:
1. **pg_stat_statements**: Query performance tracking.
2. **pg_stat_activity**: Active connections and queries.
3. **pg_stat_user_indexes**: Index usage.
4. **pg_stat_user_tables**: Table statistics.
5. **System metrics**: CPU, memory, disk, network.
6. **External tools**: Datadog, Prometheus, pgWatch2.

## Key Points:
- pg_stat_statements for queries.
- pg_stat_activity for connections.
- pg_stat_user_indexes for index usage.
- System metrics for infrastructure.
- External tools for dashboards and alerts.

## Interview Tip:
"pg_stat_statements is the most valuable tool â€” it shows your slowest queries."

---

## Question 224: Which PostgreSQL metrics do you monitor?

## Answer:
- **Connections**: Active, idle, waiting.
- **Query performance**: Latency, throughput, slow queries.
- **Cache hit ratio**: Should be >99%.
- **Replication lag**: For read replicas.
- **Disk usage**: Tablespace growth.
- **Lock waits**: Blocking queries.
- **Transaction rate**: Commits/rollbacks per second.
- **Index usage**: Scan types and frequency.

## Key Points:
- Connection count and state.
- Query latency and throughput.
- Cache hit ratio (>99% ideal).
- Replication lag.
- Disk and memory usage.
- Lock waits and deadlocks.

## Interview Tip:
"Cache hit ratio below 99% means you need more memory â€” it's the most important metric."

---

## Question 225: How do you optimize connection pooling?

## Answer:
- **Pool size**: Match to database max_connections.
- **Idle timeout**: Close unused connections.
- **Connection timeout**: Fail fast if no connections available.
- **PgBouncer modes**: Transaction mode for most apps.
- **Monitor**: Track active, idle, and waiting connections.

```javascript
// Node.js pg pool configuration
const pool = new Pool({
  max: 20,              // Max connections
  idleTimeoutMillis: 30000, // Close idle connections
  connectionTimeoutMillis: 2000 // Fail if no connection
});
```

## Key Points:
- Right pool size for workload.
- Idle timeout to release connections.
- Connection timeout for fast failure.
- PgBouncer for external pooling.
- Monitor connection usage.

## Interview Tip:
"Pool size should be less than max_connections â€” leave room for admin connections."

---

## Question 226: How do you optimize disk usage?

## Answer:
1. **VACUUM**: Reclaim dead tuple space.
2. **REINDEX**: Rebuild fragmented indexes.
3. **Partition old data**: Drop old partitions.
4. **Compression**: Compress old data.
5. **Data archiving**: Move old data to cheaper storage.
6. **Select only needed columns**: Avoid SELECT *.

## Key Points:
- VACUUM reclaims dead tuples.
- REINDEX rebuilds fragmented indexes.
- Partition and drop old data.
- Archive old data to cheaper storage.
- Monitor table and index sizes.

## Interview Tip:
"VACUUM regularly â€” it reclaims space from dead tuples."

---

## Question 227: How do you optimize memory settings?

## Answer:
Key settings:
- **shared_buffers**: 25% of system RAM (for cached data).
- **work_mem**: Per-operation memory for sorts and hashes.
- **maintenance_work_mem**: For VACUUM, REINDEX.
- **effective_cache_size**: 75% of RAM (query planner hint).

```sql
ALTER SYSTEM SET shared_buffers = '4GB';
ALTER SYSTEM SET work_mem = '256MB';
ALTER SYSTEM SET maintenance_work_mem = '1GB';
```

## Key Points:
- shared_buffers: 25% of RAM.
- work_mem: per-operation memory.
- maintenance_work_mem: for maintenance tasks.
- effective_cache_size: planner hint.
- Tune based on workload.

## Interview Tip:
"shared_buffers = 25% of RAM is the standard starting point."

---

## Question 228: How do you optimize PostgreSQL for high write throughput?

## Answer:
1. **Reduce indexes**: Each index slows writes.
2. **Batch inserts**: Insert multiple rows at once.
3. **Tune WAL settings**: wal_buffers, checkpoint_segments.
4. **Use UNLOGGED tables**: For temporary data (no WAL).
5. **Connection pooling**: Efficient connection management.
6. **Partition tables**: Distribute write load.

## Key Points:
- Fewer indexes = faster writes.
- Batch operations for bulk inserts.
- WAL tuning for write performance.
- UNLOGGED tables for temporary data.
- Partitioning distributes write load.

## Interview Tip:
"Every index slows writes â€” only index what you need."

---

## Question 229: What maintenance tasks should be scheduled regularly?

## Answer:
1. **VACUUM**: Reclaim dead tuple space (auto-vacuum enabled by default).
2. **ANALYZE**: Update statistics for query planner.
3. **REINDEX**: Rebuild fragmented indexes.
4. **Backup**: Daily pg_dump + WAL archiving.
5. **Monitor**: Check performance metrics.
6. **Update**: Apply security patches.

## Key Points:
- VACUUM and ANALYZE (auto-vacuum handles most).
- REINDEX when indexes are bloated.
- Regular backups.
- Performance monitoring.
- Security updates.

## Interview Tip:
"Auto-vacuum handles most VACUUM tasks â€” but monitor it to make sure it's running."

---

## Question 230: What production best practices do you always follow?

## Answer:
1. **Backups**: Daily pg_dump + WAL archiving.
2. **Monitoring**: pg_stat_statements, system metrics.
3. **Connection pooling**: PgBouncer or app-level.
4. **SSL/TLS**: Encrypted connections.
5. **Least privilege**: Minimal permissions.
6. **Parameterized queries**: Prevent SQL injection.
7. **Regular VACUUM**: Prevent table bloat.
8. **Documentation**: Procedures and runbooks.

## Key Points:
- Backups and tested restores.
- Performance monitoring.
- Connection pooling.
- Security (SSL, least privilege, parameterized queries).
- Regular maintenance.

## Interview Tip:
"Backups, monitoring, and security are the three pillars of production databases."

---

## Part 24 (231â€“240): Real-World Database Design

---

## Question 231: How would you design the database for an e-commerce platform?

## Answer:
```
tenants (id, name, plan)
users (id, tenant_id, name, email, role)
products (id, tenant_id, name, price, stock)
categories (id, tenant_id, name, parent_id)
orders (id, tenant_id, user_id, status, total)
order_items (id, order_id, product_id, quantity, price)
payments (id, order_id, method, amount, status)
reviews (id, user_id, product_id, rating, comment)
```

Key: multi-tenant, product catalog, order management, payments.

## Key Points:
- Multi-tenant with tenant_id.
- Product catalog with categories.
- Order management with items.
- Payment tracking.
- Review system.

## Interview Tip:
"Multi-tenant e-commerce needs tenant_id on every table and row-level security."

---

## Question 232: How would you design the database for a CRM system?

## Answer:
```
companies (id, name, industry, size)
contacts (id, company_id, name, email, phone)
deals (id, contact_id, stage, amount, close_date)
activities (id, contact_id, deal_id, type, subject, date)
notes (id, contact_id, deal_id, content)
tags (id, name)
contact_tags (contact_id, tag_id)
```

Key: contact management, deal pipeline, activity tracking.

## Key Points:
- Company and contact management.
- Deal pipeline with stages.
- Activity and note tracking.
- Tagging system.
- Pipeline reporting.

## Interview Tip:
"The deal pipeline with stages is the heart of a CRM â€” design it for flexible reporting."

---

## Question 233: How would you design the database for an ERP system?

## Answer:
```
companies (id, name, type)
employees (id, company_id, department_id, name, role)
departments (id, name, parent_id)
products (id, name, sku, price, category)
inventory (id, product_id, warehouse_id, quantity)
orders (id, company_id, type, status, total)
order_items (id, order_id, product_id, quantity, price)
invoices (id, order_id, status, due_date)
payments (id, invoice_id, amount, method)
```

Key: complex entities, inventory, invoicing, multi-company.

## Key Points:
- Multi-company support.
- Employee and department management.
- Product and inventory tracking.
- Order and invoice management.
- Payment processing.

## Interview Tip:
"ERP systems are complex â€” focus on the core entities: companies, products, orders, and invoices."

---

## Question 234: How would you design the database for a social media application?

## Answer:
```
users (id, username, email, bio, avatar_url)
posts (id, user_id, content, media_url, created_at)
comments (id, post_id, user_id, content, parent_id)
likes (id, user_id, post_id)
follows (follower_id, following_id)
messages (id, sender_id, receiver_id, content, read_at)
notifications (id, user_id, type, reference_id, read_at)
```

Key: user-generated content, social graph, real-time notifications.

## Key Points:
- User profiles and posts.
- Comments with threading (parent_id).
- Like and follow system.
- Direct messaging.
- Notifications.

## Interview Tip:
"The follows table creates the social graph â€” it's the foundation of the feed algorithm."

---

## Question 235: How would you design the database for a school management system?

## Answer:
```
students (id, name, email, enrollment_date)
teachers (id, name, email, department)
courses (id, teacher_id, name, code, semester)
enrollments (student_id, course_id, grade, status)
assignments (id, course_id, title, due_date, max_score)
submissions (id, assignment_id, student_id, score, submitted_at)
attendance (student_id, course_id, date, status)
```

Key: student enrollment, grading, attendance tracking.

## Key Points:
- Student and teacher management.
- Course and enrollment tracking.
- Assignment and submission grading.
- Attendance tracking.
- Grade management.

## Interview Tip:
"The enrollments table is the junction between students and courses â€” it tracks grades and status."

---

## Question 236: How would you design the database for a booking system?

## Answer:
```
resources (id, name, type, capacity)
bookings (id, resource_id, user_id, start_time, end_time, status)
availability (resource_id, day_of_week, start_time, end_time)
blocked_times (resource_id, start_time, end_time, reason)
```

Key: resource management, time slot booking, availability.

## Key Points:
- Resource management.
- Time-based bookings.
- Availability rules.
- Conflict prevention.
- Booking status tracking.

## Interview Tip:
"Prevent double-booking with a check constraint or exclusion constraint on time ranges."

---

## Question 237: How would you handle concurrent seat booking without double-booking?

## Answer:
Use a transaction with `FOR UPDATE` or an exclusion constraint:

```sql
-- Method 1: FOR UPDATE
BEGIN;
SELECT * FROM seats WHERE id = 1 FOR UPDATE;
-- Check if available
UPDATE seats SET status = 'booked' WHERE id = 1 AND status = 'available';
COMMIT;

-- Method 2: Exclusion constraint (PostgreSQL-specific)
ALTER TABLE bookings ADD CONSTRAINT no_overlap
  EXCLUDE USING gist (
    resource_id WITH =,
    tstzrange(start_time, end_time) WITH &&
  );
```

## Key Points:
- FOR UPDATE for pessimistic locking.
- Exclusion constraint for automatic conflict prevention.
- Transactions ensure atomicity.
- Retry logic for conflicts.
- Exclusion constraints are the cleanest solution.

## Interview Tip:
"Exclusion constraints are the PostgreSQL way to prevent overlapping bookings â€” they're elegant and efficient."

---

## Question 238: How would you design an inventory management database?

## Answer:
```
products (id, sku, name, category)
warehouses (id, name, location)
inventory (product_id, warehouse_id, quantity, reorder_level)
stock_movements (id, product_id, warehouse_id, quantity, type, reference)
purchase_orders (id, supplier_id, status, total)
purchase_order_items (po_id, product_id, quantity, cost)
```

Key: multi-warehouse inventory, stock movements, reorder management.

## Key Points:
- Product catalog with SKUs.
- Multi-warehouse support.
- Inventory tracking per warehouse.
- Stock movement history.
- Purchase order management.

## Interview Tip:
"Stock_movements is the audit trail â€” it tracks every quantity change."

---

## Question 239: How would you design an order and payment system?

## Answer:
```
orders (id, user_id, status, total, currency)
order_items (id, order_id, product_id, quantity, price)
payments (id, order_id, method, amount, status, transaction_id)
refunds (id, payment_id, amount, reason, status)
coupons (id, code, discount_type, discount_value, valid_until)
order_coupons (order_id, coupon_id)
```

Key: order lifecycle, payment processing, refunds, promotions.

## Key Points:
- Order lifecycle (pending, paid, shipped, delivered).
- Payment processing with transaction IDs.
- Refund management.
- Coupon and promotion system.
- Order items with pricing snapshot.

## Interview Tip:
"Snapshot the price in order_items â€” product prices change, but order prices shouldn't."

---

## Question 240: How would you migrate a large production database with minimal downtime?

## Answer:
1. **Create a copy**: Clone the database.
2. **Apply changes**: Run migrations on the copy.
3. **Sync data**: Keep both databases in sync.
4. **Switch traffic**: Update connection strings.
5. **Verify**: Monitor the new database.
6. **Cleanup**: Remove the old database.

Use logical replication for continuous sync during migration.

## Key Points:
- Clone the database first.
- Apply migrations on the copy.
- Sync data during migration.
- Switch traffic atomically.
- Verify before cleanup.

## Interview Tip:
"The key is keeping both databases in sync during the migration â€” logical replication helps."

---

## Part 25 (241â€“250): Senior Real-World Interview Questions

---

## Question 241: Describe the largest PostgreSQL database you've worked with.

## Answer:
Pick a real project and describe:
- **Scale**: Rows, size, queries per second.
- **Architecture**: Single server, replicas, sharding.
- **Challenges**: What was hard and how you solved it.
- **Your role**: What you specifically contributed.
- **Results**: Performance improvements, cost savings.

## Key Points:
- Quantify the scale (rows, size, QPS).
- Describe the architecture.
- Highlight challenges and solutions.
- Explain your specific contributions.
- Show the impact of your work.

## Interview Tip:
"Tell a story with a beginning (problem), middle (solution), and end (result)."

---

## Question 242: What was the most difficult database issue you've solved?

## Answer:
Describe:
1. **Symptoms**: What was happening.
2. **Investigation**: How you diagnosed it.
3. **Root cause**: What was actually wrong.
4. **Fix**: How you resolved it.
5. **Lesson**: What you learned.

Choose an issue that shows your debugging process.

## Key Points:
- Describe symptoms, investigation, root cause, fix, and lesson.
- Show systematic debugging approach.
- Mention tools you used.
- Explain what you learned.
- Choose a technically interesting issue.

## Interview Tip:
"Interviewers want to see your debugging process, not just the fix."

---

## Question 243: How do you debug production database performance issues?

## Answer:
1. **Check pg_stat_statements**: Find slow queries.
2. **EXPLAIN ANALYZE**: Analyze execution plans.
3. **Check locks**: Blocking queries.
4. **Check connections**: Too many connections.
5. **Check memory**: shared_buffers, work_mem.
6. **Check disk**: I/O, table bloat.
7. **Check statistics**: ANALYZE outdated?

## Key Points:
- Start with pg_stat_statements.
- EXPLAIN ANALYZE for individual queries.
- Check for blocking and locks.
- Monitor connections and memory.
- Check disk I/O and table bloat.

## Interview Tip:
"Start with pg_stat_statements â€” it shows your slowest queries."

---

## Question 244: How do you review SQL queries during a pull request?

## Answer:
Check for:
1. **Missing indexes**: Are WHERE/JOIN columns indexed?
2. **N+1 queries**: Are there loops of queries?
3. **SELECT ***: Are only needed columns selected?
4. **Parameterized queries**: Is SQL injection prevented?
5. **Transaction scope**: Are transactions as short as possible?
6. **EXPLAIN ANALYZE**: Has the query been profiled?
7. **Data integrity**: Are constraints and foreign keys used?

## Key Points:
- Check for missing indexes.
- Look for N+1 queries.
- Verify parameterized queries.
- Keep transactions short.
- Test with EXPLAIN ANALYZE.

## Interview Tip:
"Run EXPLAIN ANALYZE on every new query in the PR â€” catch performance issues early."

---

## Question 245: What SQL coding standards do you enforce?

## Answer:
1. **Consistent formatting**: Uppercase keywords, lowercase identifiers.
2. **Meaningful names**: `users` not `tbl1`, `created_at` not `col2`.
3. **Explicit JOINs**: Never use implicit comma joins.
4. **Parameterized queries**: No string concatenation.
5. **Comments**: Explain complex logic.
6. **EXPLAIN ANALYZE**: Test new queries.
7. **No SELECT ***: Select only needed columns.

## Key Points:
- Consistent formatting and naming.
- Explicit JOIN syntax.
- Parameterized queries for security.
- Comments for complex logic.
- Profile new queries.

## Interview Tip:
"Consistent SQL style makes code review easier and reduces bugs."

---

## Question 246: How do you mentor junior developers on database design?

## Answer:
1. **Explain normalization**: Why it matters.
2. **Review their schemas**: Provide feedback.
3. **Teach indexing**: When and why to index.
4. **Show EXPLAIN ANALYZE**: How to profile queries.
5. **Pair on design**: Work through schema design together.
6. **Share resources**: Documentation, books, courses.

## Key Points:
- Teach normalization principles.
- Review schemas with them.
- Explain indexing strategy.
- Show how to profile queries.
- Pair on design decisions.

## Interview Tip:
"The best way to teach database design is to review their work and explain the why."

---

## Question 247: What PostgreSQL features do you use most often in production?

## Answer:
- **JSONB**: For flexible, queryable document storage.
- **CTEs**: For readable complex queries.
- **Window functions**: For analytics and rankings.
- **Partial indexes**: For filtered queries.
- **Materialized views**: For expensive aggregations.
- **Row-level security**: For multi-tenancy.
- **pg_stat_statements**: For query performance monitoring.

## Key Points:
- JSONB for document storage.
- CTEs for query readability.
- Window functions for analytics.
- Partial indexes for filtered queries.
- Materialized views for performance.

## Interview Tip:
"JSONB, CTEs, and window functions are the most used PostgreSQL features in production."

---

## Question 248: If you were building a production SaaS today, how would you design the database?

## Answer:
- **PostgreSQL**: Primary database.
- **Multi-tenancy**: tenant_id + row-level security.
- **UUIDs**: For primary keys (distributed generation).
- **JSONB**: For flexible user configuration.
- **Read replicas**: For read scaling.
- **PgBouncer**: Connection pooling.
- **Redis**: Caching and sessions.
- **Backups**: pg_dump + WAL archiving.

## Key Points:
- PostgreSQL as primary database.
- Multi-tenant with row-level security.
- UUIDs for distributed generation.
- JSONB for flexible schemas.
- Read replicas and connection pooling.

## Interview Tip:
"PostgreSQL + row-level security + read replicas is the standard SaaS database architecture."

---

## Question 249: What PostgreSQL best practices do you always follow?

## Answer:
1. **Primary keys**: SERIAL or UUID on every table.
2. **Foreign keys**: Enforce all relationships.
3. **Indexes**: On foreign keys and frequent queries.
4. **NOT NULL**: For required fields.
5. **Timestamps**: created_at and updated_at.
6. **Parameterized queries**: Prevent SQL injection.
7. **Backups**: Daily and tested restores.
8. **Monitoring**: pg_stat_statements and system metrics.

## Key Points:
- Primary keys and foreign keys on every table.
- Indexes for performance.
- Constraints for integrity.
- Timestamps for auditing.
- Security and monitoring.

## Interview Tip:
"Primary keys, foreign keys, indexes, and constraints â€” the four pillars of good database design."

---

## Question 250: In your opinion, what separates a junior, mid-level, and senior PostgreSQL developer?

## Answer:
- **Junior**: Knows basic SQL â€” SELECT, INSERT, JOIN. Can write simple queries with guidance.
- **Mid-level**: Understands indexes, transactions, and performance. Can design schemas and optimize queries independently.
- **Senior**: Designs scalable architectures, handles production issues, mentors others. Understands trade-offs, replication, partitioning, and security.

The biggest differentiator: a senior developer understands WHY, not just WHAT.

## Key Points:
- Junior: basic SQL, guided work.
- Mid-level: indexes, transactions, schema design.
- Senior: architecture, production, mentoring.
- Senior understands trade-offs.
- Senior thinks about scalability and security.

## Interview Tip:
"The best answer shows self-awareness. Pick your level and explain what you're doing to grow."

---

# End of PostgreSQL Interview Questions & Answers
