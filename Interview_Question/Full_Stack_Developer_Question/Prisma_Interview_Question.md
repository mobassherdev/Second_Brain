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

# ANSWERS


---

## Part 1 (1â€“10): Introduction

---

## Question 1: What is Prisma ORM?

## Answer:
Prisma is a modern, type-safe ORM (Object-Relational Mapper) for Node.js and TypeScript. It consists of three parts:

1. **Prisma Schema**: Defines your data models and relationships.
2. **Prisma Client**: Auto-generated, type-safe database client.
3. **Prisma Migrate**: Database migration tool.

Unlike traditional ORMs, Prisma doesn't map objects to database rows. Instead, it generates a client based on your schema that gives you full type safety and auto-completion.

```typescript
const users = await prisma.user.findMany({
  where: { email: "alice@example.com" },
  include: { posts: true }
});
// TypeScript knows: users is User[], each with posts
```

## Key Points:
- Modern ORM for Node.js and TypeScript.
- Schema-first approach (not code-first).
- Auto-generated, type-safe client.
- Built-in migrations and seeding.
- Supports PostgreSQL, MySQL, SQLite, MongoDB, SQL Server.

## Interview Tip:
"Prisma is schema-first â€” you define the schema, and the client is generated from it. This gives you type safety without writing type annotations manually."

---

## Question 2: Why was Prisma created?

## Answer:
Prisma was created to solve problems with existing Node.js ORMs:
- **TypeScript support**: Most ORMs had poor or manual TypeScript types.
- **Migration complexity**: Migrations were error-prone and manual.
- **Developer experience**: Auto-completion and type safety were missing.
- **Database abstraction**: Hard to switch databases.
- **Query complexity**: Raw SQL was often needed for complex queries.

Prisma provides a clean, type-safe API with automatic migrations and excellent developer experience.

## Key Points:
- Solves poor TypeScript support in existing ORMs.
- Automatic, reliable migrations.
- Excellent developer experience (auto-completion, type safety).
- Database abstraction (switch databases easily).
- Clean API that generates raw SQL under the hood.

## Interview Tip:
"Prisma was created because existing ORMs had bad TypeScript support and complex migrations â€” Prisma solved both."

---

## Question 3: What problems does Prisma solve?

## Answer:
1. **Type safety**: Auto-generated TypeScript types from schema.
2. **Migrations**: Automatic, version-controlled database migrations.
3. **Query building**: Type-safe query builder instead of raw SQL.
4. **Introspection**: Generate schema from existing database.
5. **Database abstraction**: Switch databases with minimal code changes.
6. **Developer experience**: Auto-completion, inline documentation.
7. **Relation handling**: Easy nested queries and relation management.

## Key Points:
- Type safety without manual type definitions.
- Automatic migrations from schema changes.
- Type-safe queries with auto-completion.
- Introspect existing databases.
- Switch databases easily.
- Excellent DX with auto-completion.

## Interview Tip:
"Prisma solves the type safety problem â€” your queries are fully typed without writing type annotations."

---

## Question 4: What are the advantages of Prisma over traditional ORMs?

## Answer:
- **Type safety**: Auto-generated types from schema.
- **Schema-first**: Schema is the source of truth.
- **Auto-completion**: Full IntelliSense support.
- **Migrations**: Automatic, version-controlled.
- **Introspection**: Generate schema from existing DB.
- **Query simplicity**: Clean, readable queries.
- **No model classes**: Lightweight, no class overhead.
- **Raw SQL escape hatch**: `$queryRaw` when needed.

```typescript
// Type-safe, auto-completed, readable
const user = await prisma.user.findUnique({
  where: { id: 1 },
  include: { posts: true, profile: true }
});
// TypeScript knows: user.posts is Post[], user.profile is Profile | null
```

## Key Points:
- Type safety from schema.
- Schema-first (not code-first).
- Auto-completion everywhere.
- Automatic migrations.
- Lightweight â€” no model classes.
- Raw SQL escape hatch.

## Interview Tip:
"The biggest advantage is type safety â€” Prisma generates types from your schema, so every query is fully typed."

---

## Question 5: What are the disadvantages of Prisma?

## Answer:
- **Learning curve**: Schema syntax and Prisma-specific concepts.
- **Limited raw SQL**: Some complex queries need `$queryRaw`.
- **No model classes**: Can't add methods to models.
- **Bundle size**: Generated client can be large.
- **Migration limitations**: Some schema changes require manual SQL.
- **Performance overhead**: Extra abstraction layer.
- **MongoDB support**: Less mature than SQL database support.

## Key Points:
- Schema syntax has a learning curve.
- Some queries need raw SQL escape hatch.
- No model classes (no `user.save()` pattern).
- Generated client can be large.
- Some migrations need manual intervention.
- Performance overhead from abstraction.

## Interview Tip:
"Honesty about disadvantages shows maturity â€” 'Prisma's biggest limitation is no model classes, which means I sometimes need raw SQL for complex logic.'"

---

## Question 6: How does Prisma differ from TypeORM?

## Answer:
| Feature | Prisma | TypeORM |
|---------|--------|---------|
| Approach | Schema-first | Code-first |
| Type safety | Auto-generated | Manual decorators |
| Migrations | Automatic from schema | Manual from entities |
| Query style | Method chaining | Query builder/Query API |
| Model classes | No | Yes (Active Record/Data Mapper) |
| DX | Excellent auto-completion | Good with decorators |

Prisma is simpler and more type-safe; TypeORM is more traditional and flexible.

## Key Points:
- Prisma: schema-first, auto-generated types.
- TypeORM: code-first, decorator-based.
- Prisma has better auto-completion.
- TypeORM has model classes (Active Record pattern).
- Prisma migrations are automatic; TypeORM requires manual setup.

## Interview Tip:
"Prisma is schema-first; TypeORM is code-first. Prisma has better type safety; TypeORM has more flexibility."

---

## Question 7: How does Prisma differ from Sequelize?

## Answer:
| Feature | Prisma | Sequelize |
|---------|--------|-----------|
| TypeScript | Auto-generated types | Manual type definitions |
| Approach | Schema-first | Code-first (model definitions) |
| Migrations | Automatic from schema | Manual generation |
| Query style | Method chaining | Method chaining (similar) |
| Model classes | No | Yes |
| Community | Growing, modern | Large, established |

## Key Points:
- Prisma: schema-first, auto-generated TypeScript.
- Sequelize: code-first, model-based.
- Prisma has better TypeScript support.
- Sequelize has model classes and more traditional ORM patterns.
- Both use method chaining for queries.

## Interview Tip:
"Prisma is modern and type-safe; Sequelize is established with model classes. Choose based on your team's needs."

---

## Question 8: How does Prisma differ from Mongoose?

## Answer:
| Feature | Prisma | Mongoose |
|---------|--------|----------|
| Database | SQL + MongoDB | MongoDB only |
| Schema | Declarative schema | Schema definitions |
| Type safety | Auto-generated | Manual types |
| Queries | Type-safe API | Query builder |
| Validation | Schema-based | Schema-based |

Prisma works with both SQL and MongoDB; Mongoose is MongoDB-specific.

## Key Points:
- Prisma: SQL + MongoDB support.
- Mongoose: MongoDB-specific.
- Prisma has auto-generated types.
- Both have schema-based validation.
- Prisma is database-agnostic; Mongoose is MongoDB-focused.

## Interview Tip:
"If you're using MongoDB, Mongoose is more mature. If you need SQL + MongoDB, Prisma is the choice."

---

## Question 9: What are the main components of Prisma?

## Answer:
1. **Prisma Schema**: Defines data models, relationships, and configuration.
2. **Prisma Client**: Auto-generated, type-safe database client.
3. **Prisma Migrate**: Database migration tool.
4. **Prisma Studio**: GUI for viewing and editing data.
5. **Prisma Introspection**: Generate schema from existing database.
6. **Prisma Seed**: Database seeding tool.

## Key Points:
- Schema: data model definitions.
- Client: type-safe database access.
- Migrate: automatic migrations.
- Studio: GUI for data.
- Introspection: generate schema from DB.
- Seed: seed initial data.

## Interview Tip:
"Prisma has six main components â€” schema, client, migrate, studio, introspection, and seed."

---

## Question 10: What is Prisma Client?

## Answer:
Prisma Client is an auto-generated, type-safe database client. It's generated from your Prisma schema and provides methods for CRUD operations, filtering, sorting, pagination, and relation queries.

```typescript
import { PrismaClient } from "@prisma/client";
const prisma = new PrismaClient();

// Type-safe queries
const users = await prisma.user.findMany({
  where: { isActive: true },
  include: { posts: true }
});
// TypeScript knows: users is UserWithPosts[]
```

Regenerate with `npx prisma generate` after schema changes.

## Key Points:
- Auto-generated from schema.
- Type-safe with full auto-completion.
- CRUD methods for all models.
- Supports filtering, sorting, pagination.
- Regenerate after schema changes.

## Interview Tip:
"Prisma Client is generated from your schema â€” every query is fully typed without manual type definitions."

---

## Part 2 (11â€“20): Prisma Schema

---

## Question 11: What is the Prisma Schema?

## Answer:
The Prisma Schema is a declarative data modeling language that defines your database structure. It's the single source of truth for your database.

```prisma
generator client {
  provider = "prisma-client-js"
}

datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
}

model User {
  id        Int      @id @default(autoincrement())
  email     String   @unique
  name      String?
  posts     Post[]
  createdAt DateTime @default(now())
}
```

## Key Points:
- Single source of truth for database structure.
- Defines models, fields, relations, and indexes.
- Used to generate Prisma Client.
- Used to create migrations.
- Supports multiple database providers.

## Interview Tip:
"The schema is the foundation â€” everything in Prisma starts from the schema."

---

## Question 12: What is the purpose of `schema.prisma`?

## Answer:
`schema.prisma` is the file that contains your Prisma schema definition. It's used by:
- **Prisma Client**: Generated types and methods.
- **Prisma Migrate**: Creates database migrations.
- **Prisma Introspection**: Writes schema from existing DB.
- **Prisma Studio**: Displays data based on schema.

```prisma
// schema.prisma
generator client {
  provider = "prisma-client-js"
}

datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
}

model User {
  id    Int    @id @default(autoincrement())
  name  String
}
```

## Key Points:
- Defines your database structure.
- Source of truth for client generation.
- Used by migrate, introspect, and studio.
- Lives at the project root.
- Supports comments with `//`.

## Interview Tip:
"Everything in Prisma starts from `schema.prisma` â€” it's the single source of truth."

---

## Question 13: What are datasource blocks?

## Answer:
Datasource blocks configure the database connection. They specify the database provider and connection URL.

```prisma
datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
}
```

You can have multiple datasources for different databases.

## Key Points:
- Configure database connection.
- `provider`: database type (postgresql, mysql, sqlite, mongodb).
- `url`: connection string (usually from environment variable).
- Multiple datasources supported.
- Must be present in every Prisma schema.

## Interview Tip:
"Always use environment variables for the database URL â€” never hardcode credentials."

---

## Question 14: What are generator blocks?

## Answer:
Generator blocks configure how Prisma generates code. The default is the JavaScript/TypeScript client.

```prisma
generator client {
  provider = "prisma-client-js"
}

// Custom generator example
generator client {
  provider      = "prisma-client-js"
  binaryTargets = ["native", "rhel-openssl-1.0.x"]
}
```

## Key Points:
- Configure code generation.
- Default: `prisma-client-js`.
- Can specify binary targets for deployment.
- Custom generators available (e.g., for documentation).
- Must be present in every schema.

## Interview Tip:
"The default generator works for most projects â€” only customize it for specific deployment targets."

---

## Question 15: How do you configure PostgreSQL in Prisma?

## Answer:
```prisma
datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
}

model User {
  id        Int      @id @default(autoincrement())
  email     String   @unique
  bio       String?
  metadata  Json?
  createdAt DateTime @default(now())
}
```

Connection string format:
```
postgresql://user:password@host:port/database?schema=public
```

## Key Points:
- `provider = "postgresql"`.
- Supports all PostgreSQL types.
- JSON type maps to `Json` in Prisma.
- UUID, arrays, and other PG types supported.
- Connection string with schema parameter.

## Interview Tip:
"PostgreSQL is the most commonly used database with Prisma â€” it has the best feature support."

---

## Question 16: How do you configure MySQL in Prisma?

## Answer:
```prisma
datasource db {
  provider = "mysql"
  url      = env("DATABASE_URL")
}

model User {
  id        Int      @id @default(autoincrement())
  email     String   @unique
  createdAt DateTime @default(now())
}
```

Connection string format:
```
mysql://user:password@host:port/database
```

## Key Points:
- `provider = "mysql"`.
- No JSON type (use String instead).
- No array types.
- Connection string without schema.
- MySQL-specific features available.

## Interview Tip:
"MySQL doesn't support JSON as a native type in Prisma â€” use String and parse manually."

---

## Question 17: How do you configure MongoDB in Prisma?

## Answer:
```prisma
datasource db {
  provider = "mongodb"
  url      = env("DATABASE_URL")
}

model User {
  id    String @id @default(auto()) @map("_id")
  name  String
  email String
}
```

MongoDB uses `@map("_id")` to map the `id` field to MongoDB's `_id`.

## Key Points:
- `provider = "mongodb"`.
- Requires `@map("_id")` for the ID field.
- No relations (use embedded documents or manual references).
- No SQL features (no joins, no constraints).
- Less mature than SQL database support.

## Interview Tip:
"MongoDB in Prisma has limitations â€” no relations, no SQL features. Consider Mongoose for MongoDB-heavy projects."

---

## Question 18: What are models in Prisma?

## Answer:
Models represent database tables. Each model maps to a table and defines its fields, types, and attributes.

```prisma
model User {
  id        Int      @id @default(autoincrement())
  email     String   @unique
  name      String
  role      Role     @default(USER)
  posts     Post[]
  createdAt DateTime @default(now())
}
```

## Key Points:
- Maps to a database table.
- Defines fields and their types.
- Supports relations to other models.
- Attributes define behavior (@id, @unique, etc.).
- Used to generate Prisma Client methods.

## Interview Tip:
"Models are the building blocks â€” each model becomes a table and generates CRUD methods."

---

## Question 19: What are scalar types in Prisma?

## Answer:
Scalar types map to database column types:
- **`String`**: Text (VARCHAR, TEXT).
- **`Boolean`**: True/false.
- **`Int`**: 32-bit integer.
- **`BigInt`**: 64-bit integer.
- **`Float`**: Floating-point number.
- **`Decimal`**: Precise decimal (for money).
- **`DateTime`**: Date and time.
- **`Json`**: JSON data (PostgreSQL, MySQL).
- **`Bytes`**: Binary data.

```prisma
model Product {
  id          Int      @id @default(autoincrement())
  name        String
  price       Decimal
  description String?
  metadata    Json?
  image       Bytes?
  isActive    Boolean  @default(true)
}
```

## Key Points:
- String, Boolean, Int, BigInt, Float, Decimal, DateTime, Json, Bytes.
- Map to database-specific types.
- Use Decimal for money (not Float).
- Json for flexible data (PostgreSQL, MySQL).
- Optional fields use `?`.

## Interview Tip:
"Always use Decimal for money â€” Float has rounding errors."

---

## Question 20: What are enums in Prisma?

## Answer:
Enums define a set of allowed values for a field.

```prisma
enum Role {
  USER
  ADMIN
  MODERATOR
}

enum OrderStatus {
  PENDING
  PAID
  SHIPPED
  DELIVERED
}

model User {
  id   Int  @id @default(autoincrement())
  role Role @default(USER)
}
```

Enums create actual database enum types in PostgreSQL.

## Key Points:
- Define allowed values for a field.
- Created as database enum types in PostgreSQL.
- Type-safe â€” only allowed values accepted.
- Can have defaults.
- Used with `@default()` for default values.

## Interview Tip:
"Enums give you type safety at the database level â€” only allowed values can be stored."

---

## Part 3 (21â€“30): Fields & Relations

---

## Question 21: What is the `@id` attribute?

## Answer:
The `@id` attribute marks a field as the primary key. Every model needs exactly one `@id`.

```prisma
model User {
  id Int @id @default(autoincrement())
}

model Post {
  id String @id @default(cuid())
}

model Product {
  id UUID @id @default(uuid())
}
```

## Key Points:
- Marks the primary key field.
- Every model needs exactly one.
- Can use autoincrement, cuid, or uuid.
- Required for all models.
- Defines the unique identifier.

## Interview Tip:
"Use `@default(autoincrement())` for integers, `@default(cuid())` for strings, or `@default(uuid())` for UUIDs."

---

## Question 22: What is `@default()`?

## Answer:
`@default()` provides a default value when a field is not specified during creation.

```prisma
model User {
  id        Int      @id @default(autoincrement())
  role      Role     @default(USER)
  isActive  Boolean  @default(true)
  createdAt DateTime @default(now())
}
```

Can use functions like `now()`, `uuid()`, `cuid()`.

## Key Points:
- Provides default values.
- Functions: `now()`, `uuid()`, `cuid()`, `auto()`.
- Static values: `true`, `"default"`, `0`.
- Applied on create when field is omitted.
- Doesn't affect updates.

## Interview Tip:
"`@default(now())` for timestamps, `@default(autoincrement())` for IDs â€” these are the most common defaults."

---

## Question 23: What is `@unique`?

## Answer:
`@unique` ensures all values in a field are unique across the table.

```prisma
model User {
  id    Int    @id @default(autoincrement())
  email String @unique
}
```

Creates a unique index in the database.

## Key Points:
- Ensures unique values.
- Creates a unique index.
- Only one value per field.
- Can be combined with `@default()`.
- Different from `@id` (only one `@id`, multiple `@unique`).

## Interview Tip:
"`@unique` prevents duplicate emails, usernames, or any identifier that must be unique."

---

## Question 24: What is `@updatedAt`?

## Answer:
`@updatedAt` automatically updates the field to the current timestamp whenever the record is modified.

```prisma
model User {
  id        Int      @id @default(autoincrement())
  name      String
  updatedAt DateTime @updatedAt
}
```

The field is automatically set on every update.

## Key Points:
- Auto-updates on every record modification.
- Sets to current timestamp.
- No manual setting needed.
- Useful for tracking record modifications.
- Works with `update()` and `updateMany()`.

## Interview Tip:
"`@updatedAt` is essential for tracking when records were last modified â€” use it on every table."

---

## Question 25: What is `@map`?

## Answer:
`@map` renames a field in the database without changing the Prisma model name.

```prisma
model User {
  id        Int    @id @default(autoincrement())
  firstName String @map("first_name")
  lastName  String @map("last_name")
}
```

Prisma uses `firstName`; the database stores `first_name`.

## Key Points:
- Renames field in database.
- Prisma model keeps original name.
- Database uses mapped name.
- Useful for naming convention differences.
- Prisma Client uses the Prisma name.

## Interview Tip:
"`@map` lets you use camelCase in Prisma while the database uses snake_case."

---

## Question 26: What is `@@map`?

## Answer:
`@@map` renames the table in the database without changing the Prisma model name.

```prisma
model User {
  id   Int @id @default(autoincrement())
  name String

  @@map("app_users")
}
```

Prisma uses `User`; the database table is `app_users`.

## Key Points:
- Renames table in database.
- Prisma model keeps original name.
- Database uses mapped name.
- Useful for existing databases with different naming.
- Prisma Client uses the model name.

## Interview Tip:
"`@@map` is useful for integrating with existing databases that have different table names."

---

## Question 27: What is `@@index`?

## Answer:
`@@index` creates a database index on one or more fields.

```prisma
model User {
  id    Int    @id @default(autoincrement())
  email String
  role  String

  @@index([email])
  @@index([role])
  @@index([email, role]) // Composite index
}
```

## Key Points:
- Creates database indexes.
- Supports single and composite indexes.
- Improves query performance.
- Can be added to any field.
- Important for WHERE and JOIN performance.

## Interview Tip:
"Add `@@index` on fields you frequently query â€” it dramatically improves performance."

---

## Question 28: What is `@@unique`?

## Answer:
`@@unique` creates a composite unique constraint across multiple fields.

```prisma
model OrderItem {
  id        Int @id @default(autoincrement())
  orderId   Int
  productId Int

  @@unique([orderId, productId])
}
```

Ensures one order item per product per order.

## Key Points:
- Composite unique constraint.
- Ensures unique combinations.
- Multiple fields involved.
- Creates composite unique index.
- Different from `@unique` (single field).

## Interview Tip:
"`@@unique` prevents duplicate combinations â€” like one review per user per product."

---

## Question 29: What is a one-to-one relationship?

## Answer:
A one-to-one relationship links one record in a table to exactly one record in another table.

```prisma
model User {
  id      Int     @id @default(autoincrement())
  profile Profile?
}

model Profile {
  id     Int  @id @default(autoincrement())
  bio    String
  user   User @relation(fields: [userId], references: [id])
  userId Int  @unique
}
```

The `@unique` on `userId` ensures one profile per user.

## Key Points:
- One record links to exactly one other record.
- `@unique` on foreign key ensures one-to-one.
- Optional with `?` (profile may not exist).
- Foreign key on one side.
- Bidirectional query support.

## Interview Tip:
"The `@unique` on the foreign key is what makes it one-to-one â€” without it, it's one-to-many."

---

## Question 30: What is a one-to-many relationship?

## Answer:
A one-to-many relationship links one record to multiple records in another table.

```prisma
model User {
  id    Int    @id @default(autoincrement())
  posts Post[]
}

model Post {
  id       Int  @id @default(autoincrement())
  title    String
  author   User @relation(fields: [authorId], references: [id])
  authorId Int
}
```

One user has many posts; each post has one author.

## Key Points:
- One record links to many records.
- Foreign key on the "many" side.
- `Post[]` array on the "one" side.
- Most common relationship type.
- Bidirectional query support.

## Interview Tip:
"Foreign key on the many side, array on the one side â€” that's the pattern for one-to-many."

---

## Part 4 (31â€“40): Relationships

---

## Question 31: What is a many-to-many relationship?

## Answer:
A many-to-many relationship links multiple records in one table to multiple records in another table.

```prisma
model Post {
  id    Int    @id @default(autoincrement())
  tags  Tag[]
}

model Tag {
  id    Int    @id @default(autoincrement())
  posts Post[]
}
```

Prisma creates a join table automatically (implicit many-to-many).

## Key Points:
- Multiple records link to multiple records.
- Prisma creates join table automatically.
- Both sides have array fields.
- Implicit (automatic) or explicit (manual join table).
- Most complex relationship type.

## Interview Tip:
"Prisma's implicit many-to-many is convenient â€” it creates and manages the join table for you."

---

## Question 32: How do you define relationships in Prisma?

## Answer:
```prisma
model User {
  id    Int    @id @default(autoincrement())
  posts Post[]
}

model Post {
  id       Int  @id @default(autoincrement())
  author   User @relation(fields: [authorId], references: [id])
  authorId Int
}
```

Steps:
1. Add array field on the "one" side (`Post[]`).
2. Add relation field on the "many" side (`author User`).
3. Add foreign key field (`authorId Int`).
4. Connect with `@relation`.

## Key Points:
- Array field on the "one" side.
- Relation field + foreign key on the "many" side.
- `@relation` connects them.
- `fields` = foreign key in this model.
- `references` = primary key in related model.

## Interview Tip:
"The pattern is: array on one side, foreign key + relation on the other side."

---

## Question 33: What is the `@relation` attribute?

## Answer:
The `@relation` attribute connects two models and defines the foreign key relationship.

```prisma
model Post {
  id       Int  @id @default(autoincrement())
  author   User @relation(fields: [authorId], references: [id])
  authorId Int
}
```

- `fields`: the foreign key field in this model.
- `references`: the primary key field in the related model.

## Key Points:
- Connects two models.
- `fields`: foreign key in this model.
- `references`: primary key in related model.
- Required for non-implicit relations.
- Defines how models are linked.

## Interview Tip:
"`@relation` is the bridge between models â€” it tells Prisma how they're connected."

---

## Question 34: How do implicit many-to-many relations work?

## Answer:
Prisma automatically creates and manages a join table for implicit many-to-many relations.

```prisma
model Post {
  id    Int    @id @default(autoincrement())
  tags  Tag[]
}

model Tag {
  id    Int    @id @default(autoincrement())
  posts Post[]
}
// Prisma creates: _PostToTag join table
```

You don't need to define the join table â€” Prisma handles it.

## Key Points:
- Prisma creates join table automatically.
- Named `_ModelAToModelB`.
- Managed by Prisma (not visible in schema).
- Convenient for simple many-to-many.
- Can't add extra fields to join table.

## Interview Tip:
"Implicit many-to-many is convenient but limited â€” you can't add extra fields to the join table."

---

## Question 35: How do explicit many-to-many relations work?

## Answer:
For many-to-many with extra fields, define the join table explicitly:

```prisma
model Post {
  id         Int         @id @default(autoincrement())
  postTags   PostTag[]
}

model Tag {
  id         Int         @id @default(autoincrement())
  postTags   PostTag[]
}

model PostTag {
  post       Post        @relation(fields: [postId], references: [id])
  postId     Int
  tag        Tag         @relation(fields: [tagId], references: [id])
  tagId      Int
  assignedAt DateTime    @default(now())

  @@id([postId, tagId])
}
```

## Key Points:
- Define join table explicitly.
- Can add extra fields (timestamps, metadata).
- Composite primary key on join table.
- Full control over the relationship.
- Use when join table needs additional data.

## Interview Tip:
"Explicit many-to-many is needed when the join table has extra data â€” like who assigned the tag and when."

---

## Question 36: What are relation fields?

## Answer:
Relation fields connect models but don't create database columns. They're virtual fields that enable queries.

```prisma
model User {
  id    Int    @id @default(autoincrement())
  posts Post[] // Relation field â€” no DB column
}

model Post {
  id       Int  @id @default(autoincrement())
  author   User // Relation field â€” no DB column
  authorId Int  // Scalar field â€” creates DB column
}
```

Relation fields are for queries; scalar fields create actual columns.

## Key Points:
- Virtual fields for queries.
- Don't create database columns.
- Enable `include` and nested queries.
- Scalar fields (like `authorId`) create columns.
- Relation fields are for navigation.

## Interview Tip:
"Relation fields are virtual â€” they don't create columns. Scalar fields like `authorId` create the actual column."

---

## Question 37: What are foreign keys?

## Answer:
Foreign keys are scalar fields that reference the primary key of another model. They create actual database columns.

```prisma
model Post {
  id       Int  @id @default(autoincrement())
  author   User @relation(fields: [authorId], references: [id])
  authorId Int  // This is the foreign key column
}
```

Foreign keys enforce referential integrity at the database level.

## Key Points:
- Scalar fields that reference another model's primary key.
- Create actual database columns.
- Enforce referential integrity.
- Required for explicit relations.
- Used in `@relation(fields: [...], references: [...])`.

## Interview Tip:
"Foreign keys are the actual columns in the database â€” they enforce relationships."

---

## Question 38: How does referential integrity work?

## Answer:
Referential integrity ensures that foreign keys always point to valid records. If you try to create a post with a non-existent `authorId`, the database rejects it.

Prisma enforces this through foreign key constraints in the database.

## Key Points:
- Foreign keys must reference existing records.
- Prevents orphaned records.
- Database enforces constraints.
- Prisma generates foreign key constraints.
- Prevents invalid data at database level.

## Interview Tip:
"Referential integrity prevents orphaned data â€” you can't create a post for a user that doesn't exist."

---

## Question 39: What happens when related records are deleted?

## Answer:
When a record with related data is deleted, the behavior depends on the referential action:

- **Cascade**: Delete related records too.
- **Restrict**: Prevent deletion if related records exist.
- **SetNull**: Set foreign key to NULL.
- **NoAction**: Same as Restrict (default).

```prisma
model Post {
  author   User @relation(fields: [authorId], references: [id], onDelete: Cascade)
  authorId Int
}
```

## Key Points:
- Behavior depends on referential action.
- Cascade: delete related records.
- Restrict: prevent deletion.
- SetNull: set FK to NULL.
- NoAction: same as Restrict.

## Interview Tip:
"Choose your referential actions carefully â€” Cascade can delete more data than intended."

---

## Question 40: What are referential actions (`Cascade`, `Restrict`, `SetNull`, etc.)?

## Answer:
Referential actions define what happens when a referenced record is deleted or updated:

- **Cascade**: Delete/update related records.
- **Restrict**: Prevent if references exist.
- **SetNull**: Set foreign key to NULL.
- **NoAction**: Same as Restrict (default).
- **SetDefault**: Set foreign key to default value.

```prisma
model Post {
  author   User @relation(fields: [authorId], references: [id], onDelete: Cascade, onUpdate: Restrict)
  authorId Int
}
```

## Key Points:
- Cascade: delete/update references.
- Restrict: prevent if references exist.
- SetNull: set FK to NULL.
- NoAction: same as Restrict.
- SetDefault: set FK to default.

## Interview Tip:
"Cascade is powerful but dangerous â€” make sure you really want to delete related data."

---

## Part 5 (41â€“50): Migrations

---

## Question 41: What are Prisma Migrations?

## Answer:
Prisma Migrations are SQL migration files generated from schema changes. They track and apply database structure changes.

```bash
# Create a migration
npx prisma migrate dev --name add-user-role

# Apply migrations
npx prisma migrate deploy
```

Migrations are stored in `prisma/migrations/` and version-controlled.

## Key Points:
- SQL files generated from schema changes.
- Stored in `prisma/migrations/`.
- Version-controlled with your code.
- Applied automatically or manually.
- Track database evolution over time.

## Interview Tip:
"Prisma Migrations are version-controlled SQL files â€” they track every database change."

---

## Question 42: Why are migrations important?

## Answer:
- **Version control**: Track database changes in git.
- **Reproducibility**: Apply same changes across environments.
- **Collaboration**: Team members get consistent databases.
- **Rollback**: Undo changes if needed.
- **Documentation**: Record what changed and when.

## Key Points:
- Track changes in version control.
- Reproducible across environments.
- Enable team collaboration.
- Support rollback.
- Document database evolution.

## Interview Tip:
"Migrations are the database equivalent of git commits â€” they track every change."

---

## Question 43: What is `prisma migrate dev`?

## Answer:
`prisma migrate dev` is for development. It creates a migration, applies it, and regenerates the client.

```bash
npx prisma migrate dev --name add-post-table
```

It also resets the database if needed and generates test data.

## Key Points:
- For development only.
- Creates migration from schema changes.
- Applies migration immediately.
- Regenerates Prisma Client.
- Can reset database with `--create-only`.

## Interview Tip:
"Use `migrate dev` in development â€” it creates, applies, and regenerates in one command."

---

## Question 44: What is `prisma migrate deploy`?

## Answer:
`prisma migrate deploy` applies pending migrations in production. It doesn't create new migrations or regenerate the client.

```bash
npx prisma migrate deploy
```

Run this in your CI/CD pipeline to apply migrations automatically.

## Key Points:
- For production deployments.
- Applies pending migrations only.
- Doesn't create new migrations.
- Run in CI/CD pipeline.
- Safe for production use.

## Interview Tip:
"Use `migrate deploy` in CI/CD â€” it applies migrations without modifying the schema."

---

## Question 45: What is `prisma db push`?

## Answer:
`prisma db push` pushes schema changes directly to the database without creating migration files. It's for rapid prototyping.

```bash
npx prisma db push
```

Warning: It doesn't create migration files, so changes aren't version-controlled.

## Key Points:
- Pushes schema changes directly.
- No migration files created.
- For prototyping only.
- Not for production.
- Changes aren't version-controlled.

## Interview Tip:
"`db push` is for prototyping â€” it's fast but doesn't create migration files."

---

## Question 46: What is the difference between `migrate` and `db push`?

## Answer:
| Feature | migrate dev | db push |
|---------|------------|---------|
| Migration files | Yes | No |
| Version control | Yes | No |
| Production safe | Yes (deploy) | No |
| Prototyping | Slower | Faster |
| Rollback | Yes | No |

Use `migrate` for production; `db push` for prototyping.

## Key Points:
- `migrate`: creates migration files, version-controlled.
- `db push`: direct schema push, no files.
- `migrate` is for production; `db push` is for prototyping.
- `migrate` supports rollback; `db push` doesn't.
- `migrate deploy` for CI/CD.

## Interview Tip:
"Use `migrate dev` in development and `migrate deploy` in production. Use `db push` only for prototyping."

---

## Question 47: What is Prisma Introspection?

## Answer:
Introspection generates a Prisma schema from an existing database. It reads the database structure and creates the corresponding models.

```bash
npx prisma db pull
```

Useful for:
- Adopting Prisma in an existing project.
- Syncing schema with database.
- Understanding database structure.

## Key Points:
- Generates schema from existing database.
- `prisma db pull` command.
- Useful for adopting Prisma.
- Syncs schema with database.
- Doesn't create migration files.

## Interview Tip:
"Introspection is how you adopt Prisma in an existing project â€” it generates the schema from your database."

---

## Question 48: What is `prisma db pull`?

## Answer:
`prisma db pull` is the command for introspection. It reads the existing database structure and writes it to `schema.prisma`.

```bash
npx prisma db pull
```

This generates models, relations, and indexes from the database.

## Key Points:
- Reads database structure.
- Writes to `schema.prisma`.
- Generates models and relations.
- Creates indexes from database.
- Useful for existing databases.

## Interview Tip:
"`db pull` is the introspection command â€” it generates your schema from the existing database."

---

## Question 49: What is Prisma Studio?

## Answer:
Prisma Studio is a GUI for viewing and editing data in your database.

```bash
npx prisma studio
```

It opens a web interface where you can browse tables, view records, and make edits.

## Key Points:
- GUI for database data.
- Browse tables and records.
- Edit data directly.
- Opens in web browser.
- Useful for debugging and development.

## Interview Tip:
"Prisma Studio is like phpMyAdmin but integrated with your schema â€” great for debugging."

---

## Question 50: How do you seed a database using Prisma?

## Answer:
Create a seed file and configure it in `package.json`:

```typescript
// prisma/seed.ts
import { PrismaClient } from "@prisma/client";
const prisma = new PrismaClient();

async function main() {
  await prisma.user.create({
    data: { name: "Alice", email: "alice@example.com" }
  });
}

main();
```

```json
// package.json
{
  "prisma": {
    "seed": "ts-node prisma/seed.ts"
  }
}
```

```bash
npx prisma db seed
```

## Key Points:
- Seed file in `prisma/seed.ts`.
- Configure in `package.json`.
- Run with `prisma db seed`.
- Useful for development and testing.
- Can create test data.

## Interview Tip:
"Seeding is essential for development â€” create realistic test data with `prisma db seed`."

---

## Part 6 (51â€“60): CRUD Operations

---

## Question 51: How do you create a record using Prisma Client?

## Answer:
```typescript
// Create single record
const user = await prisma.user.create({
  data: {
    name: "Alice",
    email: "alice@example.com"
  }
});

// Create with default values
const user = await prisma.user.create({
  data: {
    name: "Bob",
    email: "bob@example.com"
    // role defaults to USER, createdAt defaults to now()
  }
});
```

## Key Points:
- `create()` for single records.
- `data` object with field values.
- Defaults are applied automatically.
- Returns the created record.
- Throws error if required fields are missing.

## Interview Tip:
"`create()` is straightforward â€” provide the data object and Prisma handles the rest."

---

## Question 52: What is the difference between `create()` and `createMany()`?

## Answer:
- **`create()`**: Creates one record at a time.
- **`createMany()`**: Creates multiple records in one query.

```typescript
// create() â€” one at a time
await prisma.user.create({ data: { name: "Alice" } });

// createMany() â€” multiple at once
await prisma.user.createMany({
  data: [
    { name: "Alice" },
    { name: "Bob" },
    { name: "Charlie" }
  ]
});
```

`createMany()` is faster for bulk inserts.

## Key Points:
- `create()`: one record, returns the record.
- `createMany()`: multiple records, returns count.
- `createMany()` is faster for bulk inserts.
- `create()` supports nested writes; `createMany()` doesn't.
- `createMany()` skips duplicate records with `skipDuplicates`.

## Interview Tip:
"`createMany()` is faster for bulk inserts â€” use it when creating multiple records at once."

---

## Question 53: How do you retrieve a single record?

## Answer:
```typescript
// By unique field
const user = await prisma.user.findUnique({
  where: { email: "alice@example.com" }
});

// By ID
const user = await prisma.user.findUnique({
  where: { id: 1 }
});

// First matching record
const user = await prisma.user.findFirst({
  where: { role: "ADMIN" }
});
```

## Key Points:
- `findUnique()`: by unique field (id, email, etc.).
- `findFirst()`: first matching record.
- Returns `null` if not found.
- Type-safe â€” returns correct type.

## Interview Tip:
"`findUnique()` for exact matches (id, email); `findFirst()` for first matching record."

---

## Question 54: What is the difference between `findUnique()` and `findFirst()`?

## Answer:
- **`findUnique()`**: Requires a unique field (id, email, @unique). Returns one record or null.
- **`findFirst()`: First record matching the condition. Returns one record or null.

```typescript
// findUnique â€” requires unique field
const user = await prisma.user.findUnique({ where: { id: 1 } });

// findFirst â€” any condition
const user = await prisma.user.findFirst({ where: { role: "ADMIN" } });
```

## Key Points:
- `findUnique()`: unique field required.
- `findFirst()`: any condition, returns first match.
- Both return one record or null.
- `findFirst()` without conditions returns first record in table.
- `findUnique()` is faster (uses unique index).

## Interview Tip:
"`findUnique()` is faster because it uses a unique index â€” use it when possible."

---

## Question 55: How do you retrieve multiple records?

## Answer:
```typescript
const users = await prisma.user.findMany({
  where: { isActive: true },
  orderBy: { createdAt: "desc" },
  take: 10,
  skip: 0
});
```

`findMany()` supports filtering, sorting, pagination, and relation loading.

## Key Points:
- `findMany()` for multiple records.
- Supports `where`, `orderBy`, `take`, `skip`.
- Returns array of records.
- Supports `include` and `select`.
- Returns empty array if no matches.

## Interview Tip:
"`findMany()` is the workhorse for retrieving lists of records."

---

## Question 56: What is `findMany()`?

## Answer:
`findMany()` retrieves multiple records with filtering, sorting, pagination, and relation loading.

```typescript
const users = await prisma.user.findMany({
  where: { role: "USER" },
  include: { posts: true },
  orderBy: { name: "asc" },
  take: 20,
  skip: 0
});
```

## Key Points:
- Retrieves multiple records.
- Supports all query options.
- Returns array of records.
- Empty array if no matches.
- Most commonly used query method.

## Interview Tip:
"`findMany()` is the most versatile query â€” it supports filtering, sorting, pagination, and relations."

---

## Question 57: How do you update a record?

## Answer:
```typescript
// Update by ID
const user = await prisma.user.update({
  where: { id: 1 },
  data: { name: "Alice Smith" }
});

// Update by unique field
const user = await prisma.user.update({
  where: { email: "alice@example.com" },
  data: { role: "ADMIN" }
});
```

## Key Points:
- `update()` for single record.
- Requires `where` with unique field.
- `data` with updated values.
- Returns updated record.
- Throws error if record not found.

## Interview Tip:
"`update()` requires a unique field in `where` â€” use `updateMany()` for multiple records."

---

## Question 58: What is the difference between `update()` and `updateMany()`?

## Answer:
- **`update()`**: Updates one record (requires unique field).
- **`updateMany()`**: Updates all matching records.

```typescript
// update() â€” one record
await prisma.user.update({
  where: { id: 1 },
  data: { role: "ADMIN" }
});

// updateMany() â€” all matching
await prisma.user.updateMany({
  where: { role: "USER" },
  data: { isActive: false }
});
```

## Key Points:
- `update()`: one record, unique field required.
- `updateMany()`: all matching records.
- `update()` returns updated record.
- `updateMany()` returns count.
- `updateMany()` doesn't support nested writes.

## Interview Tip:
"`updateMany()` is for bulk updates â€” it returns the count of updated records."

---

## Question 59: How do you delete a record?

## Answer:
```typescript
// Delete by ID
const user = await prisma.user.delete({
  where: { id: 1 }
});

// Delete by unique field
const user = await prisma.user.delete({
  where: { email: "alice@example.com" }
});
```

## Key Points:
- `delete()` for single record.
- Requires unique field in `where`.
- Returns deleted record.
- Throws error if record not found.
- Cascading deletes based on referential actions.

## Interview Tip:
"`delete()` returns the deleted record â€” useful for confirmation."

---

## Question 60: What is the difference between `delete()` and `deleteMany()`?

## Answer:
- **`delete()`**: Deletes one record (requires unique field).
- **`deleteMany()`**: Deletes all matching records.

```typescript
// delete() â€” one record
await prisma.user.delete({ where: { id: 1 } });

// deleteMany() â€” all matching
await prisma.user.deleteMany({ where: { role: "USER" } });
```

## Key Points:
- `delete()`: one record, unique field required.
- `deleteMany()`: all matching records.
- `delete()` returns deleted record.
- `deleteMany()` returns count.
- Use `deleteMany()` carefully â€” it can delete many rows.

## Interview Tip:
"`deleteMany()` without a `where` clause deletes ALL records â€” be careful."

---

## Part 7 (61â€“70): Filtering & Sorting

---

## Question 61: How do you filter records using `where`?

## Answer:
```typescript
// Equality
await prisma.user.findMany({ where: { role: "ADMIN" } });

// Comparison
await prisma.user.findMany({ where: { age: { gt: 18 } } });

// Contains
await prisma.user.findMany({ where: { email: { contains: "example.com" } } });

// In list
await prisma.user.findMany({ where: { role: { in: ["ADMIN", "MODERATOR"] } } });
```

## Key Points:
- `where` clause for filtering.
- Equality: `field: value`.
- Comparison: `gt`, `gte`, `lt`, `lte`.
- String: `contains`, `startsWith`, `endsWith`.
- List: `in`, `notIn`.

## Interview Tip:
"Prisma's `where` clause is powerful â€” it supports comparison, string matching, and list operations."

---

## Question 62: How do you combine multiple filter conditions?

## Answer:
```typescript
// AND (implicit)
await prisma.user.findMany({
  where: { role: "ADMIN", isActive: true }
});

// AND (explicit)
await prisma.user.findMany({
  where: { AND: [{ role: "ADMIN" }, { isActive: true }] }
});

// OR
await prisma.user.findMany({
  where: { OR: [{ role: "ADMIN" }, { role: "MODERATOR" }] }
});
```

## Key Points:
- Implicit AND with multiple fields.
- Explicit AND with `AND: [...]`.
- OR with `OR: [...]`.
- NOT with `NOT: {...}`.
- Can combine AND, OR, NOT.

## Interview Tip:
"Implicit AND is cleaner â€” use it unless you need complex combinations."

---

## Question 63: How do you use logical operators (`AND`, `OR`, `NOT`)?

## Answer:
```typescript
// AND
await prisma.user.findMany({
  where: { AND: [{ role: "ADMIN" }, { isActive: true }] }
});

// OR
await prisma.user.findMany({
  where: { OR: [{ role: "ADMIN" }, { role: "MODERATOR" }] }
});

// NOT
await prisma.user.findMany({
  where: { NOT: { role: "ADMIN" } }
});

// Combined
await prisma.user.findMany({
  where: {
    AND: [
      { OR: [{ role: "ADMIN" }, { role: "MODERATOR" }] },
      { isActive: true }
    ]
  }
});
```

## Key Points:
- `AND`: all conditions must match.
- `OR`: any condition can match.
- `NOT`: negates the condition.
- Can nest and combine.
- Powerful for complex filtering.

## Interview Tip:
"Combine AND, OR, and NOT for complex filtering â€” Prisma supports nested logic."

---

## Question 64: How do you perform case-insensitive searches?

## Answer:
Use `mode: "insensitive"` on string fields:

```typescript
await prisma.user.findMany({
  where: {
    name: { contains: "alice", mode: "insensitive" }
  }
});

// Also works with startsWith, endsWith
await prisma.user.findMany({
  where: {
    email: { endsWith: "@example.com", mode: "insensitive" }
  }
});
```

## Key Points:
- `mode: "insensitive"` for case-insensitive matching.
- Works with `contains`, `startsWith`, `endsWith`.
- PostgreSQL and MySQL only.
- SQLite is case-insensitive by default.

## Interview Tip:
"`mode: 'insensitive'` is the easiest way to do case-insensitive searches in Prisma."

---

## Question 65: How do you search for partial matches?

## Answer:
Use `contains` for partial matches:

```typescript
// Contains "alice" anywhere
await prisma.user.findMany({
  where: { name: { contains: "alice" } }
});

// Starts with "Ali"
await prisma.user.findMany({
  where: { name: { startsWith: "Ali" } }
});

// Ends with "son"
await prisma.user.findMany({
  where: { name: { endsWith: "son" } }
});
```

## Key Points:
- `contains`: matches anywhere in the string.
- `startsWith`: matches beginning of string.
- `endsWith`: matches end of string.
- Combine with `mode: "insensitive"`.
- Requires database index for performance.

## Interview Tip:
"`contains` is Prisma's LIKE operator â€” it's great for search functionality."

---

## Question 66: How do you filter by date ranges?

## Answer:
```typescript
// After a date
await prisma.post.findMany({
  where: { createdAt: { gt: new Date("2024-01-01") } }
});

// Between dates
await prisma.post.findMany({
  where: {
    createdAt: {
      gte: new Date("2024-01-01"),
      lte: new Date("2024-12-31")
    }
  }
});

// Before a date
await prisma.post.findMany({
  where: { createdAt: { lt: new Date("2024-01-01") } }
});
```

## Key Points:
- `gt`, `gte`, `lt`, `lte` for date comparisons.
- `gte` + `lte` for date ranges.
- Use `Date` objects.
- Index date columns for performance.

## Interview Tip:
"Date ranges use `gte` and `lte` â€” same as SQL's `BETWEEN`."

---

## Question 67: How do you filter by related records?

## Answer:
```typescript
// Users who have posts
await prisma.user.findMany({
  where: { posts: { some: {} } }
});

// Users with specific post title
await prisma.user.findMany({
  where: {
    posts: { some: { title: { contains: "Prisma" } } }
  }
});

// Users with no posts
await prisma.user.findMany({
  where: { posts: { none: {} } }
});

// Users with all posts matching
await prisma.user.findMany({
  where: { posts: { every: { isPublished: true } } }
});
```

## Key Points:
- `some`: at least one related record matches.
- `none`: no related records match.
- `every`: all related records match.
- `every` with empty filter: all related records exist.
- Powerful for relation-based filtering.

## Interview Tip:
"`some`, `none`, and `every` let you filter based on related records without raw SQL."

---

## Question 68: How do you sort results using `orderBy`?

## Answer:
```typescript
// Ascending (default)
await prisma.user.findMany({ orderBy: { name: "asc" } });

// Descending
await prisma.user.findMany({ orderBy: { createdAt: "desc" } });

// Multiple fields
await prisma.user.findMany({
  orderBy: [
    { role: "asc" },
    { name: "asc" }
  ]
});
```

## Key Points:
- `orderBy: { field: "asc" }` for ascending.
- `orderBy: { field: "desc" }` for descending.
- Array for multiple sort fields.
- Default is ascending.
- Can sort by any field.

## Interview Tip:
"Use an array for multiple sort fields â€” the first field is the primary sort."

---

## Question 69: How do you sort by multiple fields?

## Answer:
```typescript
await prisma.user.findMany({
  orderBy: [
    { role: "asc" },     // Primary sort
    { name: "asc" },     // Secondary sort
    { createdAt: "desc" } // Tertiary sort
  ]
});
```

The order of fields in the array determines priority.

## Key Points:
- Array of sort objects.
- First field is primary sort.
- Second field is secondary sort.
- And so on.
- Each field can have different direction.

## Interview Tip:
"The order of fields in the array determines sort priority â€” first is primary, second is secondary."

---

## Question 70: How do you sort by related model fields?

## Answer:
```typescript
// Sort users by their most recent post
await prisma.user.findMany({
  orderBy: {
    posts: { _count: "desc" }
  }
});

// Sort by related field (with include)
const users = await prisma.user.findMany({
  include: { posts: { orderBy: { createdAt: "desc" }, take: 1 } }
});
```

Direct sorting on related fields is limited â€” use subqueries or include for complex cases.

## Key Points:
- Limited direct support for sorting on related fields.
- `_count` for sorting by count of related records.
- Use `include` with `orderBy` for nested sorting.
- Complex cases may need raw SQL.

## Interview Tip:
"Sorting by related fields is limited in Prisma â€” use `_count` or raw SQL for complex cases."

---

## Part 8 (71â€“80): Pagination

---

## Question 71: How do you implement pagination in Prisma?

## Answer:
```typescript
// Offset pagination
const users = await prisma.user.findMany({
  skip: 0,  // Offset
  take: 10  // Limit
});

// Cursor-based pagination
const users = await prisma.user.findMany({
  take: 10,
  cursor: { id: lastId },
  skip: 1  // Skip the cursor itself
});
```

## Key Points:
- `skip` and `take` for offset pagination.
- `cursor` for cursor-based pagination.
- `take` is the page size.
- `skip` is the offset.
- Cursor-based is better for large datasets.

## Interview Tip:
"Offset pagination is simpler; cursor-based is better for performance and real-time data."

---

## Question 72: What is offset pagination?

## Answer:
Offset pagination skips a number of records and returns a fixed number.

```typescript
const page = 1;
const pageSize = 10;

const users = await prisma.user.findMany({
  skip: (page - 1) * pageSize,
  take: pageSize
});
```

Simple but can have performance issues with large offsets.

## Key Points:
- Skip N records, take M records.
- Simple to implement.
- Works for small datasets.
- Performance degrades with large offsets.
- Total count needed for page indicators.

## Interview Tip:
"Offset pagination is fine for small datasets â€” use cursor-based for large ones."

---

## Question 73: What is cursor-based pagination?

## Answer:
Cursor-based pagination uses a reference point (cursor) to fetch the next page.

```typescript
const firstPage = await prisma.user.findMany({
  take: 10,
  orderBy: { id: "asc" }
});

const lastId = firstPage[firstPage.length - 1].id;

const nextPage = await prisma.user.findMany({
  take: 10,
  cursor: { id: lastId },
  skip: 1, // Skip the cursor itself
  orderBy: { id: "asc" }
});
```

## Key Points:
- Uses a cursor (usually ID or timestamp).
- Consistent performance regardless of page.
- Better for large datasets.
- No total count without extra query.
- Works well with infinite scrolling.

## Interview Tip:
"Cursor-based pagination is the standard for large datasets â€” it's consistent regardless of position."

---

## Question 74: What are the advantages of cursor pagination?

## Answer:
- **Consistent performance**: No slowdown with large offsets.
- **Real-time safe**: New records don't shift results.
- **Efficient**: Uses index for cursor lookup.
- **Infinite scroll friendly**: Natural for UI patterns.
- **No skipped records**: Items don't disappear.

## Key Points:
- Consistent performance.
- Real-time safe.
- Efficient index usage.
- Natural for infinite scroll.
- No skipped or duplicated records.

## Interview Tip:
"Cursor pagination is the standard for modern apps â€” it's consistent and efficient."

---

## Question 75: When should you use offset pagination?

## Answer:
- **Small datasets**: Few records total.
- **Page numbers**: UI shows page numbers.
- **Simple implementation**: Quick to set up.
- **Admin panels**: Browsing small datasets.

Use cursor pagination for large datasets or real-time data.

## Key Points:
- Small datasets.
- Page number UI.
- Simple implementation.
- Admin panels and dashboards.
- Not for large datasets or real-time data.

## Interview Tip:
"Offset pagination is fine for admin panels â€” use cursor for user-facing lists."

---

## Question 76: How do `skip` and `take` work?

## Answer:
- **`skip`**: Number of records to skip (offset).
- **`take`**: Maximum number of records to return (limit).

```typescript
// Page 3, 10 per page
const users = await prisma.user.findMany({
  skip: 20, // Skip first 20 records
  take: 10  // Return next 10 records
});
```

`skip: 0` starts from the beginning. `take: -10` returns last 10 records.

## Key Points:
- `skip`: offset (how many to skip).
- `take`: limit (how many to return).
- `skip: 0` = start from beginning.
- `take: -10` = last 10 records.
- Combine for pagination.

## Interview Tip:
"`skip` is offset; `take` is limit. Simple and straightforward."

---

## Question 77: How does the `cursor` option work?

## Answer:
The `cursor` option specifies the starting point for the next page. It must be a unique field.

```typescript
const users = await prisma.user.findMany({
  take: 10,
  cursor: { id: 100 }, // Start after ID 100
  skip: 1,              // Skip the cursor itself
  orderBy: { id: "asc" }
});
```

The cursor must reference a unique field (usually ID).

## Key Points:
- Specifies starting point.
- Must be a unique field.
- `skip: 1` skips the cursor itself.
- Used with `take` for page size.
- Requires `orderBy` for consistent results.

## Interview Tip:
"Cursor must be a unique field â€” use ID or a unique timestamp."

---

## Question 78: How do you implement infinite scrolling with Prisma?

## Answer:
```typescript
async function getMoreUsers(cursor?: number) {
  return prisma.user.findMany({
    take: 20,
    ...(cursor && {
      cursor: { id: cursor },
      skip: 1
    }),
    orderBy: { id: "asc" }
  });
}
```

The frontend sends the last ID as the cursor to load more.

## Key Points:
- Cursor-based pagination.
- Last ID as cursor.
- `take` for batch size.
- `skip: 1` to avoid duplicates.
- Natural for infinite scroll UI.

## Interview Tip:
"Infinite scrolling is cursor pagination â€” send the last ID as the cursor to load more."

---

## Question 79: How do you count the total number of records?

## Answer:
```typescript
// Count all users
const count = await prisma.user.count();

// Count with filter
const count = await prisma.user.count({
  where: { role: "ADMIN" }
});

// Count related records
const count = await prisma.user.count({
  where: { posts: { some: {} } }
});
```

## Key Points:
- `count()` for total records.
- Supports `where` for filtered counts.
- Supports relation filtering.
- Returns a number.
- Useful for pagination metadata.

## Interview Tip:
"`count()` is essential for pagination â€” it gives you the total for page indicators."

---

## Question 80: What pagination strategy do you use in production?

## Answer:
- **Cursor-based**: For user-facing lists (infinite scroll, API pagination).
- **Offset-based**: For admin panels with page numbers.
- **Hybrid**: Cursor for main list, offset for specific pages.

Always:
- Use `take` to limit results.
- Order by a unique field for consistency.
- Include total count for UI page indicators.

## Key Points:
- Cursor for user-facing lists.
- Offset for admin panels.
- Always limit with `take`.
- Order by unique field.
- Count for page indicators.

## Interview Tip:
"Cursor-based for user-facing; offset for admin. That's the production standard."

---

## Part 9 (81â€“90): Relations & Nested Queries

---

## Question 81: How do you query related records?

## Answer:
```typescript
// Include related records
const user = await prisma.user.findUnique({
  where: { id: 1 },
  include: { posts: true }
});

// Select specific fields
const user = await prisma.user.findUnique({
  where: { id: 1 },
  select: {
    name: true,
    posts: { select: { title: true } }
  }
});
```

## Key Points:
- `include: { relation: true }` loads related records.
- `select` for specific fields.
- `include` loads all fields of related records.
- `select` gives more control.
- Supports nested includes.

## Interview Tip:
"`include` for all fields; `select` for specific fields â€” both load related records."

---

## Question 82: What is the `include` option?

## Answer:
`include` loads related records with all their fields.

```typescript
const user = await prisma.user.findUnique({
  where: { id: 1 },
  include: {
    posts: true,
    profile: true
  }
});
// user.posts is Post[], user.profile is Profile | null
```

## Key Points:
- Loads related records.
- Returns all fields of related records.
- Supports nested includes.
- Makes queries type-safe.
- Can cause over-fetching.

## Interview Tip:
"`include` is convenient but can over-fetch â€” use `select` when you need specific fields."

---

## Question 83: What is the `select` option?

## Answer:
`select` specifies which fields to return, giving you more control than `include`.

```typescript
const user = await prisma.user.findUnique({
  where: { id: 1 },
  select: {
    name: true,
    email: true,
    posts: {
      select: { id: true, title: true }
    }
  }
});
```

## Key Points:
- Specifies exact fields to return.
- More control than `include`.
- Supports nested selects.
- Reduces over-fetching.
- More verbose but more precise.

## Interview Tip:
"`select` gives you precise control â€” only fetch what you need."

---

## Question 84: What is the difference between `include` and `select`?

## Answer:
| Feature | include | select |
|---------|---------|--------|
| Fields | All fields | Specified fields only |
| Control | Less | More |
| Verbosity | Concise | More verbose |
| Over-fetching | Possible | Prevented |
| Type safety | Yes | Yes |

Use `include` for convenience; `select` for precision.

## Key Points:
- `include`: all fields, concise.
- `select`: specific fields, precise.
- Both are type-safe.
- `select` prevents over-fetching.
- Choose based on needs.

## Interview Tip:
"`include` for convenience; `select` for performance. Know both."

---

## Question 85: How do you create related records in a single query?

## Answer:
```typescript
// Create user with posts
const user = await prisma.user.create({
  data: {
    name: "Alice",
    email: "alice@example.com",
    posts: {
      create: [
        { title: "Post 1" },
        { title: "Post 2" }
      ]
    }
  }
});
```

This creates the user and posts in one query.

## Key Points:
- Nested `create` in `data`.
- Creates parent and children atomically.
- Supports multiple children.
- Type-safe.
- Single query.

## Interview Tip:
"Nested `create` is atomic â€” user and posts are created together."

---

## Question 86: What are nested writes?

## Answer:
Nested writes create, update, or delete related records in the same query as the parent.

```typescript
// Create with nested create
await prisma.user.create({
  data: {
    name: "Alice",
    posts: { create: { title: "Post 1" } }
  }
});

// Update with nested update
await prisma.user.update({
  where: { id: 1 },
  data: {
    posts: { update: { where: { id: 1 }, data: { title: "Updated" } } }
  }
});
```

## Key Points:
- Create, update, or delete related records.
- Single query for parent and children.
- Type-safe.
- Atomic operations.
- Supports all CRUD operations.

## Interview Tip:
"Nested writes are powerful â€” create, update, or delete related records in one query."

---

## Question 87: How do you update related records?

## Answer:
```typescript
// Update a specific post
await prisma.user.update({
  where: { id: 1 },
  data: {
    posts: {
      update: {
        where: { id: 1 },
        data: { title: "Updated Title" }
      }
    }
  }
});

// Update multiple posts
await prisma.user.update({
  where: { id: 1 },
  data: {
    posts: {
      updateMany: {
        where: { isPublished: false },
        data: { isPublished: true }
      }
    }
  }
});
```

## Key Points:
- `update`: update one related record.
- `updateMany`: update multiple related records.
- Requires `where` for the related record.
- Type-safe.

## Interview Tip:
"`update` for one related record; `updateMany` for multiple â€” both are nested in the parent update."

---

## Question 88: How do you delete related records?

## Answer:
```typescript
// Delete a specific post
await prisma.user.update({
  where: { id: 1 },
  data: {
    posts: {
      delete: { id: 1 }
    }
  }
});

// Delete multiple posts
await prisma.user.update({
  where: { id: 1 },
  data: {
    posts: {
      deleteMany: { isPublished: false }
    }
  }
});
```

## Key Points:
- `delete`: delete one related record.
- `deleteMany`: delete multiple related records.
- Nested in parent update.
- Cascading deletes with referential actions.

## Interview Tip:
"Nested deletes are useful for cleaning up related data when updating the parent."

---

## Question 89: How do you connect existing related records?

## Answer:
```typescript
// Connect existing post to user
await prisma.user.update({
  where: { id: 1 },
  data: {
    posts: {
      connect: { id: 100 }
    }
  }
});

// Connect multiple posts
await prisma.user.update({
  where: { id: 1 },
  data: {
    posts: {
      connect: [{ id: 100 }, { id: 101 }]
    }
  }
});
```

## Key Points:
- `connect` links to existing records.
- Uses unique field to find the record.
- Doesn't create new records.
- Updates the foreign key.
- Supports multiple connections.

## Interview Tip:
"`connect` links existing records â€” it updates the foreign key without creating new data."

---

## Question 90: What is the difference between `connect`, `disconnect`, `set`, and `connectOrCreate`?

## Answer:
- **`connect`**: Link to existing record.
- **`disconnect`**: Unlink from related record.
- **`set`**: Replace all related records.
- **`connectOrCreate`**: Connect if exists, create if not.

```typescript
await prisma.user.update({
  where: { id: 1 },
  data: {
    posts: {
      connect: { id: 100 },           // Link existing
      disconnect: { id: 101 },        // Unlink
      connectOrCreate: {              // Connect or create
        where: { id: 102 },
        create: { title: "New Post" }
      }
    }
  }
});
```

## Key Points:
- `connect`: link existing.
- `disconnect`: unlink.
- `set`: replace all.
- `connectOrCreate`: connect or create.
- All are nested operations.

## Interview Tip:
"`connectOrCreate` is great for upsert patterns â€” connect if exists, create if not."

---

## Part 10 (91â€“100): Transactions & Advanced Queries

---

## Question 91: What are database transactions?

## Answer:
Transactions group multiple operations into a single atomic unit. All succeed or all fail.

```typescript
// Without transaction (risky)
await prisma.user.create({ data: { name: "Alice" } });
await prisma.post.create({ data: { title: "Post", authorId: 1 } });
// If second fails, first is committed â€” inconsistency!

// With transaction (safe)
await prisma.$transaction([
  prisma.user.create({ data: { name: "Alice" } }),
  prisma.post.create({ data: { title: "Post", authorId: 1 } })
]);
// Both succeed or both fail
```

## Key Points:
- Atomic operations (all or nothing).
- Prevents data inconsistency.
- Prisma supports two types: batch and interactive.
- Essential for multi-step operations.
- Rollback on failure.

## Interview Tip:
"Transactions ensure data consistency â€” use them for multi-step operations."

---

## Question 92: How do you use `$transaction()` in Prisma?

## Answer:
Two types:

```typescript
// Batch transaction
await prisma.$transaction([
  prisma.user.create({ data: { name: "Alice" } }),
  prisma.post.create({ data: { title: "Post", authorId: 1 } })
]);

// Interactive transaction
await prisma.$transaction(async (tx) => {
  const user = await tx.user.create({ data: { name: "Alice" } });
  const post = await tx.post.create({ data: { title: "Post", authorId: user.id } });
  return { user, post };
});
```

## Key Points:
- Batch: array of operations (simple).
- Interactive: callback with `tx` client (complex logic).
- Interactive supports conditional logic.
- Both ensure atomicity.
- Interactive has a time limit (default 5s).

## Interview Tip:
"Batch for simple operations; interactive for complex logic with conditions."

---

## Question 93: When should you use transactions?

## Answer:
- **Multi-step operations**: Creating a user and their profile.
- **Financial operations**: Transferring money between accounts.
- **Inventory updates**: Decreasing stock and creating an order.
- **Any operation that must be atomic**: All steps succeed or all fail.

## Key Points:
- Multi-step operations.
- Financial transactions.
- Inventory updates.
- Atomic operations.
- Data consistency critical.

## Interview Tip:
"If the operation involves multiple tables and must be atomic, use a transaction."

---

## Question 94: How do interactive transactions work?

## Answer:
Interactive transactions give you a transaction client (`tx`) for complex logic:

```typescript
await prisma.$transaction(async (tx) => {
  const user = await tx.user.findUnique({ where: { id: 1 } });
  if (!user) throw new Error("User not found");

  const post = await tx.post.create({
    data: { title: "Post", authorId: user.id }
  });

  return post;
});
```

The callback receives `tx` â€” use it instead of `prisma` for all operations.

## Key Points:
- Callback receives transaction client (`tx`).
- Use `tx` for all operations inside callback.
- Supports conditional logic.
- Automatic rollback on error.
- Time limit (default 5s).

## Interview Tip:
"Use `tx` inside the callback â€” it's your transaction-scoped client."

---

## Question 95: What are aggregations in Prisma?

## Answer:
Aggregations perform calculations across multiple records:
- **`count()`**: Count records.
- **`sum()`**: Sum numeric fields.
- **`avg()`**: Average of numeric fields.
- **`min()`**: Minimum value.
- **`max()`**: Maximum value.

```typescript
const stats = await prisma.order.aggregate({
  _sum: { amount: true },
  _avg: { amount: true },
  _count: true,
  where: { status: "PAID" }
});
```

## Key Points:
- `count()`: count records.
- `sum()`: sum numeric fields.
- `avg()`: average numeric fields.
- `min()`/`max()`: minimum/maximum values.
- Type-safe aggregations.

## Interview Tip:
"Prisma's aggregations are type-safe â€” you get `sum`, `avg`, `count`, `min`, `max` built in."

---

## Question 96: How do you use `count()`?

## Answer:
```typescript
// Count all users
const count = await prisma.user.count();

// Count with filter
const count = await prisma.user.count({
  where: { role: "ADMIN" }
});

// Count with relation filter
const count = await prisma.user.count({
  where: { posts: { some: { isPublished: true } } }
});
```

## Key Points:
- `count()` returns a number.
- Supports `where` for filtered counts.
- Supports relation filtering.
- Useful for pagination metadata.
- Efficient database-level counting.

## Interview Tip:
"`count()` is essential for pagination â€” it gives you the total for page indicators."

---

## Question 97: How do you use `aggregate()`?

## Answer:
```typescript
const stats = await prisma.order.aggregate({
  _sum: { amount: true },
  _avg: { amount: true },
  _min: { amount: true },
  _max: { amount: true },
  _count: true,
  where: { status: "PAID" }
});
// stats._sum.amount, stats._avg.amount, etc.
```

## Key Points:
- `aggregate()` for multiple calculations.
- `_sum`, `_avg`, `_min`, `_max`, `_count`.
- Specify which fields to aggregate.
- Supports `where` for filtering.
- Returns an object with results.

## Interview Tip:
"`aggregate()` is for multiple calculations at once â€” sum, average, min, max, count."

---

## Question 98: How do you use `groupBy()`?

## Answer:
```typescript
const salesByRole = await prisma.user.groupBy({
  by: ["role"],
  _count: { id: true },
  _sum: { orders: { select: { amount: true } } },
  orderBy: { role: "asc" }
});
// [{ role: "ADMIN", _count: { id: 5 }, _sum: {...} }, ...]
```

## Key Points:
- Groups results by specified fields.
- Supports aggregations per group.
- `by` specifies group-by fields.
- Supports `where`, `orderBy`, `having`.
- Useful for reports and analytics.

## Interview Tip:
"`groupBy` is like SQL's GROUP BY â€” it's great for reports and analytics."

---

## Question 99: When would you use raw SQL with Prisma?

## Answer:
- **Complex queries**: Window functions, CTEs, recursive queries.
- **Database-specific features**: PostgreSQL-specific SQL.
- **Performance**: Optimized queries Prisma can't generate.
- **Migrations**: Custom SQL in migrations.
- **Bulk operations**: Large-scale data operations.

## Key Points:
- Complex queries (window functions, CTEs).
- Database-specific features.
- Performance optimization.
- Custom migrations.
- Bulk operations.

## Interview Tip:
"Raw SQL is the escape hatch â€” use it when Prisma's API isn't sufficient."

---

## Question 100: What are `$queryRaw()` and `$executeRaw()`?

## Answer:
- **`$queryRaw()`**: Executes a read query and returns results.
- **`$executeRaw()`**: Executes a write query and returns affected count.

```typescript
// Read
const users = await prisma.$queryRaw`
  SELECT * FROM "User" WHERE "role" = ${"ADMIN"}
`;

// Write
const count = await prisma.$executeRaw`
  UPDATE "User" SET "isActive" = false WHERE "lastLogin" < ${cutoffDate}
`;
```

## Key Points:
- `$queryRaw()`: read queries.
- `$executeRaw()`: write queries.
- Template literals for safe parameterization.
- Type-safe with Prisma's types.
- Use when Prisma API isn't sufficient.

## Interview Tip:
"Use template literals with `$queryRaw` â€” they're automatically parameterized to prevent SQL injection."

---

## Part 11 (101â€“110): Performance Optimization

---

## Question 101: How do you optimize Prisma queries?

## Answer:
1. **Use `select` instead of `include`**: Fetch only needed fields.
2. **Add `take`**: Limit results.
3. **Use `findUnique` over `findFirst`**: Uses unique index.
4. **Add indexes**: On frequently queried fields.
5. **Avoid N+1**: Use `include` instead of separate queries.
6. **Use `cursor` pagination**: For large datasets.
7. **Enable query logging**: Find slow queries.

## Key Points:
- Select only needed fields.
- Limit results with `take`.
- Use unique indexes when possible.
- Index frequently queried fields.
- Avoid N+1 queries.
- Log slow queries.

## Interview Tip:
"Select only what you need, index what you query, and avoid N+1."

---

## Question 102: What is the N+1 query problem?

## Answer:
The N+1 problem occurs when you make 1 query for the main list, then N additional queries for each related record.

```typescript
// BAD: N+1 problem
const users = await prisma.user.findMany();
for (const user of users) {
  user.posts = await prisma.post.findMany({ where: { authorId: user.id } });
}
// 1 query for users + N queries for posts = N+1 queries

// GOOD: Use include
const users = await prisma.user.findMany({ include: { posts: true } });
// 1 query total (with JOIN)
```

## Key Points:
- 1 query + N queries for related data.
- Causes performance degradation.
- Use `include` to fix.
- `include` uses JOINs (1 query).
- Critical for performance.

## Interview Tip:
"The N+1 problem is the most common Prisma performance issue â€” use `include` to fix it."

---

## Question 103: How do you avoid N+1 queries in Prisma?

## Answer:
```typescript
// Use include
const users = await prisma.user.findMany({
  include: { posts: true }
});

// Use select for specific fields
const users = await prisma.user.findMany({
  select: {
    name: true,
    posts: { select: { title: true } }
  }
});

// For complex cases, use findUnique with include
const user = await prisma.user.findUnique({
  where: { id: 1 },
  include: { posts: true, profile: true }
});
```

## Key Points:
- Use `include` for related records.
- Use `select` for specific fields.
- Prisma uses JOINs under the hood.
- Single query instead of N+1.
- Type-safe.

## Interview Tip:
"`include` is the fix for N+1 â€” Prisma generates a single query with JOINs."

---

## Question 104: How do `select` and `include` affect performance?

## Answer:
- **`include`**: Loads all fields of related records (may over-fetch).
- **`select`**: Loads only specified fields (reduces data transfer).

```typescript
// Slower: includes all post fields
const users = await prisma.user.findMany({ include: { posts: true } });

// Faster: only fetches needed fields
const users = await prisma.user.findMany({
  select: { name: true, posts: { select: { title: true } } }
});
```

## Key Points:
- `include` may over-fetch.
- `select` reduces data transfer.
- Both are type-safe.
- `select` is generally faster.
- Choose based on needs.

## Interview Tip:
"`select` is generally faster because it fetches less data â€” use it when you need specific fields."

---

## Question 105: When should you use `select` instead of `include`?

## Answer:
- **Fewer fields needed**: Only need 2-3 fields from related model.
- **Large related models**: Related model has many fields.
- **Performance critical**: Every millisecond matters.
- **API responses**: Return minimal data to client.

Use `include` when you need all fields or for convenience.

## Key Points:
- Few fields needed.
- Large related models.
- Performance critical.
- API responses.
- `include` for convenience.

## Interview Tip:
"Use `select` for performance; `include` for convenience. Know the trade-off."

---

## Question 106: How do you reduce over-fetching of data?

## Answer:
1. **Use `select`**: Specify exact fields.
2. **Limit with `take`**: Don't fetch more than needed.
3. **Use cursor pagination**: Fetch only current page.
4. **Lazy load**: Fetch related data only when needed.
5. **Use views**: Pre-computed queries for complex data.

## Key Points:
- `select` for specific fields.
- `take` to limit results.
- Cursor pagination for pages.
- Lazy load for on-demand data.
- Views for complex queries.

## Interview Tip:
"Over-fetching wastes bandwidth and memory â€” use `select` and `take` to minimize it."

---

## Question 107: How do you optimize queries that return large datasets?

## Answer:
```typescript
// Pagination
const users = await prisma.user.findMany({
  take: 20,
  skip: 0
});

// Cursor-based
const users = await prisma.user.findMany({
  take: 20,
  cursor: { id: lastId },
  skip: 1
});

// Select only needed fields
const users = await prisma.user.findMany({
  select: { id: true, name: true },
  take: 20
});
```

## Key Points:
- Pagination (offset or cursor).
- Limit with `take`.
- Select only needed fields.
- Index queried fields.
- Avoid loading all records.

## Interview Tip:
"Never load all records â€” always paginate and select only needed fields."

---

## Question 108: How do you monitor slow Prisma queries?

## Answer:
Enable query logging:

```typescript
const prisma = new PrismaClient({
  log: ["query", "info", "warn", "error"]
});

// Or log slow queries
const prisma = new PrismaClient({
  log: [{ level: "query", emit: "event" }]
});

prisma.$on("query", (e) => {
  console.log("Query: " + e.query);
  console.log("Duration: " + e.duration + "ms");
});
```

## Key Points:
- Enable query logging in PrismaClient.
- Log query duration.
- Use `EXPLAIN ANALYZE` for database analysis.
- Check for N+1 queries.
- Monitor in production.

## Interview Tip:
"Query logging shows you what SQL Prisma generates â€” use it to find slow queries."

---

## Question 109: How do you enable Prisma query logging?

## Answer:
```typescript
// In development
const prisma = new PrismaClient({
  log: ["query"]
});

// With events
const prisma = new PrismaClient({
  log: [{ level: "query", emit: "event" }]
});

prisma.$on("query", (e) => {
  console.log("Query: " + e.query);
  console.log("Duration: " + e.duration + "ms");
  console.log("Params: " + e.params);
});
```

## Key Points:
- `log: ["query"]` for simple logging.
- Event-based for custom logging.
- Shows SQL query, duration, and params.
- Use in development; disable in production.

## Interview Tip:
"Query logging shows the actual SQL â€” use it to understand what Prisma generates."

---

## Question 110: What Prisma best practices improve application performance?

## Answer:
1. **Select only needed fields**: Use `select` over `include`.
2. **Limit results**: Always use `take`.
3. **Avoid N+1**: Use `include` for related data.
4. **Index frequently queried fields**: In schema.
5. **Use cursor pagination**: For large datasets.
6. **Use `findUnique`**: When possible (uses unique index).
7. **Enable connection pooling**: For production.
8. **Monitor slow queries**: Enable logging.

## Key Points:
- Select only needed fields.
- Limit results.
- Avoid N+1 queries.
- Index frequently queried fields.
- Use cursor pagination.
- Enable connection pooling.

## Interview Tip:
"Select only what you need, limit what you fetch, and index what you query."

---

## Part 12 (111â€“120): Database Design & Indexing

---

## Question 111: What is database indexing?

## Answer:
An index is a data structure that speeds up data retrieval by allowing the database to find rows without scanning the entire table.

```prisma
model User {
  id    Int    @id @default(autoincrement())
  email String @unique
  role  String

  @@index([role])
  @@index([email, role])
}
```

## Key Points:
- Speeds up data retrieval.
- Created on frequently queried fields.
- Slows down writes slightly.
- Essential for performance.
- Prisma uses `@@index` for composite indexes.

## Interview Tip:
"Indexes are the most important optimization â€” most slow queries are missing an index."

---

## Question 112: When should you create an index?

## Answer:
- **WHERE clauses**: Frequently filtered columns.
- **JOIN columns**: Foreign keys.
- **ORDER BY columns**: Sorting fields.
- **GROUP BY columns**: Aggregation fields.
- **High cardinality**: Many distinct values.

Don't index: small tables, low cardinality fields, rarely queried columns.

## Key Points:
- WHERE, JOIN, ORDER BY, GROUP BY columns.
- High cardinality fields.
- Foreign keys.
- Don't index small tables.
- Don't over-index.

## Interview Tip:
"Index columns you frequently query â€” they're the most common performance bottleneck."

---

## Question 113: How do you define indexes in Prisma?

## Answer:
```prisma
model User {
  id    Int    @id @default(autoincrement())
  email String @unique
  role  String

  // Single index
  @@index([role])

  // Composite index
  @@index([email, role])

  // Composite unique
  @@unique([email, role])
}
```

## Key Points:
- `@@index([field])` for single index.
- `@@index([field1, field2])` for composite.
- `@unique` for unique constraint.
- `@@unique([f1, f2])` for composite unique.
- Indexes are created during migration.

## Interview Tip:
"Use `@@index` for performance; `@unique` for uniqueness constraints."

---

## Question 114: What is the difference between `@unique` and `@@index`?

## Answer:
| Feature | @unique | @@index |
|---------|---------|---------|
| Purpose | Uniqueness constraint | Performance |
| Creates | Unique index | Regular index |
| Enforces | Unique values | No |
| Use case | Email, username | WHERE, JOIN columns |

`@unique` is for data integrity; `@@index` is for performance.

## Key Points:
- `@unique`: uniqueness constraint + index.
- `@@index`: performance index only.
- `@unique` prevents duplicates.
- `@@index` speeds up queries.
- Use both for different purposes.

## Interview Tip:
"`@unique` for uniqueness; `@@index` for performance. Know the difference."

---

## Question 115: What is a composite index?

## Answer:
A composite index covers multiple columns in one index.

```prisma
model User {
  id    Int    @id @default(autoincrement())
  email String
  role  String

  @@index([email, role])
}
```

The column order matters â€” the index works for queries that filter on the leading columns.

## Key Points:
- Index on multiple columns.
- Column order matters (leftmost prefix).
- More efficient than multiple single-column indexes.
- Reduces index count.
- Useful for multi-column queries.

## Interview Tip:
"Put the most selective column first in a composite index."

---

## Question 116: When should you use a composite unique constraint?

## Answer:
When you need uniqueness across multiple fields:

```prisma
model OrderItem {
  id        Int @id @default(autoincrement())
  orderId   Int
  productId Int

  @@unique([orderId, productId])
}
```

One order item per product per order.

## Key Points:
- Unique combinations across fields.
- Junction tables (many-to-many).
- Prevents duplicate relationships.
- Creates composite unique index.

## Interview Tip:
"`@@unique` prevents duplicate combinations â€” like one review per user per product."

---

## Question 117: How do foreign keys affect performance?

## Answer:
Foreign keys create implicit indexes that speed up JOINs. But they also add overhead on INSERT and UPDATE.

Best practice: index foreign keys for JOIN performance.

```prisma
model Post {
  authorId Int
  author   User @relation(fields: [authorId], references: [id])

  @@index([authorId])
}
```

## Key Points:
- Speed up JOINs.
- Add overhead on writes.
- Index foreign keys for performance.
- Implicit indexes in some databases.
- Trade-off: read performance vs write overhead.

## Interview Tip:
"Always index foreign keys â€” they're used in JOINs and speed up queries."

---

## Question 118: How do you optimize relational database schemas?

## Answer:
1. **Normalize**: 3NF for most tables.
2. **Index appropriately**: Foreign keys, WHERE columns.
3. **Choose right data types**: Smallest type that fits.
4. **Avoid over-normalization**: Too many JOINs.
5. **Use composite indexes**: For multi-column queries.
6. **Partition large tables**: By date or key range.
7. **Denormalize selectively**: For read-heavy workloads.

## Key Points:
- Normalize for integrity.
- Index for performance.
- Right data types.
- Balance normalization.
- Composite indexes.
- Partition large tables.

## Interview Tip:
"Normalize first, index second, denormalize only when needed."

---

## Question 119: How do you design efficient Prisma models?

## Answer:
1. **Use appropriate types**: `Int` vs `BigInt`, `Decimal` for money.
2. **Add `@default` values**: Timestamps, statuses.
3. **Mark required fields**: No `?` for required data.
4. **Add `@@index`**: On frequently queried fields.
5. **Use `@unique`**: For unique identifiers.
6. **Design relations carefully**: One-to-many vs many-to-many.
7. **Consider query patterns**: Design for how you'll query.

## Key Points:
- Appropriate types.
- Default values.
- Required vs optional fields.
- Indexes for performance.
- Unique constraints.
- Relation design.
- Query-driven design.

## Interview Tip:
"Design models for how you'll query them â€” think about access patterns."

---

## Question 120: What database design mistakes should you avoid?

## Answer:
1. **No primary key**: Every table needs one.
2. **No foreign keys**: Leads to orphaned data.
3. **Wrong data types**: VARCHAR(255) for everything.
4. **No indexes**: Missing indexes on queried columns.
5. **Over-normalization**: Too many JOINs.
6. **Over-indexing**: Slows down writes.
7. **No timestamps**: Missing created_at/updated_at.
8. **No constraints**: Missing NOT NULL, UNIQUE.

## Key Points:
- Every table needs a primary key.
- Foreign keys for relationships.
- Right data types.
- Indexes for performance.
- Balance normalization.
- Timestamps for auditing.
- Constraints for integrity.

## Interview Tip:
"Primary keys, foreign keys, indexes, and timestamps â€” the four pillars of good schema design."

---

## Part 13 (121â€“130): Transactions & Concurrency

---

## Question 121: What is database concurrency?

## Answer:
Concurrency is the ability to handle multiple operations simultaneously. In databases, multiple transactions can run at the same time.

PostgreSQL uses MVCC to allow concurrent reads and writes without blocking.

## Key Points:
- Multiple operations simultaneously.
- Multiple transactions at once.
- PostgreSQL uses MVCC.
- Readers don't block writers.
- Writers don't block readers.

## Interview Tip:
"Concurrency is about multiple transactions running simultaneously â€” MVCC makes it efficient."

---

## Question 122: What problems can occur with concurrent updates?

## Answer:
- **Lost updates**: Two transactions update the same row, one overwrites the other.
- **Dirty reads**: Reading uncommitted data.
- **Non-repeatable reads**: Reading the same row twice gives different results.
- **Phantoms**: New rows appear between reads.

PostgreSQL's isolation levels prevent these issues.

## Key Points:
- Lost updates.
- Dirty reads.
- Non-repeatable reads.
- Phantoms.
- Isolation levels prevent these.

## Interview Tip:
"Concurrent updates can cause data loss â€” transactions and isolation levels prevent this."

---

## Question 123: How do Prisma transactions help maintain data consistency?

## Answer:
Prisma transactions ensure that multiple operations either all succeed or all fail:

```typescript
await prisma.$transaction(async (tx) => {
  const order = await tx.order.create({ data: { userId: 1, total: 100 } });
  await tx.inventory.update({
    where: { productId: 1 },
    data: { quantity: { decrement: 1 } }
  });
  // If either fails, both are rolled back
});
```

## Key Points:
- Atomic operations.
- All succeed or all fail.
- Prevent data inconsistency.
- Automatic rollback on error.
- Essential for multi-step operations.

## Interview Tip:
"Transactions ensure data consistency â€” use them for any multi-step operation."

---

## Question 124: When should you use interactive transactions?

## Answer:
When you need conditional logic within a transaction:

```typescript
await prisma.$transaction(async (tx) => {
  const user = await tx.user.findUnique({ where: { id: 1 } });
  if (!user) throw new Error("User not found");
  if (user.balance < 100) throw new Error("Insufficient balance");

  await tx.user.update({
    where: { id: 1 },
    data: { balance: { decrement: 100 } }
  });
  await tx.order.create({ data: { userId: 1, total: 100 } });
});
```

Batch transactions don't support conditions.

## Key Points:
- Conditional logic needed.
- Multiple steps with decisions.
- Error handling within transaction.
- Complex business logic.
- Batch transactions don't support conditions.

## Interview Tip:
"Use interactive transactions when you need if/else logic inside the transaction."

---

## Question 125: How do you ensure atomic operations?

## Answer:
```typescript
// Atomic increment
await prisma.user.update({
  where: { id: 1 },
  data: { balance: { increment: 100 } }
});

// Atomic decrement
await prisma.user.update({
  where: { id: 1 },
  data: { balance: { decrement: 50 } }
});

// Transaction for multi-step atomicity
await prisma.$transaction(async (tx) => {
  await tx.account.update({ where: { id: 1 }, data: { balance: { decrement: 100 } } });
  await tx.account.update({ where: { id: 2 }, data: { balance: { increment: 100 } } });
});
```

## Key Points:
- `increment`/`decrement` for atomic math.
- Transactions for multi-step atomicity.
- Database-level atomicity.
- No race conditions.

## Interview Tip:
"Use `increment`/`decrement` for atomic operations â€” they're database-level and race-condition safe."

---

## Question 126: What is optimistic concurrency control?

## Answer:
Optimistic concurrency assumes conflicts are rare. It checks for conflicts at commit time using a version column.

```typescript
// Read with version
const user = await prisma.user.findUnique({ where: { id: 1 } });

// Update with version check
await prisma.user.update({
  where: { id: 1, version: user.version },
  data: { name: "Alice", version: { increment: 1 } }
});
// If rows affected = 0, conflict occurred â€” retry
```

## Key Points:
- Assumes conflicts are rare.
- Version column for conflict detection.
- Check at commit time.
- Retry on conflict.
- More concurrent than pessimistic locking.

## Interview Tip:
"Optimistic concurrency is better for most web apps â€” check the version and retry on conflict."

---

## Question 127: What is pessimistic locking?

## Answer:
Pessimistic locking locks rows before modifying, preventing other transactions from accessing them.

```typescript
// Prisma doesn't have native pessimistic locking
// Use raw SQL for SELECT FOR UPDATE
const user = await prisma.$queryRaw`
  SELECT * FROM "User" WHERE id = ${1} FOR UPDATE
`;
```

Pessimistic locking is less common with Prisma.

## Key Points:
- Lock rows before modifying.
- Prevents concurrent access.
- Less concurrent than optimistic.
- Prisma doesn't have native support.
- Use raw SQL for `FOR UPDATE`.

## Interview Tip:
"Prisma doesn't have native pessimistic locking â€” use raw SQL with `FOR UPDATE` when needed."

---

## Question 128: How do you prevent race conditions in Prisma?

## Answer:
1. **Transactions**: Atomic operations.
2. **Optimistic concurrency**: Version column.
3. **Atomic operations**: `increment`/`decrement`.
4. **Unique constraints**: Prevent duplicates.
5. **SELECT FOR UPDATE**: Pessimistic locking (raw SQL).

```typescript
// Atomic increment prevents race conditions
await prisma.user.update({
  where: { id: 1 },
  data: { counter: { increment: 1 } }
});
```

## Key Points:
- Transactions for atomicity.
- Optimistic concurrency with version column.
- Atomic operations (increment/decrement).
- Unique constraints.
- Pessimistic locking for critical sections.

## Interview Tip:
"Atomic operations with `increment`/`decrement` prevent race conditions at the database level."

---

## Question 129: What are idempotent operations?

## Answer:
Idempotent operations produce the same result regardless of how many times they're run.

```typescript
// Idempotent: create if not exists
await prisma.user.upsert({
  where: { email: "alice@example.com" },
  update: {},
  create: { name: "Alice", email: "alice@example.com" }
});

// Not idempotent: creates duplicate
await prisma.user.create({ data: { name: "Alice", email: "alice@example.com" } });
```

## Key Points:
- Same result on repeated execution.
- `upsert` for idempotent creates.
- Important for retry logic.
- Prevents duplicates.
- Safe for network failures.

## Interview Tip:
"`upsert` is idempotent â€” safe for retries because it won't create duplicates."

---

## Question 130: What transaction best practices do you follow?

## Answer:
1. **Keep transactions short**: Don't hold locks long.
2. **Use interactive transactions**: For complex logic.
3. **Handle errors**: Catch and retry on conflicts.
4. **Use atomic operations**: `increment`/`decrement`.
5. **Test transaction logic**: Verify rollback behavior.
6. **Set timeouts**: Prevent long-running transactions.

## Key Points:
- Short transactions.
- Interactive for complex logic.
- Error handling and retry.
- Atomic operations.
- Test rollback behavior.
- Set timeouts.

## Interview Tip:
"Keep transactions short â€” long transactions cause lock contention and performance issues."

---

## Part 14 (131â€“140): Production Best Practices

---

## Question 131: How do you manage Prisma in production?

## Answer:
1. **Connection pooling**: Use Prisma Accelerate or PgBouncer.
2. **Migrations**: Use `prisma migrate deploy` in CI/CD.
3. **Environment variables**: Secure DATABASE_URL.
4. **Logging**: Monitor slow queries.
5. **Error handling**: Graceful error responses.
6. **Monitoring**: Track query performance.

## Key Points:
- Connection pooling for performance.
- Automated migrations in CI/CD.
- Secure environment variables.
- Query logging and monitoring.
- Graceful error handling.

## Interview Tip:
"Production Prisma needs connection pooling, automated migrations, and monitoring."

---

## Question 132: How do you handle database connection pooling?

## Answer:
Options:
1. **Prisma Accelerate**: Managed connection pooling.
2. **PgBouncer**: External connection pooler.
3. **Application-level**: Pool in your app.

```typescript
// Prisma with connection URL parameters
datasource db {
  provider = "postgresql"
  url      = "${DATABASE_URL}?connection_limit=20&pool_timeout=10"
}
```

## Key Points:
- Prisma Accelerate for managed pooling.
- PgBouncer for external pooling.
- Connection limit in URL.
- Pool timeout for waiting.
- Essential for serverless/containers.

## Interview Tip:
"Connection pooling is essential for production â€” use Prisma Accelerate or PgBouncer."

---

## Question 133: What is Prisma Accelerate?

## Answer:
Prisma Accelerate is a managed connection pooling and caching service for Prisma. It sits between your application and database.

Benefits:
- Connection pooling (no need for PgBouncer).
- Global edge caching.
- Improved performance.
- Serverless-friendly.

## Key Points:
- Managed connection pooling.
- Edge caching.
- Serverless-friendly.
- No PgBouncer needed.
- Improved performance.

## Interview Tip:
"Prisma Accelerate is the easiest way to add connection pooling â€” no external tools needed."

---

## Question 134: What is Prisma Data Proxy?

## Answer:
Prisma Data Proxy was the predecessor to Prisma Accelerate. It provided connection pooling and edge caching. It's now replaced by Accelerate.

## Key Points:
- Predecessor to Accelerate.
- Connection pooling.
- Edge caching.
- Now replaced by Accelerate.
- Use Accelerate instead.

## Interview Tip:
"Data Proxy is deprecated â€” use Prisma Accelerate instead."

---

## Question 135: How do you manage environment variables securely?

## Answer:
```typescript
// .env (gitignored)
DATABASE_URL="postgresql://user:pass@localhost:5432/mydb"

// schema.prisma
datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
}
```

- Never commit `.env` to git.
- Use platform secrets (Vercel, AWS).
- Rotate credentials regularly.
- Use different credentials per environment.

## Key Points:
- `.env` file (gitignored).
- Platform secrets for production.
- Never commit credentials.
- Rotate regularly.
- Different per environment.

## Interview Tip:
"Never commit `.env` to git â€” use platform secrets for production."

---

## Question 136: How do you deploy Prisma migrations in production?

## Answer:
```bash
# In CI/CD pipeline
npx prisma migrate deploy
npx prisma generate
```

Always:
1. Test migrations in staging first.
2. Use `migrate deploy` (not `migrate dev`).
3. Generate client after migrations.
4. Run in CI/CD pipeline.

## Key Points:
- `migrate deploy` for production.
- Test in staging first.
- Generate client after migrations.
- Automate in CI/CD.
- Don't use `migrate dev` in production.

## Interview Tip:
"Use `migrate deploy` in CI/CD â€” it applies migrations without modifying the schema."

---

## Question 137: How do you seed production and development databases safely?

## Answer:
```typescript
// prisma/seed.ts
async function main() {
  // Only seed in development
  if (process.env.NODE_ENV === "development") {
    await prisma.user.create({ data: { name: "Test User" } });
  }
}
```

- Seed development with test data.
- Don't seed production with test data.
- Use fixtures for production data.
- Check environment before seeding.

## Key Points:
- Development: test data.
- Production: no test data.
- Check environment.
- Use fixtures for production.
- Idempotent seeding.

## Interview Tip:
"Seed development freely, seed production carefully â€” check environment before inserting data."

---

## Question 138: How do you handle Prisma errors gracefully?

## Answer:
```typescript
import { PrismaClientKnownRequestError } from "@prisma/client/runtime/library";

try {
  await prisma.user.create({ data: { email: "duplicate@example.com" } });
} catch (error) {
  if (error instanceof PrismaClientKnownRequestError) {
    if (error.code === "P2002") {
      // Unique constraint violation
      return { error: "Email already exists" };
    }
    if (error.code === "P2025") {
      // Record not found
      return { error: "User not found" };
    }
  }
  throw error;
}
```

## Key Points:
- Catch `PrismaClientKnownRequestError`.
- Check `error.code` for specific errors.
- P2002: unique constraint violation.
- P2025: record not found.
- Handle gracefully in API responses.

## Interview Tip:
"Prisma error codes are your friend â€” P2002 for duplicates, P2025 for not found."

---

## Question 139: How do you test Prisma-based applications?

## Answer:
1. **Test database**: Separate test database.
2. **BeforeAll/AfterAll**: Reset database per test suite.
3. **Factories**: Create test data consistently.
4. **Mock Prisma**: For unit tests.
5. **Integration tests**: Test real queries.

```typescript
beforeEach(async () => {
  await prisma.user.deleteMany();
});

it("creates a user", async () => {
  const user = await prisma.user.create({
    data: { name: "Test", email: "test@example.com" }
  });
  expect(user.name).toBe("Test");
});
```

## Key Points:
- Separate test database.
- Reset data per test.
- Factories for test data.
- Mock for unit tests.
- Integration tests for real queries.

## Interview Tip:
"Test with a real database â€” mocking Prisma hides bugs."

---

## Question 140: What logging and monitoring practices do you use with Prisma?

## Answer:
```typescript
const prisma = new PrismaClient({
  log: [
    { level: "query", emit: "event" },
    { level: "error", emit: "event" }
  ]
});

prisma.$on("query", (e) => {
  if (e.duration > 1000) {
    console.warn("Slow query:", e.query, e.duration + "ms");
  }
});
```

- Log slow queries (>1000ms).
- Monitor query count and duration.
- Use APM tools (Datadog, New Relic).
- Alert on performance degradation.

## Key Points:
- Log slow queries.
- Monitor query metrics.
- APM integration.
- Alert on degradation.
- Track query patterns.

## Interview Tip:
"Log queries slower than 1 second â€” they're usually optimization candidates."

---

## Part 15 (141â€“150): Senior Real-World Interview Questions

---

## Question 141: Describe the largest Prisma project you've worked on.

## Answer:
Pick a real project and describe:
- **Scale**: Tables, records, queries per second.
- **Architecture**: Services, databases, deployment.
- **Challenges**: What was hard and how you solved it.
- **Your role**: What you specifically contributed.
- **Results**: Performance improvements, features delivered.

## Key Points:
- Quantify the scale.
- Describe the architecture.
- Highlight challenges and solutions.
- Explain your contributions.
- Show impact.

## Interview Tip:
"Tell a story with a beginning (problem), middle (solution), and end (result)."

---

## Question 142: What was the most challenging Prisma issue you've solved?

## Answer:
Describe:
1. **Symptoms**: What was happening.
2. **Investigation**: How you diagnosed it.
3. **Root cause**: What was actually wrong.
4. **Fix**: How you resolved it.
5. **Lesson**: What you learned.

Choose an issue that shows your debugging process.

## Key Points:
- Symptoms, investigation, root cause, fix, lesson.
- Systematic debugging approach.
- Tools used.
- What you learned.
- Technically interesting issue.

## Interview Tip:
"Interviewers want to see your debugging process, not just the fix."

---

## Question 143: How do you debug slow Prisma queries?

## Answer:
1. **Enable query logging**: See actual SQL.
2. **EXPLAIN ANALYZE**: Database-level analysis.
3. **Check N+1**: Are you loading related data efficiently?
4. **Check indexes**: Are queried columns indexed?
5. **Check `include` vs `select`**: Are you over-fetching?
6. **Check `take`**: Are you limiting results?

## Key Points:
- Query logging first.
- EXPLAIN ANALYZE for database analysis.
- Check for N+1 queries.
- Verify indexes.
- Check over-fetching.
- Verify result limits.

## Interview Tip:
"Start with query logging â€” it shows what SQL Prisma generates."

---

## Question 144: How do you review Prisma schema changes during a pull request?

## Answer:
Check for:
1. **Missing indexes**: Are new queried columns indexed?
2. **Relation changes**: Are referential actions correct?
3. **Type choices**: Right data types for the data?
4. **Constraints**: NOT NULL, UNIQUE where needed?
5. **Migration compatibility**: Will it work in production?
6. **Naming conventions**: Consistent naming?

## Key Points:
- Indexes on new queried columns.
- Correct referential actions.
- Appropriate data types.
- Required constraints.
- Migration compatibility.
- Consistent naming.

## Interview Tip:
"Review schema changes like code â€” check indexes, types, constraints, and naming."

---

## Question 145: What naming conventions do you follow in Prisma schemas?

## Answer:
- **Models**: PascalCase (`User`, `OrderItem`).
- **Fields**: camelCase (`firstName`, `createdAt`).
- **Enums**: PascalCase (`OrderStatus`).
- **Enum values**: SCREAMING_SNAKE (`PENDING`, `IN_PROGRESS`).
- **Tables**: snake_case with `@@map` if needed.
- **Indexes**: `idx_tablename_fieldname`.

## Key Points:
- PascalCase for models and enums.
- camelCase for fields.
- SCREAMING_SNAKE for enum values.
- snake_case for database tables (via `@@map`).
- Consistent naming across project.

## Interview Tip:
"Consistent naming makes schemas readable â€” PascalCase models, camelCase fields."

---

## Question 146: How would you migrate a legacy SQL project to Prisma?

## Answer:
1. **Introspect existing database**: `npx prisma db pull`.
2. **Review generated schema**: Verify models and relations.
3. **Add Prisma Client**: Install and configure.
4. **Replace raw SQL**: Gradually replace with Prisma Client.
5. **Test thoroughly**: Verify all queries work.
6. **Deploy incrementally**: One feature at a time.

## Key Points:
- Introspect first.
- Review generated schema.
- Gradual replacement.
- Test thoroughly.
- Deploy incrementally.

## Interview Tip:
"Introspect first, then gradually replace â€” don't rewrite everything at once."

---

## Question 147: How would you design a multi-tenant SaaS database using Prisma?

## Answer:
```prisma
model Tenant {
  id    Int    @id @default(autoincrement())
  name  String
  users User[]
}

model User {
  id       Int    @id @default(autoincrement())
  tenantId Int
  tenant   Tenant @relation(fields: [tenantId], references: [id])
  name     String

  @@index([tenantId])
}
```

- `tenantId` on every table.
- Row-level security (database-level).
- Filter by `tenantId` in every query.
- Use Prisma middleware for automatic filtering.

## Key Points:
- `tenantId` on every table.
- Row-level security.
- Filter by tenant in queries.
- Prisma middleware for automatic filtering.
- Index `tenantId` for performance.

## Interview Tip:
"Multi-tenancy needs `tenantId` on every table and automatic filtering via middleware."

---

## Question 148: What Prisma features do you use most frequently in production?

## Answer:
- **`findMany`**: For lists with filtering, sorting, pagination.
- **`include`/`select`**: For relation loading.
- **`create`/`update`**: For CRUD operations.
- **`upsert`**: For idempotent creates.
- **`$transaction`**: For atomic operations.
- **`@@index`**: For performance.
- **`@@unique`**: For data integrity.
- **`@default`**: For auto-values.

## Key Points:
- CRUD operations.
- Relation loading with include/select.
- Upsert for idempotent operations.
- Transactions for atomicity.
- Indexes and constraints for performance.

## Interview Tip:
"findMany, include/select, upsert, and transactions â€” these are the Prisma workhorses."

---

## Question 149: If you were starting a new production project today, how would you structure Prisma, migrations, and database access?

## Answer:
```
prisma/
  schema.prisma     # Schema definition
  migrations/       # Migration files
  seed.ts           # Seed script
src/
  db/
    client.ts       # PrismaClient instance
    middleware.ts    # Query middleware
  services/         # Business logic using Prisma
  routes/           # API routes
```

- Schema at project root.
- Migrations version-controlled.
- Single PrismaClient instance.
- Middleware for tenant filtering.
- Services for business logic.

## Key Points:
- Schema at project root.
- Migrations in version control.
- Single PrismaClient instance.
- Middleware for cross-cutting concerns.
- Services for business logic.

## Interview Tip:
"Single PrismaClient instance, middleware for cross-cutting concerns, services for business logic."

---

## Question 150: In your opinion, what separates a junior, mid-level, and senior Prisma developer?

## Answer:
- **Junior**: Knows basic CRUD operations. Can create models and run queries.
- **Mid-level**: Understands relations, transactions, and performance. Can design schemas and optimize queries.
- **Senior**: Designs scalable schemas, handles production issues, mentors others. Understands trade-offs, migrations, and architecture.

The biggest differentiator: a senior developer understands WHY, not just WHAT.

## Key Points:
- Junior: basic CRUD, guided work.
- Mid-level: relations, transactions, schema design.
- Senior: architecture, production, mentoring.
- Senior understands trade-offs.
- Senior thinks about scalability and performance.

## Interview Tip:
"The best answer shows self-awareness. Pick your level and explain what you're doing to grow."

---

# End of Prisma ORM Interview Questions & Answers
