# Testing Interview Questions (150 Total)

---

# Testing Fundamentals

1. What is software testing?
2. Why is testing important?
3. What are the benefits of automated testing?
4. What are the different types of software testing?
5. What is manual testing?
6. What is automated testing?
7. What is the testing pyramid?
8. What are unit tests?
9. What are integration tests?
10. What are end-to-end tests?

---

# Testing Concepts

11. What is the difference between unit testing and integration testing?
12. What is the difference between functional and non-functional testing?
13. What is regression testing?
14. What is smoke testing?
15. What is sanity testing?
16. What is acceptance testing?
17. What is performance testing?
18. What is load testing?
19. What is stress testing?
20. What testing strategy do you follow in projects?

---

# Unit Testing

21. What is a unit in unit testing?
22. What makes a good unit test?
23. What should you test in a unit?
24. What should you avoid testing in unit tests?
25. What are test cases?
26. What are test suites?
27. What is test coverage?
28. What is code coverage?
29. What percentage of test coverage is ideal?
30. What are the characteristics of a good test?

---

# Jest Fundamentals

31. What is Jest?
32. Why is Jest popular in JavaScript projects?
33. What features does Jest provide?
34. How do you install Jest?
35. How do you create a Jest test file?
36. What is the `test()` function in Jest?
37. What is the `it()` function in Jest?
38. What is the difference between `test()` and `it()`?
39. What is `describe()` in Jest?
40. What are Jest matchers?

---

# Jest Assertions & Testing

41. What is `expect()` in Jest?
42. What are common Jest matchers?
43. What is the difference between `toBe()` and `toEqual()`?
44. What is `toContain()`?
45. What is `toHaveLength()`?
46. What is `toThrow()`?
47. How do you test asynchronous code in Jest?
48. How do you test promises in Jest?
49. How do you test async/await functions?
50. What Jest testing best practices do you follow?

---

# React Testing Library (RTL)

51. What is React Testing Library?
52. Why was React Testing Library created?
53. How is React Testing Library different from Enzyme?
54. What is the testing philosophy of React Testing Library?
55. Why should you test user behavior instead of implementation details?
56. What are the main APIs provided by React Testing Library?
57. What is `render()` in React Testing Library?
58. What is `screen` in React Testing Library?
59. What are queries in React Testing Library?
60. What is the difference between getBy, queryBy, and findBy?

---

# Component Testing

61. How do you test a React component?
62. What should you test in a React component?
63. Should you test component internal state?
64. How do you test component props?
65. How do you test conditional rendering?
66. How do you test lists and dynamic content?
67. How do you test loading states?
68. How do you test error states?
69. How do you test components with external dependencies?
70. What React component testing best practices do you follow?

---

# User Interaction Testing

71. How do you simulate user actions in React Testing Library?
72. What is `fireEvent`?
73. What is `userEvent`?
74. What is the difference between fireEvent and userEvent?
75. How do you test button clicks?
76. How do you test form submissions?
77. How do you test input changes?
78. How do you test keyboard interactions?
79. How do you test accessibility behavior?
80. What user interaction testing practices do you follow?

---

# Testing Hooks & State Management

81. How do you test React hooks?
82. What is React Hooks Testing Library?
83. How do you test custom hooks?
84. How do you test useState logic?
85. How do you test useEffect behavior?
86. How do you test context providers?
87. How do you test Redux applications?
88. How do you test Redux Toolkit slices?
89. How do you test Zustand stores?
90. What state management testing practices do you follow?

---

# API Mocking & Integration Testing

91. How do you test API calls in frontend applications?
92. What is mocking?
93. Why do we mock API requests?
94. What is Mock Service Worker (MSW)?
95. How does MSW work?
96. What is the difference between mocking and stubbing?
97. How do you test API success responses?
98. How do you test API error responses?
99. How do you test authentication flows?
100. What frontend integration testing practices do you follow?

---

# End-to-End (E2E) Testing

101. What is end-to-end testing?
102. Why is E2E testing important?
103. How is E2E testing different from unit testing?
104. How is E2E testing different from integration testing?
105. What tools are used for E2E testing?
106. What is Cypress?
107. What is Playwright?
108. What is the difference between Cypress and Playwright?
109. When should you use Cypress?
110. When should you use Playwright?

---

# Cypress

111. How does Cypress work internally?
112. What are Cypress commands?
113. What is Cypress test runner?
114. How do you write Cypress tests?
115. How do you select elements in Cypress?
116. How do you test forms using Cypress?
117. How do you test authentication flows using Cypress?
118. How do you mock API responses in Cypress?
119. How do you run Cypress tests in CI/CD?
120. What Cypress best practices do you follow?

---

# Playwright

121. What is Playwright?
122. Why is Playwright popular for modern applications?
123. What browsers does Playwright support?
124. How do you write Playwright tests?
125. What are Playwright locators?
126. How do you handle multiple pages in Playwright?
127. How do you handle authentication in Playwright?
128. How do you run Playwright tests in CI/CD?
129. What are Playwright fixtures?
130. What Playwright best practices do you follow?

---

# Testing Architecture & Strategy

131. How do you decide what to test?
132. How do you design a testing strategy for a large application?
133. How do you balance unit, integration, and E2E tests?
134. What is test-driven development (TDD)?
135. What is behavior-driven development (BDD)?
136. What is the difference between TDD and BDD?
137. What is test automation strategy?
138. How do you maintain test cases as applications grow?
139. How do you handle flaky tests?
140. What testing architecture practices do you follow?

---

# Senior Real-World Testing Questions

141. Describe the testing strategy you used in a real project.
142. How do you test a large Next.js application?
143. How would you test a full-stack application with React, Node.js, and PostgreSQL?
144. How do you test authentication and authorization?
145. How do you test database-related functionality?
146. How do you integrate tests into CI/CD pipelines?
147. How do you improve slow-running test suites?
148. What testing mistakes do junior developers commonly make?
149. What testing practices do senior engineers follow?
150. In your opinion, what separates a junior, mid-level, and senior developer regarding testing?

---

# ANSWERS


---

## Part 1 (1â€“10): Testing Fundamentals

---

## Question 1: What is software testing?

## Answer:
Software testing is the process of evaluating software to find bugs, verify functionality, and ensure it meets requirements. It includes manual and automated approaches.

## Key Points:
- Evaluate software quality.
- Find bugs before users do.
- Verify functionality.
- Ensure requirements are met.
- Manual and automated.

## Interview Tip:
"Testing finds bugs before users do â€” that's its primary value."

---

## Question 2: Why is testing important?

## Answer:
- **Catch bugs early**: Cheaper to fix before production.
- **Confidence**: Safe to refactor and add features.
- **Documentation**: Tests describe expected behavior.
- **Regression prevention**: Ensure changes don't break existing functionality.
- **Quality**: Better user experience.

## Key Points:
- Early bug detection.
- Refactoring confidence.
- Documentation.
- Regression prevention.
- Quality assurance.

## Interview Tip:
"Testing is an investment â€” it costs time now but saves exponentially more later."

---

## Question 3: What are the benefits of automated testing?

## Answer:
- **Speed**: Run thousands of tests in seconds.
- **Consistency**: Same tests every time.
- **Confidence**: Safe to deploy.
- **CI/CD**: Integrate into pipelines.
- **Regression**: Catch bugs automatically.

## Key Points:
- Fast execution.
- Consistent results.
- Deployment confidence.
- CI/CD integration.
- Automatic regression detection.

## Interview Tip:
"Automated tests are the safety net for continuous deployment."

---

## Question 4: What are the different types of software testing?

## Answer:
- **Unit testing**: Test individual functions/components.
- **Integration testing**: Test component interactions.
- **End-to-end testing**: Test full user flows.
- **Performance testing**: Test speed and scalability.
- **Security testing**: Test for vulnerabilities.
- **Acceptance testing**: Verify business requirements.

## Key Points:
- Unit, integration, E2E.
- Performance and security.
- Acceptance testing.
- Each serves a different purpose.

## Interview Tip:
"Different types of testing catch different types of bugs."

---

## Question 5: What is manual testing?

## Answer:
Manual testing is when humans manually test the application by interacting with it â€” clicking buttons, filling forms, verifying behavior.

## Key Points:
- Human-driven testing.
- Exploratory testing.
- Usability testing.
- Slow and expensive.
- Not repeatable.

## Interview Tip:
"Manual testing is for exploratory and usability testing â€” automate everything else."

---

## Question 6: What is automated testing?

## Answer:
Automated testing uses scripts and tools to run tests automatically without human intervention.

## Key Points:
- Script-driven testing.
- Fast and repeatable.
- CI/CD integration.
- Consistent results.
- Requires initial investment.

## Interview Tip:
"Automated testing is an investment that pays off in confidence and speed."

---

## Question 7: What is the testing pyramid?

## Answer:
The testing pyramid recommends:
- **Many unit tests**: Fast, cheap, focused.
- **Some integration tests**: Test component interactions.
- **Few E2E tests**: Slow, expensive, broad.

```
      /\
     /E2E\      (few)
    /------\
   / Integr.\   (some)
  /----------\
 /    Unit    \  (many)
/--------------\
```

## Key Points:
- Many unit tests at the base.
- Some integration tests in the middle.
- Few E2E tests at the top.
- Balance speed and coverage.

## Interview Tip:
"The testing pyramid: many unit tests, some integration, few E2E."

---

## Question 8: What are unit tests?

## Answer:
Unit tests test individual functions or components in isolation, verifying they produce correct output for given input.

```javascript
test("adds two numbers", () => {
  expect(add(1, 2)).toBe(3);
});
```

## Key Points:
- Test individual units.
- Isolated from dependencies.
- Fast execution.
- Many unit tests.
- Foundation of testing.

## Interview Tip:
"Unit tests are the foundation â€” fast, focused, and numerous."

---

## Question 9: What are integration tests?

## Answer:
Integration tests verify that multiple components work together correctly â€” testing the integration between units.

```javascript
test("creates user and sends email", async () => {
  const user = await createUser({ email: "test@example.com" });
  expect(user.id).toBeDefined();
  expect(emailService.sendWelcome).toHaveBeenCalledWith("test@example.com");
});
```

## Key Points:
- Test component interactions.
- Test integrations between units.
- Slower than unit tests.
- More realistic.
- Test boundaries.

## Interview Tip:
"Integration tests verify that components work together â€” unit tests verify they work alone."

---

## Question 10: What are end-to-end tests?

## Answer:
E2E tests simulate real user interactions across the entire application â€” from UI to database.

```javascript
test("user can login", async () => {
  await page.goto("/login");
  await page.fill("#email", "user@example.com");
  await page.fill("#password", "password");
  await page.click("#submit");
  expect(page.url()).toContain("/dashboard");
});
```

## Key Points:
- Simulate real user behavior.
- Test full application flow.
- Slow and expensive.
- Few E2E tests.
- High confidence.

## Interview Tip:
"E2E tests give the highest confidence but are the slowest â€” use sparingly."

---

## Part 2 (11â€“20): Testing Concepts

---

## Question 11: What is the difference between unit testing and integration testing?

## Answer:
- **Unit**: Tests individual functions in isolation. Fast, cheap.
- **Integration**: Tests component interactions. Slower, more realistic.

## Key Points:
- Unit: isolated, fast, many.
- Integration: interactions, slower, some.
- Unit for logic, integration for boundaries.

## Interview Tip:
"Unit tests verify logic; integration tests verify interactions."

---

## Question 12: What is the difference between functional and non-functional testing?

## Answer:
- **Functional**: Does it work correctly? (features, logic)
- **Non-functional**: How well does it work? (performance, security, usability)

## Key Points:
- Functional: correctness.
- Non-functional: quality attributes.
- Functional for features.
- Non-functional for performance, security.

## Interview Tip:
"Functional testing checks what; non-functional testing checks how well."

---

## Question 13: What is regression testing?

## Answer:
Regression testing verifies that new changes don't break existing functionality. Automated tests are ideal for regression.

## Key Points:
- Verify changes don't break existing features.
- Automated for speed.
- Run after every change.
- Catch unintended side effects.

## Interview Tip:
"Regression testing prevents 'I didn't mean to break that' moments."

---

## Question 14: What is smoke testing?

## Answer:
Smoke testing is a quick check to verify the most critical functionality works after a deployment or change.

## Key Points:
- Quick sanity check.
- Critical functionality only.
- After deployment.
- "Does it work at all?"

## Interview Tip:
"Smoke testing is the first line of defense after deployment."

---

## Question 15: What is sanity testing?

## Answer:
Sanity testing verifies that specific functionality works after a change. It's narrower than smoke testing.

## Key Points:
- Verify specific functionality.
- After targeted changes.
- Narrower than smoke testing.
- Quick verification.

## Interview Tip:
"Sanity testing verifies specific changes; smoke testing verifies overall health."

---

## Question 16: What is acceptance testing?

## Answer:
Acceptance testing verifies that the software meets business requirements and is ready for release.

## Key Points:
- Verify business requirements.
- Ready for release.
- User acceptance testing (UAT).
- Often manual.

## Interview Tip:
"Acceptance testing answers: 'Does it meet the requirements?'"

---

## Question 17: What is performance testing?

## Answer:
Performance testing evaluates how the application performs under load â€” speed, scalability, and stability.

## Key Points:
- Speed and responsiveness.
- Scalability under load.
- Stability under stress.
- Load testing, stress testing.

## Interview Tip:
"Performance testing ensures your app handles real-world traffic."

---

## Question 18: What is load testing?

## Answer:
Load testing evaluates how the system performs under expected load â€” simulating many concurrent users.

## Key Points:
- Expected load simulation.
- Concurrent users.
- Response times.
- Throughput measurement.

## Interview Tip:
"Load testing answers: 'Can it handle the expected traffic?'"

---

## Question 19: What is stress testing?

## Answer:
Stress testing evaluates how the system performs under extreme load â€” beyond normal capacity.

## Key Points:
- Beyond normal capacity.
- Find breaking points.
- Recovery behavior.
- Failure modes.

## Interview Tip:
"Stress testing finds the breaking point â€” what happens when it's overwhelmed?"

---

## Question 20: What testing strategy do you follow in projects?

## Answer:
1. **Unit tests**: For business logic and utilities.
2. **Integration tests**: For API endpoints and database operations.
3. **E2E tests**: For critical user flows.
4. **Continuous testing**: Run tests in CI/CD.

## Key Points:
- Unit for logic.
- Integration for APIs.
- E2E for critical flows.
- Continuous in CI/CD.

## Interview Tip:
"Unit for logic, integration for APIs, E2E for critical flows â€” the testing pyramid."

---

## Part 3 (21â€“30): Unit Testing

---

## Question 21: What is a unit in unit testing?

## Answer:
A unit is the smallest testable part of an application â€” a function, method, or component.

## Key Points:
- Smallest testable part.
- Function, method, or component.
- Isolated from dependencies.
- Testable in isolation.

## Interview Tip:
"A unit is the smallest piece you can test independently."

---

## Question 22: What makes a good unit test?

## Answer:
- **Fast**: Runs in milliseconds.
- **Isolated**: No dependencies on external systems.
- **Repeatable**: Same result every time.
- **Self-validating**: Clear pass/fail.
- **Timely**: Written alongside the code.

## Key Points:
- Fast, isolated, repeatable.
- Self-validating.
- Written alongside code.
- Tests behavior, not implementation.

## Interview Tip:
"Good unit tests are FAST: Fast, Isolated, Self-validating, Timely."

---

## Question 23: What should you test in a unit?

## Answer:
- **Public API**: Functions and methods exposed to other code.
- **Edge cases**: Boundary conditions.
- **Error handling**: What happens on failure.
- **Business logic**: Core functionality.

## Key Points:
- Public API.
- Edge cases.
- Error handling.
- Business logic.

## Interview Tip:
"Test the public API, edge cases, and error handling."

---

## Question 24: What should you avoid testing in unit tests?

## Answer:
- **Implementation details**: Don't test how, test what.
- **Third-party code**: Trust library tests.
- **Trivial code**: Getters, setters, simple assignments.
- **External systems**: Use mocks for databases, APIs.

## Key Points:
- Don't test implementation details.
- Don't test third-party code.
- Don't test trivial code.
- Mock external systems.

## Interview Tip:
"Test behavior, not implementation â€” if you refactor internals, tests shouldn't break."

---

## Question 25: What are test cases?

## Answer:
A test case is a set of conditions and expected results for testing a specific functionality.

## Key Points:
- Specific scenario to test.
- Input and expected output.
- Clear pass/fail criteria.
- Documented test scenario.

## Interview Tip:
"A test case = input + expected output + assertion."

---

## Question 26: What are test suites?

## Answer:
A test suite is a collection of related test cases grouped together.

```javascript
describe("UserService", () => {
  test("creates user", () => { /* ... */ });
  test("validates email", () => { /* ... */ });
  test("hashes password", () => { /* ... */ });
});
```

## Key Points:
- Group of related tests.
- Organized by feature or module.
- `describe()` in Jest.
- Run together.

## Interview Tip:
"Test suites organize tests by feature or module."

---

## Question 27: What is test coverage?

## Answer:
Test coverage measures how much of the codebase is executed by tests. It's expressed as a percentage.

## Key Points:
- Percentage of code tested.
- Lines, branches, functions.
- Metric, not a goal.
- High coverage â‰  good tests.

## Interview Tip:
"Coverage is a metric, not a goal â€” 100% coverage doesn't mean bug-free."

---

## Question 28: What is code coverage?

## Answer:
Code coverage is the percentage of code executed during tests â€” measured by lines, branches, and functions.

## Key Points:
- Lines covered.
- Branches covered.
- Functions covered.
- Percentage metric.

## Interview Tip:
"Code coverage tells you what's tested â€” not how well it's tested."

---

## Question 29: What percentage of test coverage is ideal?

## Answer:
There's no magic number, but aim for:
- **Critical paths**: 100% coverage.
- **Business logic**: 80-90% coverage.
- **UI components**: 60-70% coverage.
- **Overall**: 70-80% is a good target.

## Key Points:
- Critical paths: 100%.
- Business logic: 80-90%.
- UI: 60-70%.
- Quality over quantity.

## Interview Tip:
"Quality over quantity â€” 80% coverage with good tests beats 100% with bad tests."

---

## Question 30: What are the characteristics of a good test?

## Answer:
- **Readable**: Easy to understand.
- **Maintainable**: Easy to update.
- **Fast**: Runs quickly.
- **Isolated**: Independent of other tests.
- **Descriptive**: Clear test names.

## Key Points:
- Readable and maintainable.
- Fast and isolated.
- Descriptive names.
- Tests behavior.

## Interview Tip:
"Good tests are readable, fast, isolated, and descriptive."

---

## Part 4 (31â€“40): Jest Fundamentals

---

## Question 31: What is Jest?

## Answer:
Jest is a JavaScript testing framework created by Facebook. It provides a test runner, assertion library, mocking, and code coverage.

## Key Points:
- JavaScript testing framework.
- Created by Facebook.
- Test runner, assertions, mocking.
- Built-in code coverage.
- Zero configuration.

## Interview Tip:
"Jest is the most popular JavaScript testing framework â€” it does everything out of the box."

---

## Question 32: Why is Jest popular in JavaScript projects?

## Answer:
- **Zero configuration**: Works out of the box.
- **Fast**: Parallel test execution.
- **Built-in mocking**: Mock functions, modules.
- **Snapshot testing**: For UI components.
- **Code coverage**: Built-in.

## Key Points:
- Zero configuration.
- Fast parallel execution.
- Built-in mocking.
- Snapshot testing.
- Code coverage.

## Interview Tip:
"Jest is popular because it just works â€” zero configuration, fast, and feature-rich."

---

## Question 33: What features does Jest provide?

## Answer:
- **Test runner**: Execute tests.
- **Assertions**: `expect()`, matchers.
- **Mocking**: Mock functions, modules, timers.
- **Code coverage**: Built-in coverage reports.
- **Snapshot testing**: For UI components.
- **Parallel execution**: Fast test runs.

## Key Points:
- Test runner, assertions, mocking.
- Code coverage, snapshots.
- Parallel execution.
- All-in-one solution.

## Interview Tip:
"Jest is all-in-one: runner, assertions, mocking, coverage, and snapshots."

---

## Question 34: How do you install Jest?

## Answer:
```bash
npm install --save-dev jest
```

Add to `package.json`:
```json
{
  "scripts": {
    "test": "jest"
  }
}
```

## Key Points:
- `npm install --save-dev jest`.
- Add test script to package.json.
- Run with `npm test`.
- Zero configuration needed.

## Interview Tip:
"`npm install --save-dev jest` and add a test script â€” that's it."

---

## Question 35: How do you create a Jest test file?

## Answer:
Name the file `*.test.js` or `*.spec.js`:

```javascript
// sum.test.js
const { sum } = require("./sum");

test("adds 1 + 2 to equal 3", () => {
  expect(sum(1, 2)).toBe(3);
});
```

## Key Points:
- `*.test.js` or `*.spec.js` naming.
- `test()` function for test cases.
- `expect()` for assertions.
- Auto-discovered by Jest.

## Interview Tip:
"Name files `*.test.js` â€” Jest finds them automatically."

---

## Question 36: What is the `test()` function in Jest?

## Answer:
`test()` defines an individual test case.

```javascript
test("description", () => {
  // Test logic
  expect(result).toBe(expected);
});
```

## Key Points:
- Defines a test case.
- Description string.
- Test function with assertions.
- Can be async.

## Interview Tip:
"`test('description', () => { expect(...) })` â€” the basic test structure."

---

## Question 37: What is the `it()` function in Jest?

## Answer:
`it()` is an alias for `test()` â€” they're identical.

```javascript
it("adds numbers", () => {
  expect(sum(1, 2)).toBe(3);
});
```

## Key Points:
- Alias for `test()`.
- Identical behavior.
- BDD-style naming.
- Use whichever you prefer.

## Interview Tip:
"`test()` and `it()` are the same â€” use whichever reads better."

---

## Question 38: What is the difference between `test()` and `it()`?

## Answer:
No difference â€” they're aliases. `it()` comes from BDD (Behavior-Driven Development) style.

```javascript
// These are identical
test("adds numbers", () => { /* ... */ });
it("adds numbers", () => { /* ... */ });
```

## Key Points:
- Aliases â€” identical behavior.
- `it()` is BDD style.
- Use consistently.

## Interview Tip:
"Pick one and be consistent â€” I prefer `test()` for clarity."

---

## Question 39: What is `describe()` in Jest?

## Answer:
`describe()` groups related tests into a test suite.

```javascript
describe("UserService", () => {
  test("creates user", () => { /* ... */ });
  test("validates email", () => { /* ... */ });
  test("hashes password", () => { /* ... */ });
});
```

## Key Points:
- Groups related tests.
- Test suite organization.
- Nested describes for sub-groups.
- Improves readability.

## Interview Tip:
"`describe()` organizes tests â€” group by feature or module."

---

## Question 40: What are Jest matchers?

## Answer:
Matchers are assertion methods that check if a value meets expectations.

```javascript
expect(value).toBe(expected);        // Strict equality
expect(value).toEqual(expected);     // Deep equality
expect(array).toContain(item);       // Array contains
expect(fn).toThrow();                // Function throws
```

## Key Points:
- `toBe()`: strict equality.
- `toEqual()`: deep equality.
- `toContain()`: array/string contains.
- `toThrow()`: function throws.
- Many more matchers.

## Interview Tip:
"`toBe()` for primitives, `toEqual()` for objects, `toContain()` for arrays."

---

## Part 5 (41â€“50): Jest Assertions & Testing

---

## Question 41: What is `expect()` in Jest?

## Answer:
`expect()` creates an assertion â€” it takes a value and chains matchers to verify expectations.

```javascript
expect(sum(1, 2)).toBe(3);
expect(user.name).toBe("Alice");
expect(users).toHaveLength(3);
```

## Key Points:
- Creates assertions.
- Chain matchers.
- Clear pass/fail.
- Many matchers available.

## Interview Tip:
"`expect(value).matcher()` â€” the assertion pattern."

---

## Question 42: What are common Jest matchers?

## Answer:
- `toBe()`: Strict equality.
- `toEqual()`: Deep equality.
- `toContain()`: Array/string contains.
- `toHaveLength()`: Length check.
- `toThrow()`: Exception check.
- `toBeTruthy()` / `toBeFalsy()`: Boolean checks.
- `toBeNull()` / `toBeUndefined()`: Null checks.
- `toHaveBeenCalled()`: Mock function called.

## Key Points:
- Equality: toBe, toEqual.
- Containment: toContain.
- Length: toHaveLength.
- Exceptions: toThrow.
- Mocks: toHaveBeenCalled.

## Interview Tip:
"Know the common matchers â€” toBe, toEqual, toContain, toThrow, toHaveBeenCalled."

---

## Question 43: What is the difference between `toBe()` and `toEqual()`?

## Answer:
- `toBe()`: Strict reference equality (`===`).
- `toEqual()`: Deep value equality (for objects/arrays).

```javascript
expect(1 + 2).toBe(3);              // Primitives
expect({ a: 1 }).toEqual({ a: 1 });  // Objects
```

## Key Points:
- `toBe()`: reference equality.
- `toEqual()`: deep equality.
- `toBe` for primitives.
- `toEqual` for objects/arrays.

## Interview Tip:
"`toBe()` for primitives, `toEqual()` for objects."

---

## Question 44: What is `toContain()`?

## Answer:
`toContain()` checks if an array or string contains a specific value.

```javascript
expect([1, 2, 3]).toContain(2);
expect("hello world").toContain("world");
```

## Key Points:
- Array contains value.
- String contains substring.
- Simple containment check.

## Interview Tip:
"`toContain()` for arrays and strings â€” it checks for presence."

---

## Question 45: What is `toHaveLength()`?

## Answer:
`toHaveLength()` checks the length of an array or string.

```javascript
expect([1, 2, 3]).toHaveLength(3);
expect("hello").toHaveLength(5);
```

## Key Points:
- Array length check.
- String length check.
- Clear assertion.

## Interview Tip:
"`toHaveLength()` is cleaner than `expect(arr.length).toBe(3)`."

---

## Question 46: What is `toThrow()`?

## Answer:
`toThrow()` verifies that a function throws an exception.

```javascript
expect(() => divide(1, 0)).toThrow("Division by zero");
expect(() => JSON.parse("invalid")).toThrow();
```

## Key Points:
- Verifies function throws.
- Can check error message.
- Works with arrow functions.
- Test error handling.

## Interview Tip:
"`toThrow()` verifies error handling â€” always test error cases."

---

## Question 47: How do you test asynchronous code in Jest?

## Answer:
```javascript
// Async/await
test("fetches data", async () => {
  const data = await fetchData();
  expect(data).toBeDefined();
});

// Promises
test("fetches data", () => {
  return fetchData().then(data => {
    expect(data).toBeDefined();
  });
});
```

## Key Points:
- `async/await` for async tests.
- Return promise for promise tests.
- Jest waits for async to complete.
- Handle rejections.

## Interview Tip:
"Use `async/await` for async tests â€” it's the cleanest approach."

---

## Question 48: How do you test promises in Jest?

## Answer:
```javascript
test("resolves with data", () => {
  return expect(fetchData()).resolves.toBe("data");
});

test("rejects with error", () => {
  return expect(fetchData()).rejects.toThrow("Error");
});
```

## Key Points:
- `resolves` for fulfilled promises.
- `rejects` for rejected promises.
- Return the promise.
- Clean assertion syntax.

## Interview Tip:
"`expect(promise).resolves.toBe(value)` â€” clean promise testing."

---

## Question 49: How do you test async/await functions?

## Answer:
```javascript
test("creates user", async () => {
  const user = await createUser({ name: "Alice" });
  expect(user.name).toBe("Alice");
  expect(user.id).toBeDefined();
});

test("throws on invalid input", async () => {
  await expect(createUser({})).rejects.toThrow("Name required");
});
```

## Key Points:
- `async` test function.
- `await` the async call.
- Assert on the result.
- `rejects.toThrow()` for errors.

## Interview Tip:
"`async/await` with `expect` â€” the standard async test pattern."

---

## Question 50: What Jest testing best practices do you follow?

## Answer:
1. **Test behavior, not implementation**.
2. **Use descriptive test names**.
3. **One assertion per test** (when practical).
4. **Arrange, Act, Assert** pattern.
5. **Mock external dependencies**.
6. **Test edge cases and errors**.
7. **Keep tests fast and isolated**.

## Key Points:
- Test behavior.
- Descriptive names.
- Arrange, Act, Assert.
- Mock dependencies.
- Edge cases and errors.

## Interview Tip:
"Arrange, Act, Assert â€” the test structure that makes tests readable."

---

## Part 6 (51â€“60): React Testing Library (RTL)

---

## Question 51: What is React Testing Library?

## Answer:
React Testing Library (RTL) is a testing utility for React components that encourages testing behavior over implementation details.

```javascript
import { render, screen } from "@testing-library/react";

test("renders user name", () => {
  render(<UserCard name="Alice" />);
  expect(screen.getByText("Alice")).toBeInTheDocument();
});
```

## Key Points:
- Test behavior, not implementation.
- User-centric queries.
- Encourages accessible code.
- Industry standard for React testing.

## Interview Tip:
"RTL tests what the user sees â€” not how the component works internally."

---

## Question 52: Why was React Testing Library created?

## Answer:
RTL was created to encourage testing practices that lead to more maintainable tests. It focuses on testing what users see and do, rather than implementation details.

## Key Points:
- Test user behavior.
- Avoid implementation details.
- More maintainable tests.
- Encourages accessibility.

## Interview Tip:
"RTL was created because testing implementation details leads to brittle tests."

---

## Question 53: How is React Testing Library different from Enzyme?

## Answer:
- **RTL**: Tests behavior (what users see).
- **Enzyme**: Tests implementation (component internals).

RTL is the modern standard; Enzyme is legacy.

## Key Points:
- RTL: behavior-focused.
- Enzyme: implementation-focused.
- RTL is the standard.
- Enzyme is legacy.

## Interview Tip:
"RTL for new projects; Enzyme is legacy."

---

## Question 54: What is the testing philosophy of React Testing Library?

## Answer:
"The more your tests resemble the way your software is used, the more confidence they give you."

Test what users see and do, not implementation details.

## Key Points:
- Test user behavior.
- Resemble real usage.
- Confidence from realistic tests.
- Avoid implementation details.

## Interview Tip:
"Test what users see and do â€” that's RTL's philosophy."

---

## Question 55: Why should you test user behavior instead of implementation details?

## Answer:
- **Maintainability**: Implementation changes don't break tests.
- **Confidence**: Tests verify what users experience.
- **Refactoring**: Safe to refactor internals.
- **Accessibility**: Encourages accessible code.

## Key Points:
- More maintainable tests.
- Higher confidence.
- Safe refactoring.
- Accessibility benefits.

## Interview Tip:
"Behavior tests survive refactoring; implementation tests break."

---

## Question 56: What are the main APIs provided by React Testing Library?

## Answer:
- **`render()`**: Render a component.
- **`screen`**: Query rendered elements.
- **`fireEvent`**: Simulate user interactions.
- **`userEvent`**: More realistic interactions.
- **`waitFor`**: Wait for async operations.
- **`within()`**: Scope queries to a container.

## Key Points:
- render, screen, fireEvent, userEvent.
- waitFor for async.
- within for scoped queries.
- All you need for component testing.

## Interview Tip:
"render + screen + fireEvent/userEvent â€” the RTL essentials."

---

## Question 57: What is `render()` in React Testing Library?

## Answer:
`render()` renders a React component into a virtual DOM for testing.

```javascript
import { render } from "@testing-library/react";

render(<MyComponent />);
```

## Key Points:
- Renders component for testing.
- Returns utilities for querying.
- Cleans up automatically.
- Wraps component in necessary providers.

## Interview Tip:
"`render()` is the starting point â€” it renders the component for testing."

---

## Question 58: What is `screen` in React Testing Library?

## Answer:
`screen` provides methods to query the rendered component.

```javascript
import { screen } from "@testing-library/react";

screen.getByText("Hello");        // Find by text
screen.getByRole("button");       // Find by role
screen.queryByText("Missing");    // Returns null if not found
```

## Key Points:
- Query rendered elements.
- getBy, queryBy, findBy methods.
- User-centric queries.
- Debug with `screen.debug()`.

## Interview Tip:
"`screen.getByText()` â€” the most common query."

---

## Question 59: What are queries in React Testing Library?

## Answer:
Queries are methods to find elements in the rendered component.

- **getBy**: Throws if not found (for elements that should exist).
- **queryBy**: Returns null if not found (for elements that might not exist).
- **findBy**: Async, waits for element (for async rendering).

## Key Points:
- getBy: throws if not found.
- queryBy: returns null.
- findBy: async, waits.
- User-centric: getByRole, getByText, getByLabelText.

## Interview Tip:
"getBy for must-exist, queryBy for might-not-exist, findBy for async."

---

## Question 60: What is the difference between getBy, queryBy, and findBy?

## Answer:
- **getBy**: Throws error if not found. For elements that should exist.
- **queryBy**: Returns null if not found. For elements that might not exist.
- **findBy**: Returns promise, waits for element. For async rendering.

## Key Points:
- getBy: immediate, throws.
- queryBy: immediate, returns null.
- findBy: async, waits.
- Choose based on expectations.

## Interview Tip:
"getBy = must exist, queryBy = might exist, findBy = will exist eventually."

---

## Part 7 (61â€“70): Component Testing

---

## Question 61: How do you test a React component?

## Answer:
```javascript
import { render, screen, fireEvent } from "@testing-library/react";

test("increments counter", () => {
  render(<Counter />);
  expect(screen.getByText("0")).toBeInTheDocument();
  fireEvent.click(screen.getByRole("button"));
  expect(screen.getByText("1")).toBeInTheDocument();
});
```

## Key Points:
- Render component.
- Query elements.
- Simulate interactions.
- Assert on output.

## Interview Tip:
"Render, query, interact, assert â€” the component test pattern."

---

## Question 62: What should you test in a React component?

## Answer:
- **Rendering**: Does it render correctly?
- **User interactions**: Click, type, submit.
- **Conditional rendering**: Different states.
- **Props**: Different prop values.
- **Error states**: Error handling.

## Key Points:
- Rendering and interactions.
- Conditional rendering.
- Props and state.
- Error states.

## Interview Tip:
"Test what the user sees and does â€” not implementation details."

---

## Question 63: Should you test component internal state?

## Answer:
No. Test what the user sees (output), not how the component works internally (state). If the user sees the correct result, the test passes regardless of implementation.

## Key Points:
- Test output, not state.
- User-centric testing.
- Avoids brittle tests.
- Survives refactoring.

## Interview Tip:
"Never test state directly â€” test what the user sees."

---

## Question 64: How do you test component props?

## Answer:
```javascript
test("renders user name", () => {
  render(<UserCard name="Alice" />);
  expect(screen.getByText("Alice")).toBeInTheDocument();
});

test("shows admin badge for admin users", () => {
  render(<UserCard name="Alice" role="admin" />);
  expect(screen.getByText("Admin")).toBeInTheDocument();
});
```

## Key Points:
- Pass props to render.
- Assert on rendered output.
- Test different prop combinations.
- Test default props.

## Interview Tip:
"Test props by passing them and asserting on the output."

---

## Question 65: How do you test conditional rendering?

## Answer:
```javascript
test("shows loading state", () => {
  render(<DataList isLoading={true} />);
  expect(screen.getByText("Loading...")).toBeInTheDocument();
});

test("shows data", () => {
  render(<DataList isLoading={false} items={["a", "b"]} />);
  expect(screen.getByText("a")).toBeInTheDocument();
});

test("shows error", () => {
  render(<DataList error="Failed" />);
  expect(screen.getByText("Failed")).toBeInTheDocument();
});
```

## Key Points:
- Test each condition.
- Loading, data, error states.
- Different prop combinations.
- All branches covered.

## Interview Tip:
"Test all conditional branches â€” loading, success, error."

---

## Question 66: How do you test lists and dynamic content?

## Answer:
```javascript
test("renders list of users", () => {
  const users = [
    { id: 1, name: "Alice" },
    { id: 2, name: "Bob" }
  ];
  render(<UserList users={users} />);
  expect(screen.getByText("Alice")).toBeInTheDocument();
  expect(screen.getByText("Bob")).toBeInTheDocument();
});

test("shows empty state", () => {
  render(<UserList users={[]} />);
  expect(screen.getByText("No users found")).toBeInTheDocument();
});
```

## Key Points:
- Pass list data as props.
- Assert on rendered items.
- Test empty state.
- Test with multiple items.

## Interview Tip:
"Test with data and without data â€” both states matter."

---

## Question 67: How do you test loading states?

## Answer:
```javascript
test("shows loading indicator", () => {
  render(<UserProfile isLoading={true} />);
  expect(screen.getByText("Loading...")).toBeInTheDocument();
});

test("shows content after loading", async () => {
  render(<UserProfile isLoading={false} user={{ name: "Alice" }} />);
  expect(screen.getByText("Alice")).toBeInTheDocument();
});
```

## Key Points:
- Test loading indicator.
- Test content after loading.
- Test transitions between states.

## Interview Tip:
"Test loading â†’ loaded transitions â€” that's what users experience."

---

## Question 68: How do you test error states?

## Answer:
```javascript
test("shows error message", () => {
  render(<UserProfile error="User not found" />);
  expect(screen.getByText("User not found")).toBeInTheDocument();
});

test("shows retry button on error", () => {
  render(<UserProfile error="Failed" />);
  expect(screen.getByRole("button", { name: "Retry" })).toBeInTheDocument();
});
```

## Key Points:
- Test error message display.
- Test retry functionality.
- Test error recovery.

## Interview Tip:
"Error states are as important as success states â€” always test them."

---

## Question 69: How do you test components with external dependencies?

## Answer:
Mock external dependencies:

```javascript
jest.mock("./api", () => ({
  fetchUsers: jest.fn().mockResolvedValue([{ id: 1, name: "Alice" }])
}));

test("fetches and displays users", async () => {
  render(<UserList />);
  expect(await screen.findByText("Alice")).toBeInTheDocument();
});
```

## Key Points:
- Mock API calls.
- Mock external modules.
- Control test data.
- Verify interactions.

## Interview Tip:
"Mock external dependencies â€” test the component, not the API."

---

## Question 70: What React component testing best practices do you follow?

## Answer:
1. **Test behavior, not implementation**.
2. **Use user-centric queries** (getByRole, getByText).
3. **Test all states**: Loading, success, error.
4. **Mock external dependencies**.
5. **Keep tests independent**.
6. **Use `screen` for queries**.

## Key Points:
- Behavior over implementation.
- User-centric queries.
- All states tested.
- Mock dependencies.
- Independent tests.

## Interview Tip:
"Test what users see â€” RTL makes this natural."

---

## Part 8 (71â€“80): User Interaction Testing

---

## Question 71: How do you simulate user actions in React Testing Library?

## Answer:
```javascript
import { fireEvent, userEvent } from "@testing-library/react";

// fireEvent
fireEvent.click(button);
fireEvent.change(input, { target: { value: "hello" } });

// userEvent (more realistic)
await userEvent.click(button);
await userEvent.type(input, "hello");
```

## Key Points:
- fireEvent: basic simulation.
- userEvent: realistic simulation.
- userEvent is preferred.
- Simulate clicks, typing, keyboard.

## Interview Tip:
"userEvent is preferred â€” it simulates real user behavior more accurately."

---

## Question 72: What is `fireEvent`?

## Answer:
`fireEvent` dispatches DOM events on elements.

```javascript
fireEvent.click(button);
fireEvent.change(input, { target: { value: "text" } });
fireEvent.submit(form);
```

## Key Points:
- Dispatches DOM events.
- Basic simulation.
- Synchronous.
- Less realistic than userEvent.

## Interview Tip:
"fireEvent for quick tests; userEvent for realistic simulations."

---

## Question 73: What is `userEvent`?

## Answer:
`userEvent` simulates real user interactions more realistically than `fireEvent`.

```javascript
await userEvent.click(button);
await userEvent.type(input, "hello");
await userEvent.keyboard("{Enter}");
```

## Key Points:
- Realistic user simulation.
- Async API.
- Simulates full interaction sequence.
- Preferred over fireEvent.

## Interview Tip:
"userEvent simulates real users â€” it's the preferred approach."

---

## Question 74: What is the difference between fireEvent and userEvent?

## Answer:
- **fireEvent**: Dispatches single DOM events. Sync.
- **userEvent**: Simulates full user interaction. Async. More realistic.

userEvent simulates the entire interaction sequence (focus, keydown, keyup, input, etc.).

## Key Points:
- fireEvent: single events, sync.
- userEvent: full interactions, async.
- userEvent is more realistic.
- userEvent is preferred.

## Interview Tip:
"userEvent for realistic tests; fireEvent for quick ones."

---

## Question 75: How do you test button clicks?

## Answer:
```javascript
test("increments counter on click", async () => {
  render(<Counter />);
  await userEvent.click(screen.getByRole("button"));
  expect(screen.getByText("1")).toBeInTheDocument();
});
```

## Key Points:
- Find button by role.
- Click with userEvent.
- Assert on result.
- Test behavior.

## Interview Tip:
"getByRole('button') + userEvent.click() â€” the standard button test."

---

## Question 76: How do you test form submissions?

## Answer:
```javascript
test("submits form", async () => {
  const onSubmit = jest.fn();
  render(<LoginForm onSubmit={onSubmit} />);
  
  await userEvent.type(screen.getByLabelText("Email"), "test@example.com");
  await userEvent.type(screen.getByLabelText("Password"), "password");
  await userEvent.click(screen.getByRole("button", { name: "Login" }));
  
  expect(onSubmit).toHaveBeenCalledWith({
    email: "test@example.com",
    password: "password"
  });
});
```

## Key Points:
- Fill form fields.
- Submit form.
- Assert on submission data.
- Test validation errors.

## Interview Tip:
"Fill fields, submit, assert â€” the form test pattern."

---

## Question 77: How do you test input changes?

## Answer:
```javascript
test("updates input value", async () => {
  render(<SearchInput />);
  const input = screen.getByRole("textbox");
  await userEvent.type(input, "hello");
  expect(input).toHaveValue("hello");
});
```

## Key Points:
- Find input by role.
- Type with userEvent.
- Assert on value.
- Test onChange handler.

## Interview Tip:
"getByRole('textbox') + userEvent.type() + toHaveValue() â€” the input test."

---

## Question 78: How do you test keyboard interactions?

## Answer:
```javascript
test("submits on Enter", async () => {
  const onSubmit = jest.fn();
  render(<SearchInput onSubmit={onSubmit} />);
  await userEvent.type(screen.getByRole("textbox"), "query{Enter}");
  expect(onSubmit).toHaveBeenCalledWith("query");
});
```

## Key Points:
- Use keyboard syntax: `{Enter}`, `{Escape}`.
- Test keyboard shortcuts.
- Test accessibility interactions.

## Interview Tip:
"userEvent.type(input, 'text{Enter}') â€” type text and press Enter."

---

## Question 79: How do you test accessibility behavior?

## Answer:
```javascript
test("button is accessible", () => {
  render(<Button>Click me</Button>);
  const button = screen.getByRole("button", { name: "Click me" });
  expect(button).toBeEnabled();
});

test("input has label", () => {
  render(<Input label="Email" />);
  expect(screen.getByLabelText("Email")).toBeInTheDocument();
});
```

## Key Points:
- Test by role.
- Test by label.
- Test keyboard navigation.
- Test ARIA attributes.

## Interview Tip:
"RTL encourages accessible code â€” test by role and label."

---

## Question 80: What user interaction testing practices do you follow?

## Answer:
1. **Use userEvent over fireEvent**.
2. **Test by role, not by test-id**.
3. **Test keyboard interactions**.
4. **Test accessibility**.
5. **Test all user flows**.

## Key Points:
- userEvent for realism.
- Role-based queries.
- Keyboard interactions.
- Accessibility testing.
- Complete user flows.

## Interview Tip:
"userEvent + role-based queries + accessibility = robust interaction tests."

---

## Part 9 (81â€“90): Testing Hooks & State Management

---

## Question 81: How do you test React hooks?

## Answer:
```javascript
import { renderHook, act } from "@testing-library/react";

test("useCounter increments", () => {
  const { result } = renderHook(() => useCounter());
  
  act(() => {
    result.current.increment();
  });
  
  expect(result.current.count).toBe(1);
});
```

## Key Points:
- `renderHook` for hook testing.
- `act` for state updates.
- Access via `result.current`.
- Test hook behavior.

## Interview Tip:
"renderHook + act â€” the hook testing pattern."

---

## Question 82: What is React Hooks Testing Library?

## Answer:
React Hooks Testing Library (now part of RTL) provides `renderHook` for testing hooks in isolation.

## Key Points:
- Part of RTL.
- `renderHook` for hook testing.
- Test hooks independently.
- Mock dependencies.

## Interview Tip:
"renderHook is part of @testing-library/react â€” no separate package needed."

---

## Question 83: How do you test custom hooks?

## Answer:
```javascript
test("useLocalStorage persists value", () => {
  const { result } = renderHook(() => useLocalStorage("key", "default"));
  
  expect(result.current[0]).toBe("default");
  
  act(() => {
    result.current[1]("new value");
  });
  
  expect(result.current[0]).toBe("new value");
  expect(localStorage.getItem("key")).toBe("new value");
});
```

## Key Points:
- Test initial value.
- Test state changes.
- Test side effects.
- Mock external dependencies.

## Interview Tip:
"Test custom hooks like functions â€” input, output, side effects."

---

## Question 84: How do you test useState logic?

## Answer:
```javascript
test("useCounter state", () => {
  const { result } = renderHook(() => useCounter(0));
  
  expect(result.current.count).toBe(0);
  
  act(() => { result.current.increment(); });
  expect(result.current.count).toBe(1);
  
  act(() => { result.current.decrement(); });
  expect(result.current.count).toBe(0);
});
```

## Key Points:
- Test initial state.
- Test state changes.
- Use `act` for updates.
- Assert on each state.

## Interview Tip:
"Test state transitions â€” initial â†’ increment â†’ decrement."

---

## Question 85: How do you test useEffect behavior?

## Answer:
```javascript
test("fetches data on mount", async () => {
  const fetchSpy = jest.spyOn(api, "fetchUsers").mockResolvedValue([]);
  
  renderHook(() => useUsers());
  
  await waitFor(() => {
    expect(fetchSpy).toHaveBeenCalled();
  });
});
```

## Key Points:
- Mock side effects.
- Use `waitFor` for async.
- Verify effect ran.
- Test cleanup.

## Interview Tip:
"Mock the side effect, render, wait for it to happen."

---

## Question 86: How do you test context providers?

## Answer:
```javascript
test("provides theme context", () => {
  const wrapper = ({ children }) => (
    <ThemeProvider theme="dark">{children}</ThemeProvider>
  );
  
  const { result } = renderHook(() => useTheme(), { wrapper });
  expect(result.current.theme).toBe("dark");
});
```

## Key Points:
- Wrap with provider.
- Pass wrapper to renderHook.
- Test context value.
- Test context updates.

## Interview Tip:
"Wrap renderHook with the provider â€” that's how you test context."

---

## Question 87: How do you test Redux applications?

## Answer:
```javascript
import { Provider } from "react-redux";
import { store } from "./store";

test("increments counter", () => {
  render(
    <Provider store={store}>
      <Counter />
    </Provider>
  );
  
  fireEvent.click(screen.getByRole("button"));
  expect(screen.getByText("1")).toBeInTheDocument();
});
```

## Key Points:
- Wrap with Provider.
- Use real or mock store.
- Test dispatched actions.
- Test connected components.

## Interview Tip:
"Wrap with Provider, interact, assert â€” Redux testing."

---

## Question 88: How do you test Redux Toolkit slices?

## Answer:
```javascript
test("increments counter", () => {
  const state = counterSlice.reducer({ count: 0 }, counterSlice.actions.increment());
  expect(state.count).toBe(1);
});
```

Reducers are pure functions â€” test them directly.

## Key Points:
- Test reducers directly.
- Pure functions â€” easy to test.
- No mocking needed.
- Test each action.

## Interview Tip:
"Reducers are pure functions â€” test them like any other function."

---

## Question 89: How do you test Zustand stores?

## Answer:
```javascript
test("increments count", () => {
  const { getState, setState } = useStore;
  setState({ count: 0 });
  getState().increment();
  expect(getState().count).toBe(1);
});
```

## Key Points:
- Use `getState()` and `setState()`.
- No Provider needed.
- Test directly.
- Reset in beforeEach.

## Interview Tip:
"Zustand stores can be tested without React â€” just call getState()."

---

## Question 90: What state management testing practices do you follow?

## Answer:
1. **Test reducers directly** (Redux).
2. **Test stores directly** (Zustand).
3. **Wrap components with providers** (Redux, Context).
4. **Reset state between tests**.
5. **Mock external dependencies**.

## Key Points:
- Direct testing for pure functions.
- Provider wrapping for components.
- State reset between tests.
- Mock external dependencies.

## Interview Tip:
"Test state logic directly â€” no need to render components for reducer tests."

---

## Part 10 (91â€“100): API Mocking & Integration Testing

---

## Question 91: How do you test API calls in frontend applications?

## Answer:
Mock the API layer:
- **MSW**: Intercept network requests.
- **Jest mocks**: Mock fetch or axios.
- **Mock service workers**: Realistic API mocking.

## Key Points:
- MSW for realistic mocking.
- Jest mocks for unit tests.
- Control API responses.
- Test success and error cases.

## Interview Tip:
"MSW for integration tests; Jest mocks for unit tests."

---

## Question 92: What is mocking?

## Answer:
Mocking replaces real dependencies with controlled substitutes for testing. Mocks simulate the behavior of real objects.

## Key Points:
- Replace real dependencies.
- Controlled behavior.
- Simulate responses.
- Isolate unit under test.

## Interview Tip:
"Mocking isolates the unit under test â€” you control the environment."

---

## Question 93: Why do we mock API requests?

## Answer:
- **Speed**: No network calls.
- **Reliability**: No flaky network.
- **Control**: Simulate any response.
- **Isolation**: Test component, not API.
- **Offline**: Tests work without network.

## Key Points:
- Fast and reliable.
- Full control over responses.
- Isolate component testing.
- Work offline.

## Interview Tip:
"Mock APIs for speed, reliability, and control."

---

## Question 94: What is Mock Service Worker (MSW)?

## Answer:
MSW intercepts network requests at the network level, returning mock responses. It doesn't mock fetch â€” it intercepts actual HTTP requests.

```javascript
import { http, HttpResponse } from "msw";
import { setupServer } from "msw/node";

const server = setupServer(
  http.get("/api/users", () => {
    return HttpResponse.json([{ id: 1, name: "Alice" }]);
  })
);

beforeAll(() => server.listen());
afterAll(() => server.close());
```

## Key Points:
- Intercepts network requests.
- Realistic API mocking.
- Works in browser and Node.js.
- No code changes needed.

## Interview Tip:
"MSW intercepts at the network level â€” more realistic than mocking fetch."

---

## Question 95: How does MSW work?

## Answer:
1. Register request handlers.
2. MSW intercepts matching requests.
3. Returns mock response.
4. Application code doesn't know it's mocked.

## Key Points:
- Register handlers.
- Intercept requests.
- Return mock responses.
- Transparent to application.

## Interview Tip:
"MSW is transparent â€” your app doesn't know it's mocked."

---

## Question 96: What is the difference between mocking and stubbing?

## Answer:
- **Mock**: Verifies interactions (was the function called?).
- **Stub**: Provides canned responses (returns fake data).

## Key Points:
- Mock: verify interactions.
- Stub: provide responses.
- Mocks have assertions.
- Stubs are passive.

## Interview Tip:
"Mock to verify; stub to provide. Use mocks for behavior, stubs for data."

---

## Question 97: How do you test API success responses?

## Answer:
```javascript
test("displays users", async () => {
  server.use(
    http.get("/api/users", () => {
      return HttpResponse.json([{ id: 1, name: "Alice" }]);
    })
  );
  
  render(<UserList />);
  expect(await screen.findByText("Alice")).toBeInTheDocument();
});
```

## Key Points:
- Mock successful response.
- Render component.
- Assert on rendered data.
- Use `findBy` for async.

## Interview Tip:
"Mock success, render, assert â€” the success test pattern."

---

## Question 98: How do you test API error responses?

## Answer:
```javascript
test("shows error on failure", async () => {
  server.use(
    http.get("/api/users", () => {
      return new HttpResponse(null, { status: 500 });
    })
  );
  
  render(<UserList />);
  expect(await screen.findByText("Failed to load")).toBeInTheDocument();
});
```

## Key Points:
- Mock error response.
- Render component.
- Assert on error display.
- Test error handling.

## Interview Tip:
"Test error handling as thoroughly as success handling."

---

## Question 99: How do you test authentication flows?

## Answer:
```javascript
test("login flow", async () => {
  server.use(
    http.post("/api/login", () => {
      return HttpResponse.json({ token: "abc123" });
    })
  );
  
  render(<LoginPage />);
  await userEvent.type(screen.getByLabelText("Email"), "test@example.com");
  await userEvent.type(screen.getByLabelText("Password"), "password");
  await userEvent.click(screen.getByRole("button", { name: "Login" }));
  
  expect(await screen.findByText("Welcome")).toBeInTheDocument();
});
```

## Key Points:
- Mock login endpoint.
- Fill credentials.
- Submit form.
- Verify success.

## Interview Tip:
"Test the full auth flow â€” login, success, error, logout."

---

## Question 100: What frontend integration testing practices do you follow?

## Answer:
1. **Use MSW for API mocking**.
2. **Test full user flows**.
3. **Test success and error cases**.
4. **Mock external services**.
5. **Test authentication flows**.
6. **Clean up after tests**.

## Key Points:
- MSW for realistic mocking.
- Full user flows.
- Success and error cases.
- Auth flow testing.
- Cleanup.

## Interview Tip:
"MSW + full flows + error cases = robust integration tests."

---

## Part 11 (101â€“110): End-to-End (E2E) Testing

---

## Question 101: What is end-to-end testing?

## Answer:
E2E testing simulates real user interactions across the entire application â€” from UI to database.

## Key Points:
- Real user simulation.
- Full application stack.
- UI to database.
- Highest confidence.

## Interview Tip:
"E2E tests verify the entire system works together."

---

## Question 102: Why is E2E testing important?

## Answer:
- **Confidence**: Verifies the full stack works.
- **User perspective**: Tests what users actually do.
- **Integration**: Catches issues between layers.
- **Regression**: Prevents breaking critical flows.

## Key Points:
- Full stack verification.
- User perspective.
- Integration testing.
- Regression prevention.

## Interview Tip:
"E2E tests catch what unit and integration tests miss â€” real user flows."

---

## Question 103: How is E2E testing different from unit testing?

## Answer:
- **Unit**: Tests individual functions. Fast, cheap.
- **E2E**: Tests full user flows. Slow, expensive.

## Key Points:
- Unit: isolated, fast, many.
- E2E: full flows, slow, few.
- Unit for logic, E2E for user flows.

## Interview Tip:
"Unit tests verify logic; E2E tests verify user flows."

---

## Question 104: How is E2E testing different from integration testing?

## Answer:
- **Integration**: Tests component interactions. Mocked dependencies.
- **E2E**: Tests full application. Real dependencies.

## Key Points:
- Integration: mocked dependencies.
- E2E: real dependencies.
- E2E is slower but more realistic.

## Interview Tip:
"Integration mocks; E2E uses real services."

---

## Question 105: What tools are used for E2E testing?

## Answer:
- **Playwright**: Cross-browser, fast, modern.
- **Cypress**: Browser-based, great DX.
- **Selenium**: Established, multi-language.

## Key Points:
- Playwright: modern, fast.
- Cypress: great DX.
- Selenium: established.
- Playwright and Cypress are the modern choices.

## Interview Tip:
"Playwright for modern apps; Cypress for great DX."

---

## Question 106: What is Cypress?

## Answer:
Cypress is a JavaScript E2E testing framework that runs in the browser. It provides real-time reloading, automatic waiting, and time-travel debugging.

## Key Points:
- Browser-based testing.
- Real-time reloading.
- Automatic waiting.
- Time-travel debugging.
- Great developer experience.

## Interview Tip:
"Cypress runs in the browser â€” you can see tests execute in real time."

---

## Question 107: What is Playwright?

## Answer:
Playwright is a cross-browser E2E testing framework by Microsoft. It supports Chromium, Firefox, and WebKit.

## Key Points:
- Cross-browser testing.
- Microsoft-backed.
- Fast and reliable.
- Auto-waiting.
- Codegen tool.

## Interview Tip:
"Playwright for cross-browser testing â€” Chromium, Firefox, and WebKit."

---

## Question 108: What is the difference between Cypress and Playwright?

## Answer:
| Feature | Cypress | Playwright |
|---------|---------|------------|
| Browsers | Chromium, Firefox | Chromium, Firefox, WebKit |
| Speed | Fast | Faster |
| Parallel | Limited | Full parallel |
| Tab support | No | Yes |
| Language | JavaScript | JS, Python, Java, C# |

## Key Points:
- Playwright: more browsers, faster, parallel.
- Cypress: better DX, simpler API.
- Playwright for cross-browser.
- Cypress for simplicity.

## Interview Tip:
"Playwright for cross-browser and speed; Cypress for simplicity and DX."

---

## Question 109: When should you use Cypress?

## Answer:
- **Simple test suites**: Easy setup and API.
- **Developer experience**: Real-time feedback.
- **Chromium-only**: When cross-browser isn't needed.
- **Component testing**: Cypress supports it.

## Key Points:
- Simple test suites.
- Great DX.
- Chromium-focused.
- Component testing support.

## Interview Tip:
"Cypress for simplicity and DX â€” Playwright for cross-browser."

---

## Question 110: When should you use Playwright?

## Answer:
- **Cross-browser testing**: All major browsers.
- **Parallel execution**: Fast test suites.
- **Complex scenarios**: Multiple tabs, iframes.
- **CI/CD**: Reliable and fast.

## Key Points:
- Cross-browser support.
- Parallel execution.
- Complex scenarios.
- CI/CD optimized.

## Interview Tip:
"Playwright for cross-browser, parallel, and complex scenarios."

---

## Part 12 (111â€“120): Cypress

---

## Question 111: How does Cypress work internally?

## Answer:
Cypress runs inside the browser, alongside your application. It has direct access to the DOM, network, and browser APIs.

## Key Points:
- Runs in the browser.
- Direct DOM access.
- Real-time execution.
- Automatic waiting.

## Interview Tip:
"Cypress runs in the browser â€” that's why it's so fast and reliable."

---

## Question 112: What are Cypress commands?

## Answer:
Cypress commands are chainable methods for interacting with the application.

```javascript
cy.visit("/login");
cy.get("#email").type("test@example.com");
cy.get("#password").type("password");
cy.get("button").click();
cy.url().should("include", "/dashboard");
```

## Key Points:
- Chainable API.
- Visit, get, type, click.
- Assertions with `should()`.
- Automatic waiting.

## Interview Tip:
"Cypress commands are chainable â€” cy.get().type().click().should()"

---

## Question 113: What is Cypress test runner?

## Answer:
Cypress test runner is a GUI that shows tests executing in real-time with time-travel debugging.

## Key Points:
- Real-time test execution.
- Time-travel debugging.
- Visual feedback.
- Interactive debugging.

## Interview Tip:
"Cypress test runner lets you see exactly what happened at each step."

---

## Question 114: How do you write Cypress tests?

## Answer:
```javascript
describe("Login", () => {
  it("logs in successfully", () => {
    cy.visit("/login");
    cy.get("#email").type("user@example.com");
    cy.get("#password").type("password");
    cy.get("button").click();
    cy.url().should("include", "/dashboard");
  });
});
```

## Key Points:
- `describe` for suites.
- `it` for test cases.
- `cy` commands for actions.
- `should` for assertions.

## Interview Tip:
"describe + it + cy commands + should â€” the Cypress test structure."

---

## Question 115: How do you select elements in Cypress?

## Answer:
```javascript
cy.get("#id");                    // By ID
cy.get(".class");                 // By class
cy.get("[data-testid='item']");  // By data-testid
cy.contains("Click me");          // By text
cy.get("button").first();         // First button
```

## Key Points:
- `cy.get()` for CSS selectors.
- `cy.contains()` for text.
- `data-testid` for stability.
- Prefer `data-testid` over classes.

## Interview Tip:
"Use `data-testid` for stable selectors â€” classes and IDs change frequently."

---

## Question 116: How do you test forms using Cypress?

## Answer:
```javascript
it("submits form", () => {
  cy.visit("/form");
  cy.get("#name").type("Alice");
  cy.get("#email").type("alice@example.com");
  cy.get("form").submit();
  cy.contains("Success").should("be.visible");
});
```

## Key Points:
- Type into inputs.
- Submit form.
- Assert on result.
- Test validation errors.

## Interview Tip:
"Fill, submit, assert â€” the Cypress form test pattern."

---

## Question 117: How do you test authentication flows using Cypress?

## Answer:
```javascript
beforeEach(() => {
  cy.login(); // Custom command
});

it("shows dashboard", () => {
  cy.visit("/dashboard");
  cy.contains("Welcome").should("be.visible");
});
```

Custom command:
```javascript
Cypress.Commands.add("login", () => {
  cy.request("POST", "/api/login", { email: "test", password: "pass" })
    .then((res) => {
      window.localStorage.setItem("token", res.body.token);
    });
});
```

## Key Points:
- Custom commands for auth.
- Set tokens directly.
- Skip UI for speed.
- Test authenticated routes.

## Interview Tip:
"Custom login commands speed up tests â€” skip the UI, set the token directly."

---

## Question 118: How do you mock API responses in Cypress?

## Answer:
```javascript
it("shows users", () => {
  cy.intercept("GET", "/api/users", { body: [{ id: 1, name: "Alice" }] });
  cy.visit("/users");
  cy.contains("Alice").should("be.visible");
});
```

## Key Points:
- `cy.intercept()` for API mocking.
- Mock before visiting page.
- Control responses.
- Test different scenarios.

## Interview Tip:
"cy.intercept() mocks API responses â€” use it to test different scenarios."

---

## Question 119: How do you run Cypress tests in CI/CD?

## Answer:
```yaml
# GitHub Actions
- name: Run Cypress
  run: npx cypress run
```

```json
// package.json
{
  "scripts": {
    "test:e2e": "cypress run"
  }
}
```

## Key Points:
- `cypress run` for headless execution.
- CI/CD integration.
- Video and screenshot on failure.
- Parallel execution.

## Interview Tip:
"`cypress run` for CI â€” headless, fast, with video on failure."

---

## Question 120: What Cypress best practices do you follow?

## Answer:
1. **Use data-testid for selectors**.
2. **Custom commands for common flows**.
3. **Intercept API calls**.
4. **Test critical user flows**.
5. **Clean up state between tests**.
6. **Don't test implementation details**.

## Key Points:
- data-testid selectors.
- Custom commands.
- API interception.
- Critical flows.
- State cleanup.

## Interview Tip:
"data-testid + custom commands + API interception = robust Cypress tests."

---

## Part 13 (121â€“130): Playwright

---

## Question 121: What is Playwright?

## Answer:
Playwright is a cross-browser E2E testing framework by Microsoft. It supports Chromium, Firefox, and WebKit with a single API.

## Key Points:
- Cross-browser testing.
- Microsoft-backed.
- Fast and reliable.
- Auto-waiting built-in.
- Codegen tool.

## Interview Tip:
"Playwright tests all browsers with one API â€” Chromium, Firefox, WebKit."

---

## Question 122: Why is Playwright popular for modern applications?

## Answer:
- **Cross-browser**: All major browsers.
- **Fast**: Parallel execution.
- **Reliable**: Auto-waiting, no flaky tests.
- **Modern**: Supports latest web features.
- **Codegen**: Record tests automatically.

## Key Points:
- Cross-browser support.
- Fast parallel execution.
- Reliable auto-waiting.
- Modern web support.
- Code generation.

## Interview Tip:
"Playwright is fast, reliable, and cross-browser â€” the modern E2E standard."

---

## Question 123: What browsers does Playwright support?

## Answer:
- **Chromium**: Chrome, Edge.
- **Firefox**: Mozilla Firefox.
- **WebKit**: Safari.

## Key Points:
- Chromium (Chrome, Edge).
- Firefox.
- WebKit (Safari).
- All with one API.

## Interview Tip:
"Playwright tests Chrome, Firefox, and Safari â€” full browser coverage."

---

## Question 124: How do you write Playwright tests?

## Answer:
```javascript
import { test, expect } from "@playwright/test";

test("login flow", async ({ page }) => {
  await page.goto("/login");
  await page.fill("#email", "user@example.com");
  await page.fill("#password", "password");
  await page.click("button");
  await expect(page).toHaveURL("/dashboard");
});
```

## Key Points:
- `test()` for test cases.
- `page` fixture for browser page.
- `await` for all actions.
- `expect` for assertions.

## Interview Tip:
"Playwright uses async/await â€” every action is awaited."

---

## Question 125: What are Playwright locators?

## Answer:
Locators find elements on the page.

```javascript
page.getByRole("button", { name: "Submit" });
page.getByText("Welcome");
page.getByLabel("Email");
page.getByTestId("submit-btn");
page.locator(".my-class");
```

## Key Points:
- getByRole, getByText, getByLabel.
- getByTestId for stable selectors.
- locator() for CSS selectors.
- User-centric queries.

## Interview Tip:
"getByRole is the preferred locator â€” it's accessible and stable."

---

## Question 126: How do you handle multiple pages in Playwright?

## Answer:
```javascript
test("opens new tab", async ({ page, context }) => {
  const newPage = await context.newPage();
  await newPage.goto("https://example.com");
  // Work with both pages
});
```

## Key Points:
- `context.newPage()` for new tabs.
- Work with multiple pages.
- Cross-tab testing.
- Native support.

## Interview Tip:
"Playwright handles multiple pages natively â€” great for testing popups and tabs."

---

## Question 127: How do you handle authentication in Playwright?

## Answer:
```javascript
// playwright.config.ts
import { defineConfig } from "@playwright/test";

export default defineConfig({
  use: {
    storageState: "auth.json" // Saved auth state
  }
});
```

Save auth state once, reuse in all tests.

## Key Points:
- Save auth state.
- Reuse across tests.
- Skip login in most tests.
- Fast test execution.

## Interview Tip:
"Save auth state once, reuse everywhere â€” skip login in most tests."

---

## Question 128: How do you run Playwright tests in CI/CD?

## Answer:
```yaml
- name: Run Playwright
  run: npx playwright test
```

```bash
npx playwright test --reporter=html
```

## Key Points:
- `npx playwright test` for execution.
- HTML reporter for results.
- Parallel by default.
- CI/CD integration.

## Interview Tip:
"`npx playwright test` runs all tests â€” parallel by default."

---

## Question 129: What are Playwright fixtures?

## Answer:
Fixtures provide test context â€” browser, page, context.

```javascript
test("my test", async ({ page, context, browser }) => {
  // page: current page
  // context: browser context
  // browser: browser instance
});
```

## Key Points:
- Provide test context.
- page, context, browser.
- Custom fixtures possible.
- Automatic setup/teardown.

## Interview Tip:
"Fixtures provide the test environment â€” page, context, browser."

---

## Question 130: What Playwright best practices do you follow?

## Answer:
1. **Use getByRole for selectors**.
2. **Save auth state**.
3. **Test critical flows**.
4. **Use page object model for complex pages**.
5. **Parallel execution**.
6. **CI/CD integration**.

## Key Points:
- getByRole selectors.
- Saved auth state.
- Critical flows.
- Page objects for complex pages.
- Parallel execution.

## Interview Tip:
"getByRole + auth state + parallel execution = robust Playwright tests."

---

## Part 14 (131â€“140): Testing Architecture & Strategy

---

## Question 131: How do you decide what to test?

## Answer:
1. **Critical paths**: Core business flows.
2. **Complex logic**: Business rules, calculations.
3. **Edge cases**: Boundary conditions.
4. **Error handling**: Failure scenarios.
5. **Regression-prone areas**: Frequently broken code.

## Key Points:
- Critical paths first.
- Complex logic.
- Edge cases.
- Error handling.
- Regression-prone areas.

## Interview Tip:
"Test critical paths first â€” that's where bugs have the most impact."

---

## Question 132: How do you design a testing strategy for a large application?

## Answer:
1. **Unit tests**: Business logic, utilities, hooks.
2. **Integration tests**: API endpoints, component interactions.
3. **E2E tests**: Critical user flows.
4. **CI/CD**: Run tests automatically.
5. **Coverage targets**: Critical paths 100%, overall 70-80%.

## Key Points:
- Unit for logic.
- Integration for APIs.
- E2E for critical flows.
- CI/CD for automation.
- Coverage targets.

## Interview Tip:
"Testing strategy = unit + integration + E2E + CI/CD."

---

## Question 133: How do you balance unit, integration, and E2E tests?

## Answer:
Follow the testing pyramid:
- **Many unit tests**: Fast, cheap, focused.
- **Some integration tests**: Test interactions.
- **Few E2E tests**: Slow, expensive, broad.

## Key Points:
- Many unit tests.
- Some integration tests.
- Few E2E tests.
- Balance speed and coverage.

## Interview Tip:
"Testing pyramid: many unit, some integration, few E2E."

---

## Question 134: What is test-driven development (TDD)?

## Answer:
TDD is a development approach where you write tests before writing the code:
1. **Write a failing test**.
2. **Write minimal code to pass**.
3. **Refactor**.
4. **Repeat**.

## Key Points:
- Tests first, then code.
- Red-green-refactor cycle.
- Better design.
- Full test coverage.

## Interview Tip:
"TDD: write the test, make it pass, refactor â€” the red-green-refactor cycle."

---

## Question 135: What is behavior-driven development (BDD)?

## Answer:
BDD extends TDD by writing tests in natural language, describing expected behavior.

```gherkin
Given a user with valid credentials
When they submit the login form
Then they should see the dashboard
```

## Key Points:
- Natural language tests.
- Given-When-Then syntax.
- Stakeholder-readable.
- Cucumber, Jest.

## Interview Tip:
"BDD makes tests readable for non-technical stakeholders."

---

## Question 136: What is the difference between TDD and BDD?

## Answer:
- **TDD**: Tests written in code. Developer-focused.
- **BDD**: Tests written in natural language. Stakeholder-focused.

## Key Points:
- TDD: code-based, developer-focused.
- BDD: natural language, stakeholder-focused.
- Both: tests first.
- BDD extends TDD.

## Interview Tip:
"TDD for developers, BDD for collaboration with stakeholders."

---

## Question 137: What is test automation strategy?

## Answer:
1. **Automate repetitive tests**.
2. **Automate regression tests**.
3. **Automate smoke tests**.
4. **Run in CI/CD**.
5. **Report and track results**.

## Key Points:
- Automate repetitive tests.
- Regression and smoke tests.
- CI/CD integration.
- Result tracking.

## Interview Tip:
"Automate what's repetitive and critical â€” manual testing for exploration."

---

## Question 138: How do you maintain test cases as applications grow?

## Answer:
1. **Refactor tests alongside code**.
2. **Remove obsolete tests**.
3. **Keep tests focused and small**.
4. **Use page objects for E2E**.
5. **Regular test review**.

## Key Points:
- Refactor tests with code.
- Remove obsolete tests.
- Focused and small tests.
- Page objects for E2E.
- Regular review.

## Interview Tip:
"Tests need maintenance too â€” refactor and remove obsolete tests."

---

## Question 139: How do you handle flaky tests?

## Answer:
1. **Identify the flake**: Isolate the failure.
2. **Fix the root cause**: Race conditions, timing issues.
3. **Add retries**: For genuinely flaky tests.
4. **Quarantine**: Separate flaky tests.
5. **Fix or delete**: Don't ignore flaky tests.

## Key Points:
- Identify and fix root cause.
- Add retries for genuine flakes.
- Quarantine flaky tests.
- Fix or delete â€” don't ignore.

## Interview Tip:
"Flaky tests erode trust â€” fix them or delete them."

---

## Question 140: What testing architecture practices do you follow?

## Answer:
1. **Testing pyramid**: Many unit, some integration, few E2E.
2. **CI/CD integration**: Run tests automatically.
3. **Test isolation**: Tests don't depend on each other.
4. **Fast feedback**: Unit tests in seconds.
5. **Coverage monitoring**: Track and improve.

## Key Points:
- Testing pyramid.
- CI/CD integration.
- Test isolation.
- Fast feedback.
- Coverage monitoring.

## Interview Tip:
"Testing pyramid + CI/CD + isolation + fast feedback = robust testing architecture."

---

## Part 15 (141â€“150): Senior Real-World Testing Questions

---

## Question 141: Describe the testing strategy you used in a real project.

## Answer:
Choose a real project and describe:
- **Unit tests**: Business logic and utilities.
- **Integration tests**: API endpoints with MSW.
- **E2E tests**: Critical user flows with Playwright.
- **CI/CD**: All tests run on every PR.
- **Coverage**: 80%+ on critical paths.

## Key Points:
- Describe real testing strategy.
- Explain choices and trade-offs.
- Show impact and results.
- Mention tools used.

## Interview Tip:
"Describe the strategy, tools, and results â€” interviewers want to see real experience."

---

## Question 142: How do you test a large Next.js application?

## Answer:
- **Unit tests**: Server Components, utilities, hooks.
- **Integration tests**: API routes with MSW.
- **E2E tests**: Critical user flows with Playwright.
- **Server Component testing**: Render and assert.
- **API route testing**: Supertest or direct calls.

## Key Points:
- Unit for logic.
- Integration for API routes.
- E2E for user flows.
- Server Component testing.
- API route testing.

## Interview Tip:
"Next.js testing: unit for logic, integration for API routes, E2E for flows."

---

## Question 143: How would you test a full-stack application with React, Node.js, and PostgreSQL?

## Answer:
- **Frontend**: RTL for components, MSW for API mocking.
- **Backend**: Jest for services, Supertest for API endpoints.
- **Database**: Test database with migrations.
- **E2E**: Playwright for full user flows.

## Key Points:
- RTL for frontend.
- Jest + Supertest for backend.
- Test database.
- Playwright for E2E.

## Interview Tip:
"Frontend: RTL + MSW. Backend: Jest + Supertest. E2E: Playwright."

---

## Question 144: How do you test authentication and authorization?

## Answer:
- **Unit tests**: Auth logic, token validation.
- **Integration tests**: Login flow, protected routes.
- **E2E tests**: Full auth flow.
- **Security tests**: Token expiration, invalid tokens.

## Key Points:
- Auth logic unit tests.
- Login flow integration tests.
- Full auth E2E tests.
- Security edge cases.

## Interview Tip:
"Test auth at every level â€” logic, flow, and security."

---

## Question 145: How do you test database-related functionality?

## Answer:
- **Test database**: Separate test database.
- **Migrations**: Run before tests.
- **Seeding**: Consistent test data.
- **Cleanup**: Reset between tests.
- **Transactions**: Rollback after tests.

## Key Points:
- Separate test database.
- Migrations and seeding.
- Cleanup between tests.
- Transaction rollback.

## Interview Tip:
"Use a separate test database with migrations and cleanup."

---

## Question 146: How do you integrate tests into CI/CD pipelines?

## Answer:
```yaml
- name: Run tests
  run: npm test
  
- name: Run E2E tests
  run: npx playwright test
  
- name: Check coverage
  run: npm run test:coverage
```

## Key Points:
- Run unit tests on every push.
- Run E2E tests on PR.
- Check coverage.
- Block merge on failure.

## Interview Tip:
"Unit tests on every push; E2E tests on PR; block merge on failure."

---

## Question 147: How do you improve slow-running test suites?

## Answer:
1. **Parallel execution**: Run tests in parallel.
2. **Test isolation**: Independent tests.
3. **Mock external services**: Avoid real API calls.
4. **Skip unnecessary tests**: Only run affected tests.
5. **Optimize setup**: Reduce test setup time.

## Key Points:
- Parallel execution.
- Test isolation.
- Mock external services.
- Skip unnecessary tests.
- Optimize setup.

## Interview Tip:
"Parallel execution and mocking are the biggest wins for test speed."

---

## Question 148: What testing mistakes do junior developers commonly make?

## Answer:
1. **Testing implementation details**.
2. **Not testing error states**.
3. **Brittle selectors** (classes instead of roles).
4. **Slow tests** (not mocking).
5. **Flaky tests** (race conditions).
6. **100% coverage obsession**.

## Key Points:
- Implementation details.
- Missing error tests.
- Brittle selectors.
- Slow and flaky tests.
- Coverage obsession.

## Interview Tip:
"The biggest mistake is testing implementation details â€” test behavior."

---

## Question 149: What testing practices do senior engineers follow?

## Answer:
1. **Test behavior, not implementation**.
2. **Test critical paths thoroughly**.
3. **Maintain tests alongside code**.
4. **Mock external dependencies**.
5. **Keep tests fast and reliable**.
6. **Review tests in PRs**.

## Key Points:
- Behavior over implementation.
- Critical paths.
- Maintain tests.
- Mock dependencies.
- Fast and reliable.
- Review tests.

## Interview Tip:
"Seniors test behavior, maintain tests, and review tests in PRs."

---

## Question 150: In your opinion, what separates a junior, mid-level, and senior developer regarding testing?

## Answer:
- **Junior**: Writes basic unit tests. Tests happy paths.
- **Mid-level**: Writes integration tests. Tests edge cases and errors. Uses mocking.
- **Senior**: Designs testing strategy. Tests critical paths thoroughly. Maintains test quality. Mentors team.

## Key Points:
- Junior: basic unit tests.
- Mid-level: integration, edge cases, mocking.
- Senior: strategy, critical paths, mentoring.

## Interview Tip:
"Seniors design testing strategy and mentor the team â€” not just write tests."

---

# End of Testing Interview Questions & Answers
