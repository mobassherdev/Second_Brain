# TypeScript Interview Questions & Answers (1–200)

---

## Part 1 (1–25): Fundamentals

---

## Question 1: What is TypeScript?

## Answer:
TypeScript is JavaScript with types. It's a superset of JavaScript, which means any valid JavaScript code is also valid TypeScript. You add type annotations on top, and then the TypeScript compiler converts it to plain JavaScript before running in the browser or Node.js.

I use it in every project now because it catches bugs at compile time rather than at runtime, which saves a lot of debugging time.

## Key Points:
- TypeScript is a superset of JavaScript developed by Microsoft.
- It adds static typing to JavaScript.
- TypeScript compiles down to plain JavaScript.
- It works with any JavaScript runtime (browser, Node.js, Deno).

## Interview Tip:
Don't just say "TypeScript is typed JavaScript." Mention that it catches errors early, improves IDE support, and is especially useful in large codebases and team projects.

---

## Question 2: Why should you use TypeScript instead of JavaScript?

## Answer:
The main reason is catching bugs before they reach production. In JavaScript, you can pass a string where a number is expected and it won't error until runtime. TypeScript catches that at compile time.

Also, the developer experience is much better. Your IDE gives you autocomplete, inline documentation, and immediate error highlighting. For team projects, it acts like self-documenting code.

## Key Points:
- Catches type-related bugs at compile time, not runtime.
- Better IDE support with autocomplete and IntelliSense.
- Makes code easier to refactor and maintain.
- Especially valuable in large teams and large codebases.

## Interview Tip:
Mention real benefits like refactoring safety and team collaboration. Avoid saying TypeScript is just for large projects — it helps even in small projects.

---

## Question 3: What are the advantages of TypeScript?

## Answer:
- **Early error detection**: Type errors are caught before running the code.
- **Better IDE support**: Autocomplete, go-to-definition, and refactoring tools work better.
- **Self-documenting code**: Types tell you exactly what shape a function expects.
- **Safer refactoring**: You can rename a property and TypeScript shows every place that breaks.
- **Generics and utility types**: Reusable type logic that JavaScript simply can't do.

## Key Points:
- Static typing reduces runtime bugs significantly.
- Works with existing JavaScript libraries via `@types` packages.
- Enables better tooling and editor integration.
- Scales well for large applications and teams.

## Interview Tip:
Give concrete examples. Say something like "When I renamed an API field in a Next.js project, TypeScript immediately showed me 15 places I needed to update."

---

## Question 4: What are the disadvantages of TypeScript?

## Answer:
- **Extra compilation step**: TypeScript needs to be compiled before running.
- **Learning curve**: Generics, utility types, and complex types take time to master.
- **More verbose code**: Sometimes you write extra type annotations that feel unnecessary.
- **Third-party library types**: Not all libraries have great type definitions.
- **Setup overhead**: Configuring `tsconfig.json` properly takes effort.

## Key Points:
- Adds build complexity to your project.
- Complex generic types can hurt readability.
- `any` overuse defeats the purpose entirely.
- Some JavaScript-only packages need separate `@types` packages.

## Interview Tip:
Be honest about the trade-offs. Saying "TypeScript has no downsides" is a red flag. Mention that the benefits outweigh the costs in most production scenarios.

---

## Question 5: What is static typing?

## Answer:
Static typing means variable types are checked at compile time, before the code ever runs. You declare what type a variable is, and the compiler enforces it throughout the code.

In TypeScript: `let age: number = 25;` — if you try to assign a string to `age`, TypeScript throws an error immediately.

## Key Points:
- Types are checked before runtime.
- Reduces type-related runtime errors.
- Makes code more predictable and self-documenting.
- Contrast: JavaScript is dynamically typed — types are checked at runtime.

## Interview Tip:
Compare with dynamic typing briefly. Show you understand the trade-off between catching errors early vs. writing code faster.

---

## Question 6: What is dynamic typing?

## Answer:
Dynamic typing means the type of a variable is determined at runtime, not at compile time. JavaScript is dynamically typed — you can assign any value to any variable and it won't complain until something actually breaks.

```js
let value = "hello";
value = 42; // No error in JavaScript
```

## Key Points:
- Variable types are resolved at runtime.
- More flexible but more prone to bugs.
- JavaScript is dynamically typed.
- Python and Ruby are also dynamically typed languages.

## Interview Tip:
Don't say dynamic typing is bad. It offers flexibility for rapid prototyping. TypeScript gives you the best of both worlds with optional type annotations.

---

## Question 7: What is a superset language?

## Answer:
A superset language includes all features of the original language and adds more on top. TypeScript is a superset of JavaScript, meaning every JavaScript file is valid TypeScript. You can rename a `.js` file to `.ts` and it still works.

This design makes TypeScript easy to adopt incrementally — you don't have to rewrite everything at once.

## Key Points:
- All valid JavaScript is valid TypeScript.
- TypeScript adds types, interfaces, generics, decorators, etc.
- You can adopt TypeScript gradually in existing JS projects.
- The TypeScript compiler removes type annotations when compiling to JS.

## Interview Tip:
This concept is important for explaining why TypeScript has no runtime overhead — all types are erased at compile time.

---

## Question 8: How does TypeScript work?

## Answer:
You write TypeScript code, and the TypeScript compiler (`tsc`) reads it, checks types, and compiles it to JavaScript. That JavaScript is what actually runs in the browser or Node.js. TypeScript itself never runs anywhere — it's a development-time tool.

The flow is: Write `.ts` → Compile with `tsc` → Get `.js` → Run in browser/Node.

## Key Points:
- TypeScript is a compile-time tool — it produces JavaScript.
- The `tsc` compiler does type checking and code transformation.
- Bundlers like Webpack/Vite can integrate this compilation step.
- In Next.js and Vite, TypeScript is compiled automatically.

## Interview Tip:
Mention that in modern projects, tools like Vite, Next.js, or ts-node handle compilation automatically. You rarely run `tsc` manually in production workflows.

---

## Question 9: Can browsers execute TypeScript directly?

## Answer:
No. Browsers only understand JavaScript. TypeScript must be compiled to JavaScript first. The browser never sees the TypeScript code — it only runs the compiled JavaScript output.

In development, tools like ts-node (for Node.js) or Vite handle this compilation transparently.

## Key Points:
- Browsers run JavaScript, not TypeScript.
- TypeScript is compiled away before deployment.
- Type information is completely removed in the output JS.
- Deno is one runtime that can run TypeScript natively (with its own handling).

## Interview Tip:
You can mention that Deno natively supports TypeScript, but standard browsers and Node.js require compilation. This shows broader knowledge.

---

## Question 10: How do you compile TypeScript?

## Answer:
You use the TypeScript compiler: `tsc`. Running `tsc` in your project reads `tsconfig.json` and compiles all TypeScript files. You can also compile a single file with `tsc filename.ts`.

In modern projects, compilation happens automatically — Next.js, Vite, and ts-node all handle it behind the scenes.

```bash
tsc                  # compile using tsconfig.json
tsc index.ts         # compile single file
tsc --watch          # watch mode for auto recompilation
```

## Key Points:
- `tsc` is the official TypeScript compiler.
- `tsconfig.json` controls compilation settings.
- `--watch` mode recompiles on file changes.
- Most modern frameworks handle TypeScript compilation automatically.

## Interview Tip:
Mention `tsc --noEmit` for type-checking without producing output files — very common in CI/CD pipelines.

---

## Question 11: What is the TypeScript compiler (`tsc`)?

## Answer:
`tsc` is the official command-line tool that compiles TypeScript to JavaScript. It reads your `.ts` files, validates types, and outputs `.js` files. It also reads `tsconfig.json` for project-wide settings.

Install it globally: `npm install -g typescript`, then run `tsc`.

## Key Points:
- `tsc` stands for TypeScript Compiler.
- Installed via npm as part of the `typescript` package.
- Reads `tsconfig.json` for configuration.
- Can also be used programmatically via the TypeScript API.

## Interview Tip:
Mention that in real projects you usually don't run `tsc` directly in development. You use ts-node, Vite, or Next.js. But `tsc --noEmit` is great for CI type-checking.

---

## Question 12: What is `tsconfig.json`?

## Answer:
`tsconfig.json` is the configuration file for the TypeScript compiler. It tells TypeScript which files to compile, how strict to be, what JavaScript version to target, and much more.

```json
{
  "compilerOptions": {
    "target": "ES2020",
    "strict": true,
    "outDir": "./dist",
    "rootDir": "./src"
  }
}
```

## Key Points:
- Controls all TypeScript compiler behavior.
- `strict: true` enables strict type checking.
- `target` sets the JavaScript version output.
- `include`/`exclude` control which files are compiled.

## Interview Tip:
Be ready to explain key options like `strict`, `target`, `module`, `paths`, and `baseUrl`. These come up often in senior interviews.

---

## Question 13: What is the purpose of `strict` mode?

## Answer:
`strict: true` in `tsconfig.json` enables a bundle of strict type-checking rules. It's like turning on all the safety features at once. Without it, TypeScript is much more lenient and lets many potential bugs through.

It enables: `strictNullChecks`, `noImplicitAny`, `strictFunctionTypes`, and several others.

## Key Points:
- `strict: true` is the recommended setting for production projects.
- Prevents implicit `any` types.
- Makes `null` and `undefined` handling explicit.
- Enables stricter function type checking.

## Interview Tip:
Always say you use `strict: true` in new projects. Not using it is a common mistake — you lose most of TypeScript's safety benefits.

---

## Question 14: What are primitive types in TypeScript?

## Answer:
Primitive types are the basic building blocks: `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, and `bigint`. They match JavaScript's primitive values directly.

```ts
let name: string = "John";
let age: number = 30;
let isActive: boolean = true;
```

## Key Points:
- TypeScript has `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, `bigint`.
- These match JavaScript's built-in primitive types.
- Type annotations are usually optional due to type inference.
- `null` and `undefined` are their own types in strict mode.

## Interview Tip:
Don't confuse `Number` (object wrapper) with `number` (primitive type). Always use lowercase in TypeScript type annotations.

---

## Question 15: What is type inference?

## Answer:
Type inference is when TypeScript automatically figures out the type of a variable without you explicitly writing it. If you write `let count = 0`, TypeScript infers that `count` is a `number` — you don't need to write `let count: number = 0`.

I rely on this heavily to keep code clean. I only add explicit types when TypeScript can't infer them correctly.

## Key Points:
- TypeScript infers types from initial values.
- Works for variables, function return types, and more.
- Reduces annotation verbosity without losing type safety.
- Use explicit types when inference is ambiguous or wrong.

## Interview Tip:
Show you understand when to let inference work and when to be explicit. Over-annotating everything is a common beginner mistake.

---

## Question 16: What is type annotation?

## Answer:
Type annotation is when you explicitly tell TypeScript what type a variable, parameter, or return value should be. You use a colon followed by the type.

```ts
let username: string = "Alice";
function greet(name: string): string {
  return `Hello, ${name}`;
}
```

## Key Points:
- Syntax: `variableName: type`
- Used for variables, function parameters, and return types.
- Overrides or clarifies TypeScript's inference.
- Necessary when TypeScript can't infer the type correctly.

## Interview Tip:
Mention that you don't annotate everything — only where inference fails or where explicit types improve readability. This shows mature TypeScript usage.

---

## Question 17: What is the `any` type?

## Answer:
`any` completely disables type checking for that variable. It can hold any value and TypeScript won't complain about anything you do with it. It's essentially an escape hatch back to plain JavaScript.

```ts
let data: any = "hello";
data = 42;          // OK
data.whatever();    // No error — dangerous!
```

## Key Points:
- `any` bypasses all type checking.
- Useful as a temporary escape hatch during migration.
- Overusing `any` defeats the purpose of TypeScript.
- Should be avoided in production code.

## Interview Tip:
Say you avoid `any` and use `unknown` instead when the type is truly unknown. This is a common differentiator between junior and senior TypeScript developers.

---

## Question 18: Why is `any` considered dangerous?

## Answer:
Because it silently disables all type checking. If you mark something as `any`, TypeScript stops checking that value — and errors that TypeScript would normally catch can sneak through to runtime.

It also spreads — if you pass an `any` value into a typed function, it can infect the types of other values.

## Key Points:
- Removes all type safety for that value.
- Errors that TypeScript would catch instead appear at runtime.
- `any` can spread to other variables silently.
- Use `unknown` instead — it's safe because you must check the type before using it.

## Interview Tip:
Mention `noImplicitAny` in `tsconfig.json`. It forces you to be explicit — TypeScript won't silently infer `any`. This is a good practice to mention.

---

## Question 19: What is the `unknown` type?

## Answer:
`unknown` is like a safe version of `any`. It means "I don't know the type yet, but I'm going to check before I use it." Unlike `any`, TypeScript forces you to do a type check before performing operations on an `unknown` value.

```ts
let input: unknown = getUserInput();
if (typeof input === "string") {
  console.log(input.toUpperCase()); // Safe!
}
```

## Key Points:
- `unknown` requires a type check before use.
- Much safer than `any` for truly unknown values.
- Common for API responses, user input, and `try/catch` errors.
- TypeScript 4.0+ types `catch` error variables as `unknown` by default.

## Interview Tip:
This is a great answer differentiator. Show you prefer `unknown` over `any` and explain why. It demonstrates real TypeScript maturity.

---

## Question 20: What is the difference between `any` and `unknown`?

## Answer:
Both accept any value, but `unknown` is the safe version. With `any`, you can do anything without checks. With `unknown`, TypeScript forces you to narrow the type before using it.

```ts
let a: any = "hello";
a.toUpperCase();     // OK — no check needed

let b: unknown = "hello";
b.toUpperCase();     // Error — must check first
if (typeof b === "string") b.toUpperCase(); // OK
```

## Key Points:
- `any`: no type checking enforced — use anything freely.
- `unknown`: type checking required — must narrow before use.
- Prefer `unknown` for values from external sources.
- `any` is for quick fixes or migration; `unknown` is for long-term safety.

## Interview Tip:
This is a very common interview question. Give the code example above — it clearly shows the difference in 5 lines.

---

## Question 21: What is the `never` type?

## Answer:
`never` represents values that never exist — functions that always throw, or infinite loops that never return. It's also what you get in an exhaustive type check when all cases are handled.

```ts
function throwError(msg: string): never {
  throw new Error(msg);
}
```

## Key Points:
- Used for functions that never return (throw or infinite loop).
- Appears in exhaustive type checking with discriminated unions.
- TypeScript uses `never` internally for impossible types.
- A variable of type `never` can't be assigned any value.

## Interview Tip:
Mention `never` in the context of exhaustive switch statements. It's the right answer when an interviewer asks "how do you handle all cases of a union type."

---

## Question 22: What is the `void` type?

## Answer:
`void` means a function doesn't return a value. It's what you use for event handlers, side-effect functions, or any function that just does something but returns nothing.

```ts
function logMessage(msg: string): void {
  console.log(msg);
  // No return statement
}
```

## Key Points:
- Used as the return type of functions that return nothing.
- Similar to `undefined` but semantically different.
- A `void` function can technically return `undefined`.
- Arrow functions without `return` implicitly return `void`.

## Interview Tip:
The difference between `void` and `never`: `void` means the function completes but returns nothing. `never` means the function never completes at all.

---

## Question 23: What is the difference between `null` and `undefined`?

## Answer:
`undefined` means a variable was declared but no value was assigned. `null` is an explicit assignment meaning "no value." In TypeScript with strict mode, both are their own types and can't be assigned to other types without explicit handling.

```ts
let a: string | undefined; // declared, no value
let b: string | null = null; // intentionally empty
```

## Key Points:
- `undefined`: variable exists but has no value assigned.
- `null`: explicitly set to "no value."
- With `strictNullChecks`, they are not assignable to other types.
- Use `null` intentionally; `undefined` often appears automatically.

## Interview Tip:
Mention `strictNullChecks` and how it forces you to handle both `null` and `undefined` explicitly. This is key for writing safe TypeScript.

---

## Question 24: What is the `object` type?

## Answer:
`object` in TypeScript represents any non-primitive value — arrays, functions, objects, etc. It's quite broad and not very useful for precise typing. In practice, you'll use interfaces or type aliases for object shapes instead.

```ts
let obj: object = { name: "John" };
obj.name; // Error — TypeScript doesn't know the shape
```

## Key Points:
- `object` accepts any non-primitive value.
- Doesn't provide information about the object's shape.
- Use interfaces or type aliases for better typing.
- Rarely used in real code — mostly appears in library types.

## Interview Tip:
Explain why you'd use an interface or type alias over `object`. This shows you understand practical TypeScript over theoretical knowledge.

---

## Question 25: What is the difference between `Object`, `object`, and `{}`?

## Answer:
- `object` (lowercase): any non-primitive value. Excludes `string`, `number`, `boolean`, etc.
- `Object` (uppercase): represents the JavaScript `Object` prototype — includes primitives via autoboxing. Avoid it.
- `{}` (empty object): accepts any value except `null` and `undefined`. Very broad and usually not what you want.

In practice, avoid all three and use specific types or interfaces instead.

## Key Points:
- `object` = non-primitive values only.
- `Object` = almost everything (including primitives) — avoid using it.
- `{}` = everything except null/undefined — too broad.
- Use typed interfaces for real objects in code.

## Interview Tip:
This is a tricky question. Most candidates confuse these. Knowing the difference shows deep TypeScript knowledge. The key answer: use `object` sparingly, avoid `Object`, and never use `{}` as a catch-all type.

---

## Part 2 (26–50): Types

---

## Question 26: What are union types?

## Answer:
Union types let a variable hold more than one type. You use the `|` (pipe) operator. It's like saying "this can be a string OR a number."

```ts
function formatId(id: string | number): string {
  return id.toString();
}
```

I use this a lot for API responses where a field might come back as different types.

## Key Points:
- Union type: `TypeA | TypeB`
- The variable can be any one of the listed types.
- TypeScript narrows the type in conditionals.
- Very common with `string | null`, `string | undefined`.

## Interview Tip:
Always mention type narrowing with union types. Show how you'd use `typeof` or `instanceof` to handle each case safely.

---

## Question 27: What are intersection types?

## Answer:
Intersection types combine multiple types into one. A variable must satisfy ALL the combined types. You use the `&` operator.

```ts
type Admin = { adminLevel: number };
type User = { name: string; email: string };
type AdminUser = Admin & User;

const admin: AdminUser = { name: "Alice", email: "a@b.com", adminLevel: 2 };
```

## Key Points:
- Intersection type: `TypeA & TypeB`
- The result must have ALL properties of all types.
- Often used to merge interfaces or extend types.
- Contrast with union: union = "one of", intersection = "all of."

## Interview Tip:
Use the visual: union is OR, intersection is AND. This is a clean way to explain it to interviewers.

---

## Question 28: What are literal types?

## Answer:
Literal types restrict a variable to exact values rather than broad types. Instead of just saying `string`, you say it must be exactly "admin" or "user".

```ts
type Role = "admin" | "user" | "guest";
let role: Role = "admin"; // OK
role = "superuser"; // Error!
```

## Key Points:
- Restricts values to specific constants.
- Works with `string`, `number`, and `boolean` literals.
- Commonly used with union types for enums-like behavior.
- Preferred over regular `enum` by many TypeScript developers.

## Interview Tip:
Mention that literal types combined with union types are often better than enums — they're simpler, more tree-shakeable, and more flexible.

---

## Question 29: What are tuple types?

## Answer:
A tuple is a fixed-length array where each position has a specific type. Unlike regular arrays where all elements share a type, tuples allow different types at each index.

```ts
type Point = [number, number];
const p: Point = [10, 20];

type Entry = [string, number];
const e: Entry = ["age", 25];
```

## Key Points:
- Fixed length with specific types per index.
- TypeScript checks both position and type.
- Common for function return values and `useState` return in React.
- You can add labels for readability: `[x: number, y: number]`.

## Interview Tip:
Mention React's `useState` which returns a tuple `[value, setter]`. It's a real-world example every React developer can relate to.

---

## Question 30: What is a readonly tuple?

## Answer:
A readonly tuple prevents modification after creation. You add the `readonly` keyword before the tuple, and TypeScript won't allow methods that change the tuple like `push` or `pop`.

```ts
const coords: readonly [number, number] = [10, 20];
coords[0] = 5; // Error!
coords.push(30); // Error!
```

## Key Points:
- `readonly` prevents mutation of the tuple.
- TypeScript enforces this at compile time.
- Useful for coordinate pairs, config values, or fixed structures.
- Similar to `as const` for arrays.

## Interview Tip:
Explain why immutability matters — it prevents accidental mutations in complex codebases. Mention `as const` as an alternative for inferring readonly tuples.

---

## Question 31: What are enum types?

## Answer:
Enums let you define a set of named constants. They're useful when you have a fixed set of options like directions, statuses, or roles.

```ts
enum Status {
  Active = "ACTIVE",
  Inactive = "INACTIVE",
  Pending = "PENDING"
}
const s: Status = Status.Active;
```

## Key Points:
- Enums group related named constants.
- Numeric enums auto-increment by default.
- String enums are more readable and debuggable.
- `const enum` inlines values at compile time for performance.

## Interview Tip:
Be ready to say why many developers prefer union literal types over enums. Enums generate extra JavaScript code; literal unions don't.

---

## Question 32: What is the difference between numeric and string enums?

## Answer:
Numeric enums auto-assign numbers starting from 0. String enums require explicit string values for each member.

```ts
enum Direction { Up, Down, Left, Right } // 0, 1, 2, 3
enum Color { Red = "RED", Blue = "BLUE" } // string values
```

String enums are generally preferred because values are readable in logs, databases, and API responses.

## Key Points:
- Numeric enums auto-increment starting at 0.
- String enums need explicit values — more readable.
- Numeric enums support reverse mapping; string enums don't.
- String enums are safer for APIs and storage.

## Interview Tip:
Always recommend string enums in real projects. Numeric enums can lead to bugs if the order changes — a member added in the middle shifts all values.

---

## Question 33: Why do many developers avoid enums?

## Answer:
Enums generate actual JavaScript code at runtime, unlike most TypeScript features which are erased. They also have some quirks — numeric enums allow invalid values to be assigned, and they don't tree-shake well.

Many developers use union literal types instead because they produce no extra JS code and behave more predictably.

```ts
// Instead of enum:
type Status = "active" | "inactive" | "pending";
```

## Key Points:
- Enums generate runtime JavaScript code.
- Literal union types are zero-cost at runtime.
- Numeric enums can be unsafely assigned any number.
- `const enum` helps with performance but has its own issues.

## Interview Tip:
This is a great "senior-level" answer. Knowing the trade-offs of enums shows deep TypeScript experience. Recommend union literals for most use cases.

---

## Question 34: What is a const enum?

## Answer:
`const enum` is a performance optimization. Instead of generating a JavaScript object for the enum, the compiler inlines the actual values wherever the enum is used. The enum itself disappears from the output.

```ts
const enum Direction { Up = "UP", Down = "DOWN" }
const d = Direction.Up; // Compiled as: const d = "UP"
```

## Key Points:
- Inlined at compile time — no runtime object generated.
- Smaller bundle size compared to regular enums.
- Cannot be used with dynamic access like `Direction[key]`.
- Can cause issues with isolated module compilation (e.g., Babel, esbuild).

## Interview Tip:
Mention the limitation — `const enum` doesn't work well with tools that compile single files without TypeScript knowledge (like Babel). This is a real gotcha in Next.js/Vite projects.

---

## Question 35: What are type aliases?

## Answer:
Type aliases let you create a custom name for any type — primitives, objects, unions, intersections, or generics. You use the `type` keyword.

```ts
type UserId = string;
type Coordinate = { x: number; y: number };
type StringOrNumber = string | number;
```

## Key Points:
- Created with the `type` keyword.
- Can alias any type — including unions and complex types.
- Cannot be reopened/extended after declaration (unlike interfaces).
- Useful for complex generic types and utility types.

## Interview Tip:
Know when to use `type` vs `interface`. The key rule: use `interface` for object shapes that might be extended; use `type` for unions, intersections, and complex types.

---

## Question 36: What is the difference between `type` and `interface`?

## Answer:
Both define object shapes, but they have key differences:
- **Interfaces** can be extended and merged (declaration merging). Better for class contracts.
- **Type aliases** can represent unions, intersections, primitives, and complex types. More flexible.

```ts
interface User { name: string }
interface User { email: string } // Merged!

type UserType = { name: string }
type UserType = { email: string } // Error — duplicate
```

## Key Points:
- `interface` supports declaration merging; `type` does not.
- `type` supports union and intersection types; `interface` doesn't natively.
- Both can be used for object shapes interchangeably in most cases.
- Prefer `interface` for public API contracts; `type` for internal complex types.

## Interview Tip:
The most common interview question on this topic. Give the declaration merging example — it's the clearest differentiator. Then mention that in practice, many teams pick one and stick to it.

---

## Question 37: When should you use `type`?

## Answer:
Use `type` when you need:
- Union or intersection types: `type ID = string | number`
- Complex or computed types using generics and utility types
- Aliasing primitives or tuples
- Any type that can't be expressed with `interface`

```ts
type ApiResponse<T> = { data: T; error: string | null };
type Status = "active" | "inactive";
```

## Key Points:
- Best for unions, intersections, and complex generic types.
- Use for aliasing primitives and tuples.
- Use when you need mapped or conditional types.
- Cannot be used with declaration merging.

## Interview Tip:
Show you have a principled reason for choosing `type` vs `interface`, not just arbitrary preference. Interviewers respect developers who can explain the "why."

---

## Question 38: When should you use `interface`?

## Answer:
Use `interface` for object shapes, especially when:
- Defining a contract for a class with `implements`
- You expect the shape to be extended by others
- You're writing a library or public API
- You want declaration merging to add properties from different files

```ts
interface Repository<T> {
  findById(id: string): Promise<T>;
  save(entity: T): Promise<void>;
}
```

## Key Points:
- Best for defining object shapes and class contracts.
- Supports `extends` for inheritance.
- Supports declaration merging.
- Preferred by many teams for consistency in object typing.

## Interview Tip:
Mentioning that interfaces work well with `extends` and `implements` shows you know the object-oriented side of TypeScript, which is valuable for backend roles.

---

## Question 39: Can interfaces extend interfaces?

## Answer:
Yes, interfaces support inheritance with the `extends` keyword. An interface can extend one or multiple other interfaces.

```ts
interface Animal { name: string }
interface Pet extends Animal { owner: string }
interface Dog extends Pet { breed: string }

const dog: Dog = { name: "Rex", owner: "John", breed: "Labrador" };
```

## Key Points:
- Interfaces use `extends` for inheritance.
- Multiple extensions are supported: `interface C extends A, B`.
- The child interface inherits all parent properties.
- Useful for building layered type hierarchies.

## Interview Tip:
Show the multi-extension example. It's a cleaner answer than just saying "yes." Also mention this is how TypeScript handles OOP-style inheritance in types.

---

## Question 40: Can types extend interfaces?

## Answer:
Yes, type aliases can extend interfaces using intersection types. And interfaces can also extend type aliases.

```ts
interface Animal { name: string }
type Pet = Animal & { owner: string }; // type extending interface

type Shape = { color: string };
interface Circle extends Shape { radius: number } // interface extending type
```

## Key Points:
- Types use `&` (intersection) to "extend" other types or interfaces.
- Interfaces can use `extends` to extend type aliases too.
- Both approaches work but produce slightly different behavior in error messages.
- Cross-extension is possible and common in real projects.

## Interview Tip:
Many candidates don't know interfaces can extend type aliases. Knowing this shows deeper TypeScript knowledge.

---

## Question 41: What are declaration merging and interface merging?

## Answer:
Declaration merging means that if you declare the same interface name multiple times, TypeScript merges them into one. This is unique to interfaces — type aliases can't do this.

```ts
interface Config { timeout: number }
interface Config { retries: number }
// Merged: Config = { timeout: number; retries: number }
```

This is how `@types` packages add properties to existing types, like adding properties to the `Window` object.

## Key Points:
- TypeScript merges duplicate interface declarations automatically.
- Only works with `interface`, not `type`.
- Used to extend third-party library types.
- Common for extending `Express.Request` or the global `Window`.

## Interview Tip:
Give the `Express.Request` example — adding `user` to the request object in Express middleware is a common real-world use of declaration merging.

---

## Question 42: What is optional chaining (`?.`)?

## Answer:
Optional chaining lets you safely access nested properties without throwing if something in the chain is `null` or `undefined`. If any part is nullish, the whole expression returns `undefined`.

```ts
const city = user?.address?.city; // No error if address is undefined
const len = user?.hobbies?.length;
```

## Key Points:
- Returns `undefined` if any part of the chain is null/undefined.
- Works for property access `?.`, method calls `?.()`, and array access `?.[index]`.
- Replaces long conditional chains like `user && user.address && user.address.city`.
- This is a JavaScript/ES2020 feature — TypeScript just types it properly.

## Interview Tip:
Combine with nullish coalescing for a common pattern: `user?.name ?? "Guest"`. This shows practical knowledge interviewers look for.

---

## Question 43: What is nullish coalescing (`??`)?

## Answer:
`??` returns the right-hand value only when the left-hand value is `null` or `undefined`. It's different from `||` which also triggers for falsy values like `0`, `""`, or `false`.

```ts
const count = user.count ?? 0;  // 0 only if count is null/undefined
const count2 = user.count || 0; // 0 even if count is 0 (bug!)
```

## Key Points:
- `??` only checks for `null` and `undefined`.
- `||` also triggers for `0`, `""`, `false` — can cause bugs.
- Use `??` when `0` or empty string are valid values.
- Combines well with optional chaining: `user?.name ?? "Guest"`.

## Interview Tip:
The `||` vs `??` comparison is a great interview point. Show a bug scenario where `||` incorrectly replaces a valid `0` value — this demonstrates real-world awareness.

---

## Question 44: What is optional property (`?`)?

## Answer:
Adding `?` after a property name in an interface or type makes it optional. The property may or may not be present on the object.

```ts
interface User {
  name: string;
  email?: string; // Optional — might be undefined
}

const u1: User = { name: "Alice" }; // Valid
const u2: User = { name: "Bob", email: "bob@example.com" }; // Also valid
```

## Key Points:
- `property?: type` means the property may be absent.
- TypeScript treats optional properties as `type | undefined`.
- Must handle the possible undefined before using the value.
- Common in form data, API responses, and config objects.

## Interview Tip:
Mention that when you access an optional property, you should use optional chaining or check for undefined first. Not doing so is a common TypeScript mistake.

---

## Question 45: What is optional parameter?

## Answer:
Optional parameters in functions use `?` after the parameter name. Callers can omit them, and inside the function, the value will be `undefined` if not provided.

```ts
function greet(name: string, greeting?: string): string {
  return `${greeting ?? "Hello"}, ${name}!`;
}
greet("Alice");           // "Hello, Alice!"
greet("Alice", "Hi");     // "Hi, Alice!"
```

## Key Points:
- Optional parameters must come after required parameters.
- The type inside the function is `type | undefined`.
- Use default values instead of optional when you have a sensible default.
- Calling with fewer arguments is valid when parameters are optional.

## Interview Tip:
Explain the difference between optional parameters (`name?`) and default parameters (`name = "Guest"`). Default parameters are often cleaner because they remove the `undefined` case.

---

## Question 46: What are default parameters?

## Answer:
Default parameters provide a fallback value when the argument is not passed or is `undefined`. They're cleaner than optional parameters when you have a sensible default.

```ts
function createUser(name: string, role: string = "user") {
  return { name, role };
}
createUser("Alice");          // { name: "Alice", role: "user" }
createUser("Bob", "admin");   // { name: "Bob", role: "admin" }
```

## Key Points:
- TypeScript infers the type from the default value.
- `undefined` is treated as "not provided" — the default kicks in.
- Default parameters eliminate the need to handle `undefined` inside the function.
- Unlike optional params, the type inside is not `type | undefined`.

## Interview Tip:
Prefer default parameters over optional parameters when possible — they lead to cleaner code with fewer null checks inside the function body.

---

## Question 47: What are rest parameters?

## Answer:
Rest parameters collect multiple arguments into an array. You use `...` before the last parameter name. TypeScript types them as an array.

```ts
function sum(...numbers: number[]): number {
  return numbers.reduce((total, n) => total + n, 0);
}
sum(1, 2, 3, 4); // 10
```

## Key Points:
- Must be the last parameter in the function signature.
- TypeScript types rest parameters as an array: `...args: string[]`.
- Can also use tuple types for rest parameters for precise typing.
- Different from the spread operator — rest collects, spread expands.

## Interview Tip:
Show you know the difference between rest parameters (function parameter collection) and the spread operator (expanding arrays/objects). They look similar but work oppositely.

---

## Question 48: What are spread operators?

## Answer:
The spread operator (`...`) expands an array or object into individual elements. In TypeScript, it works the same as in JavaScript but with type safety.

```ts
const a = [1, 2, 3];
const b = [...a, 4, 5]; // [1, 2, 3, 4, 5]

const user = { name: "Alice" };
const admin = { ...user, role: "admin" }; // merged object
```

## Key Points:
- Spreads arrays or objects into another array or object.
- Creates a shallow copy — nested objects are still references.
- TypeScript checks type compatibility when spreading.
- Used heavily in Redux for immutable state updates.

## Interview Tip:
Mention the shallow copy limitation. It's a common source of bugs — people assume spreading an object creates a deep copy of nested objects.

---

## Question 49: What are index signatures?

## Answer:
Index signatures define the type of values when you access an object with a dynamic key you don't know in advance. They're useful for dictionaries or maps.

```ts
interface StringMap {
  [key: string]: string;
}
const translations: StringMap = {
  hello: "Hola",
  goodbye: "Adiós"
};
```

## Key Points:
- Syntax: `[key: string]: ValueType`
- Useful for objects with dynamic/unknown keys.
- All values must match the index signature type.
- Can coexist with specific named properties if they match the index signature type.

## Interview Tip:
Mention a real use case like caching, locale strings, or API response transformations. Also note that `Record<string, string>` is often cleaner than writing an index signature manually.

---

## Question 50: What are template literal types?

## Answer:
Template literal types use backtick syntax to construct new string types from existing ones. They let you define precise string patterns at the type level.

```ts
type EventName = "click" | "focus" | "blur";
type Handler = `on${Capitalize<EventName>}`; // "onClick" | "onFocus" | "onBlur"
```

## Key Points:
- Uses backtick syntax like template literal strings, but at the type level.
- Can combine with union types to produce many string variants.
- Works with `Capitalize`, `Uppercase`, `Lowercase`, `Uncapitalize` intrinsic types.
- Great for defining event name patterns, CSS classes, or API endpoints.

## Interview Tip:
This is an advanced TypeScript feature. Mentioning it shows you're comfortable with TypeScript's type system beyond basics. Give a real-world example like generating event handler names.

---

## Part 3 (51–75): Advanced TypeScript

---

## Question 51: What are generics?

## Answer:
Generics let you write reusable code that works with different types. Instead of hardcoding a specific type, you use a type parameter that gets filled in when the function or class is used.

```ts
function identity<T>(value: T): T {
  return value;
}
identity<string>("hello"); // Returns string
identity<number>(42);      // Returns number
```

## Key Points:
- Type parameter is usually written as `<T>`.
- Generics make code reusable across different types.
- Type is inferred when you pass an argument — no need to explicitly write `<string>`.
- Used in functions, interfaces, classes, and type aliases.

## Interview Tip:
Give a practical example — a generic `ApiResponse<T>` wrapper for API responses is something every developer has built. It shows you use generics for real problems.

---

## Question 52: Why do we use generics?

## Answer:
Without generics, you'd either use `any` (losing type safety) or write separate functions for every type. Generics let you write one function that is both reusable and type-safe.

```ts
// Without generics — not type safe
function first(arr: any[]): any { return arr[0]; }

// With generics — type safe and reusable
function first<T>(arr: T[]): T { return arr[0]; }
```

## Key Points:
- Enables reusable, type-safe code.
- Avoids duplicating logic for different types.
- The compiler infers the type from usage.
- Better alternative to `any` for flexible functions.

## Interview Tip:
Show the contrast between `any[]` and `T[]`. This is the clearest way to explain why generics exist — they give you flexibility without sacrificing type safety.

---

## Question 53: What are generic constraints?

## Answer:
Generic constraints limit what types a generic can accept. You use `extends` to specify the constraint. This lets you access properties on the generic type that you know will exist.

```ts
function getLength<T extends { length: number }>(item: T): number {
  return item.length; // Safe — we know length exists
}
getLength("hello"); // 5
getLength([1, 2, 3]); // 3
```

## Key Points:
- Use `extends` to constrain a generic type.
- Allows accessing specific properties within the generic function.
- The constraint can be an interface, type, or primitive.
- Common constraints: `extends object`, `extends string`, `extends keyof T`.

## Interview Tip:
The `extends keyof T` constraint is worth mentioning — it's used in utility types like `Pick` and `Omit`. It shows you understand how TypeScript's built-in utilities work internally.

---

## Question 54: What is the `keyof` operator?

## Answer:
`keyof` takes a type and returns a union of its property names as string literal types. It's how you safely access object properties with dynamic keys.

```ts
interface User { name: string; age: number; email: string }
type UserKeys = keyof User; // "name" | "age" | "email"

function getProperty<T, K extends keyof T>(obj: T, key: K): T[K] {
  return obj[key];
}
```

## Key Points:
- `keyof T` produces a union of all keys of type `T`.
- Used with generics to create type-safe property access.
- Core building block for utility types like `Pick`, `Omit`, `Record`.
- Works with index signatures too.

## Interview Tip:
The `getProperty` generic function above is a classic TypeScript interview example. Being able to write and explain it shows strong TypeScript fundamentals.

---

## Question 55: What is the `typeof` operator?

## Answer:
In TypeScript, `typeof` has two uses: the JavaScript runtime operator that returns a string, and the TypeScript type operator that extracts the type of a value at the type level.

```ts
const config = { host: "localhost", port: 3000 };
type Config = typeof config; // { host: string; port: number }

function process(val: typeof config) { /* ... */ }
```

## Key Points:
- Runtime `typeof`: returns a string like "string", "number", "object".
- Type-level `typeof`: extracts the TypeScript type of a value.
- Useful for inferring types from existing objects or functions.
- Combined with `ReturnType<typeof fn>` for function return types.

## Interview Tip:
Distinguish the runtime vs type-level usage clearly. Showing `ReturnType<typeof someFunction>` is a strong practical example interviewers appreciate.

---

## Question 56: What is indexed access type?

## Answer:
Indexed access types let you look up the type of a specific property within another type. You use bracket notation at the type level.

```ts
interface User { name: string; age: number; address: { city: string } }
type NameType = User["name"]; // string
type CityType = User["address"]["city"]; // string
type UserValues = User[keyof User]; // string | number | { city: string }
```

## Key Points:
- Syntax: `Type["property"]` to get the type of that property.
- Works with nested types using chained access.
- Works with `keyof` for dynamic property type access.
- Returns a union type when used with a union of keys.

## Interview Tip:
Combine with `keyof` to show you understand how TypeScript's utility types are built. `T[keyof T]` returns a union of all value types — it's the foundation of many advanced types.

---

## Question 57: What are mapped types?

## Answer:
Mapped types create new types by iterating over the keys of an existing type and applying a transformation to each. They're how utility types like `Partial`, `Readonly`, and `Record` are built internally.

```ts
type Optional<T> = {
  [K in keyof T]?: T[K]
};
// Same as Partial<T>
```

## Key Points:
- Use `[K in keyof T]` to iterate over all keys.
- Can add or remove modifiers like `?` (optional) or `readonly`.
- Foundation for all built-in utility types.
- Can remap keys with `as` clause in newer TypeScript versions.

## Interview Tip:
Writing a simple mapped type from scratch (like `Optional<T>`) is a strong interview answer. It shows you understand TypeScript deeply, not just how to use utility types.

---

## Question 58: What are conditional types?

## Answer:
Conditional types choose between two types based on a condition. The syntax looks like a ternary expression in the type system.

```ts
type IsString<T> = T extends string ? "yes" : "no";
type A = IsString<string>; // "yes"
type B = IsString<number>; // "no"
```

## Key Points:
- Syntax: `T extends Condition ? TrueType : FalseType`
- Used to build type-level logic.
- Foundation of utility types like `Exclude`, `Extract`, `NonNullable`.
- Can be distributive when applied to union types.

## Interview Tip:
Mention that conditional types distribute over unions automatically. `IsString<string | number>` becomes `IsString<string> | IsString<number>`, which equals `"yes" | "no"`. This is the distributive behavior.

---

## Question 59: What is the `infer` keyword?

## Answer:
`infer` is used inside conditional types to extract a type and give it a name. It's how TypeScript "captures" a type from within another type.

```ts
type ReturnType<T> = T extends (...args: any[]) => infer R ? R : never;

function greet(): string { return "hello"; }
type Greeting = ReturnType<typeof greet>; // string
```

## Key Points:
- Only used inside `extends` clauses in conditional types.
- Creates a new type variable to capture the inferred type.
- Used internally in `ReturnType`, `Parameters`, `Awaited`, etc.
- Powerful for extracting types from complex generic structures.

## Interview Tip:
Implementing `ReturnType` manually using `infer` is a classic advanced TypeScript exercise. Being able to write it shows you truly understand the type system.

---

## Question 60: What are utility types?

## Answer:
Utility types are built-in generic types that transform existing types into new ones. TypeScript ships with many of them — `Partial`, `Required`, `Readonly`, `Pick`, `Omit`, `Record`, etc.

They save you from writing repetitive type transformations manually.

```ts
interface User { name: string; email: string; age: number }
type PartialUser = Partial<User>; // All properties optional
type NameOnly = Pick<User, "name">; // Only name property
```

## Key Points:
- Built into TypeScript's standard library.
- Transform existing types without rewriting them.
- All utility types are built using generics, mapped types, and conditional types.
- Learning them saves a lot of repetitive type writing.

## Interview Tip:
Know the most commonly used ones: `Partial`, `Required`, `Readonly`, `Pick`, `Omit`, `Record`, `Exclude`, `Extract`, `ReturnType`, `NonNullable`. Be ready to use any of them in a code example.

---

## Question 61: What is `Partial<T>`?

## Answer:
`Partial<T>` makes all properties of a type optional. It's useful for update operations where you don't need to provide all fields.

```ts
interface User { name: string; email: string; age: number }
type UpdateUser = Partial<User>;
// { name?: string; email?: string; age?: number }

function updateUser(id: string, changes: Partial<User>) { /* ... */ }
```

## Key Points:
- Makes every property optional (`?`).
- Equivalent to a mapped type: `{ [K in keyof T]?: T[K] }`.
- Commonly used for PATCH request body types.
- Doesn't affect nested objects — only top-level properties.

## Interview Tip:
Mention the real use case: PATCH endpoints in REST APIs. You only send the fields you want to update. `Partial<T>` is perfect for typing the request body.

---

## Question 62: What is `Required<T>`?

## Answer:
`Required<T>` is the opposite of `Partial` — it makes all properties required, removing any optional markers. Useful when you want to ensure a fully complete object.

```ts
interface Config {
  host?: string;
  port?: number;
  timeout?: number;
}
type FullConfig = Required<Config>;
// { host: string; port: number; timeout: number }
```

## Key Points:
- Removes `?` from all properties.
- Equivalent to: `{ [K in keyof T]-?: T[K] }` (the `-?` removes optionality).
- Useful for validation or when consuming a fully populated object.
- Does not affect nested optional properties.

## Interview Tip:
Mention the `-?` mapped type modifier — it removes optionality. This shows you understand how `Required` is implemented, not just how to use it.

---

## Question 63: What is `Readonly<T>`?

## Answer:
`Readonly<T>` makes all properties of a type read-only. After creation, you can't reassign any property. Great for immutable data structures.

```ts
const config: Readonly<{ host: string; port: number }> = {
  host: "localhost",
  port: 3000
};
config.port = 8080; // Error! Cannot assign to readonly property
```

## Key Points:
- Adds `readonly` modifier to all properties.
- TypeScript enforces this at compile time.
- Doesn't affect runtime behavior — it's purely a type check.
- Like `Partial`, only affects the top level (not nested objects).

## Interview Tip:
Mention that `Object.freeze()` enforces immutability at runtime, while `Readonly` only does it at type level. For true immutability you'd need both — or use a library like Immer.

---

## Question 64: What is `Pick<T>`?

## Answer:
`Pick<T, K>` creates a new type by selecting only specific properties from an existing type. You pass the keys you want to keep.

```ts
interface User { name: string; email: string; password: string; age: number }
type PublicUser = Pick<User, "name" | "email">;
// { name: string; email: string }
```

## Key Points:
- Takes two type arguments: the base type and a union of keys.
- Creates a new type with only the selected properties.
- Keys must exist in the original type — TypeScript will error otherwise.
- Useful for creating slimmer types for specific use cases.

## Interview Tip:
Give the API response example — when your API returns a `User` but you only need to expose `name` and `email` to the frontend, `Pick` creates that slimmer type cleanly.

---

## Question 65: What is `Omit<T>`?

## Answer:
`Omit<T, K>` is the opposite of `Pick` — it creates a new type by removing specific properties from an existing type.

```ts
interface User { name: string; email: string; password: string; age: number }
type SafeUser = Omit<User, "password">;
// { name: string; email: string; age: number }
```

## Key Points:
- Takes two type arguments: the base type and a union of keys to remove.
- Equivalent to `Pick<T, Exclude<keyof T, K>>` under the hood.
- Useful for removing sensitive fields before sending data to clients.
- Common for creating "create" types that omit auto-generated fields like `id` or `createdAt`.

## Interview Tip:
The `Omit<User, "password">` example is perfect for interviews — it maps directly to a real security concern (never exposing passwords). It shows practical judgment.

---

## Question 66: What is `Exclude<T>`?

## Answer:
`Exclude<T, U>` removes types from a union that are assignable to `U`. It works on union types, not object types.

```ts
type A = string | number | boolean;
type B = Exclude<A, boolean>; // string | number

type Status = "active" | "inactive" | "banned";
type ActiveStatus = Exclude<Status, "banned">; // "active" | "inactive"
```

## Key Points:
- Works on union types, not object properties.
- Removes members from a union that match the second type argument.
- Implemented as: `T extends U ? never : T`.
- Different from `Omit` — `Exclude` is for unions, `Omit` is for object types.

## Interview Tip:
Candidates often confuse `Exclude` and `Omit`. Clarify: `Exclude` operates on union types; `Omit` operates on object types. This distinction shows TypeScript depth.

---

## Question 67: What is `Extract<T>`?

## Answer:
`Extract<T, U>` keeps only the types from union `T` that are assignable to `U`. It's the opposite of `Exclude`.

```ts
type All = string | number | boolean | null;
type StringOrNumber = Extract<All, string | number>; // string | number
```

## Key Points:
- Keeps types from the union that match the second argument.
- Opposite of `Exclude`.
- Implemented as: `T extends U ? T : never`.
- Useful for filtering union types to a subset.

## Interview Tip:
Pair with `Exclude` in your answer — interviewers often ask about both together. Show you understand they're opposites built on the same conditional type mechanism.

---

## Question 68: What is `Record<K, T>`?

## Answer:
`Record<K, T>` creates an object type where all keys are of type `K` and all values are of type `T`. It's cleaner than writing an index signature manually.

```ts
type Role = "admin" | "user" | "guest";
const permissions: Record<Role, string[]> = {
  admin: ["read", "write", "delete"],
  user: ["read"],
  guest: []
};
```

## Key Points:
- First type argument is the key type (usually `string` or a union).
- Second type argument is the value type.
- Ensures all keys in the union are present.
- Cleaner alternative to index signatures for known key sets.

## Interview Tip:
The permissions map example is great. Show that when you use a union as the key type, TypeScript forces you to include all members — it's exhaustive by default.

---

## Question 69: What is `ReturnType<T>`?

## Answer:
`ReturnType<T>` extracts the return type of a function type. You don't have to manually define the return type separately — TypeScript infers it from the function.

```ts
function getUser() {
  return { id: 1, name: "Alice", email: "alice@example.com" };
}
type User = ReturnType<typeof getUser>;
// { id: number; name: string; email: string }
```

## Key Points:
- Extracts the return type of a function.
- Must use `typeof` to get the type of a function value.
- Useful when a function's return type is complex or inferred.
- Keeps types in sync — if the function changes, `ReturnType` updates automatically.

## Interview Tip:
The "keeps types in sync" angle is powerful. If you define the type from the source of truth (the function), you never have a mismatch between what a function returns and what the type says.

---

## Question 70: What is `Parameters<T>`?

## Answer:
`Parameters<T>` extracts the parameter types of a function as a tuple. It's useful when you need to reference or reuse a function's argument types.

```ts
function createUser(name: string, age: number, role: "admin" | "user") {}
type CreateArgs = Parameters<typeof createUser>;
// [name: string, age: number, role: "admin" | "user"]
```

## Key Points:
- Returns a tuple of parameter types.
- Use `typeof` to get the function type first.
- Useful for creating wrapper functions with the same signature.
- Pairs well with `ReturnType` for full function type extraction.

## Interview Tip:
Show a wrapper function use case — creating a function with the same parameters as another is a common pattern in HOFs (higher-order functions) and middleware.

---

## Question 71: What is `Awaited<T>`?

## Answer:
`Awaited<T>` recursively unwraps the resolved type of a `Promise`. It's what TypeScript uses internally to understand `async/await` return types.

```ts
type A = Awaited<Promise<string>>;           // string
type B = Awaited<Promise<Promise<number>>>;  // number
```

## Key Points:
- Unwraps nested Promises to get the final resolved type.
- Handles deeply nested `Promise<Promise<...>>` chains.
- Introduced in TypeScript 4.5.
- TypeScript uses it internally for `async` function return types.

## Interview Tip:
This shows up when you're working with API calls. `Awaited<ReturnType<typeof fetchUser>>` gives you the actual resolved data type — useful for keeping response types in sync.

---

## Question 72: What is `NonNullable<T>`?

## Answer:
`NonNullable<T>` removes `null` and `undefined` from a type. Useful when you've already checked that a value exists and want TypeScript to know it's safe to use.

```ts
type MaybeString = string | null | undefined;
type DefiniteString = NonNullable<MaybeString>; // string
```

## Key Points:
- Removes `null` and `undefined` from the type.
- Implemented as: `T extends null | undefined ? never : T`.
- Useful after a null check when you want to narrow a type.
- Common in utility functions that filter out null values.

## Interview Tip:
Mention the non-null assertion operator (`!`) as a runtime complement. But prefer `NonNullable` in type definitions and proper null checks in code over the `!` operator.

---

## Question 73: What is `InstanceType<T>`?

## Answer:
`InstanceType<T>` extracts the type of an instance of a class constructor. It gives you the type you'd get when you `new` the class.

```ts
class User {
  name: string;
  constructor(name: string) { this.name = name; }
}
type UserInstance = InstanceType<typeof User>; // User
```

## Key Points:
- Takes a constructor type and returns the instance type.
- Useful when working with class factories or dependency injection.
- `typeof ClassName` gives the constructor type; `InstanceType` gives the instance type.
- Common in framework code that deals with class constructors dynamically.

## Interview Tip:
This is less common but shows TypeScript breadth. Mention use cases like dependency injection containers or abstract factory patterns where you work with class constructors dynamically.

---

## Question 74: What is a discriminated union?

## Answer:
A discriminated union is a union of types that all share a common literal property (the discriminant). TypeScript uses that property to narrow the type in conditional checks.

```ts
type Shape =
  | { kind: "circle"; radius: number }
  | { kind: "rect"; width: number; height: number };

function area(shape: Shape): number {
  if (shape.kind === "circle") {
    return Math.PI * shape.radius ** 2; // TypeScript knows it's a circle
  }
  return shape.width * shape.height; // TypeScript knows it's a rect
}
```

## Key Points:
- All union members share a common literal property (the discriminant).
- TypeScript narrows the type based on the discriminant value.
- Works with `if`, `switch`, and other control flow.
- Essential pattern for modeling state machines and action handlers.

## Interview Tip:
This is a very common interview question. Mention Redux actions as a real-world example — each action has a `type` discriminant that TypeScript uses to narrow the payload type.

---

## Question 75: What is type narrowing?

## Answer:
Type narrowing is when TypeScript automatically refines a broad type to a more specific one inside a conditional block. It happens whenever you use type guards like `typeof`, `instanceof`, or truthiness checks.

```ts
function process(value: string | number) {
  if (typeof value === "string") {
    console.log(value.toUpperCase()); // TypeScript knows it's a string here
  } else {
    console.log(value.toFixed(2)); // TypeScript knows it's a number here
  }
}
```

## Key Points:
- TypeScript tracks type information through control flow.
- Works with `typeof`, `instanceof`, `in`, equality checks, and truthy/falsy.
- Discriminated unions use a property value to narrow.
- TypeScript's control flow analysis makes this automatic.

## Interview Tip:
Mention several narrowing techniques: `typeof`, `instanceof`, the `in` operator, and discriminated union pattern. Showing multiple approaches demonstrates strong TypeScript knowledge.

---

## Part 4 (76–100): Real-World & Interview Questions

---

## Question 76: What are type guards?

## Answer:
Type guards are conditions that tell TypeScript what type a value is within a specific block. Built-in type guards include `typeof`, `instanceof`, and the `in` operator. You can also write custom type guards.

```ts
function isString(value: unknown): value is string {
  return typeof value === "string";
}
if (isString(input)) {
  console.log(input.toUpperCase()); // TypeScript knows it's a string
}
```

## Key Points:
- Type guards narrow a type within a conditional block.
- Built-in: `typeof`, `instanceof`, `in` operator.
- Custom type guards use the `value is Type` return type syntax.
- TypeScript's narrowing relies on type guards.

## Interview Tip:
Know all three kinds: `typeof` for primitives, `instanceof` for classes, `in` for properties, and custom predicates for complex shapes. Custom type guards are the most impressive to show.

---

## Question 77: How do you create a custom type guard?

## Answer:
A custom type guard is a function that returns a boolean and uses the special return type `value is Type`. TypeScript uses this to narrow the type inside the `if` block.

```ts
interface Cat { meow(): void }
interface Dog { bark(): void }

function isCat(animal: Cat | Dog): animal is Cat {
  return (animal as Cat).meow !== undefined;
}

const pet: Cat | Dog = getPet();
if (isCat(pet)) {
  pet.meow(); // Safe — TypeScript knows it's a Cat
}
```

## Key Points:
- Return type syntax: `parameter is Type`
- The function must return a boolean.
- TypeScript trusts the predicate — you're responsible for correctness.
- Used when `typeof` and `instanceof` aren't sufficient.

## Interview Tip:
Emphasize that TypeScript trusts your type predicate — if your function has a bug, TypeScript will still narrow based on your declaration. This responsibility is worth mentioning.

---

## Question 78: What is type assertion?

## Answer:
Type assertion tells TypeScript "trust me, I know the type of this value." You use `as` keyword or angle bracket syntax. It doesn't change the runtime value — it's purely a compile-time instruction.

```ts
const input = document.getElementById("email") as HTMLInputElement;
console.log(input.value); // TypeScript now knows it's an HTMLInputElement
```

## Key Points:
- `as Type` or `<Type>value` syntax.
- Only the `as` syntax works in JSX/TSX files.
- Doesn't perform any runtime conversion — no type checking at runtime.
- Use when you know more about the type than TypeScript can infer.

## Interview Tip:
Warn that type assertion can be dangerous — you're overriding TypeScript's judgment. Prefer type guards when possible. Double assertion (`value as unknown as TargetType`) is a red flag.

---

## Question 79: What is the difference between type assertion and type casting?

## Answer:
Type assertion is a TypeScript compile-time feature — it only tells the compiler what type to use. No runtime transformation happens. Type casting (in languages like Java or C#) actually converts the value at runtime.

In TypeScript, `as number` doesn't convert a string to a number. It just silences the type error. At runtime it's still a string.

## Key Points:
- Type assertion: compile-time only — no runtime effect.
- Type casting: runtime conversion (not a TypeScript concept).
- `as` in TypeScript is purely for the type system.
- Use `Number("42")` for actual runtime conversion, not `as number`.

## Interview Tip:
This distinction is important. Many developers coming from Java/C# assume `as number` converts the value. Clarifying this shows deep understanding of TypeScript's compile-time nature.

---

## Question 80: What is declaration file (`.d.ts`)?

## Answer:
A `.d.ts` file is a TypeScript declaration file. It contains only type definitions — no implementation code. It tells TypeScript about the types of a JavaScript library without adding actual code.

When you install `@types/express`, you get `.d.ts` files that describe Express's types so TypeScript can check your code.

## Key Points:
- Contains only type declarations, no implementations.
- Used to add TypeScript types to JavaScript libraries.
- Generated by `tsc --declaration` from TypeScript source.
- Enabled by `"declaration": true` in `tsconfig.json`.

## Interview Tip:
Mention that you've written custom `.d.ts` files when working with JavaScript libraries that don't have types. This is a common real-world task and shows practical TypeScript experience.

---

## Question 81: What is module augmentation?

## Answer:
Module augmentation lets you add new properties to existing types from external modules. You declare the module and add your additions inside it.

```ts
// Extending Express Request type
declare module "express" {
  interface Request {
    user?: { id: string; role: string };
  }
}
```

This is how you add `req.user` to Express's Request type in authentication middleware.

## Key Points:
- Used to extend types from third-party libraries.
- Uses `declare module "moduleName"` syntax.
- Relies on interface declaration merging.
- Common for extending Express, Next.js, or Prisma types.

## Interview Tip:
The Express `Request` augmentation is the perfect real-world example. Every backend developer using TypeScript with Express has done this. Mention it confidently.

---

## Question 82: What is namespace in TypeScript?

## Answer:
Namespaces were TypeScript's original way to organize code before ES Modules became standard. They group related code under a named scope to avoid global variable conflicts.

```ts
namespace Validation {
  export function isEmail(email: string): boolean { return true; }
  export function isPhone(phone: string): boolean { return true; }
}
Validation.isEmail("test@example.com");
```

## Key Points:
- TypeScript-specific feature — older alternative to modules.
- Creates a named scope to avoid global pollution.
- Less common in modern code — ES Modules are preferred.
- Still found in legacy code and some `.d.ts` files.

## Interview Tip:
Mention that namespaces are largely obsolete in modern TypeScript. ES Modules are the right approach for new code. Knowing this shows you're up to date with current practices.

---

## Question 83: Why are ES Modules preferred over namespaces?

## Answer:
ES Modules are the JavaScript standard, supported natively by browsers and Node.js. They have better tree-shaking, work with all modern build tools, and are easier to test. Namespaces are TypeScript-specific and don't interoperate well with standard JavaScript tooling.

## Key Points:
- ES Modules are the JavaScript standard.
- Better tooling support (tree-shaking, bundlers, dynamic imports).
- Explicit imports/exports make dependencies clear.
- Namespaces are TypeScript-only and can cause issues with module bundlers.

## Interview Tip:
Use this question to show you understand modern JavaScript ecosystem. Never recommend namespaces for new projects — it immediately flags you as someone with outdated knowledge.

---

## Question 84: What are decorators?

## Answer:
Decorators are a way to add metadata or modify behavior of classes, methods, properties, or parameters. They use the `@` symbol. They're heavily used in frameworks like NestJS, Angular, and TypeORM.

```ts
function Log(target: any, key: string, descriptor: PropertyDescriptor) {
  const original = descriptor.value;
  descriptor.value = function (...args: any[]) {
    console.log(`Calling ${key}`);
    return original.apply(this, args);
  };
  return descriptor;
}

class UserService {
  @Log
  getUser(id: string) { return { id }; }
}
```

## Key Points:
- Experimental feature — requires `"experimentalDecorators": true` in tsconfig.
- Four types: class, method, property, and parameter decorators.
- Central to NestJS and Angular architectures.
- TypeScript 5.0 introduced a new decorator standard aligned with the TC39 proposal.

## Interview Tip:
Mention NestJS — it's built entirely around decorators. If you've used NestJS, say so. It demonstrates real-world decorator experience beyond theory.

---

## Question 85: What are mixins?

## Answer:
Mixins are a pattern for combining behavior from multiple sources into a class without traditional inheritance. TypeScript doesn't natively support multiple inheritance, so mixins fill that gap.

```ts
type Constructor<T = {}> = new (...args: any[]) => T;

function Timestamped<Base extends Constructor>(base: Base) {
  return class extends base {
    createdAt = new Date();
  };
}

class User { name = "Alice"; }
const TimestampedUser = Timestamped(User);
```

## Key Points:
- Pattern for composing multiple behaviors into one class.
- Workaround for TypeScript's lack of multiple inheritance.
- Uses generic functions that take and return class constructors.
- More flexible than traditional inheritance chains.

## Interview Tip:
Mixins are advanced. Knowing them is a differentiator. Frame it in terms of composition over inheritance — that's the underlying principle.

---

## Question 86: How do you organize types in a large project?

## Answer:
I keep shared types in a `types/` folder at the project root. Specific feature types go inside their feature folders. I also use barrel files (`index.ts`) to re-export everything cleanly.

```
src/
  types/          # Shared global types
    api.ts
    models.ts
  features/
    auth/
      types.ts    # Auth-specific types
    users/
      types.ts
```

## Key Points:
- Separate shared types into a `types/` folder.
- Co-locate feature-specific types with their features.
- Use barrel files for clean imports.
- For full-stack projects, consider a shared package for common types.

## Interview Tip:
Mentioning a monorepo shared package for types across frontend and backend shows senior-level thinking. Tools like Turborepo or Nx make this easy.

---

## Question 87: How do you share types between frontend and backend?

## Answer:
In a monorepo, I create a shared `packages/types` package that both the frontend and backend depend on. Both consume the same type definitions, so if an API contract changes, both sides get the type error immediately.

For standalone projects, I put shared types in a published npm package or copy them into both projects (less ideal).

## Key Points:
- Monorepo approach: shared `packages/types` package.
- Both frontend and backend import from the same source.
- Type mismatch between API contract and client is caught at compile time.
- Tools: Turborepo, Nx, or npm workspaces make this clean.

## Interview Tip:
This shows architectural thinking. Mention that the alternative (duplicating types) leads to drift and bugs. Shared types are a sign of a mature TypeScript setup.

---

## Question 88: How does TypeScript help in React projects?

## Answer:
TypeScript makes React development much safer. It types props so you know exactly what a component expects, catches missing required props at compile time, and makes refactoring components much easier.

```ts
interface ButtonProps {
  label: string;
  onClick: () => void;
  disabled?: boolean;
  variant?: "primary" | "secondary";
}
const Button = ({ label, onClick, disabled }: ButtonProps) => (
  <button onClick={onClick} disabled={disabled}>{label}</button>
);
```

## Key Points:
- Types component props and state precisely.
- Catches missing or wrong props at compile time.
- Improves autocomplete in JSX.
- Makes hook return types explicit and safe.

## Interview Tip:
Mention specific React + TypeScript features: typing `useState`, `useRef`, `useContext`, and event handlers. These are practical skills interviewers care about.

---

## Question 89: How does TypeScript help in Node.js projects?

## Answer:
In Node.js, TypeScript types the request/response objects, database query results, and service layer interfaces. This prevents the common bugs where you assume a field exists on a DB result and it doesn't.

I use it with Express, Prisma (which generates its own types), and Zod for runtime validation.

## Key Points:
- Types middleware, controllers, and service functions.
- Prisma generates TypeScript types from your schema automatically.
- `@types/node` provides types for Node.js built-ins.
- Zod bridges the gap between runtime validation and TypeScript types.

## Interview Tip:
Mention Prisma's auto-generated types — it's a killer feature that makes TypeScript extremely powerful in full-stack Node.js apps. Interviewers using Prisma will appreciate this.

---

## Question 90: What are common TypeScript mistakes?

## Answer:
- **Overusing `any`**: defeats the purpose entirely.
- **Not enabling `strict` mode**: you miss major safety checks.
- **Over-annotating**: TypeScript can infer most types — don't type everything manually.
- **Ignoring `unknown` in catch blocks**: errors caught by `catch` are `unknown`, not `Error`.
- **Not using utility types**: writing `Partial` manually instead of using the built-in.
- **Casting with `as` instead of using type guards**: masks real bugs.

## Key Points:
- `any` usage is the most common and most damaging mistake.
- Not using `strict: true` leaves many TypeScript benefits on the table.
- Unnecessary type annotations clutter code without adding safety.
- Skipping proper error handling in `catch` blocks.

## Interview Tip:
Being able to name real mistakes shows experience. Frame your answer as "things I learned the hard way" — it sounds authentic and demonstrates growth mindset.

---

## Question 91: How do you migrate a JavaScript project to TypeScript?

## Answer:
Gradually — never try to migrate everything at once. Here's my approach:
1. Add `tsconfig.json` with `allowJs: true` and `strict: false` initially.
2. Rename files from `.js` to `.ts` one by one.
3. Fix type errors file by file — start with the ones used most.
4. Enable `strict: true` when most files are typed.
5. Remove `allowJs` once all files are converted.

## Key Points:
- Start with `allowJs: true` to allow JS and TS to coexist.
- Use `// @ts-check` in JS files for partial checking without conversion.
- Prioritize high-value files: shared utilities, API handlers.
- Gradual migration reduces risk in production projects.

## Interview Tip:
The word "gradually" is key. Trying to migrate everything at once is a mistake candidates with experience know to avoid. This answer shows pragmatic thinking.

---

## Question 92: What TypeScript features do you use most often?

## Answer:
In daily work:
- **Interfaces and type aliases** for defining data shapes.
- **Generics** for reusable API utilities and hooks.
- **Utility types** — `Partial`, `Pick`, `Omit`, `Record` constantly.
- **Union types** for state management and API responses.
- **`keyof` and `typeof`** for type-safe property access.
- **Discriminated unions** for handling different action types.

## Key Points:
- Generics and utility types are the workhorses of production TypeScript.
- Union types and discriminated unions for state management.
- `typeof` for deriving types from existing values.
- Zod + TypeScript together for full-stack type safety.

## Interview Tip:
Be specific — name concrete features with real use cases. "I use Partial for PATCH request bodies" is much stronger than "I use many TypeScript features."

---

## Question 93: How do you debug TypeScript errors?

## Answer:
First I read the error message carefully — TypeScript errors are usually descriptive. I hover over the variable in VS Code to see the inferred type. If the error is complex, I break the type down using intermediate variables or utility types to isolate where it breaks.

```ts
// Break complex types into steps
type Step1 = ReturnType<typeof fn>;
type Step2 = Step1["data"]; // Debug step by step
```

## Key Points:
- VS Code hover shows inferred types — use it constantly.
- `tsc --noEmit` for a full type-check without compiling.
- Break complex types into intermediate type aliases to debug.
- `// @ts-ignore` is a last resort, not a solution.

## Interview Tip:
Mentioning VS Code's hover feature and `tsc --noEmit` shows you have practical debugging habits. Admitting `@ts-ignore` exists but is a last resort shows maturity.

---

## Question 94: How do you improve TypeScript performance in large projects?

## Answer:
- Enable **incremental compilation** (`"incremental": true`) — TypeScript caches compilation results.
- Use **project references** for monorepos — compile only changed packages.
- Enable **`skipLibCheck: true`** to skip type checking of node_modules.
- Avoid overly complex recursive generic types — they slow the type checker.
- Use `isolatedModules: true` to ensure compatibility with fast transpilers like esbuild.

## Key Points:
- `incremental: true` speeds up subsequent builds.
- Project references for monorepo compilation isolation.
- `skipLibCheck: true` skips library type re-checking.
- Complex generic types are the biggest performance bottleneck.

## Interview Tip:
This question tests senior-level knowledge. Most candidates know `skipLibCheck`. Knowing project references and incremental builds shows you've worked on large-scale TypeScript projects.

---

## Question 95: What TypeScript compiler options do you commonly use?

## Answer:
Here's my typical `tsconfig.json` setup:

```json
{
  "compilerOptions": {
    "target": "ES2020",
    "module": "ESNext",
    "moduleResolution": "bundler",
    "strict": true,
    "skipLibCheck": true,
    "paths": { "@/*": ["./src/*"] },
    "baseUrl": ".",
    "incremental": true,
    "declaration": true,
    "sourceMap": true
  }
}
```

## Key Points:
- `strict: true` — always on for new projects.
- `skipLibCheck: true` — speeds up compilation.
- `paths` and `baseUrl` — for clean absolute imports.
- `declaration: true` — when publishing libraries.
- `sourceMap: true` — for debugging in production.

## Interview Tip:
Having a mentally ready "go-to" tsconfig shows you've done this for real. Interviewers are impressed when you can name specific options and explain why you use each one.

---

## Question 96: What are the best practices for writing TypeScript?

## Answer:
- Enable `strict` mode from day one.
- Prefer `unknown` over `any`.
- Use `const` by default — `readonly` for object properties.
- Don't over-annotate — let inference work where it can.
- Use utility types instead of manually recreating type transformations.
- Avoid `// @ts-ignore` — fix the root cause instead.
- Keep type definitions close to their usage.
- Use discriminated unions for complex state.

## Key Points:
- `strict: true` is non-negotiable.
- Prefer inference over explicit annotations where types are obvious.
- Type at boundaries (API responses, function inputs) not everywhere.
- Use Zod or similar for runtime + compile-time validation.

## Interview Tip:
Framing best practices as "what I actually do in projects" rather than reciting a list sounds more authentic. Pick 3-4 and explain the "why" behind each.

---

## Question 97: What TypeScript interview questions have you been asked before?

## Answer:
Commonly asked questions I've encountered:
- Difference between `type` and `interface`.
- What is `any` vs `unknown` — with a code example.
- Write a generic function.
- Explain discriminated unions with a real use case.
- What utility types have you used?
- How does TypeScript's structural typing work?
- What is `never` and when do you use it?

## Key Points:
- `type` vs `interface` is the most common question.
- Generic functions and utility types are standard senior questions.
- Structural typing and type narrowing show deep understanding.
- Real-world examples are more impressive than theoretical answers.

## Interview Tip:
This is a meta-question. Use it to highlight the areas you're strongest in. Frame it as "the questions I always prepare for" — it shows self-awareness and interview readiness.

---

## Question 98: What is your favorite TypeScript feature and why?

## Answer:
Mine is discriminated unions with exhaustive checking using `never`. It makes state management incredibly safe. When you add a new state variant, TypeScript immediately flags every place in the code that doesn't handle it.

```ts
function assertNever(x: never): never {
  throw new Error("Unhandled case: " + x);
}
```

## Key Points:
- Discriminated unions catch unhandled cases at compile time.
- `never` at the bottom of a switch is exhaustive checking.
- Makes state machines and action reducers bulletproof.
- Any good answer here should include a "why" — not just what.

## Interview Tip:
Pick something that shows depth — generics, discriminated unions, or conditional types are stronger answers than "I like autocomplete." The answer should reflect real experience.

---

## Question 99: What are the biggest challenges you've faced with TypeScript?

## Answer:
- **Third-party library types**: Some libraries have outdated or incorrect `@types` — you end up writing your own `.d.ts` augmentations.
- **Complex generic types**: When you get deep into generic type chains, errors become very hard to read.
- **Migrating legacy JS code**: Converting large JS files to strict TypeScript can be time-consuming.
- **Type errors in runtime data**: TypeScript only checks compile-time — API responses at runtime can still have unexpected shapes.

## Key Points:
- Generic type errors can be cryptic and hard to debug.
- Runtime data always needs validation (Zod, Joi, etc.).
- Incorrect `@types` packages cause subtle bugs.
- `strict` mode migration in large projects requires patience.

## Interview Tip:
Being honest about real challenges is refreshing to interviewers. Always follow up with "and here's how I solved it" — that's the complete answer.

---

## Question 100: If you were starting a new project today, how would you configure TypeScript and why?

## Answer:
For a Next.js or Vite project, I'd start with the framework's default TypeScript template. Then I'd update `tsconfig.json`:
- `strict: true` — always.
- `skipLibCheck: true` — for faster builds.
- Path aliases with `paths` — for clean imports.
- `incremental: true` — for faster subsequent builds.

I'd also add Zod for runtime validation and a shared types package if it's a full-stack monorepo.

## Key Points:
- Start with framework-provided TypeScript template.
- Always enable `strict` from day one — retrofitting is painful.
- Set up path aliases early — hard to add cleanly later.
- Add runtime validation (Zod) alongside TypeScript types.

## Interview Tip:
This question tests whether you think about TypeScript holistically — not just types but the whole development experience. Mentioning Zod, monorepo types sharing, and CI type-checking shows senior judgment.

---

## Part 5 — Functions & Advanced Types (101–120)

---

## Question 101: What are function overloads?

## Answer:
Function overloads let you define multiple signatures for the same function. Each signature describes a different set of input and output types. The actual implementation handles all cases but has a broader signature.

```ts
function format(value: string): string;
function format(value: number): string;
function format(value: string | number): string {
  return String(value);
}
```

## Key Points:
- Multiple declaration signatures above the implementation.
- Implementation signature is not public — only the overloads are.
- TypeScript selects the correct signature based on the call.
- Used when input/output types vary in non-union ways.

## Interview Tip:
Mention when to use overloads vs union types. Use overloads when the relationship between input and output type varies — e.g., when `string` in means `string` out, and `number` in means `number[]` out.

---

## Question 102: How do function overloads work?

## Answer:
TypeScript resolves overloads by matching the call against each signature in order, top to bottom. The first matching signature wins. The implementation function is what actually runs — it must handle all the overload cases.

The implementation signature is hidden from callers — they only see the overload signatures.

## Key Points:
- Signatures are matched top-to-bottom.
- Implementation must be compatible with all overloads.
- Implementation signature is not visible to callers.
- Order matters — more specific signatures should come first.

## Interview Tip:
Mention that if no overload matches, TypeScript shows an error — even if the implementation would handle the call. This is why implementation must be broader than all overloads.

---

## Question 103: When should you use overloads instead of union types?

## Answer:
Use overloads when the output type depends on the specific input type in a non-union way. If `string` in always means `string` out and `number` in always means `number` out, a union return type `string | number` is too broad.

```ts
// With overloads — precise:
function process(x: string): string;
function process(x: number): number;

// With union — too broad:
function process(x: string | number): string | number;
// Caller gets string | number even when passing a string
```

## Key Points:
- Use overloads for conditional input-output type relationships.
- Union types are simpler but less precise.
- Overloads give callers precise return types based on input.
- Don't use overloads just because you have multiple input types.

## Interview Tip:
The key differentiator: "does the return type depend on the input type?" If yes, use overloads. If not, union types are simpler and cleaner.

---

## Question 104: What are generic functions?

## Answer:
Generic functions use type parameters to work with different types while maintaining type safety. The type is inferred from the arguments when the function is called.

```ts
function wrap<T>(value: T): { data: T } {
  return { data: value };
}
wrap("hello");  // { data: string }
wrap(42);       // { data: number }
```

## Key Points:
- Type parameters are declared in angle brackets: `<T>`.
- TypeScript infers the type from the argument — no need to specify explicitly.
- Generic functions are reusable across many types.
- Multiple type parameters are possible: `<T, U>`.

## Interview Tip:
Build on this by showing a real utility function — like a type-safe `fetch` wrapper with generic response type. It's a common pattern every full-stack developer uses.

---

## Question 105: What are generic interfaces?

## Answer:
Generic interfaces define contracts that work with different types. You specify the type parameter when implementing or using the interface.

```ts
interface Repository<T> {
  findById(id: string): Promise<T>;
  findAll(): Promise<T[]>;
  save(entity: T): Promise<T>;
  delete(id: string): Promise<void>;
}

class UserRepo implements Repository<User> {
  async findById(id: string): Promise<User> { return {} as User; }
  async findAll(): Promise<User[]> { return []; }
  async save(entity: User): Promise<User> { return entity; }
  async delete(id: string): Promise<void> {}
}
```

## Key Points:
- Type parameter defined at the interface level.
- Implementing class provides the concrete type.
- Creates a reusable contract pattern for repositories, services, etc.
- Multiple implementations can share the same interface contract.

## Interview Tip:
The Repository pattern is a very common real-world example. If you've used it in projects (especially with Prisma or TypeORM), mention it.

---

## Question 106: What are generic classes?

## Answer:
Generic classes use type parameters at the class level. The type is specified when creating an instance of the class.

```ts
class Stack<T> {
  private items: T[] = [];
  push(item: T): void { this.items.push(item); }
  pop(): T | undefined { return this.items.pop(); }
  peek(): T | undefined { return this.items[this.items.length - 1]; }
}

const numStack = new Stack<number>();
numStack.push(1);
numStack.push(2);
```

## Key Points:
- Type parameter declared on the class: `class Foo<T>`.
- All methods and properties can use the type parameter.
- Type is bound at instantiation time.
- Can have multiple type parameters: `class Map<K, V>`.

## Interview Tip:
The Stack or Queue data structure is a classic generic class example. It clearly shows why generics are needed — you want a type-safe stack that works for any type.

---

## Question 107: What are generic type aliases?

## Answer:
Type aliases can be generic, allowing you to create reusable type templates with type parameters.

```ts
type ApiResponse<T> = {
  data: T;
  error: string | null;
  status: number;
};

type UserResponse = ApiResponse<User>;
type PostResponse = ApiResponse<Post[]>;
```

## Key Points:
- Use angle brackets after the type name: `type Foo<T>`.
- Can use multiple type parameters.
- Very common for API response wrappers, paginated results, and state types.
- Combined with conditional or mapped types for powerful patterns.

## Interview Tip:
`ApiResponse<T>` is the most common real-world generic type alias. Every developer who's worked with APIs has built something like this.

---

## Question 108: What are generic constraints? (Detailed)

## Answer:
Generic constraints limit what types a generic accepts using `extends`. Without constraints, `T` can be anything, so you can't access any properties. With constraints, you guarantee certain properties exist.

```ts
function getProperty<T, K extends keyof T>(obj: T, key: K): T[K] {
  return obj[key];
}
getProperty({ name: "Alice" }, "name"); // "Alice" — type safe
getProperty({ name: "Alice" }, "email"); // Error! "email" not in type
```

## Key Points:
- `<T extends SomeType>` restricts what T can be.
- Allows accessing properties that the constraint guarantees.
- Common constraints: `extends object`, `extends string`, `extends keyof T`.
- The constraint is checked at call site.

## Interview Tip:
The `<T, K extends keyof T>` pattern is a classic TypeScript interview question. Being able to write and explain `getProperty` shows strong TypeScript fundamentals.

---

## Question 109: What is the `extends` keyword in generics?

## Answer:
In generics, `extends` creates a constraint — it means "T must be assignable to this type." In conditional types, `extends` means "if T is assignable to this type."

```ts
// As constraint:
function log<T extends { toString(): string }>(val: T): void { console.log(val.toString()); }

// In conditional type:
type IsArray<T> = T extends any[] ? "array" : "not array";
```

## Key Points:
- In generics: `T extends X` constrains T to be a subtype of X.
- In conditional types: `T extends X ? A : B` checks assignability.
- Both uses are about type compatibility, not classical inheritance.
- Very overloaded keyword — context determines meaning.

## Interview Tip:
Clarify that `extends` in TypeScript generics is about structural compatibility, not class inheritance. This distinction trips many candidates up.

---

## Question 110: What is a default generic type?

## Answer:
Default generic types provide a fallback type when a generic parameter is not specified. Similar to default function parameters.

```ts
interface ApiResponse<T = unknown> {
  data: T;
  status: number;
}

const res: ApiResponse = { data: "hello", status: 200 };
// T defaults to unknown
const typed: ApiResponse<User> = { data: {} as User, status: 200 };
```

## Key Points:
- Syntax: `<T = DefaultType>`.
- Used when a generic type has a sensible default.
- Makes the generic optional for callers.
- Common for library types where flexibility is needed.

## Interview Tip:
`unknown` is a safe default for data types since it forces explicit handling. Mentioning this shows you think about safety, not just convenience.

---

## Question 111: What is covariance?

## Answer:
Covariance means a type `A<Subtype>` is assignable to `A<Supertype>` when `Subtype` extends `Supertype`. In simpler terms, you can use a more specific type where a more general type is expected.

Arrays in TypeScript are covariant — a `string[]` can be assigned to an `(string | number)[]`.

## Key Points:
- Covariant: subtype can be used in place of supertype.
- TypeScript arrays and function return types are covariant.
- Reading from a structure is typically covariant (safe).
- Writing to a structure with covariance can be unsafe.

## Interview Tip:
This is an advanced concept. Mention that TypeScript uses structural typing, which affects how variance works. Understanding covariance shows senior-level type system knowledge.

---

## Question 112: What is contravariance?

## Answer:
Contravariance is the opposite — a type is assignable in the reverse direction. Function parameters are contravariant: a function accepting a broader type can be used where a function expecting a narrower type is needed.

```ts
type Handler<T> = (val: T) => void;
// A handler for Animal can be used where a handler for Dog is needed
// because it can handle anything a Dog handler would receive
```

## Key Points:
- Contravariant: supertype can be used in place of subtype.
- Function parameters are contravariant in TypeScript (with `strictFunctionTypes`).
- Writing to structures is typically contravariant.
- `strictFunctionTypes` enforces correct variance for function parameters.

## Interview Tip:
Contravariance is notoriously hard to explain. Use the "function parameters" angle — it's the most relatable example. `strictFunctionTypes` enforcing this is worth mentioning.

---

## Question 113: What is bivariance?

## Answer:
Bivariance means a type is assignable in both directions — both covariant and contravariant. TypeScript historically used bivariance for method parameters, which is less type-safe but more flexible. `strictFunctionTypes` fixed this for function properties but not methods.

## Key Points:
- Bivariant: assignable in both covariant and contravariant directions.
- TypeScript methods (defined with `method(): void`) are still bivariant.
- Function properties (`prop: () => void`) are checked strictly.
- Bivariance sacrifices safety for compatibility.

## Interview Tip:
This is very advanced — understanding it shows deep TypeScript knowledge. Mention that the `strictFunctionTypes` option only applies to function type literals, not method signatures. This is a known quirk.

---

## Question 114: What is type variance?

## Answer:
Type variance describes how a generic type `A<T>` relates to `A<U>` when `T` is a subtype of `U`. There are four kinds: covariant (same direction), contravariant (opposite direction), bivariant (both), and invariant (neither).

TypeScript primarily uses structural compatibility to determine assignability, which influences variance behavior.

## Key Points:
- Variance determines assignability of generic types.
- Covariant: read-only positions (return types).
- Contravariant: write-only positions (function parameters).
- Invariant: both read and write (e.g., mutable containers).

## Interview Tip:
Understanding variance at this level is impressive in interviews. Frame it practically: "return types can be specialized (covariant), parameters should be generalized (contravariant)."

---

## Question 115: What is structural typing?

## Answer:
Structural typing means TypeScript checks the shape of a type, not its name. If two types have the same properties and types, they're considered compatible — even if they have different names.

```ts
interface Point { x: number; y: number }
class Vector { constructor(public x: number, public y: number) {} }

const p: Point = new Vector(1, 2); // Works! Same shape
```

## Key Points:
- TypeScript checks structure, not type identity or name.
- If shapes match, types are compatible.
- Different from nominal typing (Java, C#) where name matters.
- Enables flexible duck typing patterns.

## Interview Tip:
Compare with nominal typing in Java/C# where you'd get a type error. TypeScript's structural approach is more flexible but requires discipline to avoid accidental compatibility.

---

## Question 116: What is nominal typing?

## Answer:
Nominal typing means type compatibility is determined by name, not structure. Two types with the same shape are still different types. TypeScript doesn't natively do this, but you can simulate it with branded types.

```ts
type UserId = string & { readonly __brand: "UserId" };
type ProductId = string & { readonly __brand: "ProductId" };
// Now you can't accidentally pass a ProductId where a UserId is expected
```

## Key Points:
- Nominal typing: types are compatible only if they have the same name.
- TypeScript is structurally typed by default.
- Branded types simulate nominal typing in TypeScript.
- Useful for distinguishing semantically different but structurally equal types.

## Interview Tip:
Branded types are a real-world pattern — mention you've used them for IDs (UserId, OrderId) to prevent accidentally swapping ID values. It's a practical answer that impresses interviewers.

---

## Question 117: Why does TypeScript use structural typing?

## Answer:
Because JavaScript is structurally typed by nature — you can pass any object to a function as long as it has the expected properties. TypeScript was designed to type-check JavaScript code, so it follows JavaScript's duck-typing conventions.

Structural typing also makes it easier to work with third-party libraries — you don't need to explicitly implement an interface to satisfy it.

## Key Points:
- TypeScript reflects JavaScript's duck-typing behavior.
- No need to explicitly declare that a class implements an interface.
- Makes integrating with external code easier.
- Can lead to accidental structural compatibility — use branded types to prevent this.

## Interview Tip:
Frame this as "TypeScript embraced JavaScript's nature rather than fighting it." This shows you understand why the language made this design choice.

---

## Question 118: What is duck typing?

## Answer:
Duck typing means "if it walks like a duck and quacks like a duck, it's a duck." In programming, if an object has the required methods and properties, it's accepted as the expected type — regardless of its declared type.

TypeScript's structural typing is essentially compile-time duck typing.

```ts
function makeSound(animal: { speak(): void }) {
  animal.speak();
}
makeSound({ speak: () => console.log("woof") }); // Works!
```

## Key Points:
- Compatibility based on shape, not declared type.
- TypeScript applies this at the type level.
- Very flexible — any object with the right shape works.
- Origin: Python community term (James Whitcomb Riley).

## Interview Tip:
Duck typing is mostly a conceptual question. Keep the answer short and give the example. Connecting it to TypeScript's structural typing is the key insight.

---

## Question 119: What is type compatibility?

## Answer:
Type compatibility determines when a type can be used in place of another. In TypeScript, type `A` is compatible with type `B` if `A` has at least all the properties that `B` has (structural compatibility).

```ts
interface Animal { name: string }
interface Dog { name: string; breed: string }

let animal: Animal;
let dog: Dog = { name: "Rex", breed: "Labrador" };
animal = dog; // OK — Dog has everything Animal needs
// dog = animal; // Error — Animal doesn't have 'breed'
```

## Key Points:
- TypeScript uses structural compatibility.
- A type with more properties is compatible with a type requiring fewer.
- Function compatibility involves checking parameters and return types.
- Compatibility is checked at every assignment and function call.

## Interview Tip:
The Animal/Dog example is perfect — it shows assignability clearly. Direction matters: you can assign a "more specific" type to a "less specific" type, but not vice versa.

---

## Question 120: How does TypeScript determine assignability?

## Answer:
TypeScript checks if the source type has all the properties required by the target type. For objects, every required property in the target must exist in the source with a compatible type. For functions, parameters are checked contravariantly and return types covariantly.

```ts
type A = { x: number; y: number };
type B = { x: number };
const a: A = { x: 1, y: 2 };
const b: B = a; // OK — A has more properties than B needs
```

## Key Points:
- Object assignability: source must have all required target properties.
- Extra properties in source are allowed.
- Function parameters: checked in reverse (contravariant).
- Return types: checked in forward direction (covariant).

## Interview Tip:
Mention excess property checking — when assigning an object literal directly, TypeScript also checks for extra properties. But when assigning through a variable, the check is purely structural. This is a subtle but common gotcha.

---

## Part 6 — Advanced Type System (121–140)

---

## Question 121: What are recursive types?

## Answer:
Recursive types reference themselves in their own definition. They're used for tree structures, nested data, or anything that can contain more of itself.

```ts
type JSONValue =
  | string
  | number
  | boolean
  | null
  | JSONValue[]
  | { [key: string]: JSONValue };
```

## Key Points:
- A type that references itself.
- Used for trees, JSON, nested objects, linked lists.
- TypeScript supports recursive type aliases (since TS 3.7).
- Can be combined with conditional types for recursive type operations.

## Interview Tip:
The JSON type example is perfect and practical. Every developer has dealt with JSON parsing — showing you can type it precisely is impressive.

---

## Question 122: What are recursive conditional types?

## Answer:
Recursive conditional types use `infer` and self-reference to deeply transform types. They're used for things like deeply unwrapping Promises or flattening nested arrays at the type level.

```ts
type DeepPartial<T> = T extends object
  ? { [K in keyof T]?: DeepPartial<T[K]> }
  : T;
```

## Key Points:
- Conditional type that references itself for recursive cases.
- Used for deep transformations: `DeepPartial`, `DeepReadonly`.
- Can cause performance issues if deeply nested.
- TypeScript has tail-call optimization for some recursive types.

## Interview Tip:
`DeepPartial` is the most common practical example. Mention you've used it for deeply nested configuration objects or form state where you need all nested properties optional.

---

## Question 123: What is distributive conditional typing?

## Answer:
When a conditional type is used with a generic type that's a union, TypeScript automatically distributes the conditional over each union member.

```ts
type ToArray<T> = T extends any ? T[] : never;
type Result = ToArray<string | number>;
// Distributes to: ToArray<string> | ToArray<number>
// Result: string[] | number[]
```

## Key Points:
- Applies automatically when T is a bare type parameter.
- Distributes over union types member by member.
- Used in `Exclude`, `Extract`, `NonNullable` implementations.
- Can be prevented by wrapping T: `[T] extends [U]`.

## Interview Tip:
Preventing distribution with `[T] extends [U]` is a good advanced point. It shows you know the edge cases and not just the basic behavior.

---

## Question 124: What is the `infer` keyword used for? (Detailed)

## Answer:
`infer` captures a type variable within a conditional type. It lets TypeScript "pull out" part of a type and give it a name so you can use it in the result.

```ts
type UnpackPromise<T> = T extends Promise<infer U> ? U : T;
type A = UnpackPromise<Promise<string>>; // string
type B = UnpackPromise<number>;          // number (not a Promise)
```

## Key Points:
- Only valid inside `extends` clauses in conditional types.
- `infer R` creates a new type variable `R` to capture part of the type.
- Used in `ReturnType`, `Parameters`, `Awaited` implementations.
- Can capture multiple types in one conditional type.

## Interview Tip:
Implementing `ReturnType<T>` or `UnpackPromise<T>` manually is a great interview exercise. It shows you understand `infer` deeply, not just how to use built-in utility types.

---

## Question 125: How does type inference work?

## Answer:
TypeScript analyzes the code and determines types automatically from context. It infers variable types from their initial values, function return types from the return statement, and generic types from the arguments passed.

```ts
const arr = [1, 2, 3];          // inferred as number[]
const obj = { name: "Alice" };  // inferred as { name: string }
const doubled = arr.map(n => n * 2); // inferred as number[]
```

## Key Points:
- Inference happens at assignment, function calls, and return statements.
- TypeScript infers the "widest" safe type from initial values.
- Inference flows bidirectionally in some cases (contextual typing).
- Explicit annotations override inference.

## Interview Tip:
Mention contextual typing — when the expected type is known from context (like an event handler), TypeScript infers parameter types automatically. This is a nice advanced detail.

---

## Question 126: What is contextual typing?

## Answer:
Contextual typing is when TypeScript infers a type based on the context it's being used in, not from the value itself. If a function parameter's type is known from the expected type, TypeScript infers the parameter types automatically.

```ts
const button = document.getElementById("btn");
button?.addEventListener("click", (event) => {
  // 'event' is automatically typed as MouseEvent — no annotation needed
  console.log(event.clientX);
});
```

## Key Points:
- TypeScript infers types from the surrounding context.
- Very common with callbacks — event handlers, array methods.
- Reduces the need for explicit type annotations.
- Part of TypeScript's bidirectional type inference.

## Interview Tip:
The event handler example is perfect. Every frontend developer has used this without realizing it's called "contextual typing." Naming it correctly impresses interviewers.

---

## Question 127: What is control flow analysis?

## Answer:
Control flow analysis means TypeScript tracks what type a variable must be at each point in the code based on the control flow (if statements, return statements, throw, etc.).

```ts
function process(value: string | null) {
  if (value === null) return;
  // TypeScript knows value is string here — null was ruled out
  console.log(value.toUpperCase()); // Safe!
}
```

## Key Points:
- TypeScript narrows types automatically based on control flow.
- Works with `if`, `switch`, `while`, `return`, `throw`.
- TypeScript tracks "what can't be here anymore" after a check.
- Powers all type narrowing behavior.

## Interview Tip:
This is what makes TypeScript's type narrowing so powerful. Mention early returns and guard clauses — they're idiomatic TypeScript patterns that leverage control flow analysis.

---

## Question 128: What is exhaustive type checking?

## Answer:
Exhaustive checking ensures you've handled every case of a union type. Using `never` at the end of a switch statement, TypeScript will error if you add a new union member without handling it.

```ts
type Shape = "circle" | "rect" | "triangle";
function area(shape: Shape): number {
  switch (shape) {
    case "circle": return Math.PI;
    case "rect": return 1;
    case "triangle": return 0.5;
    default:
      const _exhaustive: never = shape; // Error if any shape is unhandled!
      throw new Error("Unhandled shape");
  }
}
```

## Key Points:
- Assign the unmatched case to a `never` variable.
- TypeScript errors if any union members are unhandled.
- Forces you to update all switch statements when adding new types.
- Critical for discriminated unions and state machines.

## Interview Tip:
This pattern directly prevents a class of runtime bugs — forgetting to handle a new enum/union member. Showing this in an interview demonstrates production-quality TypeScript thinking.

---

## Question 129: What is the `satisfies` operator?

## Answer:
`satisfies` (TypeScript 4.9+) validates that a value conforms to a type without widening the type. Unlike a type annotation, it preserves the literal/inferred type for further use.

```ts
type Colors = "red" | "blue" | "green";
const palette = {
  red: [255, 0, 0],
  blue: "#0000FF",
} satisfies Record<Colors, string | number[]>;

// palette.red is still inferred as number[], not string | number[]
```

## Key Points:
- Validates type without losing specific inferred type.
- Different from `as` (no override) and `: Type` (no widening).
- Introduced in TypeScript 4.9.
- Great for config objects where you want validation plus inference.

## Interview Tip:
`satisfies` is relatively new and shows you're up to date with TypeScript. Explaining the difference from a type annotation is the key insight — validation without widening.

---

## Question 130: What is declaration merging? (Detailed)

## Answer:
Declaration merging is when TypeScript combines multiple declarations of the same name into one. It applies to interfaces, namespaces, and some function/class combinations. If you declare the same interface twice, TypeScript merges the properties.

```ts
interface Window { myCustomProp: string }
// Now window.myCustomProp is typed — merged with the built-in Window
```

## Key Points:
- Works for interfaces, namespaces, and enum + namespace combinations.
- Does NOT work for type aliases — they must be unique.
- Used for augmenting library types (Express, Window, etc.).
- Essential for `@types` packages to extend existing types.

## Interview Tip:
This is the same concept as interface merging. Mention the practical use case of extending global types from third-party libraries.

---

## Question 131: What are ambient declarations?

## Answer:
Ambient declarations tell TypeScript about the type of something that exists in the JavaScript environment but isn't defined in the TypeScript code. They describe existing JavaScript APIs.

```ts
declare const __DEV__: boolean; // Tells TS this global exists
declare function jQuery(selector: string): any; // jQuery declared globally
```

## Key Points:
- Use `declare` keyword — no implementation, just type information.
- Used in `.d.ts` files to describe JavaScript environments.
- `declare global { }` for global scope augmentations.
- Common in configuration files like `env.d.ts` in Vite projects.

## Interview Tip:
Vite uses `env.d.ts` with ambient declarations for `import.meta.env` — mentioning this shows real-world TypeScript experience with modern tooling.

---

## Question 132: What is `declare`?

## Answer:
`declare` tells TypeScript "this exists somewhere in JavaScript — trust me on the type, but don't generate any code for it." It's used for ambient declarations, global variables, and type-only declarations.

```ts
declare const API_URL: string;        // Global exists at runtime
declare module "*.png" { const url: string; export default url; } // Module type
declare function fetch(url: string): Promise<Response>;
```

## Key Points:
- No code is emitted — purely type information.
- Used in `.d.ts` files and for global augmentation.
- `declare module` for typing non-code imports (images, CSS).
- Essential for bridging JavaScript environments with TypeScript.

## Interview Tip:
The image import declaration (`declare module "*.png"`) is a practical example from every webpack/Vite project. Interviewers appreciate when you connect abstract concepts to real tooling.

---

## Question 133: What is a declaration file (`.d.ts`)? (Detailed)

## Answer:
`.d.ts` files are pure TypeScript type declarations with no implementation. They describe the types of JavaScript code — both code you've written and third-party libraries. TypeScript uses them for type checking without compiling the JavaScript itself.

## Key Points:
- Contains only type declarations, no runtime code.
- Generated by `tsc --declaration` or `"declaration": true`.
- `@types/packagename` packages are `.d.ts` files on npm.
- You can write manual `.d.ts` files for untyped JS libraries.

## Interview Tip:
Mention that when TypeScript finds a `.js` file in `node_modules`, it looks for a corresponding `.d.ts` for type information. Understanding this chain shows deep TypeScript knowledge.

---

## Question 134: How do you write custom declaration files?

## Answer:
Create a `.d.ts` file with `declare` statements describing the types. For modules, wrap them in `declare module`.

```ts
// custom-lib.d.ts
declare module "custom-lib" {
  export function init(config: { apiKey: string }): void;
  export function request(url: string): Promise<{ data: any }>;
}
```

Then reference it or let TypeScript discover it via `typeRoots` or `types` in `tsconfig.json`.

## Key Points:
- Use `declare module "package-name"` for module declarations.
- Use `declare global { }` for global augmentation.
- Place in a `types/` folder and reference in `tsconfig.json`.
- Keep it close to the minimum needed — don't over-type everything.

## Interview Tip:
Mention a real scenario — adding types for a legacy JavaScript utility library your team uses. This is a common task for any developer maintaining mixed JS/TS codebases.

---

## Question 135: How do third-party libraries provide types?

## Answer:
Two main ways:
1. **Bundled types**: The library ships its own `.d.ts` files (e.g., Prisma, Zod, Axios). The package includes a `types` field in `package.json`.
2. **DefinitelyTyped**: Separate `@types/packagename` packages on npm maintained by the community (e.g., `@types/react`, `@types/node`).

TypeScript automatically finds both when compiling.

## Key Points:
- Bundled types: types ship with the package itself.
- `@types/` packages: separate community-maintained type definitions.
- `typeRoots` and `types` in tsconfig control where TypeScript looks.
- Some libraries provide both — bundled takes priority.

## Interview Tip:
Mention how to check if a library has bundled types (look for `"types"` in `package.json`) vs needing `@types/`. This shows practical TypeScript setup knowledge.

---

## Question 136: What is DefinitelyTyped?

## Answer:
DefinitelyTyped is a community repository of TypeScript type definitions for JavaScript libraries that don't ship their own types. When you install `@types/express` or `@types/lodash`, you're getting types from DefinitelyTyped.

It's at github.com/DefinitelyTyped/DefinitelyTyped and has thousands of packages.

## Key Points:
- GitHub repository with community-maintained `@types/` packages.
- Separate npm packages: `@types/packagename`.
- Maintained by the TypeScript community, not library authors.
- Quality varies — some packages are excellent, others outdated.

## Interview Tip:
Mention that sometimes `@types` packages lag behind the actual library. In those cases, you may need to write your own augmentation or local declaration files. Real-world experience.

---

## Question 137: What is module augmentation? (Detailed)

## Answer:
Module augmentation extends the types of an existing module without modifying its source. You use `declare module "moduleName"` and add your additions inside.

```ts
// Extending Express Request with user property
import { Request } from "express";
declare module "express" {
  interface Request {
    user?: { id: string; email: string; role: string };
  }
}
```

## Key Points:
- Used to extend types from third-party modules.
- Must be in a module file (has at least one import/export).
- Relies on interface declaration merging.
- Very common for Express, Passport.js, and similar middleware setups.

## Interview Tip:
The Express Request augmentation is something every Node.js TypeScript developer has done. Showing it from memory in an interview is impressive.

---

## Question 138: What is global augmentation?

## Answer:
Global augmentation adds or modifies types in the global scope — things available everywhere without importing. You use `declare global { }` inside a module file.

```ts
// globals.d.ts
export {}; // makes this a module
declare global {
  interface Window {
    myTracker: { track(event: string): void };
  }
}
```

## Key Points:
- Extends global types like `Window`, `Array`, `String`.
- Use `declare global { }` inside a module file.
- Without `export {}`, the file is an ambient module (already global).
- Use carefully — polluting global types can cause confusion.

## Interview Tip:
Mention that global augmentation is powerful but should be used sparingly. Over-augmenting globals makes code harder to maintain and reason about.

---

## Question 139: What is interface merging?

## Answer:
Interface merging is TypeScript combining multiple declarations of the same interface name into a single, merged interface. Both declarations contribute their properties to the final type.

```ts
interface ApiConfig { timeout: number }
interface ApiConfig { baseUrl: string }
// Merged: ApiConfig = { timeout: number; baseUrl: string }
```

This is the mechanism behind extending third-party library types.

## Key Points:
- Same as declaration merging for interfaces.
- Properties from all declarations are combined.
- All declarations must be compatible (no conflicting types).
- Type aliases do NOT merge — they error on duplicate declarations.

## Interview Tip:
Clarify that this only works for interfaces, not type aliases. This is a key practical difference between `type` and `interface`.

---

## Question 140: What is namespace merging?

## Answer:
TypeScript can merge namespaces with each other, and also with classes, enums, and functions. This allows adding static methods to a class or additional values to an enum.

```ts
class Validator { validate(val: string) { return true; } }
namespace Validator {
  export const EMAIL_REGEX = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
}
Validator.EMAIL_REGEX; // Works — namespace merged with class
```

## Key Points:
- Namespaces can merge with classes, enums, and functions.
- Used to add static members or associated values.
- Common in library `.d.ts` files for jQuery-style APIs.
- Less common in modern code — prefer static class members.

## Interview Tip:
This is an advanced topic. Mention it's mostly relevant for typing legacy JavaScript patterns. In modern code, static class members handle the same use cases more cleanly.

---

## Part 7 — Classes & OOP (141–160)

---

## Question 141: How are classes implemented in TypeScript?

## Answer:
TypeScript classes extend JavaScript classes with access modifiers, typed properties, interfaces, and abstract classes. You declare property types in the class body and use access modifiers to control visibility.

```ts
class User {
  private id: string;
  public name: string;
  readonly createdAt: Date;

  constructor(name: string) {
    this.id = Math.random().toString();
    this.name = name;
    this.createdAt = new Date();
  }
}
```

## Key Points:
- Same syntax as JavaScript classes with added type annotations.
- Access modifiers: `public`, `private`, `protected`.
- `readonly` properties can only be set in the constructor.
- TypeScript compiles classes to JavaScript — no runtime class system.

## Interview Tip:
Mention parameter properties as a shorthand — `constructor(public name: string)` is cleaner than declaring then assigning. It's idiomatic TypeScript.

---

## Question 142: What are access modifiers?

## Answer:
Access modifiers control the visibility of class members. TypeScript provides three: `public` (accessible anywhere), `private` (class only), and `protected` (class and subclasses).

```ts
class Account {
  public balance: number = 0;
  private pin: string = "0000";
  protected accountNumber: string = "ACC001";
}
```

## Key Points:
- `public`: default — accessible anywhere.
- `private`: only within the declaring class.
- `protected`: within class and its subclasses.
- TypeScript's `private` is compile-time only — JavaScript's `#` is runtime private.

## Interview Tip:
Mention the difference between TypeScript's `private` keyword and JavaScript's `#` syntax. TypeScript `private` is erased at runtime — the property is still accessible via JavaScript. JavaScript `#` is truly private at runtime.

---

## Question 143: What is `public`?

## Answer:
`public` means the class member is accessible from anywhere — inside the class, subclasses, and external code. It's the default access level in TypeScript, so you often don't need to write it explicitly.

```ts
class Car {
  public brand: string;  // Same as just: brand: string
  constructor(brand: string) { this.brand = brand; }
}
const car = new Car("Toyota");
console.log(car.brand); // Accessible — it's public
```

## Key Points:
- Default access level — optional to write `public` explicitly.
- Accessible from inside the class, subclasses, and instances.
- Part of the public API of your class.
- No runtime difference from regular JavaScript properties.

## Interview Tip:
Since `public` is the default, omitting it is common and acceptable. Explicitly writing it is often done for clarity in code that defines clear APIs.

---

## Question 144: What is `private`?

## Answer:
`private` restricts access to the declaring class only. Subclasses and external code can't access it. It enforces encapsulation at the type-checking level.

```ts
class BankAccount {
  private balance: number = 0;
  deposit(amount: number) { this.balance += amount; }
  getBalance() { return this.balance; } // Controlled access
}
const acc = new BankAccount();
// acc.balance; // Error! 'balance' is private
```

## Key Points:
- Only accessible within the declaring class.
- Not accessible in subclasses (use `protected` for that).
- Compile-time enforcement — erased in JavaScript output.
- For true runtime privacy, use JavaScript's `#` syntax.

## Interview Tip:
Always mention the compile-time limitation. `private` doesn't prevent access via JavaScript at runtime — important for security-sensitive code.

---

## Question 145: What is `protected`?

## Answer:
`protected` allows access within the class and its subclasses, but not from outside. It's useful when you want internal inheritance access but still want to hide from external consumers.

```ts
class Animal {
  protected name: string;
  constructor(name: string) { this.name = name; }
}
class Dog extends Animal {
  bark() { console.log(`${this.name} says woof`); } // Accessible in subclass
}
const d = new Dog("Rex");
// d.name; // Error! protected outside of class hierarchy
```

## Key Points:
- Accessible in declaring class and all subclasses.
- Not accessible from outside the class hierarchy.
- Useful for template method pattern and inheritance.
- Compile-time only — erased in JavaScript output.

## Interview Tip:
Use the template method pattern as a real-world example — a base class with a `protected` method that subclasses can override. This shows OOP depth.

---

## Question 146: What are readonly properties?

## Answer:
`readonly` prevents a property from being reassigned after initialization. The value can only be set in the declaration or the constructor. Useful for immutable data like IDs and creation timestamps.

```ts
class Order {
  readonly id: string;
  readonly createdAt: Date;
  constructor() {
    this.id = Math.random().toString();
    this.createdAt = new Date();
  }
}
const o = new Order();
// o.id = "123"; // Error! Cannot assign to readonly property
```

## Key Points:
- Set only at declaration or in the constructor.
- Type-level only — doesn't freeze the object at runtime.
- Different from `const` — `const` is for variables, `readonly` for properties.
- Common for entity IDs, timestamps, and configuration values.

## Interview Tip:
Clarify that `readonly` doesn't deeply freeze nested objects — only the top-level reference is immutable. For deep immutability at runtime, use `Object.freeze()`.

---

## Question 147: What are parameter properties?

## Answer:
Parameter properties are a TypeScript shorthand that declares and initializes a class property directly from the constructor parameter. Just add an access modifier before the parameter.

```ts
// Without parameter properties:
class User {
  name: string;
  email: string;
  constructor(name: string, email: string) {
    this.name = name;
    this.email = email;
  }
}

// With parameter properties (cleaner):
class User {
  constructor(public name: string, public email: string) {}
}
```

## Key Points:
- Add `public`, `private`, `protected`, or `readonly` before a constructor parameter.
- TypeScript creates the property and assigns the value automatically.
- Significantly reduces boilerplate for simple classes.
- Works with all access modifiers and `readonly`.

## Interview Tip:
This is idiomatic TypeScript — many developers don't know about it. Showing you use parameter properties signals TypeScript maturity and care for code cleanliness.

---

## Question 148: What are abstract classes?

## Answer:
Abstract classes define a blueprint that other classes must implement. They can have implemented methods (shared behavior) and abstract methods (must be implemented by subclasses). You can't instantiate an abstract class directly.

```ts
abstract class Shape {
  abstract area(): number; // Must implement in subclass
  describe() { // Shared implementation
    return `This shape has area: ${this.area()}`;
  }
}
class Circle extends Shape {
  constructor(private radius: number) { super(); }
  area() { return Math.PI * this.radius ** 2; }
}
```

## Key Points:
- Can't be instantiated — only extended.
- Mix of abstract (must implement) and concrete (shared) methods.
- Used for the Template Method design pattern.
- TypeScript-only concept — compiled to a regular class in JavaScript.

## Interview Tip:
Compare with interfaces: abstract classes can have implementation (shared behavior), interfaces cannot. Use abstract classes when subclasses share some code.

---

## Question 149: What are abstract methods?

## Answer:
Abstract methods are method signatures inside abstract classes that have no implementation. Every non-abstract subclass must provide a concrete implementation.

```ts
abstract class Repository<T> {
  abstract findById(id: string): Promise<T>;
  abstract save(entity: T): Promise<void>;

  async findOrFail(id: string): Promise<T> {
    const entity = await this.findById(id);
    if (!entity) throw new Error("Not found");
    return entity;
  }
}
```

## Key Points:
- Declared with `abstract` keyword — no implementation body.
- Only allowed inside abstract classes.
- All concrete subclasses must implement them.
- TypeScript enforces this at compile time.

## Interview Tip:
The Repository example is strong — it shows abstract methods enabling the Template Method pattern, where the abstract class defines the algorithm structure and subclasses provide specifics.

---

## Question 150: What are interfaces with classes?

## Answer:
A class can implement an interface using the `implements` keyword. TypeScript checks that the class satisfies the interface contract. Unlike abstract classes, interfaces add no implementation — they're pure contracts.

```ts
interface Serializable {
  serialize(): string;
  deserialize(data: string): void;
}

class User implements Serializable {
  serialize() { return JSON.stringify(this); }
  deserialize(data: string) { Object.assign(this, JSON.parse(data)); }
}
```

## Key Points:
- `implements` keyword for class-interface relationship.
- A class can implement multiple interfaces.
- Interface adds no runtime code — purely type checking.
- Better than abstract classes when no shared implementation is needed.

## Interview Tip:
Mention that a class can implement multiple interfaces but only extend one class. This is often the deciding factor between using an abstract class vs an interface.

---

## Question 151: What is `implements`?

## Answer:
`implements` declares that a class must satisfy the contract of an interface. TypeScript checks all required properties and methods are present and correctly typed.

```ts
interface Logger {
  log(message: string): void;
  error(message: string): void;
}

class ConsoleLogger implements Logger {
  log(message: string) { console.log(message); }
  error(message: string) { console.error(message); }
}
```

## Key Points:
- Syntax: `class MyClass implements Interface1, Interface2`.
- Can implement multiple interfaces.
- `implements` is a TypeScript-only check — erased in output JS.
- Doesn't add interface methods — you must implement them yourself.

## Interview Tip:
Mention that `implements` is purely a type-level assertion. The JavaScript class has no knowledge of the interface at runtime. This is an important distinction from languages like Java.

---

## Question 152: What is `extends` in classes?

## Answer:
`extends` creates a class that inherits from another class. The child class gets all public and protected members of the parent and can override or extend them.

```ts
class Animal {
  constructor(public name: string) {}
  speak() { return `${this.name} makes a sound`; }
}

class Dog extends Animal {
  speak() { return `${this.name} barks`; } // Override
  fetch() { return `${this.name} fetches!`; } // New method
}
```

## Key Points:
- Single inheritance only — can only extend one class.
- `super()` must be called in the constructor before `this`.
- Overriding methods: child method replaces parent.
- TypeScript checks that overrides are type-compatible.

## Interview Tip:
Compare `extends` (class inheritance) with `implements` (interface contract). One provides shared code, the other provides a type contract. Knowing when to use which is key.

---

## Question 153: What are static members?

## Answer:
Static members belong to the class itself, not to instances. They're shared across all instances and accessed via the class name.

```ts
class UserService {
  private static instance: UserService;
  private constructor() {}

  static getInstance(): UserService {
    if (!UserService.instance) {
      UserService.instance = new UserService();
    }
    return UserService.instance;
  }
}
```

## Key Points:
- Accessed with `ClassName.property`, not `this.property`.
- Shared across all instances — not per-instance data.
- Common for singleton patterns, factory methods, constants.
- `static` compiles to a property on the constructor function in JavaScript.

## Interview Tip:
The Singleton pattern is the classic static member example. If you've implemented it in a real project (like a database connection pool), mention it.

---

## Question 154: What are getters?

## Answer:
Getters are special methods that look like property accesses but run code when accessed. They're defined with the `get` keyword.

```ts
class Circle {
  constructor(private _radius: number) {}

  get radius() { return this._radius; }

  get area() {
    return Math.PI * this._radius ** 2;
  }
}
const c = new Circle(5);
console.log(c.area); // 78.54... — called like a property
```

## Key Points:
- Defined with `get` keyword.
- Called without parentheses — looks like a property access.
- Can compute derived values on the fly.
- Useful for lazy initialization and computed properties.

## Interview Tip:
Getters are great for computed properties and controlled access to internal state. Mention they can also cache expensive computations.

---

## Question 155: What are setters?

## Answer:
Setters run code when a property is assigned. They're defined with the `set` keyword and are useful for validation before storing a value.

```ts
class Temperature {
  private _celsius: number = 0;

  get celsius() { return this._celsius; }

  set celsius(value: number) {
    if (value < -273.15) throw new Error("Below absolute zero!");
    this._celsius = value;
  }
}
const t = new Temperature();
// t.celsius = -300; // Throws error
t.celsius = 100; // OK
```

## Key Points:
- Defined with `set` keyword.
- Runs when property is assigned.
- Perfect for validation, transformation, or side effects on assignment.
- If a setter exists, usually a getter should exist too.

## Interview Tip:
The validation use case is the strongest example. Show how setters enforce business rules (like valid temperature range) without exposing the internal property directly.

---

## Question 156: What are decorators? (Classes context)

## Answer:
Decorators are functions that can modify or annotate classes, methods, properties, or parameters. They use the `@` syntax and are applied at class definition time. They're central to frameworks like NestJS and Angular.

```ts
function injectable(target: Function) {
  Reflect.defineMetadata("injectable", true, target);
}

@injectable
class UserService {
  getUser(id: string) { return { id }; }
}
```

## Key Points:
- Applied at class definition, not instance creation.
- Four types: class, method, property, parameter decorators.
- Require `"experimentalDecorators": true` in tsconfig (pre-TS5).
- TypeScript 5.0 introduced a new standard-aligned decorator API.

## Interview Tip:
NestJS is the best real-world example — it uses decorators for dependency injection, route handlers, and validation (`@Injectable()`, `@Get()`, `@Body()`). If you know NestJS, mention it.

---

## Question 157: What are property decorators?

## Answer:
Property decorators are applied to class properties. They receive the class prototype and the property name. Often used for metadata, validation, or transformation.

```ts
function Validate(target: any, propertyKey: string) {
  // Add validation metadata
  Reflect.defineMetadata("validate", true, target, propertyKey);
}

class User {
  @Validate
  email: string = "";
}
```

## Key Points:
- Receives `(target, propertyKey)` as arguments.
- Can't directly modify the property value (use descriptors for that).
- Used for ORM column definitions (TypeORM's `@Column()`).
- Common in validation libraries for schema definition.

## Interview Tip:
TypeORM's `@Column()`, `@PrimaryGeneratedColumn()` are classic property decorator examples. Any backend developer who's used TypeORM will relate to this immediately.

---

## Question 158: What are method decorators?

## Answer:
Method decorators are applied to class methods. They receive the class prototype, method name, and property descriptor. They can wrap or replace the method entirely.

```ts
function Log(target: any, key: string, descriptor: PropertyDescriptor) {
  const original = descriptor.value;
  descriptor.value = function (...args: any[]) {
    console.log(`${key} called with`, args);
    return original.apply(this, args);
  };
  return descriptor;
}

class ApiService {
  @Log
  fetchUser(id: string) { return { id }; }
}
```

## Key Points:
- Receives `(target, propertyKey, descriptor)`.
- Can wrap, replace, or augment the method.
- Common for logging, authorization, caching, and rate limiting.
- Used heavily in NestJS for `@Get()`, `@Post()`, guards, and interceptors.

## Interview Tip:
Method decorators are the most powerful and most commonly used decorators. The logging example is simple and clear for interviews.

---

## Question 159: What are class decorators?

## Answer:
Class decorators are applied to the entire class constructor. They receive the class constructor as the argument and can modify or replace the class.

```ts
function Singleton<T extends new (...args: any[]) => {}>(constructor: T) {
  let instance: any;
  return class extends constructor {
    constructor(...args: any[]) {
      if (instance) return instance;
      super(...args);
      instance = this;
    }
  } as T;
}

@Singleton
class Database { connect() { console.log("connected"); } }
```

## Key Points:
- Applied to the class constructor function.
- Can wrap, replace, or augment the entire class.
- Used for dependency injection, singleton patterns, and metadata.
- In NestJS: `@Controller()`, `@Injectable()`, `@Module()` are class decorators.

## Interview Tip:
The Singleton decorator is a clean example. Mention NestJS's `@Injectable()` which marks classes for the DI container — it's the most widely used class decorator in the Node.js ecosystem.

---

## Question 160: When should you use classes instead of interfaces?

## Answer:
Use classes when you need:
- Actual implementation code (methods with logic).
- Constructor logic and initialization.
- Inheritance with shared behavior.
- Decorators (which only apply to classes).
- `instanceof` checks at runtime.

Use interfaces when you only need a type contract with no implementation.

## Key Points:
- Classes produce runtime JavaScript code.
- Interfaces are erased at compile time — zero runtime cost.
- Use classes for entities, services, and repositories with real logic.
- Use interfaces for defining shapes, contracts, and API types.

## Interview Tip:
The "runtime cost" angle is important. Interfaces are free — they don't exist in the output. Classes always generate code. For pure typing, always prefer interfaces or type aliases.

---

## Part 8 — Modules & Configuration (161–180)

---

## Question 161: What are ES Modules in TypeScript?

## Answer:
ES Modules are the standard JavaScript module system using `import` and `export`. TypeScript supports them fully and adds type information on top.

```ts
// utils.ts
export function add(a: number, b: number): number { return a + b; }
export type AddFn = typeof add;

// main.ts
import { add } from "./utils";
import type { AddFn } from "./utils"; // Type-only import
```

## Key Points:
- `import`/`export` syntax — the JavaScript standard.
- TypeScript adds `import type` for type-only imports.
- Works with all modern bundlers: Vite, Webpack, esbuild.
- Configured via `module` option in tsconfig.

## Interview Tip:
Mention `import type` — it imports only the type, which bundlers can safely eliminate. It's a good practice for type-only imports and shows modern TypeScript knowledge.

---

## Question 162: What is CommonJS?

## Answer:
CommonJS is the older Node.js module system using `require()` and `module.exports`. It was the default in Node.js before ES Modules became the standard.

```ts
// CommonJS style
const express = require("express");
module.exports = { handler };
```

## Key Points:
- Uses `require()` and `module.exports`.
- Default module system in older Node.js projects.
- TypeScript can target CommonJS output via `"module": "CommonJS"`.
- `esModuleInterop: true` helps smooth the CJS/ESM interop.

## Interview Tip:
Mention `esModuleInterop: true` in tsconfig — it enables default imports from CommonJS modules and is almost universally needed. Without it, importing `require`-based packages gets awkward.

---

## Question 163: What is the difference between ES Modules and CommonJS?

## Answer:
- **Loading**: ES Modules are statically analyzed (supports tree-shaking); CommonJS loads dynamically at runtime.
- **Syntax**: ESM uses `import`/`export`; CJS uses `require`/`module.exports`.
- **Async**: ESM supports top-level `await`; CJS doesn't natively.
- **Node.js**: `.mjs` or `"type": "module"` for ESM; `.cjs` or default for CJS.

## Key Points:
- ESM is static and enables tree-shaking; CJS is dynamic.
- ESM is the future standard; CJS is legacy but still dominant in Node.
- Mixing them requires careful interop configuration.
- Vite and Next.js both default to ESM.

## Interview Tip:
Tree-shaking is the key advantage to mention — it's why modern bundlers prefer ES Modules. Dead code elimination only works cleanly with static `import`/`export` analysis.

---

## Question 164: What is `moduleResolution`?

## Answer:
`moduleResolution` tells TypeScript how to find modules when you write an `import` statement. Different settings mimic different module resolution strategies.

Common values:
- `"node"` — classic Node.js resolution.
- `"bundler"` — modern bundler-friendly resolution (TypeScript 5+).
- `"node16"` / `"nodenext"` — for modern Node.js ESM.

## Key Points:
- Controls how TypeScript finds imported modules.
- `"bundler"` is recommended for Vite/Next.js projects.
- `"node16"` / `"nodenext"` for pure Node.js ESM projects.
- Wrong setting causes "module not found" errors even when packages exist.

## Interview Tip:
If someone is getting mysterious import errors in a modern project, `moduleResolution` is often the culprit. Mentioning `"bundler"` for Vite/Next.js shows current knowledge.

---

## Question 165: What is `baseUrl`?

## Answer:
`baseUrl` sets the root directory for resolving non-relative imports. With `baseUrl: "."`, you can import from `src/utils` instead of `../../utils` regardless of where you are in the project.

```json
{ "compilerOptions": { "baseUrl": "." } }
```

```ts
// Instead of: import { add } from "../../utils/math"
import { add } from "utils/math"; // Works with baseUrl
```

## Key Points:
- Makes absolute imports work from the project root.
- Reduces fragile relative path chains.
- Usually set to `"."` or `"src"`.
- Works with `paths` for aliased imports.

## Interview Tip:
Mention that `baseUrl` alone is often not enough — you also need to configure your bundler (Vite, Webpack) to understand the same paths. TypeScript and the runtime must agree.

---

## Question 166: What are path aliases?

## Answer:
Path aliases let you create custom shortcuts for import paths using the `paths` option in tsconfig. Instead of deep relative paths, you use a clean alias.

```json
{
  "compilerOptions": {
    "baseUrl": ".",
    "paths": { "@/*": ["src/*"] }
  }
}
```

```ts
import { Button } from "@/components/Button"; // Instead of "../../components/Button"
```

## Key Points:
- Configured in `tsconfig.json` under `compilerOptions.paths`.
- Requires `baseUrl` to be set.
- Must also be configured in your bundler (Vite's `resolve.alias`, Webpack).
- Improves import readability and makes refactoring easier.

## Interview Tip:
Mention that you need to configure aliases in both TypeScript AND the bundler. Many developers configure tsconfig but forget the bundler, then wonder why their imports break at runtime.

---

## Question 167: What is `paths` in tsconfig?

## Answer:
`paths` is the tsconfig option that maps custom import aliases to actual filesystem paths. It works together with `baseUrl`.

```json
{
  "compilerOptions": {
    "baseUrl": ".",
    "paths": {
      "@components/*": ["src/components/*"],
      "@utils/*": ["src/utils/*"],
      "@types/*": ["src/types/*"]
    }
  }
}
```

## Key Points:
- Maps alias patterns to real paths.
- Supports wildcards for directory matching.
- Requires `baseUrl` to be set first.
- TypeScript-only — bundler must be configured separately.

## Interview Tip:
In Next.js, setting `"paths"` in tsconfig auto-configures the dev server aliases too. In Vite, you need to duplicate the config in `vite.config.ts`. Knowing this difference is practical knowledge.

---

## Question 168: What is `target` in tsconfig?

## Answer:
`target` specifies which version of JavaScript TypeScript should compile to. It affects which modern JavaScript syntax gets downleveled (converted to older JS) and which is left as-is.

```json
{ "compilerOptions": { "target": "ES2020" } }
```

Common values: `"ES5"`, `"ES6"`/`"ES2015"`, `"ES2020"`, `"ESNext"`.

## Key Points:
- Controls the JavaScript version in the output.
- Higher target = less transformation = smaller/faster output.
- Lower target = more browser compatibility = more polyfills needed.
- `target` also determines which built-in APIs TypeScript checks.

## Interview Tip:
`ES2020` or `ESNext` is standard for modern projects. `ES5` is only needed for legacy browser support. Knowing that `target` affects both syntax AND runtime API availability shows deep knowledge.

---

## Question 169: What is `lib` in tsconfig?

## Answer:
`lib` tells TypeScript which built-in JavaScript APIs are available in your environment. It adds type definitions for browser APIs (`DOM`), ES features (`ES2020`), and runtime APIs.

```json
{
  "compilerOptions": {
    "lib": ["ES2020", "DOM", "DOM.Iterable"]
  }
}
```

## Key Points:
- `DOM` includes browser APIs: `window`, `document`, `fetch`, etc.
- Without `DOM`, TypeScript doesn't know about `document.getElementById`.
- Setting `target` also affects default `lib` inclusions.
- Node.js projects typically need `@types/node` instead of `DOM`.

## Interview Tip:
Mention that for Node.js-only projects, you should exclude `DOM` from `lib` and use `@types/node`. Including both can cause conflicts where browser and Node types clash.

---

## Question 170: What is `module` in tsconfig?

## Answer:
`module` specifies the module format TypeScript uses in the output files. Common values: `"CommonJS"` for Node.js, `"ESNext"` for modern bundlers, `"NodeNext"` for Node.js ESM.

```json
{ "compilerOptions": { "module": "ESNext" } }
```

## Key Points:
- `"CommonJS"` — generates `require()`/`module.exports` output.
- `"ESNext"` — generates `import`/`export` output.
- Must match your runtime's expected module format.
- Works together with `moduleResolution`.

## Interview Tip:
`module` and `moduleResolution` are often confused. `module` affects output format; `moduleResolution` affects how imports are resolved during type checking. They're related but different settings.

---

## Question 171: What is `strictNullChecks`?

## Answer:
`strictNullChecks` makes `null` and `undefined` not assignable to other types. Without it, you can assign `null` to any variable, silently ignoring potential null reference errors.

```ts
// Without strictNullChecks:
let name: string = null; // Allowed — dangerous

// With strictNullChecks:
// let name: string = null; // Error! Must use: string | null
let safeName: string | null = null; // OK
```

## Key Points:
- Enabled by `strict: true` or explicitly with `"strictNullChecks": true`.
- Forces explicit handling of null and undefined.
- One of the most impactful TypeScript options for bug prevention.
- Prevents the "billion-dollar mistake" — Tony Hoare's null reference errors.

## Interview Tip:
This is one of the most important TypeScript options. Say you always enable it and briefly mention what a null reference error looks like without it. Shows real-world awareness.

---

## Question 172: What is `noImplicitAny`?

## Answer:
`noImplicitAny` forces you to explicitly type any value that TypeScript would otherwise infer as `any`. Without it, TypeScript silently falls back to `any` when it can't infer a type, which defeats the purpose.

```ts
// noImplicitAny: true
// function process(data) { ... } // Error! Parameter 'data' implicitly has 'any' type
function process(data: unknown) { /* ... */ } // OK
```

## Key Points:
- Enabled by `strict: true`.
- Forces explicit type annotations where TypeScript can't infer.
- Prevents silent `any` type spreading.
- Essentially requires you to be intentional about every type.

## Interview Tip:
`noImplicitAny` is one reason to enable `strict: true` from day one. Adding it later to an existing project means touching potentially hundreds of files — painful experience worth mentioning.

---

## Question 173: What is `noUnusedLocals`?

## Answer:
`noUnusedLocals` makes TypeScript error when you have local variables that are declared but never used. Keeps the codebase clean and prevents dead code accumulation.

```ts
function calculate() {
  // const temp = 42; // Error if noUnusedLocals is true and temp is never used
  return 100;
}
```

## Key Points:
- Errors on declared-but-never-used local variables.
- Helps keep codebase clean.
- Not part of `strict` — must be enabled separately.
- Usually combined with `noUnusedParameters`.

## Interview Tip:
Mention this is useful but can be annoying during development when you're mid-refactor. Some teams enable it only in CI, not during local development.

---

## Question 174: What is `noUnusedParameters`?

## Answer:
`noUnusedParameters` errors when function parameters are declared but never used inside the function body. Helps keep function signatures lean and accurate.

```ts
// Prefix with _ to signal "intentionally unused"
function greet(name: string, _greeting: string): string {
  return `Hello, ${name}`;
}
```

## Key Points:
- Errors on declared-but-never-used function parameters.
- Not part of `strict` mode.
- Prefix unused params with `_` to suppress the warning intentionally.
- Combined with `noUnusedLocals` for a clean codebase.

## Interview Tip:
The `_` prefix convention for intentionally unused parameters is a TypeScript idiom worth mentioning. It's widely used for callback parameters you're forced to declare but don't use.

---

## Question 175: What is `skipLibCheck`?

## Answer:
`skipLibCheck: true` tells TypeScript to skip type checking of all `.d.ts` declaration files (including those in `node_modules`). This significantly speeds up compilation.

```json
{ "compilerOptions": { "skipLibCheck": true } }
```

## Key Points:
- Skips type checking of `.d.ts` files in `node_modules`.
- Significantly reduces compilation time in large projects.
- Commonly needed because some `@types` packages have type errors internally.
- Recommended for most projects — you can't fix third-party type errors anyway.

## Interview Tip:
Mention that `skipLibCheck` is nearly universally used. Not having it causes mysterious compile errors from packages you're not responsible for. It's a practical, widely-adopted setting.

---

## Question 176: What is `incremental` compilation?

## Answer:
Incremental compilation (`"incremental": true`) makes TypeScript save compilation state to a `.tsbuildinfo` file. On subsequent builds, TypeScript only recompiles files that have changed, making rebuilds much faster.

```json
{ "compilerOptions": { "incremental": true } }
```

## Key Points:
- Saves compilation state in `.tsbuildinfo` file.
- Subsequent builds skip unchanged files.
- Can significantly reduce CI build times.
- Best combined with `composite: true` for project references.

## Interview Tip:
Add `.tsbuildinfo` to `.gitignore` — it's a build artifact that shouldn't be committed. Mentioning this detail shows you've actually used incremental compilation in production.

---

## Question 177: What is source mapping?

## Answer:
Source maps (`"sourceMap": true`) create `.map` files that link compiled JavaScript back to the original TypeScript source. Debuggers and error tracking tools use them to show you TypeScript code instead of compiled JavaScript.

```json
{ "compilerOptions": { "sourceMap": true } }
```

## Key Points:
- Links JavaScript output back to TypeScript source.
- Enables debugging TypeScript directly in browser devtools.
- Required for error tracking tools (Sentry, Datadog) to show original lines.
- `"inlineSourceMap": true` embeds the map in the JS file instead of separate files.

## Interview Tip:
Mention Sentry or similar error monitoring — source maps are essential for mapping production errors back to TypeScript source lines. Without them, stack traces show minified JS which is unreadable.

---

## Question 178: What is declaration generation?

## Answer:
Declaration generation (`"declaration": true`) makes TypeScript generate `.d.ts` files alongside the compiled JavaScript. These type declaration files allow other TypeScript projects to use your library with full type information.

```json
{ "compilerOptions": { "declaration": true, "declarationDir": "./types" } }
```

## Key Points:
- Needed when publishing a TypeScript library to npm.
- Generates `.d.ts` files consumers can use for type checking.
- `declarationDir` controls where the files are generated.
- The npm package's `types` field in `package.json` points to these files.

## Interview Tip:
If you've published an npm package or a shared internal library, mention that `declaration: true` is required. It shows awareness of TypeScript's library authoring workflow.

---

## Question 179: How do you organize a large TypeScript project?

## Answer:
I follow a feature-based structure rather than type-based (all controllers together, all services together):

```
src/
  features/
    auth/      (routes, controller, service, types)
    users/     (routes, controller, service, types)
    orders/    (...)
  shared/
    types/     (global types)
    utils/     (shared utilities)
    middleware/
  config/
```

Each feature is self-contained — easier to navigate and scale.

## Key Points:
- Feature-based structure scales better than role-based.
- Co-locate types with the feature that owns them.
- Shared types go in a top-level `types/` or `shared/` folder.
- Barrel files (`index.ts`) for clean exports from each folder.

## Interview Tip:
Explaining that you organize by "feature" not "technical layer" shows architectural maturity. Interviewers who've worked on large projects will immediately agree.

---

## Question 180: What is project references?

## Answer:
Project references let you split a large TypeScript project into smaller, independently compilable sub-projects. Each sub-project has its own `tsconfig.json` and they reference each other.

```json
// root tsconfig.json
{
  "references": [
    { "path": "./packages/shared" },
    { "path": "./packages/api" },
    { "path": "./packages/web" }
  ]
}
```

## Key Points:
- Enables incremental compilation per sub-project.
- Required for monorepos with multiple TypeScript packages.
- Each referenced project needs `"composite": true`.
- `tsc --build` respects the dependency graph.

## Interview Tip:
If you've worked in a monorepo (Turborepo, Nx), project references are the TypeScript-native way to handle it. Mention this context to show real-world experience.

---

## Part 9 — React & Node.js with TypeScript (181–190)

---

## Question 181: How do you type React props?

## Answer:
Define props using an interface or type alias and pass it to the component. For function components, you can use `React.FC<Props>` or define the parameter type directly.

```ts
interface ButtonProps {
  label: string;
  onClick: () => void;
  variant?: "primary" | "secondary";
  disabled?: boolean;
}

function Button({ label, onClick, variant = "primary", disabled }: ButtonProps) {
  return <button onClick={onClick} disabled={disabled}>{label}</button>;
}
```

## Key Points:
- Use interface or type alias for props.
- Many teams avoid `React.FC` because it adds implicit `children` typing issues.
- Destructure props directly in the parameter for clean code.
- Optional props should have defaults via destructuring.

## Interview Tip:
Mention why many developers avoid `React.FC<Props>` — in older versions it added `children` as an implicit prop, which was often wrong. Directly typing parameters is cleaner.

---

## Question 182: How do you type React state?

## Answer:
Pass the type as a generic argument to `useState`. TypeScript infers the type from the initial value but you need to be explicit when the initial value doesn't represent all possible states.

```ts
const [user, setUser] = useState<User | null>(null);
const [count, setCount] = useState(0); // Inferred as number
const [status, setStatus] = useState<"idle" | "loading" | "error">("idle");
```

## Key Points:
- `useState<Type>(initialValue)` for explicit typing.
- Inference works when the initial value is representative.
- Use union types for state machines: `"idle" | "loading" | "success" | "error"`.
- `null` initial values always need explicit generic type.

## Interview Tip:
The status state example is a strong answer — it shows you use TypeScript to enforce valid state transitions, not just basic typing.

---

## Question 183: How do you type event handlers in React?

## Answer:
React provides specific event types for each event kind. The generic parameter specifies which HTML element the event belongs to.

```ts
const handleChange = (e: React.ChangeEvent<HTMLInputElement>) => {
  setValue(e.target.value);
};

const handleSubmit = (e: React.FormEvent<HTMLFormElement>) => {
  e.preventDefault();
};

const handleClick = (e: React.MouseEvent<HTMLButtonElement>) => {
  console.log(e.currentTarget.id);
};
```

## Key Points:
- `React.ChangeEvent<HTMLInputElement>` for input changes.
- `React.FormEvent<HTMLFormElement>` for form submissions.
- `React.MouseEvent<HTMLButtonElement>` for click events.
- The generic parameter specifies the DOM element type.

## Interview Tip:
Show you know the generic parameter matters — `React.ChangeEvent<HTMLInputElement>` gives you `e.target.value` typed as a string. Without the generic, you lose that typing.

---

## Question 184: How do you type refs?

## Answer:
Use `useRef<ElementType>(null)` for DOM refs and `useRef<ValueType>(initialValue)` for mutable value refs. The generic specifies what type the ref holds.

```ts
const inputRef = useRef<HTMLInputElement>(null);
const timerRef = useRef<ReturnType<typeof setTimeout>>();

// Usage:
inputRef.current?.focus();
clearTimeout(timerRef.current);
```

## Key Points:
- DOM refs: `useRef<HTMLElement>(null)` — starts as null.
- Value refs: `useRef<Type>(initialValue)`.
- `inputRef.current` is typed as `HTMLInputElement | null`.
- Use optional chaining `?.` when accessing `current`.

## Interview Tip:
`useRef<HTMLInputElement>(null)` with the `null` initial value is the pattern for DOM refs. The `null` is required — TypeScript knows the ref won't be set until the component mounts.

---

## Question 185: How do you type custom hooks?

## Answer:
Type the return value explicitly — either as a tuple (for `useState`-like hooks) or as an object. Use `as const` on tuples to prevent TypeScript from widening them to `(string | function)[]`.

```ts
function useAuth() {
  const [user, setUser] = useState<User | null>(null);
  const login = async (credentials: Credentials) => { /* ... */ };
  const logout = () => setUser(null);
  return { user, login, logout };
}

// If returning a tuple:
function useToggle(initial = false): [boolean, () => void] {
  const [on, setOn] = useState(initial);
  return [on, () => setOn(prev => !prev)];
}
```

## Key Points:
- Explicitly type the return value for clarity.
- Use object return for multiple values — cleaner than long tuples.
- Tuples: add explicit return type or use `as const`.
- Custom hook types should be as precise as possible.

## Interview Tip:
Object return is generally better for more than 2 values — you get named access instead of positional. The `useToggle` tuple example is fine for simple cases.

---

## Question 186: How do you type Context API?

## Answer:
Create a typed context with `createContext`, provide a default value that matches the type, and create a custom hook that handles the undefined case.

```ts
interface AuthContextType {
  user: User | null;
  login: (creds: Credentials) => Promise<void>;
  logout: () => void;
}

const AuthContext = createContext<AuthContextType | undefined>(undefined);

export function useAuth(): AuthContextType {
  const context = useContext(AuthContext);
  if (!context) throw new Error("useAuth must be inside AuthProvider");
  return context;
}
```

## Key Points:
- Use `createContext<Type | undefined>(undefined)` — avoids fake default values.
- Custom hook throws if used outside Provider.
- Keeps consumers from dealing with the `undefined` case.
- The context type is clear and documented through the interface.

## Interview Tip:
The custom hook with the "must be inside Provider" error is the idiomatic pattern. Interviewers will recognize it as mature React + TypeScript usage.

---

## Question 187: How do you type Redux Toolkit?

## Answer:
Redux Toolkit has strong TypeScript support. Define the state type, use `createSlice` (it infers action types), and type the store with `RootState` and `AppDispatch`.

```ts
// store.ts
export type RootState = ReturnType<typeof store.getState>;
export type AppDispatch = typeof store.dispatch;

// hooks.ts
export const useAppSelector = useSelector.withTypes<RootState>();
export const useAppDispatch = useDispatch.withTypes<AppDispatch>();

// In components:
const count = useAppSelector(state => state.counter.value);
```

## Key Points:
- `RootState` derived from store using `ReturnType`.
- `AppDispatch` derived from `typeof store.dispatch`.
- Use typed hooks instead of plain `useSelector`/`useDispatch`.
- `createSlice` infers action types automatically.

## Interview Tip:
The `RootState` and `AppDispatch` derived types pattern is the official Redux Toolkit TypeScript recommendation. Using derived types means they stay in sync automatically as the store changes.

---

## Question 188: How do you type API responses?

## Answer:
Define the expected response shape as an interface and use it when calling `fetch` or Axios. For runtime safety, validate with Zod on the boundary.

```ts
interface Post { id: number; title: string; body: string }

async function fetchPost(id: number): Promise<Post> {
  const res = await fetch(`/api/posts/${id}`);
  if (!res.ok) throw new Error("Failed to fetch");
  return res.json() as Promise<Post>;
}

// Better: With Zod for runtime validation
const PostSchema = z.object({ id: z.number(), title: z.string(), body: z.string() });
// const post = PostSchema.parse(await res.json());
```

## Key Points:
- TypeScript types alone don't validate runtime data.
- `res.json()` returns `any` — cast to your type or validate with Zod.
- Zod provides both runtime validation AND TypeScript type inference.
- `z.infer<typeof Schema>` derives the TypeScript type from the schema.

## Interview Tip:
Always mention that TypeScript can't validate runtime API data — it only checks compile-time. Zod bridges this gap. This shows production maturity, not just TypeScript knowledge.

---

## Question 189: How do you share types between frontend and backend?

## Answer:
In a monorepo, I create a `packages/shared` package with all shared types and import from it on both sides. This ensures the API contract is a single source of truth.

```
packages/
  shared/        # Shared types, schemas, validation
    src/
      types.ts   # User, Post, Order interfaces
      schemas.ts # Zod schemas (shared validation)
  api/           # Backend (imports from shared)
  web/           # Frontend (imports from shared)
```

## Key Points:
- Monorepo shared package is the cleanest solution.
- Zod schemas in shared package give both runtime validation AND TypeScript types.
- Type mismatch between API and client becomes a compile-time error.
- npm workspaces, Turborepo, or Nx manage monorepo dependencies.

## Interview Tip:
This is a "system design within TypeScript" answer. Showing you think about type safety across the full stack — not just in the frontend — is a major differentiator.

---

## Question 190: How do you use TypeScript with Express.js?

## Answer:
Install `@types/express`, type your route handlers explicitly, and augment the `Request` type for custom properties like `req.user`.

```ts
import express, { Request, Response } from "express";

const app = express();

app.get("/users/:id", async (req: Request, res: Response) => {
  const { id } = req.params;
  res.json({ id });
});

// Augment Request for auth middleware
declare module "express" {
  interface Request {
    user?: { id: string; role: string };
  }
}
```

## Key Points:
- `@types/express` provides all Express type definitions.
- Type handlers with `Request`, `Response`, `NextFunction`.
- Augment `Request` for custom properties added by middleware.
- Use typed request bodies with generics: `Request<Params, ResBody, ReqBody, Query>`.

## Interview Tip:
Request augmentation for `req.user` is something every Express + TypeScript developer has done. It's a real-world example that shows practical experience.

---

## Part 10 — Senior Interview Questions (191–200)

---

## Question 191: How would you migrate a large JavaScript project to TypeScript?

## Answer:
Gradually — never all at once. My approach:

1. Add `tsconfig.json` with `allowJs: true`, `strict: false`, `noImplicitAny: false`.
2. Rename highest-value files to `.ts` first — shared utilities, API clients.
3. Add types progressively — start with function signatures.
4. Run `tsc --noEmit` in CI to catch regressions.
5. Enable `strict: true` file-by-file as each module is fully typed.
6. Remove `allowJs` when all files are converted.

## Key Points:
- Never a big-bang migration — too risky.
- Start with the most shared/critical files.
- CI type-checking (`tsc --noEmit`) prevents regressions.
- `allowJs: true` allows mixed JS/TS codebase during transition.
- Aim for gradual `strict` mode adoption per module.

## Interview Tip:
Mentioning CI integration (`tsc --noEmit` in the pipeline) shows you think about maintaining code quality during migration, not just doing the migration itself.

---

## Question 192: What are the biggest advantages of strict mode?

## Answer:
`strict: true` bundles several safety checks that individually matter enormously:

- **`strictNullChecks`**: Forces you to handle null/undefined — eliminates null reference errors.
- **`noImplicitAny`**: Prevents silent `any` spreading.
- **`strictFunctionTypes`**: Correct variance for function parameters.
- **`useUnknownInCatchVariables`**: Catch variables are `unknown` — forces proper error handling.
- **`strictPropertyInitialization`**: Ensures class properties are initialized.

## Key Points:
- Enables the full safety benefit of TypeScript.
- Each sub-flag addresses a specific class of bugs.
- Adding strict mode to legacy code is painful — start strict from day one.
- Teams that skip strict mode see most of TypeScript's bugs in production anyway.

## Interview Tip:
Name specific sub-flags and what bugs they prevent. This shows you understand `strict` at depth, not as a single checkbox.

---

## Question 193: How do you reduce TypeScript compile time?

## Answer:
- `skipLibCheck: true` — skip type checking node_modules.
- `incremental: true` — only recompile changed files.
- `isolatedModules: true` — ensures files are independently compilable.
- Use esbuild or SWC for transpilation (type check with `tsc --noEmit` separately).
- Avoid deeply recursive generic types — they're the biggest type-checking bottleneck.
- Split the project with project references.

## Key Points:
- Separate "type check" from "transpile" — esbuild just strips types; `tsc` type-checks.
- `incremental` and `skipLibCheck` are quick wins.
- Project references for monorepo compilation isolation.
- Complex generics slow down the type checker significantly.

## Interview Tip:
Separating transpilation from type checking is an advanced production optimization. Tools like Vite/esbuild strip types without checking, while `tsc --noEmit` runs in CI. This pattern is widely adopted.

---

## Question 194: What TypeScript mistakes do developers commonly make?

## Answer:
From real experience:
- Using `any` instead of proper types or `unknown`.
- Not enabling `strict: true` from the start.
- Over-annotating — typing everything instead of letting inference work.
- Using type assertions (`as`) instead of proper type guards.
- Forgetting that TypeScript checks are compile-time only — API data still needs runtime validation.
- Storing `null` without proper union typing.
- Complex generic types that become unreadable.
- Ignoring `never` in exhaustive checks.

## Key Points:
- `any` and non-strict mode are the most impactful mistakes.
- Runtime data always needs validation beyond TypeScript.
- Over-engineering types hurts maintainability.
- Skipping exhaustive checking in discriminated unions.

## Interview Tip:
This question rewards authentic answers from real experience. Don't give a generic list — pick 2-3 mistakes with brief "I learned this the hard way" framing.

---

## Question 195: What TypeScript features do you use most in production?

## Answer:
In production projects:
- **Generics** for API response wrappers, data hooks, and utilities.
- **Discriminated unions** for state management and action handling.
- **`Partial`, `Pick`, `Omit`** constantly for request/response typing.
- **Zod + TypeScript** for runtime-safe API boundaries.
- **Module augmentation** for extending Express Request.
- **`ReturnType` and `typeof`** for keeping types in sync with implementations.
- **Path aliases** for clean imports.

## Key Points:
- Utility types are used daily in API and data layer typing.
- Discriminated unions for any multi-state value.
- Zod bridges TypeScript with runtime reality.
- Generic utility types remove type duplication.

## Interview Tip:
Grounding your answer in real features you use daily is much stronger than listing everything TypeScript offers. Authenticity signals experience.

---

## Question 196: How do you design reusable types?

## Answer:
Start with generic base types and build specifics from them. Use utility types to derive related types from a single source. Keep types DRY — don't duplicate structure.

```ts
// Single source of truth
interface User { id: string; name: string; email: string; password: string; role: string }

// Derived types — no duplication
type PublicUser = Omit<User, "password">;
type CreateUserInput = Omit<User, "id">;
type UpdateUserInput = Partial<Omit<User, "id">>;
```

## Key Points:
- One source of truth — derive other types from it.
- Utility types (`Omit`, `Partial`, `Pick`) for transformations.
- Generic types for reusable patterns across the codebase.
- Co-locate types with their domain — don't create a global "types dumping ground."

## Interview Tip:
The User type example with derived `PublicUser`, `CreateUserInput`, and `UpdateUserInput` is perfect — it shows a real pattern every backend developer uses.

---

## Question 197: How do you avoid overly complex generic types?

## Answer:
When a generic type becomes hard to read, it's a sign to refactor. My rules:
- Break complex generics into smaller named utility types.
- Add type aliases at each step instead of one massive expression.
- If a type needs more than 2-3 generic parameters, reconsider the design.
- Prefer named intermediate types over inline complex generics.
- Write a comment explaining what a complex type does.

```ts
// Break it down into steps:
type PaginatedResult<T> = { items: T[]; total: number; page: number };
type ApiResponse<T> = { data: T; error: string | null };
type PaginatedApiResponse<T> = ApiResponse<PaginatedResult<T>>;
```

## Key Points:
- Complex types hurt maintainability and IDE performance.
- Named intermediate types are self-documenting.
- Set a complexity budget — if teammates can't understand it in 30 seconds, simplify.
- TypeScript error messages worsen proportionally with generic complexity.

## Interview Tip:
This shows engineering maturity — knowing when to stop and simplify is just as important as knowing how to write complex types.

---

## Question 198: What are TypeScript best practices for enterprise applications?

## Answer:
- Enable `strict: true` — non-negotiable.
- Use Zod or io-ts for runtime validation at API boundaries.
- Shared type packages in monorepos.
- Prefer `unknown` over `any`.
- Use discriminated unions for complex domain state.
- Enforce with ESLint + `@typescript-eslint` rules (ban `any`, require return types on exports).
- Document complex types with JSDoc comments.
- Run `tsc --noEmit` in CI.

## Key Points:
- Strict mode + ESLint TypeScript rules form the safety net.
- Runtime validation at boundaries (API, user input, external data).
- Automated enforcement is better than manual code review.
- Shared types reduce drift between teams.

## Interview Tip:
Mentioning ESLint + `@typescript-eslint` shows you think about enforcement, not just best practices. Teams that can't enforce standards don't maintain them.

---

## Question 199: How has TypeScript improved your real-world projects?

## Answer:
Concretely:
- **Fewer runtime bugs**: Type errors caught at build time that would've been production incidents.
- **Faster refactoring**: Renamed API fields and TypeScript immediately showed all places to update.
- **Better onboarding**: New developers understand API shapes from types without reading documentation.
- **API contract confidence**: When the backend changes a response type, the frontend compilation fails — not a user report.
- **Discoverability**: IDE autocomplete means exploring APIs without leaving the editor.

## Key Points:
- Type safety reduces debugging time significantly.
- Refactoring confidence in large codebases.
- Living documentation through types.
- Cross-team API contract enforcement.

## Interview Tip:
This is a behavioral question — speak from real experience. Concrete examples ("we caught X type of bug before production") are far more compelling than generic benefits.

---

## Question 200: If you were starting a new React/Next.js project today, how would you configure TypeScript and why?

## Answer:
I'd use `create-next-app` with TypeScript template as the starting point. Then I'd update `tsconfig.json`:

```json
{
  "compilerOptions": {
    "target": "ES2020",
    "lib": ["dom", "dom.iterable", "esnext"],
    "module": "esnext",
    "moduleResolution": "bundler",
    "strict": true,
    "skipLibCheck": true,
    "incremental": true,
    "baseUrl": ".",
    "paths": { "@/*": ["./src/*"] }
  }
}
```

Then I'd add:
- **Zod** for API response validation and form schemas.
- **ESLint** with `@typescript-eslint` for enforcement.
- **Prettier** for formatting.
- `tsc --noEmit` in CI.

## Key Points:
- Start with the framework's template — it handles most of the config.
- `strict: true` and `skipLibCheck: true` are always added.
- Path aliases from day one — painful to add later.
- CI type checking as a required pipeline step.
- Zod for the gap between TypeScript types and runtime data.

## Interview Tip:
This is the ultimate "senior developer" question. Having a ready answer shows experience. Mentioning the Zod + CI + ESLint ecosystem (not just tsconfig) signals you think about the complete development experience.

---
