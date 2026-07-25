# Mongoose Interview Questions (150 Total)

---

# Introduction

1. What is Mongoose?
2. Why was Mongoose created?
3. What problems does Mongoose solve?
4. What are the advantages of Mongoose?
5. What are the disadvantages of Mongoose?
6. How does Mongoose differ from the native MongoDB driver?
7. How does Mongoose differ from Prisma?
8. When should you use Mongoose?
9. What are the core features of Mongoose?
10. How does Mongoose fit into the MERN stack?

---

# Connection

11. How do you connect Mongoose to MongoDB?
12. What is `mongoose.connect()`?
13. How do you handle connection errors?
14. How do you close a database connection?
15. How do you manage multiple MongoDB connections?
16. What connection options are commonly used?
17. How do you configure environment variables for MongoDB?
18. What is connection pooling in Mongoose?
19. How do you monitor connection status?
20. What are common connection issues?

---

# Schema

21. What is a Mongoose Schema?
22. What is the purpose of a schema?
23. How do you define a schema?
24. What schema types does Mongoose support?
25. What is the `Schema.Types.ObjectId` type?
26. What are nested schemas?
27. What are subdocuments?
28. How do arrays work in Mongoose schemas?
29. What are schema options?
30. What is the `timestamps` option?

---

# Models

31. What is a Mongoose Model?
32. How do you create a model?
33. What is the relationship between a schema and a model?
34. What is a Mongoose document?
35. How do you create a document?
36. How do you save a document?
37. What is the difference between `new Model()` and `Model.create()`?
38. How do you delete a document?
39. How do you update a document?
40. What are static methods in Mongoose?

---

# Instance Methods & Virtuals

41. What are instance methods?
42. How do instance methods differ from static methods?
43. What are virtual properties?
44. Why would you use virtuals?
45. What is the difference between stored fields and virtual fields?
46. How do you hide sensitive fields using schema options?
47. What is the `toJSON` transform?
48. What is the `toObject` transform?
49. What are schema plugins?
50. What Mongoose schema best practices do you follow?

---

# CRUD Operations

51. How do you create a document using Mongoose?
52. What is the difference between `save()` and `create()`?
53. How do you retrieve documents?
54. What is the difference between `find()` and `findOne()`?
55. What is `findById()`?
56. How do you update documents?
57. What is the difference between `updateOne()` and `findOneAndUpdate()`?
58. How do you delete documents?
59. What is the difference between `deleteOne()` and `findOneAndDelete()`?
60. What CRUD best practices do you follow in Mongoose?

---

# Validation

61. What is schema validation?
62. What built-in validators does Mongoose provide?
63. What is the `required` validator?
64. What is the `unique` option?
65. What is the difference between `required` and `unique`?
66. How do you validate string length?
67. How do you validate numbers?
68. How do you create custom validators?
69. How do async validators work?
70. How do you handle validation errors?

---

# Middleware (Hooks)

71. What is middleware in Mongoose?
72. What is the difference between document middleware and query middleware?
73. What is `pre()` middleware?
74. What is `post()` middleware?
75. What are common use cases for middleware?
76. How do you hash passwords using middleware?
77. What is the difference between `save()` middleware and `update()` middleware?
78. How do middleware execution order and chaining work?
79. What are common mistakes when using middleware?
80. What middleware best practices do you follow?

---

# Populate & Relationships

81. What is `populate()`?
82. How does `populate()` work?
83. What is the difference between embedding and referencing?
84. When should you use `populate()`?
85. What are the performance drawbacks of `populate()`?
86. How do you populate multiple references?
87. How do you populate nested references?
88. What is virtual populate?
89. How do you limit fields returned by `populate()`?
90. What relationship modeling best practices do you follow?

---

# Queries & Performance

91. What are query helpers?
92. What is `lean()`?
93. Why is `lean()` faster than regular queries?
94. When should you use `lean()`?
95. How do you paginate query results?
96. How do you sort query results?
97. How do you create indexes in Mongoose?
98. How do you debug slow queries?
99. How do you handle duplicate key errors?
100. What Mongoose query optimization best practices do you follow?

---

# Transactions & Sessions

101. What are transactions in Mongoose?
102. How do MongoDB transactions work with Mongoose?
103. What is a session in Mongoose?
104. How do you start a session?
105. How do you commit a transaction?
106. How do you abort (rollback) a transaction?
107. When should you use transactions?
108. What are the limitations of MongoDB transactions?
109. How do transactions affect performance?
110. What transaction best practices do you follow?

---

# Performance Optimization

111. How do you optimize Mongoose queries?
112. What is the N+1 query problem in Mongoose?
113. How does `populate()` affect performance?
114. When should you avoid using `populate()`?
115. How do you reduce over-fetching of data?
116. What is query projection?
117. How do indexes improve Mongoose performance?
118. How do you optimize write-heavy applications?
119. How do you optimize read-heavy applications?
120. What Mongoose performance best practices do you follow?

---

# Advanced Features

121. What are discriminators in Mongoose?
122. When should you use discriminators?
123. What are schema plugins?
124. How do you create a custom Mongoose plugin?
125. What are query helpers?
126. What are aggregation pipelines in Mongoose?
127. How do you use the aggregation framework through Mongoose?
128. What is optimistic concurrency control?
129. How do you implement soft deletes?
130. How do you implement multi-tenancy in Mongoose?

---

# Testing & Production

131. How do you test Mongoose models?
132. How do you mock Mongoose in unit tests?
133. How do you test transactions?
134. How do you seed test databases?
135. How do you manage environment-specific MongoDB connections?
136. How do you deploy a Mongoose application?
137. How do you monitor Mongoose performance in production?
138. How do you handle database migrations in MongoDB/Mongoose projects?
139. How do you debug production database issues?
140. What production best practices do you always follow?

---

# Senior Real-World Interview Questions

141. Describe the largest Mongoose project you've worked on.
142. What was the most difficult Mongoose issue you've solved?
143. How do you debug slow Mongoose queries?
144. How do you review Mongoose schema changes in a pull request?
145. What schema design conventions do you follow?
146. How would you migrate a native MongoDB project to Mongoose?
147. How would you design a scalable Mongoose architecture for a SaaS application?
148. What Mongoose features do you use most frequently in production?
149. If you were starting a new MERN project today, how would you organize your Mongoose models and database layer?
150. In your opinion, what separates a junior, mid-level, and senior Mongoose developer?

---

# ANSWERS


---

## Part 1 (1â€“10): Introduction

---

## Question 1: What is Mongoose?

## Answer:
Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node.js. It provides a schema-based solution to model your application data, including built-in validation, type casting, business logic hooks, and query building.

```javascript
const mongoose = require("mongoose");

const userSchema = new mongoose.Schema({
  name: { type: String, required: true },
  email: { type: String, required: true, unique: true }
});

const User = mongoose.model("User", userSchema);
```

## Key Points:
- ODM (Object Data Modeling) library for MongoDB.
- Schema-based data modeling.
- Built-in validation and type casting.
- Query building with chaining.
- Middleware (hooks) for business logic.

## Interview Tip:
"Mongoose is the Prisma of MongoDB â€” it adds structure, validation, and type safety to MongoDB documents."

---

## Question 2: Why was Mongoose created?

## Answer:
Mongoose was created to bring structure to MongoDB's schemaless nature. MongoDB stores flexible JSON documents without a fixed schema, which is powerful but risky â€” you can accidentally store wrong data types or miss required fields.

Mongoose adds:
- Schema enforcement.
- Validation.
- Type casting.
- Query building.
- Middleware hooks.

## Key Points:
- Brings structure to schemaless MongoDB.
- Prevents invalid data with validation.
- Type casting for safety.
- Query building for convenience.
- Middleware for business logic.

## Interview Tip:
"MongoDB is flexible but risky â€” Mongoose adds guardrails with schemas and validation."

---

## Question 3: What problems does Mongoose solve?

## Answer:
1. **No schema enforcement**: MongoDB allows any document structure.
2. **No validation**: No built-in way to validate data.
3. **No type safety**: No guarantee of correct data types.
4. **Complex queries**: Raw MongoDB queries are verbose.
5. **No business logic hooks**: No pre/post save logic.
6. **No relationships**: No built-in way to reference other documents.

## Key Points:
- Schema enforcement for consistency.
- Validation for data integrity.
- Type casting for safety.
- Simplified query building.
- Middleware for business logic.
- Relationship modeling with populate.

## Interview Tip:
"Mongoose solves MongoDB's biggest weakness â€” no schema enforcement and no validation."

---

## Question 4: What are the advantages of Mongoose?

## Answer:
- **Schema enforcement**: Ensures consistent document structure.
- **Validation**: Built-in and custom validators.
- **Type casting**: Automatically converts types.
- **Query building**: Chainable, readable queries.
- **Middleware**: Pre/post hooks for business logic.
- **Population**: Reference and populate related documents.
- **Virtuals**: Computed fields without storage.
- **Plugins**: Extend functionality.

## Key Points:
- Schema enforcement.
- Validation and type casting.
- Simplified queries.
- Middleware hooks.
- Population for relationships.
- Virtuals for computed fields.
- Extensible with plugins.

## Interview Tip:
"Mongoose gives MongoDB the structure of a relational database with the flexibility of a document store."

---

## Question 5: What are the disadvantages of Mongoose?

## Answer:
- **Performance overhead**: Extra abstraction layer.
- **Schema rigidity**: Less flexible than raw MongoDB.
- **Learning curve**: Schema syntax and ODM concepts.
- **Memory usage**: Document instances use more memory.
- **No SQL features**: No JOINs, transactions are limited.
- **Overhead for simple apps**: Too much for basic CRUD.

## Key Points:
- Performance overhead from abstraction.
- Less flexible than raw MongoDB.
- Learning curve for schema syntax.
- Higher memory usage.
- Limited transaction support.
- Overkill for simple applications.

## Interview Tip:
"Honesty about disadvantages shows maturity â€” 'Mongoose adds overhead, but the structure and validation are worth it.'"

---

## Question 6: How does Mongoose differ from the native MongoDB driver?

## Answer:
| Feature | Mongoose | Native Driver |
|---------|----------|---------------|
| Schema | Yes | No |
| Validation | Built-in | Manual |
| Type casting | Automatic | Manual |
| Query building | Chainable API | Raw queries |
| Middleware | Pre/post hooks | None |
| Population | Built-in | Manual lookups |
| Virtuals | Built-in | None |

Mongoose adds structure; the native driver is raw and flexible.

## Key Points:
- Mongoose: schema, validation, type casting, middleware.
- Native driver: raw, flexible, no overhead.
- Mongoose for structured apps; native for performance.
- Mongoose queries are chainable; native queries are raw objects.
- Mongoose has population; native requires manual lookups.

## Interview Tip:
"Mongoose is for structure; the native driver is for performance. Know when to use each."

---

## Question 7: How does Mongoose differ from Prisma?

## Answer:
| Feature | Mongoose | Prisma |
|---------|----------|--------|
| Database | MongoDB only | SQL + MongoDB |
| Approach | ODM (code-first) | Schema-first |
| Type safety | Manual types | Auto-generated |
| Validation | Schema-based | Schema-based |
| Relations | Population | Native relations |
| Migrations | No built-in | Built-in |

Mongoose is MongoDB-specific; Prisma is database-agnostic.

## Key Points:
- Mongoose: MongoDB-only, code-first.
- Prisma: SQL + MongoDB, schema-first.
- Prisma has auto-generated types; Mongoose has manual types.
- Mongoose uses population; Prisma uses native relations.
- Prisma has built-in migrations; Mongoose doesn't.

## Interview Tip:
"Mongoose for MongoDB-only projects; Prisma for SQL + MongoDB or if you want auto-generated types."

---

## Question 8: When should you use Mongoose?

## Answer:
- **MongoDB projects**: When using MongoDB as your database.
- **Schema enforcement**: When you need consistent document structure.
- **Validation**: When you need to validate data at the application level.
- **Business logic hooks**: When you need pre/post save logic.
- **Rapid development**: When you want quick schema setup.

Don't use for: SQL databases, performance-critical apps, or simple CRUD.

## Key Points:
- MongoDB projects.
- Schema enforcement needed.
- Validation required.
- Business logic hooks.
- Rapid development.

## Interview Tip:
"Mongoose is the default choice for MongoDB projects â€” it adds structure without losing flexibility."

---

## Question 9: What are the core features of Mongoose?

## Answer:
1. **Schemas**: Define document structure.
2. **Models**: Compile schemas into usable models.
3. **Validation**: Built-in and custom validators.
4. **Type casting**: Automatic type conversion.
5. **Query building**: Chainable, readable queries.
6. **Middleware**: Pre/post hooks.
7. **Population**: Reference and populate related documents.
8. **Virtuals**: Computed fields.
9. **Plugins**: Extend functionality.

## Key Points:
- Schemas and models.
- Validation and type casting.
- Query building.
- Middleware hooks.
- Population and virtuals.
- Extensible with plugins.

## Interview Tip:
"Mongoose has nine core features â€” schemas, models, validation, type casting, queries, middleware, population, virtuals, and plugins."

---

## Question 10: How does Mongoose fit into the MERN stack?

## Answer:
MERN = MongoDB, Express, React, Node.js. Mongoose is the ODM layer between Node.js/Express and MongoDB.

```
React (Frontend)
    â†“ API calls
Express (Backend)
    â†“ Mongoose queries
Mongoose (ODM)
    â†“ MongoDB driver
MongoDB (Database)
```

## Key Points:
- Mongoose is the data layer in MERN.
- Sits between Express and MongoDB.
- Handles all database operations.
- Provides schema and validation.
- Simplifies MongoDB interactions.

## Interview Tip:
"Mongoose is the data layer in MERN â€” it connects Express to MongoDB with structure and validation."

---

## Part 2 (11â€“20): Connection

---

## Question 11: How do you connect Mongoose to MongoDB?

## Answer:
```javascript
const mongoose = require("mongoose");

async function connectDB() {
  try {
    await mongoose.connect("mongodb://localhost:27017/myapp");
    console.log("Connected to MongoDB");
  } catch (error) {
    console.error("Connection error:", error);
    process.exit(1);
  }
}

connectDB();
```

## Key Points:
- `mongoose.connect()` with connection string.
- Returns a promise.
- Handle connection errors.
- Connect once at application startup.
- Close connection on shutdown.

## Interview Tip:
"Connect at application startup and handle errors â€” a failed connection should crash the app."

---

## Question 12: What is `mongoose.connect()`?

## Answer:
`mongoose.connect()` establishes a connection to MongoDB. It returns a promise that resolves when connected.

```javascript
await mongoose.connect(uri, options);
```

Common options:
```javascript
await mongoose.connect("mongodb://localhost:27017/myapp", {
  useNewUrlParser: true,
  useUnifiedTopology: true
});
```

## Key Points:
- Establishes MongoDB connection.
- Returns a promise.
- Accepts connection URI and options.
- Connection is cached (singleton).
- Use `useNewUrlParser` and `useUnifiedTopology`.

## Interview Tip:
"Mongoose caches the connection â€” calling `connect()` multiple times reuses the same connection."

---

## Question 13: How do you handle connection errors?

## Answer:
```javascript
mongoose.connection.on("error", (err) => {
  console.error("MongoDB connection error:", err);
});

mongoose.connection.on("disconnected", () => {
  console.log("MongoDB disconnected");
});

// Handle process termination
process.on("SIGINT", async () => {
  await mongoose.connection.close();
  process.exit(0);
});
```

## Key Points:
- Listen for `error` event.
- Listen for `disconnected` event.
- Handle process termination (SIGINT).
- Attempt reconnection on disconnect.
- Log errors for debugging.

## Interview Tip:
"Always listen for connection events â€” errors and disconnects happen in production."

---

## Question 14: How do you close a database connection?

## Answer:
```javascript
// Close connection
await mongoose.connection.close();

// Or
mongoose.disconnect();
```

Close on process termination:
```javascript
process.on("SIGINT", async () => {
  await mongoose.connection.close();
  process.exit(0);
});
```

## Key Points:
- `mongoose.connection.close()` closes the connection.
- `mongoose.disconnect()` is an alias.
- Always close on process shutdown.
- Prevents hanging connections.
- Important for graceful shutdown.

## Interview Tip:
"Always close the connection on shutdown â€” hanging connections cause issues in production."

---

## Question 15: How do you manage multiple MongoDB connections?

## Answer:
```javascript
const primaryDB = mongoose.createConnection("mongodb://localhost:27017/primary");
const secondaryDB = mongoose.createConnection("mongodb://localhost:27017/secondary");

// Create models on specific connections
const User = primaryDB.model("User", userSchema);
const Log = secondaryDB.model("Log", logSchema);
```

Use `createConnection()` for multiple connections.

## Key Points:
- `createConnection()` for multiple connections.
- Each connection is independent.
- Models belong to specific connections.
- Useful for multi-database setups.
- Default `mongoose.connect()` for single connection.

## Interview Tip:
"`createConnection()` for multiple databases; `mongoose.connect()` for single database."

---

## Question 16: What connection options are commonly used?

## Key Points:
- `useNewUrlParser`: Use new URL string parser.
- `useUnifiedTopology`: Use unified topology.
- `maxPoolSize`: Maximum connection pool size.
- `serverSelectionTimeoutMS`: Timeout for server selection.
- `socketTimeoutMS`: Timeout for socket operations.

```javascript
await mongoose.connect(uri, {
  maxPoolSize: 10,
  serverSelectionTimeoutMS: 5000,
  socketTimeoutMS: 45000
});
```

## Interview Tip:
"Configure pool size and timeouts â€” they affect performance and reliability."

---

## Question 17: How do you configure environment variables for MongoDB?

## Answer:
```javascript
// .env
MONGODB_URI=mongodb://localhost:27017/myapp

// config.js
require("dotenv").config();
module.exports = {
  mongodb: process.env.MONGODB_URI
};

// connection.js
const mongoose = require("mongoose");
mongoose.connect(process.env.MONGODB_URI);
```

## Key Points:
- Use `.env` file (gitignored).
- `dotenv` package to load variables.
- Never hardcode connection strings.
- Different URIs per environment.
- Use platform secrets in production.

## Interview Tip:
"Never hardcode connection strings â€” use environment variables."

---

## Question 18: What is connection pooling in Mongoose?

## Answer:
Connection pooling maintains a pool of reusable database connections instead of creating a new connection per request.

```javascript
await mongoose.connect(uri, {
  maxPoolSize: 10  // Maximum 10 connections in pool
});
```

Mongoose/MongoDB driver handles pooling automatically.

## Key Points:
- Reuses connections instead of creating new ones.
- Configurable pool size.
- Reduces connection overhead.
- Handles concurrent requests efficiently.
- Managed by MongoDB driver automatically.

## Interview Tip:
"Connection pooling is automatic in Mongoose â€” configure `maxPoolSize` for your workload."

---

## Question 19: How do you monitor connection status?

## Answer:
```javascript
mongoose.connection.on("connected", () => console.log("Connected"));
mongoose.connection.on("disconnected", () => console.log("Disconnected"));
mongoose.connection.on("error", (err) => console.error("Error:", err));

// Check current state
console.log(mongoose.connection.readyState);
// 0: disconnected, 1: connected, 2: connecting, 3: disconnecting
```

## Key Points:
- Listen for connection events.
- `readyState` for current status.
- 0: disconnected, 1: connected, 2: connecting, 3: disconnecting.
- Log state changes for debugging.
- Monitor in production.

## Interview Tip:
"`readyState` gives you the current connection status â€” 0 to 3."

---

## Question 20: What are common connection issues?

## Answer:
1. **Authentication failed**: Wrong credentials.
2. **Connection timeout**: Server unreachable.
3. **Network issues**: Firewall or DNS problems.
4. **Max pool size**: Too many connections.
5. **MongoDB not running**: Server not started.
6. **Wrong URI format**: Invalid connection string.

## Key Points:
- Authentication failures.
- Connection timeouts.
- Network issues.
- Pool size exhaustion.
- Server not running.
- Invalid URI format.

## Interview Tip:
"Most connection issues are authentication, network, or server availability â€” check those first."

---

## Part 3 (21â€“30): Schema

---

## Question 21: What is a Mongoose Schema?

## Answer:
A schema defines the structure of documents, including field names, types, validation, defaults, and other constraints.

```javascript
const userSchema = new mongoose.Schema({
  name: { type: String, required: true },
  email: { type: String, required: true, unique: true },
  age: { type: Number, min: 0, max: 150 },
  createdAt: { type: Date, default: Date.now }
});
```

## Key Points:
- Defines document structure.
- Specifies field types and validation.
- Supports defaults and enums.
- Used to create models.
- Does NOT create the database schema (MongoDB is schemaless).

## Interview Tip:
"Mongoose schemas are application-level â€” MongoDB itself remains schemaless."

---

## Question 22: What is the purpose of a schema?

## Answer:
- **Structure**: Define what fields exist and their types.
- **Validation**: Ensure data integrity.
- **Defaults**: Provide default values.
- **Type casting**: Automatically convert types.
- **Business logic**: Add methods, virtuals, and hooks.
- **Query helpers**: Define custom query methods.

## Key Points:
- Define document structure.
- Enforce data integrity.
- Provide defaults.
- Type casting.
- Add business logic.
- Custom query helpers.

## Interview Tip:
"The schema is the blueprint â€” it defines everything about your documents."

---

## Question 23: How do you define a schema?

## Answer:
```javascript
const mongoose = require("mongoose");

const userSchema = new mongoose.Schema({
  name: {
    type: String,
    required: true,
    trim: true,
    minlength: 2,
    maxlength: 100
  },
  email: {
    type: String,
    required: true,
    unique: true,
    lowercase: true
  },
  age: {
    type: Number,
    min: 0,
    max: 150
  },
  role: {
    type: String,
    enum: ["user", "admin", "moderator"],
    default: "user"
  }
}, {
  timestamps: true
});
```

## Key Points:
- `new mongoose.Schema()` to create.
- Field definitions with types and options.
- Validation rules inline.
- Schema options as second argument.
- `timestamps: true` for automatic timestamps.

## Interview Tip:
"Define schemas with types, validation, and defaults â€” the schema is your data contract."

---

## Question 24: What schema types does Mongoose support?

## Answer:
- **String**: Text data.
- **Number**: Integer or floating point.
- **Boolean**: True/false.
- **Date**: Date and time.
- **Buffer**: Binary data.
- **Mixed**: Any type (flexible).
- **ObjectId**: Reference to another document.
- **Array**: List of values or subdocuments.

## Key Points:
- String, Number, Boolean, Date, Buffer.
- Mixed for flexible data.
- ObjectId for references.
- Array for lists.
- Subdocuments for nested objects.

## Interview Tip:
"Know the basic types: String, Number, Boolean, Date, ObjectId, Array."

---

## Question 25: What is the `Schema.Types.ObjectId` type?

## Answer:
`ObjectId` is a special type that references another document's `_id`. It's used for relationships.

```javascript
const postSchema = new mongoose.Schema({
  title: String,
  author: { type: mongoose.Schema.Types.ObjectId, ref: "User" }
});
```

`ref: "User"` tells Mongoose which model to populate.

## Key Points:
- References another document's `_id`.
- Used for relationships.
- `ref` specifies the referenced model.
- Used with `populate()` to fetch related data.
- 12-byte BSON type.

## Interview Tip:
"`ObjectId` with `ref` is how Mongoose models relationships â€” it's the foundation of population."

---

## Question 26: What are nested schemas?

## Answer:
Nested schemas define structure for embedded subdocuments.

```javascript
const addressSchema = new mongoose.Schema({
  street: String,
  city: String,
  zip: String
});

const userSchema = new mongoose.Schema({
  name: String,
  address: addressSchema  // Nested schema
});
```

## Key Points:
- Define structure for embedded documents.
- Reusable across models.
- Validated like top-level fields.
- Stored as embedded documents.
- Good for "has-a" relationships.

## Interview Tip:
"Nested schemas are for embedded documents â€” they define structure for subdocuments."

---

## Question 27: What are subdocuments?

## Answer:
Subdocuments are documents embedded within other documents. They're part of the parent document and share its lifecycle.

```javascript
const commentSchema = new mongoose.Schema({
  text: String,
  author: String,
  createdAt: { type: Date, default: Date.now }
});

const postSchema = new mongoose.Schema({
  title: String,
  comments: [commentSchema]  // Array of subdocuments
});
```

## Key Points:
- Documents embedded in parent documents.
- Share lifecycle with parent.
- Validated with parent.
- Saved with parent.
- Good for tightly coupled data.

## Interview Tip:
"Subdocuments are embedded â€” they're saved, validated, and deleted with the parent."

---

## Question 28: How do arrays work in Mongoose schemas?

## Answer:
```javascript
// Simple array
const userSchema = new mongoose.Schema({
  tags: [String]  // Array of strings
});

// Array of subdocuments
const postSchema = new mongoose.Schema({
  comments: [{
    text: String,
    author: String
  }]
});

// Array of ObjectIds
const postSchema = new mongoose.Schema({
  tags: [{ type: mongoose.Schema.Types.ObjectId, ref: "Tag" }]
});
```

## Key Points:
- `[Type]` for simple arrays.
- `[subdocSchema]` for arrays of subdocuments.
- `[ObjectId]` for arrays of references.
- Arrays are mutable (push, pull, splice).
- Validated per element.

## Interview Tip:
"Arrays in schemas are flexible â€” strings, subdocuments, or references."

---

## Question 29: What are schema options?

## Answer:
Schema options configure behavior at the schema level:

```javascript
const userSchema = new mongoose.Schema({
  name: String
}, {
  timestamps: true,      // Adds createdAt and updatedAt
  toJSON: { virtuals: true },  // Include virtuals in JSON
  toObject: { virtuals: true }, // Include virtuals in objects
  collection: "users"    // Custom collection name
});
```

## Key Points:
- `timestamps`: auto `createdAt`/`updatedAt`.
- `toJSON`/`toObject`: control serialization.
- `collection`: custom collection name.
- `versionKey`: disable `__v` field.
- `strict`: control schema strictness.

## Interview Tip:
"`timestamps: true` is the most common schema option â€” it auto-manages creation and update times."

---

## Question 30: What is the `timestamps` option?

## Answer:
`timestamps: true` automatically adds `createdAt` and `updatedAt` fields to every document.

```javascript
const userSchema = new mongoose.Schema({
  name: String
}, { timestamps: true });

// Documents automatically get:
// { name: "Alice", createdAt: Date, updatedAt: Date }
```

`updatedAt` is automatically updated on every save.

## Key Points:
- Adds `createdAt` and `updatedAt`.
- `createdAt` set on creation.
- `updatedAt` updated on every save.
- Uses `Date.now()` by default.
- Essential for auditing.

## Interview Tip:
"`timestamps: true` is essential â€” use it on every model."

---

## Part 4 (31â€“40): Models

---

## Question 31: What is a Mongoose Model?

## Answer:
A model is a compiled schema that provides an interface for creating, querying, updating, and deleting documents.

```javascript
const mongoose = require("mongoose");

const userSchema = new mongoose.Schema({
  name: String,
  email: String
});

const User = mongoose.model("User", userSchema);
// "User" is the model name
// MongoDB collection: "users" (lowercase, pluralized)
```

## Key Points:
- Compiled from a schema.
- Interface for CRUD operations.
- Model name becomes collection (pluralized).
- `mongoose.model("User", schema)` creates a model.
- Models are like classes; documents are instances.

## Interview Tip:
"Models are the interface â€” they're how you interact with MongoDB documents."

---

## Question 32: How do you create a model?

## Answer:
```javascript
const mongoose = require("mongoose");

const userSchema = new mongoose.Schema({
  name: String,
  email: String
});

const User = mongoose.model("User", userSchema);
```

`mongoose.model()` takes two arguments:
1. Model name (singular, PascalCase).
2. Schema.

## Key Points:
- `mongoose.model(name, schema)`.
- Model name should be singular (Mongoose pluralizes).
- PascalCase convention.
- Returns a model constructor.
- Models are cached by name.

## Interview Tip:
"Model name should be singular â€” `mongoose.model('User', schema)` creates the `users` collection."

---

## Question 33: What is the relationship between a schema and a model?

## Answer:
- **Schema**: Defines the structure and behavior.
- **Model**: Provides the interface for database operations.

```javascript
// Schema: blueprint
const userSchema = new mongoose.Schema({ name: String });

// Model: usable interface
const User = mongoose.model("User", userSchema);

// Document: instance
const user = new User({ name: "Alice" });
```

Schema â†’ Model â†’ Document.

## Key Points:
- Schema: blueprint for documents.
- Model: interface for database operations.
- Document: instance of a model.
- One schema can create one model.
- One model can create many documents.

## Interview Tip:
"Schema is the blueprint, Model is the class, Document is the instance."

---

## Question 34: What is a Mongoose document?

## Answer:
A document is an instance of a model. It represents a single record in MongoDB.

```javascript
const user = new User({ name: "Alice", email: "alice@example.com" });
await user.save();
// user is a document
```

Documents have methods, virtuals, and can be modified before saving.

## Key Points:
- Instance of a model.
- Represents a MongoDB document.
- Has methods and virtuals.
- Can be modified before saving.
- Reflects the schema structure.

## Interview Tip:
"Documents are instances â€” they represent individual records in MongoDB."

---

## Question 35: How do you create a document?

## Answer:
```javascript
// Method 1: new + save
const user = new User({ name: "Alice", email: "alice@example.com" });
await user.save();

// Method 2: create()
const user = await User.create({ name: "Alice", email: "alice@example.com" });

// Method 3: insertMany()
const users = await User.insertMany([
  { name: "Alice" },
  { name: "Bob" }
]);
```

## Key Points:
- `new Model()` + `save()` for single documents.
- `create()` for single or multiple.
- `insertMany()` for bulk inserts.
- `create()` is shorthand for `new + save`.

## Interview Tip:
"`create()` is the most common way â€” it's a shorthand for `new + save()`."

---

## Question 36: How do you save a document?

## Answer:
```javascript
const user = new User({ name: "Alice" });
await user.save();  // Saves to MongoDB

// Check if modified
user.name = "Alice Smith";
await user.save();  // Updates the document
```

`save()` triggers validation and middleware.

## Key Points:
- `save()` persists to MongoDB.
- Triggers validation.
- Triggers pre/post save middleware.
- Returns a promise.
- Use `create()` for one-step creation.

## Interview Tip:
"`save()` triggers validation and middleware â€” `insertMany()` doesn't."

---

## Question 37: What is the difference between `new Model()` and `Model.create()`?

## Answer:
- **`new Model()`**: Creates a document instance (not saved yet).
- **`Model.create()`**: Creates and saves in one step.

```javascript
// new + save (two steps)
const user = new User({ name: "Alice" });
await user.save();

// create (one step)
const user = await User.create({ name: "Alice" });
```

`create()` is shorthand and returns the saved document.

## Key Points:
- `new`: creates instance, not saved.
- `create`: creates and saves.
- `create` is shorthand for `new + save`.
- `create` returns saved document.
- `create` supports arrays.

## Interview Tip:
"`create()` is more concise â€” use it unless you need to modify the document before saving."

---

## Question 38: How do you delete a document?

## Answer:
```javascript
// deleteOne
await User.deleteOne({ name: "Alice" });

// deleteMany
await User.deleteMany({ role: "user" });

// findByIdAndDelete
await User.findByIdAndDelete(userId);

// Using document
const user = await User.findById(userId);
await user.deleteOne();
```

## Key Points:
- `deleteOne()`: delete one matching document.
- `deleteMany()`: delete all matching documents.
- `findByIdAndDelete()`: delete by ID.
- Document `deleteOne()`: delete the document.
- Returns deletion result.

## Interview Tip:
"`deleteOne()` and `deleteMany()` are the main deletion methods."

---

## Question 39: How do you update a document?

## Answer:
```javascript
// updateOne
await User.updateOne({ name: "Alice" }, { name: "Alice Smith" });

// updateMany
await User.updateMany({ role: "user" }, { isActive: true });

// findByIdAndUpdate
await User.findByIdAndUpdate(userId, { name: "Alice Smith" });

// Document update
const user = await User.findById(userId);
user.name = "Alice Smith";
await user.save();
```

## Key Points:
- `updateOne()`: update one matching document.
- `updateMany()`: update all matching documents.
- `findByIdAndUpdate()`: update by ID.
- Document `save()`: update modified document.
- `save()` triggers validation and middleware.

## Interview Tip:
"`save()` triggers validation; `updateOne()` and `updateMany()` don't by default."

---

## Question 40: What are static methods in Mongoose?

## Answer:
Static methods are defined on the model and called on the model itself.

```javascript
userSchema.statics.findByEmail = async function(email) {
  return this.findOne({ email });
};

// Usage
const user = await User.findByEmail("alice@example.com");
```

`this` refers to the model.

## Key Points:
- Defined on the model schema.
- Called on the model: `Model.method()`.
- `this` refers to the model.
- Useful for common queries.
- Don't have access to document data.

## Interview Tip:
"Static methods are model-level â€” they don't have access to individual documents."

---

## Part 5 (41â€“50): Instance Methods & Virtuals

---

## Question 41: What are instance methods?

## Answer:
Instance methods are defined on documents and called on document instances.

```javascript
userSchema.methods.getFullName = function() {
  return `${this.firstName} ${this.lastName}`;
};

// Usage
const user = new User({ firstName: "Alice", lastName: "Smith" });
console.log(user.getFullName()); // "Alice Smith"
```

`this` refers to the document.

## Key Points:
- Defined on the schema.
- Called on document instances.
- `this` refers to the document.
- Useful for document-specific logic.
- Can access document data.

## Interview Tip:
"Instance methods are document-level â€” they have access to the document's data."

---

## Question 42: How do instance methods differ from static methods?

## Answer:
| Feature | Instance Methods | Static Methods |
|---------|-----------------|----------------|
| Called on | Document instance | Model |
| `this` | Document | Model |
| Access | Document data | Model-level operations |
| Use case | Document logic | Common queries |

```javascript
// Instance method
userSchema.methods.getFullName = function() { return this.name; };

// Static method
userSchema.statics.findByEmail = function(email) { return this.findOne({ email }); };
```

## Key Points:
- Instance: called on documents, `this` = document.
- Static: called on model, `this` = model.
- Instance for document logic.
- Static for common queries.

## Interview Tip:
"Instance methods for documents; static methods for the model."

---

## Question 43: What are virtual properties?

## Answer:
Virtual properties are computed fields that aren't stored in MongoDB but are calculated when accessed.

```javascript
userSchema.virtual("fullName").get(function() {
  return `${this.firstName} ${this.lastName}`;
});

const user = new User({ firstName: "Alice", lastName: "Smith" });
console.log(user.fullName); // "Alice Smith" â€” computed, not stored
```

## Key Points:
- Computed fields, not stored.
- Calculated on access.
- `get` for reading, `set` for writing.
- Don't appear in MongoDB queries.
- Useful for derived data.

## Interview Tip:
"Virtuals are computed fields â€” they don't use storage but provide useful data."

---

## Question 44: Why would you use virtuals?

## Answer:
- **Derived data**: `fullName` from `firstName` + `lastName`.
- **Formatted data**: `priceDisplay` from `price` + currency.
- **References**: Virtual population for relationships.
- **Computed fields**: Any calculation based on document data.
- **No storage cost**: Don't use database space.

## Key Points:
- Derived data without storage.
- Formatted or computed fields.
- Virtual population for relationships.
- No database overhead.
- Useful for API responses.

## Interview Tip:
"Virtuals are great for API responses â€” computed data without storage cost."

---

## Question 45: What is the difference between stored fields and virtual fields?

## Answer:
| Feature | Stored Fields | Virtual Fields |
|---------|--------------|----------------|
| Storage | In MongoDB | Not stored |
| Queries | Can query | Cannot query |
| Performance | Read from DB | Computed on access |
| Use case | Actual data | Derived data |

```javascript
// Stored: email is in MongoDB
email: String

// Virtual: fullName is computed
userSchema.virtual("fullName").get(function() { ... });
```

## Key Points:
- Stored fields: in MongoDB, queryable.
- Virtual fields: not stored, computed.
- Stored fields have storage cost.
- Virtual fields have computation cost.
- Choose based on needs.

## Interview Tip:
"Stored fields for actual data; virtuals for derived data."

---

## Question 46: How do you hide sensitive fields using schema options?

## Answer:
```javascript
const userSchema = new mongoose.Schema({
  name: String,
  password: { type: String, select: false }  // Hidden by default
});

// To include password in query
const user = await User.findById(id).select("+password");
```

`select: false` hides the field unless explicitly selected.

## Key Points:
- `select: false` hides field by default.
- Use `+field` to include it.
- Useful for passwords, tokens, etc.
- Prevents accidental exposure.
- Can be overridden with `select()`.

## Interview Tip:
"`select: false` is essential for passwords â€” it prevents accidental exposure."

---

## Question 47: What is the `toJSON` transform?

## Answer:
The `toJSON` transform controls how documents are serialized to JSON (e.g., API responses).

```javascript
const userSchema = new mongoose.Schema({
  name: String,
  password: { type: String, select: false }
}, {
  toJSON: {
    transform: (doc, ret) => {
      delete ret.password;
      delete ret.__v;
      return ret;
    }
  }
});
```

## Key Points:
- Controls JSON serialization.
- Remove sensitive fields.
- Remove `__v` (version key).
- Rename fields.
- Customize API responses.

## Interview Tip:
"`toJSON` transform is great for hiding sensitive fields and cleaning up API responses."

---

## Question 48: What is the `toObject` transform?

## Answer:
The `toObject` transform controls how documents are converted to plain JavaScript objects.

```javascript
const userSchema = new mongoose.Schema({
  name: String,
  email: String
}, {
  toObject: { virtuals: true }
});

const user = await User.findById(id);
const obj = user.toObject(); // Plain JavaScript object
```

## Key Points:
- Controls object serialization.
- `virtuals: true` includes virtuals.
- `transform` function for customization.
- Used internally by `toJSON`.
- Converts Mongoose document to plain object.

## Interview Tip:
"`toObject` is for plain objects; `toJSON` is for JSON serialization."

---

## Question 49: What are schema plugins?

## Answer:
Schema plugins add reusable functionality to schemas.

```javascript
function timestampPlugin(schema) {
  schema.add({ createdAt: Date, updatedAt: Date });
  schema.pre("save", function() {
    this.updatedAt = new Date();
    if (!this.createdAt) this.createdAt = new Date();
  });
}

userSchema.plugin(timestampPlugin);
```

## Key Points:
- Reusable schema extensions.
- Add fields, methods, or middleware.
- Called with `schema.plugin()`.
- Share functionality across schemas.
- Third-party plugins available.

## Interview Tip:
"Plugins are reusable schema extensions â€” great for cross-cutting concerns."

---

## Question 50: What Mongoose schema best practices do you follow?

## Answer:
1. **Use `timestamps: true`**: Auto-manage `createdAt`/`updatedAt`.
2. **Validate fields**: Use `required`, `enum`, `min/max`.
3. **Use `select: false`**: For sensitive fields.
4. **Add indexes**: On frequently queried fields.
5. **Use virtuals**: For computed fields.
6. **Keep schemas focused**: One model per entity.
7. **Use plugins**: For reusable functionality.
8. **Document schema structure**: Add comments.

## Key Points:
- Timestamps for auditing.
- Validation for integrity.
- Select for sensitive data.
- Indexes for performance.
- Virtuals for computed data.
- Focused schemas.
- Plugins for reuse.

## Interview Tip:
"Timestamps, validation, indexes, and select:false â€” the schema best practice quartet."

---

## Part 6 (51â€“60): CRUD Operations

---

## Question 51: How do you create a document using Mongoose?

## Answer:
```javascript
// Method 1: new + save
const user = new User({ name: "Alice", email: "alice@example.com" });
await user.save();

// Method 2: create
const user = await User.create({ name: "Alice", email: "alice@example.com" });

// Method 3: insertMany
const users = await User.insertMany([
  { name: "Alice" },
  { name: "Bob" }
]);
```

## Key Points:
- `new + save()` for one document.
- `create()` for one or multiple.
- `insertMany()` for bulk inserts.
- `create()` triggers validation.
- `insertMany()` doesn't trigger middleware.

## Interview Tip:
"`create()` is the most common â€” it's concise and triggers validation."

---

## Question 52: What is the difference between `save()` and `create()`?

## Answer:
- **`save()`**: Saves an existing document instance.
- **`create()`**: Creates and saves in one step.

```javascript
// save: two steps
const user = new User({ name: "Alice" });
await user.save();

// create: one step
const user = await User.create({ name: "Alice" });
```

Both trigger validation and middleware.

## Key Points:
- `save()`: saves existing instance.
- `create()`: creates and saves.
- Both trigger validation and middleware.
- `create()` returns saved document.
- `create()` supports arrays.

## Interview Tip:
"`create()` is shorthand for `new + save()` â€” use it for simplicity."

---

## Question 53: How do you retrieve documents?

## Answer:
```javascript
// find: multiple documents
const users = await User.find({ role: "user" });

// findOne: single document
const user = await User.findOne({ email: "alice@example.com" });

// findById: by ID
const user = await User.findById(userId);

// where + equals
const users = await User.where("age").gt(18).equals(true);
```

## Key Points:
- `find()`: returns array of documents.
- `findOne()`: returns single document or null.
- `findById()`: returns document by ID.
- All support chaining.
- All return Mongoose documents (unless `lean()`).

## Interview Tip:
"`find()` for lists; `findOne()` or `findById()` for single documents."

---

## Question 54: What is the difference between `find()` and `findOne()`?

## Answer:
- **`find()`**: Returns an array of matching documents.
- **`findOne()`**: Returns the first matching document or null.

```javascript
const users = await User.find({ role: "user" }); // Array
const user = await User.findOne({ role: "user" }); // Single document or null
```

## Key Points:
- `find()`: always returns array.
- `findOne()`: returns one document or null.
- `findOne()` is faster (stops at first match).
- Use `findOne()` when you expect one result.
- Both support filtering.

## Interview Tip:
"`findOne()` is faster â€” it stops at the first match."

---

## Question 55: What is `findById()`?

## Answer:
`findById()` is shorthand for `findOne({ _id: id })`. It returns a single document by its `_id`.

```javascript
const user = await User.findById(userId);
```

Returns `null` if not found.

## Key Points:
- Shorthand for `findOne({ _id: id })`.
- Returns single document or null.
- Most common way to fetch by ID.
- Supports population.
- Efficient (uses `_id` index).

## Interview Tip:
"`findById()` is the most common way to fetch a document â€” it's efficient and readable."

---

## Question 56: How do you update documents?

## Answer:
```javascript
// updateOne
await User.updateOne({ name: "Alice" }, { name: "Alice Smith" });

// updateMany
await User.updateMany({ role: "user" }, { isActive: true });

// findByIdAndUpdate
await User.findByIdAndUpdate(userId, { name: "Alice Smith" }, { new: true });

// Document update
const user = await User.findById(userId);
user.name = "Alice Smith";
await user.save();
```

## Key Points:
- `updateOne()`: update one matching document.
- `updateMany()`: update all matching documents.
- `findByIdAndUpdate()`: update by ID.
- Document `save()`: update modified document.
- `{ new: true }` returns updated document.

## Interview Tip:
"`{ new: true }` is essential with `findByIdAndUpdate()` â€” otherwise you get the old document."

---

## Question 57: What is the difference between `updateOne()` and `findOneAndUpdate()`?

## Answer:
- **`updateOne()`**: Updates one matching document.
- **`findOneAndUpdate()`**: Finds and updates one document, returns the document.

```javascript
await User.updateOne({ name: "Alice" }, { name: "Alice Smith" }); // void

const user = await User.findOneAndUpdate(
  { name: "Alice" },
  { name: "Alice Smith" },
  { new: true }  // Return updated document
);
```

## Key Points:
- `updateOne()`: no return value.
- `findOneAndUpdate()`: returns the document.
- Use `{ new: true }` to get updated document.
- Both update one matching document.
- `findOneAndUpdate()` is more common.

## Interview Tip:
"`findOneAndUpdate()` returns the document â€” use it when you need the result."

---

## Question 58: How do you delete documents?

## Answer:
```javascript
// deleteOne
await User.deleteOne({ name: "Alice" });

// deleteMany
await User.deleteMany({ role: "user" });

// findByIdAndDelete
await User.findByIdAndDelete(userId);

// Document delete
const user = await User.findById(userId);
await user.deleteOne();
```

## Key Points:
- `deleteOne()`: delete one matching document.
- `deleteMany()`: delete all matching documents.
- `findByIdAndDelete()`: delete by ID.
- Document `deleteOne()`: delete the document.
- Returns deletion result.

## Interview Tip:
"`deleteOne()` and `deleteMany()` are the main deletion methods."

---

## Question 59: What is the difference between `deleteOne()` and `findOneAndDelete()`?

## Answer:
- **`deleteOne()`**: Deletes one matching document.
- **`findOneAndDelete()`**: Finds and deletes one document, returns the deleted document.

```javascript
await User.deleteOne({ name: "Alice" }); // void

const user = await User.findOneAndDelete({ name: "Alice" }); // returns deleted doc
```

## Key Points:
- `deleteOne()`: no return value.
- `findOneAndDelete()`: returns deleted document.
- Both delete one matching document.
- `findOneAndDelete()` is more common.
- Triggers middleware.

## Interview Tip:
"`findOneAndDelete()` returns the deleted document â€” useful for confirmation."

---

## Question 60: What CRUD best practices do you follow in Mongoose?

## Answer:
1. **Use `create()`**: For creating documents.
2. **Use `findById()`**: For fetching by ID.
3. **Use `findOneAndUpdate()` with `{ new: true }`**: For updates.
4. **Use `deleteOne()`**: For deletions.
5. **Always handle errors**: Try/catch or `.catch()`.
6. **Use `lean()`**: For read-only queries (performance).
7. **Use `select()`**: To limit returned fields.

## Key Points:
- `create()` for creation.
- `findById()` for fetching.
- `findOneAndUpdate()` with `{ new: true }`.
- `deleteOne()` for deletion.
- Error handling always.
- `lean()` for performance.
- `select()` to limit fields.

## Interview Tip:
"`create`, `findById`, `findOneAndUpdate` with `{ new: true }`, `deleteOne` â€” the CRUD essentials."

---

## Part 7 (61â€“70): Validation

---

## Question 61: What is schema validation?

## Answer:
Schema validation ensures documents meet specified criteria before saving. Mongoose validates on `save()` and `create()`, not on `updateOne()` or `updateMany()`.

```javascript
const userSchema = new mongoose.Schema({
  name: { type: String, required: true },
  age: { type: Number, min: 0, max: 150 }
});
```

## Key Points:
- Validates on `save()` and `create()`.
- Does NOT validate on `updateOne()`, `updateMany()`.
- Built-in and custom validators.
- Throws `ValidationError` on failure.
- Can be disabled with `{ validateBeforeSave: false }`.

## Interview Tip:
"Validation only happens on `save()` and `create()` â€” not on `updateOne()` or `updateMany()`."

---

## Question 62: What built-in validators does Mongoose provide?

## Answer:
- **`required`**: Field must exist.
- **`unique`**: Field value must be unique.
- **`enum`**: Value must be in allowed list.
- **`min`/`max`**: Number minimum/maximum.
- **`minlength`/`maxlength`**: String length limits.
- **`match`**: Regex pattern matching.

## Key Points:
- `required`, `unique`, `enum`.
- `min`/`max` for numbers.
- `minlength`/`maxlength` for strings.
- `match` for regex patterns.
- All throw `ValidationError` on failure.

## Interview Tip:
"Mongoose has six built-in validators: required, unique, enum, min/max, minlength/maxlength, match."

---

## Question 63: What is the `required` validator?

## Answer:
The `required` validator ensures a field exists and is not `null` or `undefined`.

```javascript
const userSchema = new mongoose.Schema({
  name: { type: String, required: true },
  email: { type: String, required: [true, "Email is required"] }
});
```

Custom error message with array syntax.

## Key Points:
- Ensures field exists.
- Rejects `null` and `undefined`.
- Custom error message with array.
- Can be a function for dynamic requirements.
- Essential for data integrity.

## Interview Tip:
"`required: [true, 'message']` gives you a custom error message."

---

## Question 64: What is the `unique` option?

## Answer:
`unique` creates a unique index in MongoDB, ensuring no duplicate values.

```javascript
const userSchema = new mongoose.Schema({
  email: { type: String, unique: true }
});
```

This creates a unique index on the `email` field.

## Key Points:
- Creates a unique index.
- Prevents duplicate values.
- Database-level constraint.
- Not a validator (it's an index).
- Async validation on save.

## Interview Tip:
"`unique` creates an index, not a validator â€” it's enforced at the database level."

---

## Question 65: What is the difference between `required` and `unique`?

## Answer:
| Feature | required | unique |
|---------|----------|--------|
| Purpose | Field must exist | Value must be unique |
| Level | Validator | Index |
| Timing | Sync | Async (database check) |
| Error | ValidationError | Duplicate key error |

## Key Points:
- `required`: validator, sync, field must exist.
- `unique`: index, async, value must be unique.
- Both enforce data integrity.
- Different error types.

## Interview Tip:
"`required` is a validator; `unique` is an index. Different mechanisms, different errors."

---

## Question 66: How do you validate string length?

## Answer:
```javascript
const userSchema = new mongoose.Schema({
  name: {
    type: String,
    minlength: [2, "Name must be at least 2 characters"],
    maxlength: [100, "Name must be at most 100 characters"]
  }
});
```

## Key Points:
- `minlength`: minimum string length.
- `maxlength`: maximum string length.
- Custom error messages with array.
- Validates on `save()` and `create()`.

## Interview Tip:
"`minlength` and `maxlength` are essential for string validation."

---

## Question 67: How do you validate numbers?

## Answer:
```javascript
const productSchema = new mongoose.Schema({
  price: {
    type: Number,
    min: [0, "Price must be positive"],
    max: [10000, "Price must be less than 10000"]
  },
  quantity: {
    type: Number,
    min: 0
  }
});
```

## Key Points:
- `min`: minimum value.
- `max`: maximum value.
- Custom error messages with array.
- Works with Integer and Float.

## Interview Tip:
"`min` and `max` for numbers â€” essential for price, quantity, and age validation."

---

## Question 68: How do you create custom validators?

## Answer:
```javascript
const userSchema = new mongoose.Schema({
  email: {
    type: String,
    validate: {
      validator: function(v) {
        return /^\w+@\w+\.\w+$/.test(v);
      },
      message: props => `${props.value} is not a valid email`
    }
  }
});
```

Custom validator function returns `true` (valid) or `false` (invalid).

## Key Points:
- `validate` option with `validator` function.
- Returns `true` (valid) or `false` (invalid).
- Custom error message with `message`.
- `this` refers to the document.
- Can be async.

## Interview Tip:
"Custom validators give you full control â€” return `true` if valid, `false` if not."

---

## Question 69: How do async validators work?

## Answer:
```javascript
const userSchema = new mongoose.Schema({
  email: {
    type: String,
    validate: {
      validator: async function(v) {
        const user = await mongoose.model("User").findOne({ email: v });
        return !user; // true if email is unique
      },
      message: "Email already exists"
    }
  }
});
```

Async validators return a promise.

## Key Points:
- `validator` function can be async.
- Returns a promise.
- Useful for database checks.
- Slower than sync validators.
- Use sparingly for performance.

## Interview Tip:
"Async validators are for database checks â€” use them sparingly for performance."

---

## Question 70: How do you handle validation errors?

## Answer:
```javascript
try {
  await user.save();
} catch (error) {
  if (error.name === "ValidationError") {
    const messages = Object.values(error.errors).map(e => e.message);
    console.error("Validation errors:", messages);
  }
}
```

## Key Points:
- Catches `ValidationError`.
- `error.errors` contains field-specific errors.
- `error.message` for overall message.
- Each error has `path` and `message`.
- Handle gracefully in API responses.

## Interview Tip:
"Check `error.name === 'ValidationError'` and map `error.errors` for field-specific messages."

---

## Part 8 (71â€“80): Middleware (Hooks)

---

## Question 71: What is middleware in Mongoose?

## Answer:
Middleware (hooks) are functions that run before or after certain operations (save, validate, remove, etc.).

```javascript
userSchema.pre("save", function(next) {
  console.log("About to save user:", this.name);
  next();
});

userSchema.post("save", function(doc) {
  console.log("User saved:", doc.name);
});
```

## Key Points:
- Pre and post hooks.
- Run before/after operations.
- `next()` in pre hooks.
- `doc` in post hooks.
- Can be async.

## Interview Tip:
"Middleware is for cross-cutting concerns â€” logging, validation, hashing, etc."

---

## Question 72: What is the difference between document middleware and query middleware?

## Answer:
| Feature | Document Middleware | Query Middleware |
|---------|-------------------|-----------------|
| Runs on | Document operations | Query operations |
| Examples | save, validate | find, update, remove |
| `this` | Document | Query |
| Use case | Document logic | Query modifications |

## Key Points:
- Document middleware: save, validate, remove.
- Query middleware: find, update, remove.
- `this` differs: document vs query.
- Document for document logic.
- Query for query modifications.

## Interview Tip:
"Document middleware for save/validate; query middleware for find/update/remove."

---

## Question 73: What is `pre()` middleware?

## Answer:
`pre()` runs before the specified operation.

```javascript
userSchema.pre("save", function(next) {
  if (this.isModified("password")) {
    this.password = bcrypt.hashSync(this.password, 10);
  }
  next();
});
```

Must call `next()` to continue.

## Key Points:
- Runs before operation.
- Must call `next()`.
- Can modify the document.
- Can abort the operation (don't call `next()`).
- Async functions don't need `next()`.

## Interview Tip:
"`pre('save')` is the most common middleware â€” it's used for password hashing."

---

## Question 74: What is `post()` middleware?

## Answer:
`post()` runs after the specified operation.

```javascript
userSchema.post("save", function(doc) {
  console.log("User saved:", doc.name);
  // Send welcome email, log activity, etc.
});
```

Receives the document as the first argument.

## Key Points:
- Runs after operation.
- Receives document/result.
- Cannot modify the document.
- Good for side effects (logging, emails).
- Async functions supported.

## Interview Tip:
"`post()` is for side effects â€” logging, notifications, emails."

---

## Question 75: What are common use cases for middleware?

## Answer:
1. **Password hashing**: Hash before save.
2. **Timestamps**: Auto-update `updatedAt`.
3. **Logging**: Log operations.
4. **Validation**: Custom validation logic.
5. **Soft deletes**: Mark as deleted instead of removing.
6. **Cascade deletes**: Delete related documents.

## Key Points:
- Password hashing.
- Timestamps.
- Logging.
- Custom validation.
- Soft deletes.
- Cascade deletes.

## Interview Tip:
"Password hashing and timestamps are the two most common middleware use cases."

---

## Question 76: How do you hash passwords using middleware?

## Answer:
```javascript
const bcrypt = require("bcrypt");

userSchema.pre("save", async function(next) {
  if (!this.isModified("password")) return next();
  this.password = await bcrypt.hash(this.password, 12);
  next();
});

// Instance method to compare
userSchema.methods.comparePassword = async function(candidatePassword) {
  return bcrypt.compare(candidatePassword, this.password);
};
```

## Key Points:
- Hash in `pre("save")` middleware.
- Check `isModified("password")` to avoid re-hashing.
- Use `bcrypt` for hashing.
- Instance method for comparison.
- Cost factor of 12+.

## Interview Tip:
"Hash in pre-save middleware â€” it's the standard pattern for password security."

---

## Question 77: What is the difference between `save()` middleware and `update()` middleware?

## Answer:
- **`save()` middleware**: Runs on `save()`, `create()`. Has access to document.
- **`update()` middleware**: Runs on `updateOne()`, `updateMany()`. Has access to query, not document.

```javascript
// save middleware
userSchema.pre("save", function(next) {
  this.password = hash(this.password); // `this` = document
  next();
});

// update middleware
userSchema.pre("updateOne", function(next) {
  this.set({ updatedAt: new Date() }); // `this` = query
  next();
});
```

## Key Points:
- `save()`: document middleware, `this` = document.
- `update()`: query middleware, `this` = query.
- Different access patterns.
- Different use cases.

## Interview Tip:
"Save middleware has the document; update middleware has the query â€” different access patterns."

---

## Question 78: How do middleware execution order and chaining work?

## Answer:
Multiple middleware on the same hook run in order:

```javascript
userSchema.pre("save", function(next) {
  console.log("First pre-save");
  next();
});

userSchema.pre("save", function(next) {
  console.log("Second pre-save");
  next();
});
// Output: "First pre-save" â†’ "Second pre-save"
```

## Key Points:
- Multiple middleware run in order.
- Each must call `next()`.
- Order depends on registration order.
- Can be async (no `next()` needed).

## Interview Tip:
"Middleware runs in registration order â€” each must call `next()` to continue."

---

## Question 79: What are common mistakes when using middleware?

## Answer:
1. **Forgetting `next()`**: Middleware hangs.
2. **Not checking `isModified`**: Re-hashing on every save.
3. **Using document middleware for queries**: Wrong `this` context.
4. **Heavy operations in pre-save**: Slows down saves.
5. **Not handling errors**: Errors swallowed silently.

## Key Points:
- Always call `next()`.
- Check `isModified` for conditionals.
- Use correct middleware type.
- Keep middleware lightweight.
- Handle errors properly.

## Interview Tip:
"Forgetting `next()` is the most common middleware bug â€” it hangs the operation."

---

## Question 80: What middleware best practices do you follow?

## Answer:
1. **Keep middleware lightweight**: Don't do heavy operations.
2. **Check `isModified`**: Only run when needed.
3. **Handle errors**: Don't swallow them.
4. **Use async/await**: For modern middleware.
5. **Document middleware behavior**: Comment on what each hook does.
6. **Test middleware**: Verify it runs correctly.

## Key Points:
- Lightweight operations.
- Conditional execution with `isModified`.
- Error handling.
- Async/await for modern code.
- Documentation and testing.

## Interview Tip:
"Keep middleware lightweight, check `isModified`, and always handle errors."

---

## Part 9 (81â€“90): Populate & Relationships

---

## Question 81: What is `populate()`?

## Answer:
`populate()` replaces ObjectId references with actual documents from the referenced collection.

```javascript
const post = await Post.findById(postId).populate("author");
// post.author is now the full User document, not just an ObjectId
```

## Key Points:
- Replaces references with actual documents.
- Like SQL JOINs.
- Uses `ref` from schema.
- Can populate multiple fields.
- Supports filtering and limiting.

## Interview Tip:
"`populate()` is MongoDB's JOIN â€” it replaces references with actual documents."

---

## Question 82: How does `populate()` work?

## Answer:
1. Mongoose sees the `ref` in the schema.
2. It queries the referenced collection.
3. Replaces the ObjectId with the actual document.

```javascript
const postSchema = new mongoose.Schema({
  title: String,
  author: { type: mongoose.Schema.Types.ObjectId, ref: "User" }
});

const post = await Post.findById(id).populate("author");
// Mongoose queries: User.findById(post.author)
// Replaces author ObjectId with User document
```

## Key Points:
- Uses `ref` to find the referenced model.
- Queries the referenced collection.
- Replaces ObjectId with document.
- Extra query (performance consideration).
- Can be chained.

## Interview Tip:
"`populate()` is an extra query â€” be mindful of performance with many references."

---

## Question 83: What is the difference between embedding and referencing?

## Answer:
| Feature | Embedding | Referencing |
|---------|-----------|-------------|
| Storage | Nested document | ObjectId reference |
| Query | Single query | Multiple queries |
| Consistency | Always consistent | May become stale |
| Size | Limited (16MB doc) | Unlimited |
| Updates | Update parent | Update separate |

```javascript
// Embedding
comments: [{ text: String, author: String }]

// Referencing
comments: [{ type: ObjectId, ref: "Comment" }]
```

## Key Points:
- Embedding: nested, single query, limited size.
- Referencing: separate, multiple queries, unlimited.
- Embedding for tightly coupled data.
- Referencing for loosely coupled data.

## Interview Tip:
"Embed for tightly coupled data; reference for loosely coupled data."

---

## Question 84: When should you use `populate()`?

## Answer:
- **Related data**: Users and their posts.
- **Lookups**: Finding related records.
- **API responses**: Including related data.
- **One-to-many**: When you need the full related document.

Avoid for:
- **Large datasets**: Performance impact.
- **Write-heavy**: Frequent updates to referenced data.
- **Simple references**: When ObjectId is enough.

## Key Points:
- Related data that needs full documents.
- API responses with related data.
- One-to-many relationships.
- Avoid for performance-critical paths.
- Avoid for large datasets.

## Interview Tip:
"Use `populate()` when you need the full related document â€” avoid it for performance-critical paths."

---

## Question 85: What are the performance drawbacks of `populate()`?

## Answer:
- **Extra queries**: Each `populate()` is an additional query.
- **N+1 problem**: Populating in loops causes N+1 queries.
- **Memory**: Loading full documents uses more memory.
- **Latency**: Additional round trips to MongoDB.

## Key Points:
- Extra queries per `populate()`.
- N+1 problem in loops.
- Higher memory usage.
- Increased latency.
- Use `lean()` and `select()` to mitigate.

## Interview Tip:
"`populate()` is convenient but expensive â€” use `lean()` and `select()` to optimize."

---

## Question 86: How do you populate multiple references?

## Answer:
```javascript
const post = await Post.findById(id)
  .populate("author")
  .populate("comments")
  .populate("tags");
```

Or as an array:
```javascript
const post = await Post.findById(id)
  .populate(["author", "comments", "tags"]);
```

## Key Points:
- Chain multiple `populate()` calls.
- Or pass an array.
- Each populates a different field.
- Extra query per field.
- Can be combined with filtering.

## Interview Tip:
"Chain multiple `populate()` calls â€” each adds a query."

---

## Question 87: How do you populate nested references?

## Answer:
```javascript
const post = await Post.findById(id).populate({
  path: "author",
  populate: {
    path: "profile",
    select: "bio avatar"
  }
});
```

Nested `populate` for references within references.

## Key Points:
- Nested `populate` for deep references.
- `path` specifies the field.
- Nested `populate` for sub-references.
- Extra queries per level.
- Can be combined with `select`.

## Interview Tip:
"Nested `populate` is for deep references â€” but it adds more queries."

---

## Question 88: What is virtual populate?

## Answer:
Virtual populate defines a virtual field that populates a reference.

```javascript
const userSchema = new mongoose.Schema({ name: String });
userSchema.virtual("posts", {
  ref: "Post",
  localField: "_id",
  foreignField: "author"
});

const user = await User.findById(id).populate("posts");
```

## Key Points:
- Virtual field for population.
- `ref`: model to populate.
- `localField`: field in this model.
- `foreignField`: field in the referenced model.
- Doesn't store data.

## Interview Tip:
"Virtual populate is great for one-to-many â€” it populates without storing references."

---

## Question 89: How do you limit fields returned by `populate()`?

## Answer:
```javascript
const post = await Post.findById(id).populate({
  path: "author",
  select: "name email"  // Only return name and email
});

// Exclude fields
const post = await Post.findById(id).populate({
  path: "author",
  select: "-password -__v"  // Exclude password and __v
});
```

## Key Points:
- `select` within `populate()`.
- Include specific fields.
- Exclude with `-` prefix.
- Reduces data transfer.
- Improves performance.

## Interview Tip:
"Use `select` in `populate()` to limit fields â€” it reduces data transfer."

---

## Question 90: What relationship modeling best practices do you follow?

## Answer:
1. **Embed for tightly coupled data**: Comments in posts.
2. **Reference for loosely coupled data**: Users and posts.
3. **Use virtual populate**: For one-to-many.
4. **Limit population depth**: Avoid deep nesting.
5. **Use `select`**: Limit populated fields.
6. **Index foreign keys**: For performance.
7. **Consider access patterns**: Design for how you query.

## Key Points:
- Embed for tight coupling; reference for loose.
- Virtual populate for one-to-many.
- Limit population depth.
- Select only needed fields.
- Index foreign keys.
- Design for query patterns.

## Interview Tip:
"Embed for tightly coupled; reference for loosely coupled. That's the golden rule."

---

## Part 10 (91â€“100): Queries & Performance

---

## Question 91: What are query helpers?

## Answer:
Query helpers are custom methods added to the query prototype.

```javascript
userSchema.query.byEmail = function(email) {
  return this.where({ email });
};

// Usage
const users = await User.find().byEmail("alice@example.com");
```

## Key Points:
- Custom methods on query prototype.
- Chainable with other query methods.
- `this` refers to the query.
- Useful for common query patterns.
- Keep queries DRY.

## Interview Tip:
"Query helpers keep your queries DRY â€” define common patterns once."

---

## Question 92: What is `lean()`?

## Answer:
`lean()` returns plain JavaScript objects instead of Mongoose documents. It's faster because it skips document hydration.

```javascript
const users = await User.find().lean();
// users is an array of plain objects, not Mongoose documents
```

## Key Points:
- Returns plain JavaScript objects.
- Skips document hydration.
- Faster queries.
- No methods, virtuals, or middleware.
- Read-only (can't save).

## Interview Tip:
"`lean()` is a performance optimization â€” use it for read-only queries."

---

## Question 93: Why is `lean()` faster than regular queries?

## Answer:
Regular Mongoose queries return full Mongoose documents with:
- Methods
- Virtuals
- Validation
- Change tracking
- Middleware

`lean()` skips all of this, returning plain objects. This reduces memory and CPU overhead.

## Key Points:
- Skips document hydration.
- No methods, virtuals, or validation.
- Reduces memory usage.
- Reduces CPU overhead.
- Significant performance improvement.

## Interview Tip:
"`lean()` skips the Mongoose overhead â€” it's significantly faster for read-only queries."

---

## Question 94: When should you use `lean()`?

## Answer:
- **Read-only queries**: When you don't need to modify documents.
- **API responses**: When returning data to client.
- **Aggregation results**: When processing data.
- **Large datasets**: When performance matters.

Don't use when:
- You need to save the document.
- You need methods or virtuals.
- You need validation.

## Key Points:
- Read-only queries.
- API responses.
- Aggregation results.
- Large datasets.
- Don't use when you need to modify.

## Interview Tip:
"`lean()` for read-only; regular documents for modifications. Know the trade-off."

---

## Question 95: How do you paginate query results?

## Answer:
```javascript
// Offset pagination
const page = 1;
const limit = 10;
const users = await User.find()
  .skip((page - 1) * limit)
  .limit(limit);

// Cursor-based pagination
const users = await User.find()
  .where("_id").gt(lastId)
  .limit(10)
  .sort({ _id: 1 });
```

## Key Points:
- `skip()` and `limit()` for offset pagination.
- Cursor-based for better performance.
- Always sort for consistent results.
- Use `lean()` for performance.
- Count total for page indicators.

## Interview Tip:
"Offset pagination is simpler; cursor-based is better for large datasets."

---

## Question 96: How do you sort query results?

## Answer:
```javascript
// Ascending
const users = await User.find().sort({ name: 1 });

// Descending
const users = await User.find().sort({ createdAt: -1 });

// Multiple fields
const users = await User.find().sort({ role: 1, name: 1 });
```

## Key Points:
- `sort({ field: 1 })` for ascending.
- `sort({ field: -1 })` for descending.
- Multiple fields for multi-level sorting.
- Index sorted fields for performance.

## Interview Tip:
"Sort with `1` for ascending, `-1` for descending."

---

## Question 97: How do you create indexes in Mongoose?

## Answer:
```javascript
const userSchema = new mongoose.Schema({
  email: { type: String, unique: true },
  name: String
});

// Single index
userSchema.index({ name: 1 });

// Compound index
userSchema.index({ name: 1, role: 1 });

// TTL index (auto-delete after time)
userSchema.index({ createdAt: 1 }, { expireAfterSeconds: 3600 });
```

## Key Points:
- `schema.index()` to define indexes.
- `unique: true` for unique indexes.
- Compound indexes for multi-field.
- TTL indexes for auto-expiration.
- Indexes created on first `ensureIndexes()` or app start.

## Interview Tip:
"Define indexes in your schema â€” they're created automatically."

---

## Question 98: How do you debug slow queries?

## Answer:
```javascript
// Enable debug mode
mongoose.set("debug", true);

// Log query execution
const user = await User.findById(id).explain("executionStats");
```

Check:
- Missing indexes.
- N+1 queries.
- Large result sets.
- Unoptimized populate.

## Key Points:
- Enable debug mode.
- Use `explain()` for query analysis.
- Check for missing indexes.
- Look for N+1 queries.
- Optimize populate usage.

## Interview Tip:
"Enable debug mode and use `explain()` to find slow queries."

---

## Question 99: How do you handle duplicate key errors?

## Answer:
```javascript
try {
  await User.create({ email: "duplicate@example.com" });
} catch (error) {
  if (error.code === 11000) {
    // Duplicate key error
    console.error("Email already exists");
  }
}
```

Error code `11000` indicates duplicate key.

## Key Points:
- Error code `11000` for duplicate key.
- Check `error.keyValue` for the duplicate field.
- Handle gracefully in API responses.
- Use `upsert` to avoid duplicates.

## Interview Tip:
"Error code `11000` is the duplicate key error â€” handle it gracefully."

---

## Question 100: What Mongoose query optimization best practices do you follow?

## Answer:
1. **Use `lean()`**: For read-only queries.
2. **Add indexes**: On frequently queried fields.
3. **Use `select()`**: Limit returned fields.
4. **Avoid N+1**: Use `populate()` instead of loops.
5. **Use cursor pagination**: For large datasets.
6. **Batch operations**: Use `insertMany()`, `updateMany()`.
7. **Profile queries**: Use `explain()`.

## Key Points:
- `lean()` for performance.
- Indexes for speed.
- `select()` for minimal data.
- Avoid N+1 queries.
- Cursor pagination.
- Batch operations.
- Profile with `explain()`.

## Interview Tip:
"`lean()`, indexes, and avoiding N+1 are the big three for Mongoose performance."

---

## Part 11 (101â€“110): Transactions & Sessions

---

## Question 101: What are transactions in Mongoose?

## Answer:
Transactions group multiple operations into an atomic unit â€” all succeed or all fail.

```javascript
const session = await mongoose.startSession();
session.startTransaction();

try {
  await User.create([{ name: "Alice" }], { session });
  await Post.create([{ title: "Post", author: userId }], { session });
  await session.commitTransaction();
} catch (error) {
  await session.abortTransaction();
} finally {
  session.endSession();
}
```

## Key Points:
- Atomic operations (all or nothing).
- `startSession()` to begin.
- `commitTransaction()` to save.
- `abortTransaction()` to rollback.
- Requires MongoDB replica set.

## Interview Tip:
"Transactions require a MongoDB replica set â€” make sure it's configured."

---

## Question 102: How do MongoDB transactions work with Mongoose?

## Answer:
```javascript
const session = await mongoose.startSession();
session.startTransaction();

try {
  // Pass session to each operation
  await User.create([{ name: "Alice" }], { session });
  await Account.updateOne({ userId: 1 }, { $inc: { balance: -100 } }, { session });
  await Account.updateOne({ userId: 2 }, { $inc: { balance: 100 } }, { session });
  await session.commitTransaction();
} catch (error) {
  await session.abortTransaction();
  throw error;
} finally {
  session.endSession();
}
```

## Key Points:
- `session` passed to each operation.
- All operations use the same session.
- Commit or abort atomically.
- End session when done.
- Requires replica set.

## Interview Tip:
"Pass the session to every operation â€” that's what makes them atomic."

---

## Question 103: What is a session in Mongoose?

## Answer:
A session is a logical grouping of operations. It provides context for transactions.

```javascript
const session = await mongoose.startSession();
// session is now active
session.startTransaction();
// operations here are part of the transaction
await session.commitTransaction();
session.endSession();
```

## Key Points:
- Logical grouping of operations.
- Context for transactions.
- Created with `startSession()`.
- Must be ended when done.
- Can have one active transaction at a time.

## Interview Tip:
"A session is the container for a transaction â€” create it, use it, end it."

---

## Question 104: How do you start a session?

## Answer:
```javascript
const session = await mongoose.startSession();
session.startTransaction();
```

`startSession()` returns a session object. `startTransaction()` begins the transaction.

## Key Points:
- `mongoose.startSession()` creates a session.
- `session.startTransaction()` begins the transaction.
- Session must be ended after use.
- Only one transaction per session.

## Interview Tip:
"Two steps: start session, then start transaction."

---

## Question 105: How do you commit a transaction?

## Answer:
```javascript
await session.commitTransaction();
```

Commits all operations in the transaction.

## Key Points:
- `commitTransaction()` saves all changes.
- All operations succeed or all fail.
- Must be called to persist changes.
- Throws error if transaction fails.

## Interview Tip:
"`commitTransaction()` persists all changes â€” call it when all operations succeed."

---

## Question 106: How do you abort (rollback) a transaction?

## Answer:
```javascript
await session.abortTransaction();
```

Undoes all operations in the transaction.

## Key Points:
- `abortTransaction()` undoes all changes.
- No changes are persisted.
- Call in catch block on error.
- Safe rollback mechanism.

## Interview Tip:
"`abortTransaction()` in the catch block â€” it rolls back everything."

---

## Question 107: When should you use transactions?

## Answer:
- **Financial operations**: Transfers, payments.
- **Multi-document updates**: When multiple documents must be consistent.
- **Critical operations**: When failure would leave inconsistent data.
- **Inventory operations**: Stock updates with orders.

Don't use for:
- Simple single-document operations.
- Non-critical operations.
- Performance-sensitive paths.

## Key Points:
- Financial and inventory operations.
- Multi-document consistency.
- Critical data operations.
- Avoid for simple operations.
- Performance cost.

## Interview Tip:
"Use transactions for financial and inventory operations â€” consistency is critical."

---

## Question 108: What are the limitations of MongoDB transactions?

## Answer:
- **Replica set required**: Transactions need a replica set.
- **Performance cost**: Transactions add overhead.
- **Time limit**: Transactions have a time limit (default 60s).
- **Document size**: Operations must fit in memory.
- **Write conflicts**: Concurrent transactions may conflict.

## Key Points:
- Requires replica set.
- Performance overhead.
- Time limit.
- Memory constraints.
- Write conflicts possible.

## Interview Tip:
"Transactions need a replica set and add performance overhead â€” use them only when necessary."

---

## Question 109: How do transactions affect performance?

## Answer:
Transactions add overhead:
- **Locking**: Documents are locked during transaction.
- **Memory**: Operations must fit in memory.
- **Network**: Extra round trips for commit/abort.
- **Conflict handling**: Retries on conflicts.

## Key Points:
- Locking overhead.
- Memory constraints.
- Network overhead.
- Conflict handling.
- Use only when necessary.

## Interview Tip:
"Transactions are expensive â€” use them only when consistency is critical."

---

## Question 110: What transaction best practices do you follow?

## Answer:
1. **Keep transactions short**: Don't hold locks long.
2. **Handle errors**: Always have abort in catch.
3. **End sessions**: Always end session when done.
4. **Use try/finally**: Ensure session cleanup.
5. **Limit operations**: Don't put too much in one transaction.
6. **Test thoroughly**: Verify rollback behavior.

## Key Points:
- Short transactions.
- Error handling with abort.
- Always end sessions.
- try/finally for cleanup.
- Limit operations.
- Test rollback.

## Interview Tip:
"Short transactions, error handling, and session cleanup â€” the transaction trifecta."

---

## Part 12 (111â€“120): Performance Optimization

---

## Question 111: How do you optimize Mongoose queries?

## Answer:
1. **Use `lean()`**: For read-only queries.
2. **Add indexes**: On frequently queried fields.
3. **Use `select()`**: Limit returned fields.
4. **Avoid N+1**: Use `populate()` instead of loops.
5. **Use cursor pagination**: For large datasets.
6. **Batch operations**: Use `insertMany()`, `updateMany()`.
7. **Profile queries**: Use `explain()`.

## Key Points:
- `lean()` for performance.
- Indexes for speed.
- `select()` for minimal data.
- Avoid N+1 queries.
- Cursor pagination.
- Batch operations.
- Profile with `explain()`.

## Interview Tip:
"`lean()`, indexes, and avoiding N+1 are the big three."

---

## Question 112: What is the N+1 query problem in Mongoose?

## Answer:
The N+1 problem occurs when you make 1 query for the main list, then N additional queries for each related document.

```javascript
// BAD: N+1 problem
const posts = await Post.find();
for (const post of posts) {
  post.author = await User.findById(post.author); // N queries
}

// GOOD: Use populate
const posts = await Post.find().populate("author"); // 1 query
```

## Key Points:
- 1 query + N queries for related data.
- Causes performance degradation.
- Use `populate()` to fix.
- `populate()` uses lookup (1 query).
- Critical for performance.

## Interview Tip:
"The N+1 problem is the most common Mongoose performance issue â€” use `populate()` to fix it."

---

## Question 113: How does `populate()` affect performance?

## Answer:
- **Extra queries**: Each `populate()` is an additional query.
- **N+1 in loops**: Populating in loops causes N+1.
- **Memory**: Loading full documents uses more memory.
- **Latency**: Additional round trips.

Mitigate with:
- `select()` to limit fields.
- `lean()` for plain objects.
- Batch population.

## Key Points:
- Extra queries per `populate()`.
- N+1 in loops.
- Higher memory usage.
- Increased latency.
- Mitigate with `select()` and `lean()`.

## Interview Tip:
"`populate()` is expensive â€” use `select()` and `lean()` to optimize."

---

## Question 114: When should you avoid using `populate()`?

## Answer:
- **Performance-critical paths**: When every millisecond counts.
- **Large datasets**: When populating thousands of documents.
- **Write-heavy**: When references change frequently.
- **Simple references**: When ObjectId is enough.

Use alternatives:
- `aggregate()` with `$lookup`.
- Manual lookups.
- Embedded documents.

## Key Points:
- Performance-critical paths.
- Large datasets.
- Write-heavy applications.
- Simple references.
- Use `$lookup` or manual lookups.

## Interview Tip:
"Avoid `populate()` for performance-critical paths â€” use `$lookup` or manual lookups."

---

## Question 115: How do you reduce over-fetching of data?

## Answer:
```javascript
// Use select to limit fields
const users = await User.find().select("name email");

// Use lean for plain objects
const users = await User.find().select("name email").lean();

// Use projection
const users = await User.find({}, { name: 1, email: 1 });
```

## Key Points:
- `select()` for specific fields.
- `lean()` for plain objects.
- Projection for minimal data.
- Avoid `find()` without selection.
- Reduce data transfer.

## Interview Tip:
"`select()` and `lean()` together minimize data transfer."

---

## Question 116: What is query projection?

## Answer:
Projection specifies which fields to include or exclude in query results.

```javascript
// Include only name and email
const users = await User.find({}, { name: 1, email: 1 });

// Exclude password
const users = await User.find({}, { password: 0 });

// Using select()
const users = await User.find().select("name email");
```

## Key Points:
- `{ field: 1 }` to include.
- `{ field: 0 }` to exclude.
- `select()` as alternative.
- Reduces data transfer.
- Improves performance.

## Interview Tip:
"Projection is the same as `select()` â€” specify which fields to return."

---

## Question 117: How do indexes improve Mongoose performance?

## Answer:
Indexes speed up queries by allowing MongoDB to find documents without scanning the entire collection.

```javascript
userSchema.index({ email: 1 }); // Single index
userSchema.index({ name: 1, role: 1 }); // Compound index
```

Without indexes, MongoDB does a collection scan (slow on large collections).

## Key Points:
- Speed up queries.
- Avoid collection scans.
- Defined in schema.
- Trade-off: slower writes.
- Essential for performance.

## Interview Tip:
"Indexes are the most important optimization â€” most slow queries are missing an index."

---

## Question 118: How do you optimize write-heavy applications?

## Answer:
1. **Use `insertMany()`**: Bulk inserts.
2. **Use `updateMany()`**: Bulk updates.
3. **Reduce indexes**: Each index slows writes.
4. **Use transactions sparingly**: They add overhead.
5. **Batch operations**: Group writes together.
6. **Use write concerns**: Control durability.

## Key Points:
- Bulk operations.
- Reduce indexes.
- Minimize transactions.
- Batch writes.
- Write concerns.

## Interview Tip:
"Bulk operations and fewer indexes are the keys to write performance."

---

## Question 119: How do you optimize read-heavy applications?

## Answer:
1. **Add indexes**: On frequently queried fields.
2. **Use `lean()`**: For plain objects.
3. **Use `select()`**: Limit fields.
4. **Cache results**: Use Redis or in-memory cache.
5. **Use read replicas**: Distribute read load.
6. **Use `populate()` with `select`**: Limit populated fields.

## Key Points:
- Indexes for speed.
- `lean()` for performance.
- `select()` for minimal data.
- Caching.
- Read replicas.
- Limited population.

## Interview Tip:
"Indexes, `lean()`, and caching are the big three for read performance."

---

## Question 120: What Mongoose performance best practices do you follow?

## Answer:
1. **Use `lean()`**: For read-only queries.
2. **Add indexes**: On frequently queried fields.
3. **Use `select()`**: Limit returned fields.
4. **Avoid N+1**: Use `populate()` instead of loops.
5. **Use cursor pagination**: For large datasets.
6. **Batch operations**: Use `insertMany()`, `updateMany()`.
7. **Profile queries**: Use `explain()`.
8. **Cache frequently accessed data**: Redis or in-memory.

## Key Points:
- `lean()` for performance.
- Indexes for speed.
- `select()` for minimal data.
- Avoid N+1.
- Cursor pagination.
- Batch operations.
- Profile queries.
- Cache data.

## Interview Tip:
"`lean()`, indexes, and avoiding N+1 â€” the performance trifecta."

---

## Part 13 (121â€“130): Advanced Features

---

## Question 121: What are discriminators in Mongoose?

## Answer:
Discriminators allow you to have different schemas for documents in the same collection, based on a type field.

```javascript
const eventSchema = new mongoose.Schema({ message: String }, { discriminatorKey: "kind" });
const Event = mongoose.model("Event", eventSchema);

// Click event
Event.discriminator("Click", new mongoose.Schema({ url: String }));

// Purchase event
Event.discriminator("Purchase", new mongoose.Schema({ amount: Number }));
```

## Key Points:
- Different schemas in same collection.
- `discriminatorKey` identifies the type.
- Like inheritance in OOP.
- Useful for event systems.
- Query by type.

## Interview Tip:
"Discriminators are like inheritance â€” different schemas in the same collection."

---

## Question 122: When should you use discriminators?

## Answer:
- **Event systems**: Different event types.
- **Product types**: Different product categories.
- **Notification types**: Different notification formats.
- **Log entries**: Different log types.
- **Polymorphic data**: Same collection, different structures.

## Key Points:
- Event systems.
- Product categories.
- Notification types.
- Log entries.
- Polymorphic data.

## Interview Tip:
"Discriminators are for polymorphic data â€” same collection, different structures."

---

## Question 123: What are schema plugins?

## Answer:
Schema plugins add reusable functionality to schemas.

```javascript
function timestampPlugin(schema) {
  schema.add({ createdAt: Date, updatedAt: Date });
  schema.pre("save", function() {
    this.updatedAt = new Date();
  });
}

userSchema.plugin(timestampPlugin);
postSchema.plugin(timestampPlugin);
```

## Key Points:
- Reusable schema extensions.
- Add fields, methods, or middleware.
- Called with `schema.plugin()`.
- Share across schemas.
- Third-party plugins available.

## Interview Tip:
"Plugins are reusable schema extensions â€” great for cross-cutting concerns."

---

## Question 124: How do you create a custom Mongoose plugin?

## Answer:
```javascript
function softDeletePlugin(schema) {
  schema.add({ isDeleted: { type: Boolean, default: false } });
  
  schema.methods.softDelete = function() {
    this.isDeleted = true;
    return this.save();
  };
  
  schema.pre("find", function() {
    this.where({ isDeleted: false });
  });
}

module.exports = softDeletePlugin;

// Usage
userSchema.plugin(softDeletePlugin);
```

## Key Points:
- Function that receives schema.
- Add fields, methods, or middleware.
- Export the function.
- Use with `schema.plugin()`.
- Share across projects.

## Interview Tip:
"A plugin is just a function that receives the schema â€” add whatever you need."

---

## Question 125: What are query helpers?

## Answer:
Query helpers add custom methods to the query prototype.

```javascript
userSchema.query.byEmail = function(email) {
  return this.where({ email });
};

userSchema.query.active = function() {
  return this.where({ isActive: true });
};

// Usage
const users = await User.find().byEmail("alice@example.com").active();
```

## Key Points:
- Custom methods on query prototype.
- Chainable.
- `this` refers to the query.
- Keep queries DRY.
- Useful for common patterns.

## Interview Tip:
"Query helpers keep your queries DRY â€” define common patterns once."

---

## Question 126: What are aggregation pipelines in Mongoose?

## Answer:
Aggregation pipelines process documents through a series of stages.

```javascript
const results = await User.aggregate([
  { $match: { role: "user" } },
  { $group: { _id: "$department", count: { $sum: 1 } } },
  { $sort: { count: -1 } }
]);
```

## Key Points:
- Series of processing stages.
- `$match`, `$group`, `$sort`, `$project`, etc.
- Powerful data transformation.
- Returns plain objects.
- Similar to SQL GROUP BY.

## Interview Tip:
"Aggregation pipelines are MongoDB's equivalent of SQL's GROUP BY and JOIN."

---

## Question 127: How do you use the aggregation framework through Mongoose?

## Answer:
```javascript
const results = await User.aggregate([
  { $match: { isActive: true } },
  { $lookup: {
      from: "posts",
      localField: "_id",
      foreignField: "author",
      as: "posts"
  }},
  { $unwind: "$posts" },
  { $group: {
      _id: "$_id",
      name: { $first: "$name" },
      postCount: { $sum: 1 }
  }}
]);
```

## Key Points:
- `Model.aggregate()` method.
- Array of pipeline stages.
- `$lookup` for joins.
- `$match`, `$group`, `$sort` for processing.
- Returns plain objects.

## Interview Tip:
"`Model.aggregate()` takes an array of stages â€” process documents step by step."

---

## Question 128: What is optimistic concurrency control?

## Answer:
Optimistic concurrency uses a version field to detect conflicts. It assumes conflicts are rare.

```javascript
const userSchema = new mongoose.Schema({
  name: String,
  versionKey: "__v"  // Default
});

// Read with version
const user = await User.findById(id);

// Update with version check
await User.updateOne(
  { _id: id, __v: user.__v },
  { name: "Alice", $inc: { __v: 1 } }
);
// If rows affected = 0, conflict occurred
```

## Key Points:
- Version field for conflict detection.
- Check version at update time.
- Retry on conflict.
- No locking.
- Assume conflicts are rare.

## Interview Tip:
"Optimistic concurrency checks the version â€” if it changed, retry the operation."

---

## Question 129: How do you implement soft deletes?

## Answer:
```javascript
const userSchema = new mongoose.Schema({
  name: String,
  isDeleted: { type: Boolean, default: false },
  deletedAt: { type: Date }
});

// Soft delete method
userSchema.methods.softDelete = function() {
  this.isDeleted = true;
  this.deletedAt = new Date();
  return this.save();
};

// Auto-filter deleted documents
userSchema.pre("find", function() {
  this.where({ isDeleted: false });
});
```

## Key Points:
- `isDeleted` or `deletedAt` field.
- Custom `softDelete()` method.
- Pre-find middleware to filter.
- Data preserved for recovery.
- Partial index for performance.

## Interview Tip:
"Soft deletes preserve data â€” add a pre-find middleware to filter automatically."

---

## Question 130: How do you implement multi-tenancy in Mongoose?

## Answer:
```javascript
// Add tenantId to every schema
const userSchema = new mongoose.Schema({
  tenantId: { type: mongoose.Schema.Types.ObjectId, required: true },
  name: String
});

// Middleware to filter by tenant
userSchema.pre("find", function() {
  const tenantId = this.getOptions().tenantId;
  if (tenantId) this.where({ tenantId });
});

// Usage
const users = await User.find().setOptions({ tenantId: currentTenant });
```

## Key Points:
- `tenantId` on every document.
- Middleware for automatic filtering.
- `setOptions()` for tenant context.
- Index `tenantId` for performance.
- Row-level security.

## Interview Tip:
"Multi-tenancy needs `tenantId` on every document and automatic filtering via middleware."

---

## Part 14 (131â€“140): Testing & Production

---

## Question 131: How do you test Mongoose models?

## Answer:
```javascript
beforeAll(async () => {
  await mongoose.connect("mongodb://localhost/test_db");
});

afterEach(async () => {
  await User.deleteMany();
});

afterAll(async () => {
  await mongoose.connection.close();
});

it("creates a user", async () => {
  const user = await User.create({ name: "Test", email: "test@example.com" });
  expect(user.name).toBe("Test");
});
```

## Key Points:
- Separate test database.
- Clear data after each test.
- Close connection after tests.
- Test validation and middleware.
- Use factories for test data.

## Interview Tip:
"Test with a real database â€” it catches integration issues."

---

## Question 132: How do you mock Mongoose in unit tests?

## Answer:
```javascript
// Using jest-mock
jest.mock("mongoose", () => {
  const mockModel = {
    find: jest.fn(),
    findOne: jest.fn(),
    create: jest.fn()
  };
  return { model: jest.fn(() => mockModel) };
});
```

Or use `mongodb-memory-server` for in-memory testing.

## Key Points:
- Mock the model methods.
- `mongodb-memory-server` for in-memory testing.
- Mock for unit tests.
- Real database for integration tests.

## Interview Tip:
"`mongodb-memory-server` is the best way to test Mongoose â€” fast and isolated."

---

## Question 133: How do you test transactions?

## Answer:
```javascript
it("transfers money atomically", async () => {
  const session = await mongoose.startSession();
  session.startTransaction();

  try {
    await Account.updateOne({ _id: 1 }, { $inc: { balance: -100 } }, { session });
    await Account.updateOne({ _id: 2 }, { $inc: { balance: 100 } }, { session });
    await session.commitTransaction();
  } catch (error) {
    await session.abortTransaction();
    throw error;
  } finally {
    session.endSession();
  }

  const account1 = await Account.findById(1);
  expect(account1.balance).toBe(900);
});
```

## Key Points:
- Test commit and rollback.
- Verify atomicity.
- Test error scenarios.
- Use real or in-memory database.

## Interview Tip:
"Test both success and failure paths â€” verify rollback works correctly."

---

## Question 134: How do you seed test databases?

## Answer:
```javascript
beforeAll(async () => {
  await User.create([
    { name: "Alice", email: "alice@test.com" },
    { name: "Bob", email: "bob@test.com" }
  ]);
});

afterEach(async () => {
  await User.deleteMany();
});
```

Use factories for complex test data.

## Key Points:
- Seed before tests.
- Clear after each test.
- Use factories for consistency.
- Keep test data minimal.

## Interview Tip:
"Seed minimal test data â€” just enough to test your scenarios."

---

## Question 135: How do you manage environment-specific MongoDB connections?

## Answer:
```javascript
// config.js
const connections = {
  development: "mongodb://localhost:27017/myapp_dev",
  test: "mongodb://localhost:27017/myapp_test",
  production: process.env.MONGODB_URI
};

module.exports = connections[process.env.NODE_ENV];
```

## Key Points:
- Different URIs per environment.
- Environment variables for production.
- Test database separate from dev.
- Configuration module.

## Interview Tip:
"Separate test, dev, and production databases â€” different URIs per environment."

---

## Question 136: How do you deploy a Mongoose application?

## Answer:
1. **Environment variables**: Secure `MONGODB_URI`.
2. **Connection pooling**: Configure pool size.
3. **Indexes**: Ensure indexes are created.
4. **Migrations**: Run any schema changes.
5. **Monitoring**: Track connection and query performance.

## Key Points:
- Environment variables.
- Connection pooling.
- Index creation.
- Migrations.
- Monitoring.

## Interview Tip:
"Deploy with environment variables, connection pooling, and monitoring."

---

## Question 137: How do you monitor Mongoose performance in production?

## Answer:
```javascript
mongoose.set("debug", (collectionName, method, query, doc) => {
  console.log(`${collectionName}.${method}`, JSON.stringify(query));
});

// Monitor slow queries
mongoose.set("debug", function(collectionName, method, query, doc, options) {
  const start = Date.now();
  this.on("end", () => {
    const duration = Date.now() - start;
    if (duration > 100) console.warn(`Slow query: ${duration}ms`);
  });
});
```

## Key Points:
- Enable debug logging.
- Monitor query duration.
- Use MongoDB Atlas monitoring.
- Track connection status.
- Log slow queries.

## Interview Tip:
"Enable debug mode and monitor slow queries in production."

---

## Question 138: How do you handle database migrations in MongoDB/Mongoose projects?

## Answer:
MongoDB doesn't have built-in migrations. Options:
- **Migrate-mongo**: Popular migration tool.
- **Custom scripts**: Write migration scripts.
- **MongoDB Atlas**: Built-in migration tools.

```javascript
// migrate-mongo
exports.up = async function(db) {
  await db.collection("users").updateMany({}, { $set: { role: "user" } });
};

exports.down = async function(db) {
  await db.collection("users").updateMany({}, { $unset: { role: "" } });
};
```

## Key Points:
- No built-in migrations.
- Use migrate-mongo or custom scripts.
- Version-controlled migrations.
- Up and down functions.
- Test migrations thoroughly.

## Interview Tip:
"MongoDB doesn't have built-in migrations â€” use migrate-mongo or custom scripts."

---

## Question 139: How do you debug production database issues?

## Answer:
1. **Check logs**: Application and MongoDB logs.
2. **Monitor connections**: Check connection pool.
3. **Profile slow queries**: Use `explain()`.
4. **Check indexes**: Verify indexes exist.
5. **Monitor resources**: CPU, memory, disk.
6. **Check replication**: If using replica set.

## Key Points:
- Application and MongoDB logs.
- Connection monitoring.
- Query profiling.
- Index verification.
- Resource monitoring.

## Interview Tip:
"Start with logs and connection status â€” most issues are visible there."

---

## Question 140: What production best practices do you always follow?

## Answer:
1. **Environment variables**: Secure credentials.
2. **Connection pooling**: Configure appropriately.
3. **Indexes**: Ensure performance.
4. **Error handling**: Graceful error responses.
5. **Logging**: Monitor queries and errors.
6. **Testing**: Unit and integration tests.
7. **Monitoring**: Track performance metrics.

## Key Points:
- Environment variables.
- Connection pooling.
- Indexes.
- Error handling.
- Logging.
- Testing.
- Monitoring.

## Interview Tip:
"Environment variables, connection pooling, indexes, and monitoring â€” the production essentials."

---

## Part 15 (141â€“150): Senior Real-World Interview Questions

---

## Question 141: Describe the largest Mongoose project you've worked on.

## Answer:
Pick a real project and describe:
- **Scale**: Documents, collections, queries per second.
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

## Question 142: What was the most difficult Mongoose issue you've solved?

## Answer:
Describe:
1. **Symptoms**: What was happening.
2. **Investigation**: How you diagnosed it.
3. **Root cause**: What was actually wrong.
4. **Fix**: How you resolved it.
5. **Lesson**: What you learned.

## Key Points:
- Symptoms, investigation, root cause, fix, lesson.
- Systematic debugging approach.
- Tools used.
- What you learned.

## Interview Tip:
"Interviewers want to see your debugging process, not just the fix."

---

## Question 143: How do you debug slow Mongoose queries?

## Answer:
1. **Enable debug mode**: See actual queries.
2. **Use `explain()`**: Database-level analysis.
3. **Check indexes**: Are queried fields indexed?
4. **Check `populate()`**: Is it causing N+1?
5. **Check `lean()`**: Are you using it for reads?
6. **Check `select()`**: Are you over-fetching?

## Key Points:
- Debug mode for query visibility.
- `explain()` for analysis.
- Index verification.
- N+1 check with `populate()`.
- `lean()` for performance.
- `select()` for minimal data.

## Interview Tip:
"Enable debug mode and use `explain()` â€” they show you exactly what's slow."

---

## Question 144: How do you review Mongoose schema changes in a pull request?

## Answer:
Check for:
1. **Missing indexes**: Are new queried fields indexed?
2. **Validation changes**: Are they backward compatible?
3. **Type choices**: Right types for the data?
4. **Required fields**: Will they break existing documents?
5. **Middleware changes**: Do they affect performance?
6. **Naming conventions**: Consistent naming?

## Key Points:
- Indexes on new queried fields.
- Backward-compatible validation.
- Appropriate data types.
- Required fields impact.
- Middleware performance.
- Consistent naming.

## Interview Tip:
"Review schema changes like code â€” check indexes, types, validation, and naming."

---

## Question 145: What schema design conventions do you follow?

## Answer:
- **PascalCase**: Model names (`User`, `OrderItem`).
- **camelCase**: Field names (`firstName`, `createdAt`).
- **Timestamps**: `timestamps: true` on every model.
- **Indexes**: On frequently queried fields.
- **Validation**: Required, enum, min/max.
- **Select**: `select: false` for sensitive fields.
- **Virtuals**: For computed fields.

## Key Points:
- PascalCase for models.
- camelCase for fields.
- Timestamps on every model.
- Indexes for performance.
- Validation for integrity.
- Select for sensitive data.
- Virtuals for computed fields.

## Interview Tip:
"Timestamps, validation, indexes, and select:false â€” the schema conventions quartet."

---

## Question 146: How would you migrate a native MongoDB project to Mongoose?

## Answer:
1. **Install Mongoose**: `npm install mongoose`.
2. **Define schemas**: Match existing document structure.
3. **Create models**: From schemas.
4. **Replace queries**: Gradually replace native queries.
5. **Add validation**: To schemas.
6. **Test thoroughly**: Verify all operations work.

## Key Points:
- Install Mongoose.
- Define schemas matching existing structure.
- Create models.
- Replace queries gradually.
- Add validation.
- Test thoroughly.

## Interview Tip:
"Introspect your existing documents, define matching schemas, then replace queries gradually."

---

## Question 147: How would you design a scalable Mongoose architecture for a SaaS application?

## Answer:
```javascript
// Multi-tenant schema
const userSchema = new mongoose.Schema({
  tenantId: { type: mongoose.Schema.Types.ObjectId, required: true },
  name: String,
  email: String
});

// Index for tenant queries
userSchema.index({ tenantId: 1, email: 1 });

// Middleware for automatic filtering
userSchema.pre("find", function() {
  const tenantId = this.getOptions().tenantId;
  if (tenantId) this.where({ tenantId });
});
```

- `tenantId` on every document.
- Indexes for tenant queries.
- Middleware for automatic filtering.
- Connection pooling.
- Read replicas for scaling.

## Key Points:
- `tenantId` on every document.
- Indexes for performance.
- Automatic filtering middleware.
- Connection pooling.
- Read replicas.

## Interview Tip:
"Multi-tenancy needs `tenantId` on every document and automatic filtering via middleware."

---

## Question 148: What Mongoose features do you use most frequently in production?

## Answer:
- **CRUD operations**: `create`, `find`, `findOne`, `update`, `delete`.
- **`populate()`**: For relationships.
- **`lean()`**: For performance.
- **`select()`**: To limit fields.
- **Validation**: Built-in and custom.
- **Middleware**: Pre/post hooks.
- **Indexes**: For performance.
- **`timestamps: true`**: For auditing.

## Key Points:
- CRUD operations.
- `populate()` for relationships.
- `lean()` for performance.
- `select()` for minimal data.
- Validation and middleware.
- Indexes.
- Timestamps.

## Interview Tip:
"CRUD, populate, lean, select, validation, middleware, indexes, and timestamps â€” the essentials."

---

## Question 149: If you were starting a new MERN project today, how would you organize your Mongoose models and database layer?

## Answer:
```
src/
  models/
    user.model.js
    post.model.js
  services/
    user.service.js
    post.service.js
  config/
    db.js
  middleware/
    tenant.js
```

- Models in `models/` folder.
- Business logic in `services/`.
- Database connection in `config/`.
- Middleware for cross-cutting concerns.
- Single connection instance.

## Key Points:
- Models in dedicated folder.
- Services for business logic.
- Config for database connection.
- Middleware for cross-cutting concerns.
- Single connection instance.

## Interview Tip:
"Models for schema, services for business logic, config for connection â€” clean separation."

---

## Question 150: In your opinion, what separates a junior, mid-level, and senior Mongoose developer?

## Answer:
- **Junior**: Knows basic CRUD. Can create models and run queries.
- **Mid-level**: Understands `populate()`, middleware, and performance. Can design schemas and optimize queries.
- **Senior**: Designs scalable schemas, handles production issues, mentors others. Understands trade-offs, transactions, and architecture.

The biggest differentiator: a senior developer understands WHY, not just WHAT.

## Key Points:
- Junior: basic CRUD, guided work.
- Mid-level: populate, middleware, schema design.
- Senior: architecture, production, mentoring.
- Senior understands trade-offs.
- Senior thinks about scalability and performance.

## Interview Tip:
"The best answer shows self-awareness. Pick your level and explain what you're doing to grow."

---

# End of Mongoose Interview Questions & Answers
