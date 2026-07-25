# Web Security Interview Questions (200 Total)

---

# Web Security Fundamentals

1. What is web security?
2. Why is web security important?
3. What are common web security threats?
4. What is the difference between authentication and authorization?
5. What is identity management?
6. What is access control?
7. What is the principle of least privilege?
8. What is a security vulnerability?
9. What is an exploit?
10. What is the difference between threat, vulnerability, and risk?

---

# Authentication Fundamentals

11. What is authentication?
12. What are different authentication methods?
13. What is password-based authentication?
14. What is token-based authentication?
15. What is session-based authentication?
16. What is multi-factor authentication (MFA)?
17. Why is MFA important?
18. What are the best practices for password storage?
19. Why should passwords never be stored as plain text?
20. What is password hashing?

---

# Password Security

21. What is hashing?
22. How is hashing different from encryption?
23. What hashing algorithms are commonly used for passwords?
24. What is bcrypt?
25. What is salt in password hashing?
26. Why are salts used?
27. What is password stretching?
28. What is brute-force attack?
29. How do you prevent brute-force attacks?
30. What is account lockout?

---

# Session-Based Authentication

31. What is session authentication?
32. How does session-based authentication work?
33. Where are sessions stored?
34. What is a session ID?
35. How are sessions secured?
36. What are session cookies?
37. What is session expiration?
38. What happens when a session expires?
39. What is session hijacking?
40. How do you prevent session hijacking?

---

# Authorization & Access Control

41. What is authorization?
42. What is Role-Based Access Control (RBAC)?
43. What is Attribute-Based Access Control (ABAC)?
44. What is permission-based authorization?
45. What is the difference between roles and permissions?
46. How do you implement RBAC in a Node.js application?
47. How do you secure admin routes?
48. What is privilege escalation?
49. How do you prevent unauthorized access?
50. What authorization strategies have you implemented?

---

# JWT Authentication

51. What is JWT?
52. Why is JWT commonly used for authentication?
53. How does JWT authentication work?
54. What are the three parts of a JWT?
55. What is JWT header?
56. What is JWT payload?
57. What is JWT signature?
58. Is JWT encrypted or encoded?
59. What information should not be stored in JWT payload?
60. What are the advantages of JWT?

---

# JWT Security

61. What are the disadvantages of JWT authentication?
62. How do you invalidate a JWT token?
63. What is JWT expiration time?
64. What is an access token?
65. What is a refresh token?
66. Why do we need refresh tokens?
67. How does refresh token rotation work?
68. Where should JWT tokens be stored?
69. JWT in localStorage vs cookies: which is safer?
70. How do you secure JWT-based authentication?

---

# OAuth & OpenID Connect

71. What is OAuth?
72. Why is OAuth used?
73. What problem does OAuth solve?
74. What are OAuth roles?
75. What is a resource owner?
76. What is a client in OAuth?
77. What is an authorization server?
78. What is an access token in OAuth?
79. What is OpenID Connect?
80. OAuth vs OpenID Connect: what is the difference?

---

# Cookies & Browser Security

81. What are HTTP cookies?
82. How do cookies work?
83. What are session cookies?
84. What are persistent cookies?
85. What is HttpOnly cookie?
86. What is Secure cookie flag?
87. What is SameSite cookie attribute?
88. How do cookies help authentication?
89. What are cookie security risks?
90. How do you secure authentication cookies?

---

# CORS

91. What is CORS?
92. Why does CORS exist?
93. How does the browser enforce CORS?
94. What is a preflight request?
95. What is an OPTIONS request?
96. What are CORS headers?
97. How do you configure CORS in Express.js?
98. What is the difference between CORS and CSRF?
99. Why does CORS not protect APIs completely?
100. What CORS mistakes do developers commonly make?

---

# OWASP Top 10 Fundamentals

101. What is OWASP?
102. What is OWASP Top 10?
103. Why is OWASP important for developers?
104. What are the most common web application vulnerabilities?
105. How do you use OWASP guidelines in development?
106. What is broken access control?
107. How do you prevent broken access control?
108. What is security misconfiguration?
109. What is insecure design?
110. What is software supply chain security?

---

# Cross-Site Scripting (XSS)

111. What is XSS attack?
112. Why does XSS happen?
113. What are the different types of XSS?
114. What is stored XSS?
115. What is reflected XSS?
116. What is DOM-based XSS?
117. How can attackers exploit XSS?
118. How do you prevent XSS attacks?
119. What is input sanitization?
120. What is output encoding?

---

# Cross-Site Request Forgery (CSRF)

121. What is CSRF attack?
122. How does CSRF work?
123. Why are cookies vulnerable to CSRF?
124. What is a CSRF token?
125. How do CSRF tokens prevent attacks?
126. What is SameSite cookie protection?
127. CSRF vs XSS: what is the difference?
128. How do you prevent CSRF in Express.js?
129. Does JWT prevent CSRF?
130. When is CSRF protection required?

---

# SQL Injection & Database Security

131. What is SQL Injection?
132. How does SQL Injection happen?
133. What damage can SQL Injection cause?
134. How do you prevent SQL Injection?
135. What are prepared statements?
136. How do ORMs prevent SQL Injection?
137. Is Prisma completely safe from SQL Injection?
138. What is NoSQL Injection?
139. How do you prevent NoSQL Injection?
140. What database security practices do you follow?

---

# API Security

141. What are common API security threats?
142. How do you secure REST APIs?
143. What is API authentication?
144. What is API authorization?
145. What is API rate limiting?
146. Why is rate limiting important?
147. What is API throttling?
148. How do you prevent API abuse?
149. How do you secure API keys?
150. What API security practices do you follow?

---

# Encryption & Data Protection

151. What is encryption?
152. What is the difference between encryption and hashing?
153. What are symmetric encryption and asymmetric encryption?
154. How does symmetric encryption work?
155. How does asymmetric encryption work?
156. What is public key encryption?
157. What is private key encryption?
158. What is AES encryption?
159. What is RSA encryption?
160. When should you use encryption?

---

# HTTPS & TLS

161. What is HTTPS?
162. How does HTTPS work?
163. What is TLS?
164. What happens during a TLS handshake?
165. What is an SSL certificate?
166. How does certificate validation work?
167. Why is HTTPS important?
168. What attacks does HTTPS prevent?
169. What happens if HTTPS is not used?
170. How do you configure HTTPS in production?

---

# Security Headers

171. What are HTTP security headers?
172. Why are security headers important?
173. What is Content Security Policy (CSP)?
174. How does CSP prevent XSS?
175. What is X-Frame-Options?
176. What is HSTS?
177. What is X-Content-Type-Options?
178. What is Referrer-Policy?
179. What security headers should every production app have?
180. How do you configure security headers in Node.js?

---

# Secure Application Architecture

181. How do you design a secure full-stack application?
182. What security layers should a modern application have?
183. How do you secure a Next.js application?
184. How do you secure a Node.js API?
185. How do you implement authentication securely?
186. How do you design authorization for large applications?
187. How do you protect sensitive user data?
188. How do you handle secrets in production?
189. How do you perform security reviews?
190. What security practices do you follow during development?

---

# Production Security & Monitoring

191. How do you detect security attacks in production?
192. What is security logging?
193. What information should not be logged?
194. How do you monitor suspicious activities?
195. What is intrusion detection?
196. How do you handle a security breach?
197. How do you manage dependency vulnerabilities?
198. What tools can scan applications for vulnerabilities?
199. What security mistakes do junior developers commonly make?
200. What separates junior, mid-level, and senior developers in web security?

---

# ANSWERS


---

## Part 1 (1â€“10): Web Security Fundamentals

---

## Question 1: What is web security?

## Answer:
Web security is the practice of protecting web applications, servers, and users from cyber threats. It encompasses authentication, authorization, data protection, input validation, and defense against common attacks like XSS, CSRF, and SQL injection.

## Key Points:
- Protecting web apps from threats.
- Authentication and authorization.
- Data protection and encryption.
- Input validation and sanitization.
- Defense against common attacks.

## Interview Tip:
"Web security is defense in depth â€” multiple layers of protection."

---

## Question 2: Why is web security important?

## Answer:
- **Data protection**: Prevent data breaches and leaks.
- **User trust**: Users expect their data to be safe.
- **Legal compliance**: GDPR, HIPAA, PCI-DSS requirements.
- **Financial impact**: Breaches cost millions.
- **Reputation**: Security incidents damage brands.

## Key Points:
- Data protection and privacy.
- User trust and reputation.
- Legal compliance.
- Financial impact.
- Business continuity.

## Interview Tip:
"Security is not optional â€” it's a business requirement."

---

## Question 3: What are common web security threats?

## Answer:
- **XSS**: Cross-Site Scripting.
- **CSRF**: Cross-Site Request Forgery.
- **SQL Injection**: Database manipulation.
- **Authentication bypass**: Unauthorized access.
- **Data exposure**: Sensitive data leaks.
- **DDoS**: Distributed Denial of Service.

## Key Points:
- XSS, CSRF, SQL Injection.
- Authentication bypass.
- Data exposure.
- DDoS attacks.

## Interview Tip:
"OWASP Top 10 covers the most common threats â€” know them all."

---

## Question 4: What is the difference between authentication and authorization?

## Answer:
- **Authentication**: "Who are you?" â€” verifying identity.
- **Authorization**: "What can you do?" â€” checking permissions.

Authentication happens first, then authorization.

## Key Points:
- Authentication: identity verification.
- Authorization: permission checking.
- Authentication first, then authorization.
- 401 for auth failure, 403 for authorization failure.

## Interview Tip:
"401 = not authenticated. 403 = not authorized."

---

## Question 5: What is identity management?

## Answer:
Identity management is the process of managing user identities â€” creation, authentication, authorization, and lifecycle management.

## Key Points:
- User identity lifecycle.
- Account creation and deletion.
- Authentication and authorization.
- Single Sign-On (SSO).

## Interview Tip:
"Identity management is the foundation of security â€” know who your users are."

---

## Question 6: What is access control?

## Answer:
Access control determines who can access what resources. It's the enforcement of authorization policies.

## Key Points:
- Who can access what.
- Enforcement of authorization.
- RBAC, ABAC models.
- Principle of least privilege.

## Interview Tip:
"Access control is authorization in action â€” enforcing who can do what."

---

## Question 7: What is the principle of least privilege?

## Answer:
Give users and systems only the minimum permissions needed to perform their task. No more.

## Key Points:
- Minimum necessary permissions.
- Reduces attack surface.
- Limits damage from compromised accounts.
- Apply to users, services, and databases.

## Interview Tip:
"Least privilege = minimum permissions for the minimum time."

---

## Question 8: What is a security vulnerability?

## Answer:
A security vulnerability is a weakness in a system that can be exploited by an attacker to gain unauthorized access or cause damage.

## Key Points:
- Weakness in a system.
- Can be exploited by attackers.
- Software bugs, misconfigurations, design flaws.
- CVE database tracks vulnerabilities.

## Interview Tip:
"Vulnerabilities are weaknesses â€” find and fix them before attackers do."

---

## Question 9: What is an exploit?

## Answer:
An exploit is code or technique that takes advantage of a vulnerability to compromise a system.

## Key Points:
- Takes advantage of vulnerabilities.
- Can be code, technique, or tool.
- Used by attackers to compromise systems.
- Zero-day exploits target unknown vulnerabilities.

## Interview Tip:
"An exploit is a weapon that targets a vulnerability."

---

## Question 10: What is the difference between threat, vulnerability, and risk?

## Answer:
- **Threat**: A potential danger (attacker, malware).
- **Vulnerability**: A weakness that can be exploited.
- **Risk**: The likelihood and impact of a threat exploiting a vulnerability.

Risk = Threat Ã— Vulnerability Ã— Impact

## Key Points:
- Threat: potential danger.
- Vulnerability: weakness.
- Risk: likelihood Ã— impact.
- Reduce risk by reducing vulnerabilities.

## Interview Tip:
"Risk = Threat Ã— Vulnerability â€” reduce either to reduce risk."

---

## Part 2 (11â€“20): Authentication Fundamentals

---

## Question 11: What is authentication?

## Answer:
Authentication is the process of verifying a user's identity â€” confirming they are who they claim to be.

## Key Points:
- Verifying identity.
- "Who are you?"
- Credentials verification.
- Foundation of security.

## Interview Tip:
"Authentication proves identity â€” it's the first step in security."

---

## Question 12: What are different authentication methods?

## Answer:
- **Password-based**: Username and password.
- **Token-based**: JWT, API keys.
- **Session-based**: Server-side sessions.
- **OAuth**: Third-party authentication.
- **Biometric**: Fingerprint, face recognition.
- **Passwordless**: Magic links, passkeys.

## Key Points:
- Password-based, token-based, session-based.
- OAuth for third-party.
- Biometric and passwordless emerging.

## Interview Tip:
"Choose authentication method based on security requirements and user experience."

---

## Question 13: What is password-based authentication?

## Answer:
Users provide a username and password. The server hashes the password and compares it with the stored hash.

## Key Points:
- Username and password.
- Server hashes and compares.
- Never store plain text passwords.
- Use bcrypt, scrypt, or Argon2.

## Interview Tip:
"Password-based auth is simple but requires careful password storage."

---

## Question 14: What is token-based authentication?

## Answer:
The server issues a token (usually JWT) after successful authentication. The client sends the token with each request.

## Key Points:
- Server issues token after authentication.
- Client sends token with requests.
- Stateless â€” no server-side session.
- JWT is the most common token format.

## Interview Tip:
"Token-based auth is stateless â€” the token contains all needed information."

---

## Question 15: What is session-based authentication?

## Answer:
The server creates a session and stores session data. A session ID is sent to the client as a cookie.

## Key Points:
- Server creates and stores session.
- Session ID sent as cookie.
- Server-side state.
- Session expires after timeout.

## Interview Tip:
"Session-based auth is stateful â€” the server stores session data."

---

## Question 16: What is multi-factor authentication (MFA)?

## Answer:
MFA requires two or more verification factors:
- **Something you know**: Password.
- **Something you have**: Phone, token.
- **Something you are**: Biometric.

## Key Points:
- Two or more factors.
- Password + phone (most common).
- Significantly increases security.
- Industry standard for sensitive accounts.

## Interview Tip:
"MFA is the single most effective security improvement â€” implement it."

---

## Question 17: Why is MFA important?

## Answer:
- **Passwords are weak**: Users reuse passwords, choose weak ones.
- **Credential stuffing**: Stolen passwords from breaches.
- **Phishing**: Users give away passwords.
- **99% reduction**: MFA blocks 99% of automated attacks.

## Key Points:
- Passwords are inherently weak.
- Blocks automated attacks.
- Reduces breach impact.
- Industry standard.

## Interview Tip:
"MFA blocks 99% of automated attacks â€” it's the most impactful security measure."

---

## Question 18: What are the best practices for password storage?

## Answer:
1. **Hash passwords**: Use bcrypt, scrypt, or Argon2.
2. **Salt passwords**: Unique salt per password.
3. **Never store plain text**: Always hash.
4. **Use strong algorithms**: bcrypt with cost factor 12+.
5. **Don't use MD5 or SHA**: Too fast for password hashing.

## Key Points:
- Hash with bcrypt, scrypt, or Argon2.
- Unique salt per password.
- Never store plain text.
- Strong algorithms only.

## Interview Tip:
"bcrypt with cost factor 12+ is the standard â€” it's slow by design to prevent brute force."

---

## Question 19: Why should passwords never be stored as plain text?

## Answer:
- **Data breaches**: Attackers get all passwords.
- **Insider threats**: Employees can see passwords.
- **Legal liability**: Negligence in security.
- **User trust**: Users expect password protection.

## Key Points:
- Breaches expose plain text passwords.
- Insider threats.
- Legal liability.
- User trust.

## Interview Tip:
"Plain text passwords are a liability â€” always hash them."

---

## Question 20: What is password hashing?

## Answer:
Hashing converts a password into a fixed-length string using a one-way function. The same input always produces the same output, but the output can't be reversed.

## Key Points:
- One-way function.
- Same input = same output.
- Can't reverse the hash.
- Salt prevents rainbow table attacks.

## Interview Tip:
"Hashing is one-way â€” you can verify a password but never recover it."

---

## Part 3 (21â€“30): Password Security

---

## Question 21: What is hashing?

## Answer:
Hashing is a one-way function that converts input data into a fixed-length string. It's deterministic (same input = same output) and irreversible.

## Key Points:
- One-way function.
- Deterministic.
- Irreversible.
- Fixed-length output.

## Interview Tip:
"Hashing is one-way; encryption is two-way."

---

## Question 22: How is hashing different from encryption?

## Answer:
- **Hashing**: One-way, irreversible. Used for passwords.
- **Encryption**: Two-way, reversible with key. Used for data protection.

## Key Points:
- Hashing: one-way, irreversible.
- Encryption: two-way, reversible.
- Hashing for passwords.
- Encryption for data.

## Interview Tip:
"Hashing for passwords, encryption for data."

---

## Question 23: What hashing algorithms are commonly used for passwords?

## Answer:
- **bcrypt**: Industry standard, slow by design.
- **scrypt**: Memory-hard, resistant to GPU attacks.
- **Argon2**: Winner of Password Hashing Competition.
- **PBKDF2**: NIST recommended.

Never use MD5, SHA-1, or SHA-256 for passwords â€” they're too fast.

## Key Points:
- bcrypt, scrypt, Argon2, PBKDF2.
- Slow by design.
- Never use MD5 or SHA for passwords.

## Interview Tip:
"bcrypt is the standard; Argon2 is the modern choice."

---

## Question 24: What is bcrypt?

## Answer:
bcrypt is a password hashing algorithm designed to be slow and resistant to brute-force attacks. It automatically handles salting and supports a configurable cost factor.

## Key Points:
- Slow by design.
- Automatic salting.
- Configurable cost factor.
- Industry standard for password hashing.

## Interview Tip:
"bcrypt is slow on purpose â€” that's a feature, not a bug."

---

## Question 25: What is salt in password hashing?

## Answer:
Salt is random data added to a password before hashing. Each password gets a unique salt, preventing rainbow table attacks.

## Key Points:
- Random data added to password.
- Unique per password.
- Prevents rainbow table attacks.
- Stored alongside the hash.

## Interview Tip:
"Salt makes each hash unique â€” even identical passwords produce different hashes."

---

## Question 26: Why are salts used?

## Answer:
- **Prevent rainbow table attacks**: Pre-computed hash tables become useless.
- **Unique hashes**: Same password produces different hashes.
- **Security**: Makes brute-force harder.

## Key Points:
- Prevent rainbow table attacks.
- Unique hashes per password.
- Increased security.

## Interview Tip:
"Salts prevent pre-computed attacks â€” each password needs its own brute-force effort."

---

## Question 27: What is password stretching?

## Answer:
Password stretching applies the hashing function multiple times to make brute-force attacks slower. bcrypt's cost factor controls this.

## Key Points:
- Multiple hash iterations.
- Slows brute-force attacks.
- bcrypt cost factor.
- Configurable difficulty.

## Interview Tip:
"Password stretching makes brute-force impractical â€” that's why bcrypt is slow."

---

## Question 28: What is brute-force attack?

## Answer:
A brute-force attack tries every possible password until the correct one is found. With fast hashing (MD5), billions of attempts per second are possible.

## Key Points:
- Try every possible password.
- Fast hashing enables billions of attempts.
- Slow hashing (bcrypt) makes it impractical.
- Rate limiting adds protection.

## Interview Tip:
"Brute-force is why we use slow hashing â€” bcrypt makes billions of attempts impossible."

---

## Question 29: How do you prevent brute-force attacks?

## Answer:
1. **Rate limiting**: Limit login attempts per IP/account.
2. **Account lockout**: Lock after failed attempts.
3. **Slow hashing**: bcrypt makes each attempt expensive.
4. **CAPTCHA**: Distinguish humans from bots.
5. **MFA**: Second factor blocks automated attacks.

## Key Points:
- Rate limiting.
- Account lockout.
- Slow hashing.
- CAPTCHA.
- MFA.

## Interview Tip:
"Rate limiting + slow hashing + MFA = strong brute-force protection."

---

## Question 30: What is account lockout?

## Answer:
Account lockout temporarily disables an account after too many failed login attempts, preventing brute-force attacks.

## Key Points:
- Disable after failed attempts.
- Temporary lockout.
- Prevents brute-force.
- Notify user of lockout.

## Interview Tip:
"Account lockout protects against brute-force but can be abused for DoS â€” use progressive delays instead."

---

## Part 4 (31â€“40): Session-Based Authentication

---

## Question 31: What is session authentication?

## Answer:
Session authentication stores user state on the server. After login, the server creates a session and sends a session ID cookie to the client.

## Key Points:
- Server-side state.
- Session ID cookie.
- Server validates session on each request.
- Stateful authentication.

## Interview Tip:
"Session auth stores state on the server â€” the cookie is just a key."

---

## Question 32: How does session-based authentication work?

## Answer:
1. User logs in with credentials.
2. Server creates session, stores session data.
3. Server sends session ID as cookie.
4. Client sends cookie with each request.
5. Server looks up session by ID.

## Key Points:
- Login creates session.
- Session ID sent as cookie.
- Server validates on each request.
- Stateful.

## Interview Tip:
"The session ID is just a key â€” the real data is on the server."

---

## Question 33: Where are sessions stored?

## Answer:
- **Memory**: Fast but lost on restart.
- **Database**: Persistent but slower.
- **Redis**: Fast and persistent (recommended).
- **File system**: Simple but not scalable.

## Key Points:
- Memory: fast, not persistent.
- Database: persistent, slower.
- Redis: fast and persistent (recommended).
- File: simple, not scalable.

## Interview Tip:
"Redis is the standard for session storage â€” fast and persistent."

---

## Question 34: What is a session ID?

## Answer:
A session ID is a unique, random string that identifies a user's session. It's stored as a cookie and used to look up session data on the server.

## Key Points:
- Unique, random string.
- Stored as cookie.
- Identifies user session.
- Used for server lookup.

## Interview Tip:
"The session ID should be cryptographically random â€” predictable IDs are a security risk."

---

## Question 35: How are sessions secured?

## Answer:
1. **HttpOnly cookie**: Prevents JavaScript access.
2. **Secure flag**: HTTPS only.
3. **SameSite**: Prevents CSRF.
4. **Short expiration**: Limit session lifetime.
5. **Regenerate ID**: After login to prevent fixation.

## Key Points:
- HttpOnly, Secure, SameSite flags.
- Short expiration.
- Regenerate after login.
- Secure random session IDs.

## Interview Tip:
"HttpOnly + Secure + SameSite + regeneration = secure sessions."

---

## Question 36: What are session cookies?

## Answer:
Session cookies are cookies that expire when the browser closes. They store the session ID.

## Key Points:
- Expire when browser closes.
- Store session ID.
- HttpOnly and Secure flags.
- SameSite for CSRF protection.

## Interview Tip:
"Session cookies expire on browser close â€” use them for sensitive sessions."

---

## Question 37: What is session expiration?

## Answer:
Session expiration limits how long a session is valid. After expiration, the user must re-authenticate.

## Key Points:
- Limits session lifetime.
- Absolute timeout (max lifetime).
- Idle timeout (inactivity).
- Reduces risk of stolen sessions.

## Interview Tip:
"Use both absolute and idle timeouts for session expiration."

---

## Question 38: What happens when a session expires?

## Answer:
The server rejects the session ID and redirects the user to login. The session data is deleted from the server.

## Key Points:
- Session ID rejected.
- User redirected to login.
- Session data deleted.
- Must re-authenticate.

## Interview Tip:
"Expired sessions should redirect to login â€” don't silently fail."

---

## Question 39: What is session hijacking?

## Answer:
Session hijacking is when an attacker steals a session ID and impersonates the user.

## Key Points:
- Steal session ID.
- Impersonate user.
- Via XSS, network sniffing, or prediction.
- Prevent with HttpOnly, Secure, and HTTPS.

## Interview Tip:
"HttpOnly cookies prevent JavaScript from stealing session IDs."

---

## Question 40: How do you prevent session hijacking?

## Answer:
1. **HttpOnly cookies**: Prevent JavaScript access.
2. **Secure flag**: HTTPS only.
3. **Regenerate session ID**: After login.
4. **Short expiration**: Limit stolen session lifetime.
5. **Bind to IP/User-Agent**: Detect unusual sessions.

## Key Points:
- HttpOnly, Secure flags.
- Regenerate after login.
- Short expiration.
- IP/User-Agent binding.

## Interview Tip:
"HttpOnly + Secure + regeneration + short expiration = strong session security."

---

## Part 5 (41â€“50): Authorization & Access Control

---

## Question 41: What is authorization?

## Answer:
Authorization determines what an authenticated user can access and what actions they can perform.

## Key Points:
- What can you do?
- Permission checking.
- After authentication.
- RBAC, ABAC models.

## Interview Tip:
"Authorization is about permissions â€” what resources can this user access?"

---

## Question 42: What is Role-Based Access Control (RBAC)?

## Answer:
RBAC assigns permissions to roles, and users are assigned roles. Users inherit permissions from their roles.

```javascript
const roles = {
  admin: ["read", "write", "delete"],
  editor: ["read", "write"],
  viewer: ["read"],
};
```

## Key Points:
- Permissions assigned to roles.
- Users assigned to roles.
- Users inherit role permissions.
- Simple and widely used.

## Interview Tip:
"RBAC is simple and effective â€” assign roles, not permissions, to users."

---

## Question 43: What is Attribute-Based Access Control (ABAC)?

## Answer:
ABAC makes decisions based on attributes (user, resource, environment). More flexible than RBAC.

## Key Points:
- Decisions based on attributes.
- User, resource, environment attributes.
- More flexible than RBAC.
- Complex to implement.

## Interview Tip:
"ABAC for complex policies, RBAC for simple role-based access."

---

## Question 44: What is permission-based authorization?

## Answer:
Permission-based authorization checks specific permissions rather than roles.

```javascript
if (user.hasPermission("delete:posts")) {
  // Allow deletion
}
```

## Key Points:
- Check specific permissions.
- More granular than roles.
- Can be combined with RBAC.
- Fine-grained access control.

## Interview Tip:
"Permissions for fine-grained control, roles for grouping permissions."

---

## Question 45: What is the difference between roles and permissions?

## Answer:
- **Roles**: Named collections of permissions (admin, editor).
- **Permissions**: Individual access rights (read:posts, delete:users).

Roles group permissions; permissions define access.

## Key Points:
- Roles: collections of permissions.
- Permissions: individual access rights.
- Roles simplify assignment.
- Permissions define granularity.

## Interview Tip:
"Roles are groups of permissions â€” assign roles to users, permissions to roles."

---

## Question 46: How do you implement RBAC in a Node.js application?

## Answer:
```javascript
const rolePermissions = {
  admin: ["read", "write", "delete"],
  editor: ["read", "write"],
  viewer: ["read"],
};

function authorize(requiredPermission) {
  return (req, res, next) => {
    const userRole = req.user.role;
    const permissions = rolePermissions[userRole];
    if (permissions.includes(requiredPermission)) {
      next();
    } else {
      res.status(403).json({ error: "Forbidden" });
    }
  };
}

app.delete("/posts/:id", authenticate, authorize("delete"), deletePost);
```

## Key Points:
- Define role-permission mapping.
- Middleware checks permission.
- Apply to routes.
- 403 for insufficient permissions.

## Interview Tip:
"RBAC middleware checks permissions before the route handler runs."

---

## Question 47: How do you secure admin routes?

## Answer:
```javascript
function requireAdmin(req, res, next) {
  if (req.user?.role !== "admin") {
    return res.status(403).json({ error: "Admin access required" });
  }
  next();
}

app.get("/admin/users", authenticate, requireAdmin, getUsers);
```

## Key Points:
- Middleware checks admin role.
- Apply to all admin routes.
- 403 for non-admins.
- Don't expose admin endpoints to non-admins.

## Interview Tip:
"Admin routes need dedicated middleware â€” don't check role in every handler."

---

## Question 48: What is privilege escalation?

## Answer:
Privilege escalation is when a user gains higher privileges than intended â€” either by exploiting a vulnerability or misconfiguration.

## Key Points:
- Gaining higher privileges.
- Exploiting vulnerabilities.
- Misconfiguration.
- Horizontal (same level) or vertical (higher level).

## Interview Tip:
"Privilege escalation is a critical vulnerability â€” always enforce authorization server-side."

---

## Question 49: How do you prevent unauthorized access?

## Answer:
1. **Authentication middleware**: Verify identity on every request.
2. **Authorization middleware**: Check permissions before access.
3. **Validate on server**: Never trust client-side checks.
4. **Least privilege**: Minimum necessary permissions.
5. **Audit logging**: Track access attempts.

## Key Points:
- Authentication middleware.
- Authorization middleware.
- Server-side validation.
- Least privilege.
- Audit logging.

## Interview Tip:
"Never trust client-side authorization â€” always enforce on the server."

---

## Question 50: What authorization strategies have you implemented?

## Answer:
- **RBAC**: Role-based access for admin panels.
- **Permission-based**: Fine-grained API access control.
- **Resource-level**: Users can only access their own data.
- **Tenant-based**: Multi-tenant isolation.

## Key Points:
- RBAC for admin.
- Permission-based for APIs.
- Resource-level for data isolation.
- Tenant-based for SaaS.

## Interview Tip:
"RBAC for admin panels, resource-level for data isolation â€” combine as needed."

---

## Part 6 (51â€“60): JWT Authentication

---

## Question 51: What is JWT?

## Answer:
JWT (JSON Web Token) is a compact, self-contained token format for securely transmitting information. It contains claims (user data) and is signed to prevent tampering.

```
eyJhbGciOiJIUzI1NiJ9.eyJ1c2VySWQiOjF9.signature
```

## Key Points:
- Compact, self-contained token.
- Contains claims (user data).
- Signed, not encrypted.
- Stateless authentication.
- Three parts: header, payload, signature.

## Interview Tip:
"JWT is self-contained â€” the server can verify it without a database lookup."

---

## Question 52: Why is JWT commonly used for authentication?

## Answer:
- **Stateless**: No server-side session storage.
- **Scalable**: Works across multiple servers.
- **Compact**: Small size, easy to transmit.
- **Self-contained**: Contains user information.
- **Standard**: Widely supported.

## Key Points:
- Stateless and scalable.
- Compact and self-contained.
- No server-side storage.
- Industry standard.

## Interview Tip:
"JWT is stateless â€” the token itself contains the authentication data."

---

## Question 53: How does JWT authentication work?

## Answer:
1. User logs in with credentials.
2. Server verifies credentials.
3. Server creates JWT with user claims.
4. Server sends JWT to client.
5. Client sends JWT with each request.
6. Server verifies JWT signature and extracts claims.

## Key Points:
- Login creates JWT.
- Client stores and sends JWT.
- Server verifies on each request.
- Stateless â€” no server-side session.

## Interview Tip:
"JWT flow: login â†’ get token â†’ send with requests â†’ verify server-side."

---

## Question 54: What are the three parts of a JWT?

## Answer:
1. **Header**: Algorithm and token type.
2. **Payload**: Claims (user data, expiration).
3. **Signature**: Verification signature.

```
header.payload.signature
```

All three are Base64-encoded.

## Key Points:
- Header: algorithm, type.
- Payload: claims, data.
- Signature: verification.
- Base64-encoded.
- Dot-separated.

## Interview Tip:
"Header.payload.signature â€” three Base64-encoded parts."

---

## Question 55: What is JWT header?

## Answer:
The header specifies the signing algorithm and token type.

```json
{
  "alg": "HS256",
  "typ": "JWT"
}
```

## Key Points:
- Signing algorithm (HS256, RS256).
- Token type (JWT).
- Base64-encoded.
- Not encrypted (readable).

## Interview Tip:
"The header tells you how the token is signed."

---

## Question 56: What is JWT payload?

## Answer:
The payload contains claims â€” statements about the user and token.

```json
{
  "sub": "123",
  "name": "Alice",
  "iat": 1234567890,
  "exp": 1234571490
}
```

## Key Points:
- Contains claims.
- Standard claims: `sub`, `iat`, `exp`.
- Custom claims: user data.
- Not encrypted (readable).
- Don't store sensitive data.

## Interview Tip:
"The payload is readable â€” don't store passwords or secrets in it."

---

## Question 57: What is JWT signature?

## Answer:
The signature verifies the token hasn't been tampered with. It's created by signing the header and payload with a secret key.

```
HMACSHA256(base64(header) + "." + base64(payload), secret)
```

## Key Points:
- Verifies token integrity.
- Created with secret key.
- Prevents tampering.
- Server verifies with same secret.

## Interview Tip:
"The signature prevents tampering â€” if the token is modified, verification fails."

---

## Question 58: Is JWT encrypted or encoded?

## Answer:
JWT is **encoded** (Base64), not encrypted. Anyone can decode and read the payload. JWT is signed to prevent tampering, but the data is visible.

## Key Points:
- Base64-encoded, not encrypted.
- Payload is readable.
- Signed to prevent tampering.
- Don't store sensitive data.

## Interview Tip:
"JWT is signed, not encrypted â€” anyone can read the payload."

---

## Question 59: What information should not be stored in JWT payload?

## Answer:
- **Passwords**: Never.
- **API keys**: Never.
- **Credit card numbers**: Never.
- **Sensitive personal data**: Minimize.
- **Anything you don't want the client to see**: Payload is readable.

## Key Points:
- No passwords or API keys.
- No financial data.
- Minimize sensitive data.
- Payload is readable by anyone.

## Interview Tip:
"If it's sensitive, don't put it in JWT â€” the payload is just Base64-encoded."

---

## Question 60: What are the advantages of JWT?

## Answer:
- **Stateless**: No server-side storage.
- **Scalable**: Works across multiple servers.
- **Compact**: Small size.
- **Self-contained**: Contains user data.
- **Standard**: Widely supported.

## Key Points:
- Stateless and scalable.
- Compact and self-contained.
- No server-side storage.
- Industry standard.

## Interview Tip:
"JWT's biggest advantage is statelessness â€” no session storage needed."

---

## Part 7 (61â€“70): JWT Security

---

## Question 61: What are the disadvantages of JWT authentication?

## Answer:
- **Can't be invalidated**: Once issued, valid until expiration.
- **Payload is readable**: Not encrypted.
- **Token size**: Larger than session IDs.
- **Revocation is hard**: Need blacklist or short expiration.
- **Stateless means no server control**: Can't force logout easily.

## Key Points:
- Can't invalidate easily.
- Payload is readable.
- Larger than session IDs.
- Revocation requires extra work.

## Interview Tip:
"JWT's biggest disadvantage is that you can't easily invalidate a token â€” use short expiration and refresh tokens."

---

## Question 62: How do you invalidate a JWT token?

## Answer:
1. **Token blacklist**: Store invalidated tokens in Redis.
2. **Short expiration**: Tokens expire quickly.
3. **Token version**: Increment version on user, invalidate old tokens.
4. **Refresh token rotation**: Invalidate old refresh tokens.

## Key Points:
- Token blacklist in Redis.
- Short expiration.
- Token version in database.
- Refresh token rotation.

## Interview Tip:
"JWT can't be invalidated directly â€” use a blacklist or short expiration."

---

## Question 63: What is JWT expiration time?

## Answer:
The `exp` claim specifies when the token expires. After expiration, the token is rejected.

```json
{
  "exp": 1234571490  // Unix timestamp
}
```

## Key Points:
- `exp` claim.
- Unix timestamp.
- Server checks expiration.
- Short expiration for security.
- Refresh tokens for renewal.

## Interview Tip:
"Access tokens should expire in 15-30 minutes â€” short expiration limits damage from stolen tokens."

---

## Question 64: What is an access token?

## Answer:
An access token is a short-lived JWT used to access protected resources. It's sent with each API request.

## Key Points:
- Short-lived (15-30 minutes).
- Used for API access.
- Sent with each request.
- Contains user claims.

## Interview Tip:
"Access tokens are short-lived for security â€” use refresh tokens for renewal."

---

## Question 65: What is a refresh token?

## Answer:
A refresh token is a long-lived token used to obtain new access tokens without re-authentication.

## Key Points:
- Long-lived (days or weeks).
- Used to get new access tokens.
- Stored securely (HttpOnly cookie).
- Can be revoked.

## Interview Tip:
"Refresh tokens extend sessions without re-authentication."

---

## Question 66: Why do we need refresh tokens?

## Answer:
- **Short access token lifetime**: Limits damage from stolen tokens.
- **Long sessions**: Users stay logged in.
- **Token renewal**: Get new access tokens without re-login.
- **Security**: Refresh tokens can be revoked.

## Key Points:
- Short access tokens for security.
- Long sessions for UX.
- Token renewal without re-login.
- Revocable refresh tokens.

## Interview Tip:
"Access tokens are short for security; refresh tokens are long for UX."

---

## Question 67: How does refresh token rotation work?

## Answer:
Each time a refresh token is used, it's invalidated and a new one is issued. If a stolen refresh token is used, the legitimate user's next refresh will fail, detecting the compromise.

## Key Points:
- Invalidate old refresh token on use.
- Issue new refresh token.
- Detect stolen tokens.
- Invalidate family on reuse.

## Interview Tip:
"Refresh token rotation detects stolen tokens â€” if a token is reused, the entire family is invalidated."

---

## Question 68: Where should JWT tokens be stored?

## Answer:
- **HttpOnly cookie**: Most secure (XSS-resistant).
- **Memory**: Most secure but lost on refresh.
- **localStorage**: Convenient but vulnerable to XSS.

## Key Points:
- HttpOnly cookie: most secure.
- Memory: secure but not persistent.
- localStorage: convenient but risky.
- Always use HTTPS.

## Interview Tip:
"Http-only cookies are the most secure â€” they're invisible to JavaScript."

---

## Question 69: JWT in localStorage vs cookies: which is safer?

## Answer:
**Cookies (HttpOnly)** are safer:
- **HttpOnly**: JavaScript can't access.
- **Secure**: HTTPS only.
- **SameSite**: CSRF protection.

**localStorage** is vulnerable to XSS â€” any injected script can steal the token.

## Key Points:
- HttpOnly cookies: XSS-resistant.
- localStorage: vulnerable to XSS.
- Cookies with Secure + SameSite.
- Always use HttpOnly for auth tokens.

## Interview Tip:
"HttpOnly cookies for auth tokens â€” localStorage is never secure for sensitive data."

---

## Question 70: How do you secure JWT-based authentication?

## Answer:
1. **Short expiration**: 15-30 minutes for access tokens.
2. **HttpOnly cookies**: Prevent JavaScript access.
3. **Secure flag**: HTTPS only.
4. **SameSite**: CSRF protection.
5. **Refresh token rotation**: Detect stolen tokens.
6. **Token blacklist**: For logout and revocation.

## Key Points:
- Short expiration.
- HttpOnly, Secure, SameSite cookies.
- Refresh token rotation.
- Token blacklist.

## Interview Tip:
"Short expiration + HttpOnly cookies + refresh rotation = secure JWT auth."

---

## Part 8 (71â€“80): OAuth & OpenID Connect

---

## Question 71: What is OAuth?

## Answer:
OAuth is an authorization framework that allows third-party applications to access user resources without sharing credentials.

## Key Points:
- Authorization framework.
- Third-party access.
- No credential sharing.
- Industry standard.

## Interview Tip:
"OAuth is for authorization â€” allowing third-party access to user resources."

---

## Question 72: Why is OAuth used?

## Answer:
- **Third-party access**: Apps access user data safely.
- **No credential sharing**: Users don't share passwords.
- **Limited access**: Scopes control what's accessible.
- **Revocable**: Users can revoke access.

## Key Points:
- Safe third-party access.
- No credential sharing.
- Scoped permissions.
- Revocable access.

## Interview Tip:
"OAuth lets users grant access without sharing passwords."

---

## Question 73: What problem does OAuth solve?

## Answer:
OAuth solves the problem of giving third-party applications limited access to user resources without sharing user credentials.

## Key Points:
- Third-party access without credentials.
- Limited, scoped access.
- User consent.
- Revocable.

## Interview Tip:
"OAuth solves 'how do I let this app access my data without giving it my password?'"

---

## Question 74: What are OAuth roles?

## Answer:
1. **Resource Owner**: The user.
2. **Client**: The third-party application.
3. **Authorization Server**: Issues tokens.
4. **Resource Server**: Hosts protected resources.

## Key Points:
- Resource Owner: user.
- Client: third-party app.
- Authorization Server: issues tokens.
- Resource Server: hosts resources.

## Interview Tip:
"Four roles: user, app, auth server, resource server."

---

## Question 75: What is a resource owner?

## Answer:
The resource owner is the user who owns the protected resources and can grant access to them.

## Key Points:
- The user.
- Owns protected resources.
- Grants access to clients.
- Provides consent.

## Interview Tip:
"The resource owner is the user â€” they own the data."

---

## Question 76: What is a client in OAuth?

## Answer:
The client is the third-party application that wants to access the user's resources.

## Key Points:
- Third-party application.
- Requests access to resources.
- Receives access tokens.
- Must be registered with authorization server.

## Interview Tip:
"The client is the app requesting access â€” like a third-party calendar app accessing your Google Calendar."

---

## Question 77: What is an authorization server?

## Answer:
The authorization server issues access tokens after authenticating the user and obtaining consent.

## Key Points:
- Issues access tokens.
- Authenticates users.
- Obtains user consent.
- Examples: Google, GitHub, Auth0.

## Interview Tip:
"The authorization server is the gatekeeper â€” it issues tokens after user consent."

---

## Question 78: What is an access token in OAuth?

## Answer:
An access token is a credential that represents the authorization granted to the client. It's used to access protected resources.

## Key Points:
- Represents authorization.
- Used to access resources.
- Has expiration.
- Can be JWT or opaque.

## Interview Tip:
"The access token is the key to the resource server."

---

## Question 79: What is OpenID Connect?

## Answer:
OpenID Connect (OIDC) is an identity layer on top of OAuth 2.0. It adds authentication (who the user is) on top of OAuth's authorization (what the user can access).

## Key Points:
- Identity layer on OAuth 2.0.
- Adds authentication.
- Issues ID tokens.
- Standard for identity federation.

## Interview Tip:
"OIDC = OAuth + authentication. OAuth is for authorization; OIDC adds identity."

---

## Question 80: OAuth vs OpenID Connect: what is the difference?

## Answer:
- **OAuth**: Authorization framework (what can you access).
- **OIDC**: Authentication layer on OAuth (who are you).

OAuth issues access tokens; OIDC issues ID tokens.

## Key Points:
- OAuth: authorization.
- OIDC: authentication.
- OAuth: access tokens.
- OIDC: ID tokens.

## Interview Tip:
"OAuth for authorization, OIDC for authentication â€” OIDC builds on OAuth."

---

## Part 9 (81â€“90): Cookies & Browser Security

---

## Question 81: What are HTTP cookies?

## Answer:
Cookies are small pieces of data stored by the browser and sent with every request to the server.

## Key Points:
- Small data stored by browser.
- Sent with every request.
- Used for sessions, preferences, tracking.
- 4KB size limit.

## Interview Tip:
"Cookies are the browser's way of remembering state across requests."

---

## Question 82: How do cookies work?

## Answer:
1. Server sends `Set-Cookie` header.
2. Browser stores the cookie.
3. Browser sends cookie with every request to that domain.
4. Server reads cookie to identify user/session.

## Key Points:
- Server sets cookie via header.
- Browser stores and sends automatically.
- Sent with every request.
- Domain-scoped.

## Interview Tip:
"Cookies are automatic â€” the browser handles storage and transmission."

---

## Question 83: What are session cookies?

## Answer:
Session cookies expire when the browser closes. They don't have an `Expires` or `Max-Age` attribute.

## Key Points:
- Expire when browser closes.
- No expiration attribute.
- Temporary storage.
- Used for session IDs.

## Interview Tip:
"Session cookies = browser close = cookie gone."

---

## Question 84: What are persistent cookies?

## Answer:
Persistent cookies have an `Expires` or `Max-Age` attribute and persist until that time.

## Key Points:
- Have expiration time.
- Persist across browser sessions.
- Used for "remember me" functionality.
- `Expires` or `Max-Age` attribute.

## Interview Tip:
"Persistent cookies survive browser close â€” use for 'remember me'."

---

## Question 85: What is HttpOnly cookie?

## Answer:
HttpOnly cookies can't be accessed by JavaScript. They're only sent with HTTP requests, preventing XSS attacks from stealing cookies.

## Key Points:
- JavaScript can't access.
- Only sent with HTTP requests.
- Prevents XSS cookie theft.
- Essential for auth cookies.

## Interview Tip:
"HttpOnly cookies are invisible to JavaScript â€” essential for security."

---

## Question 86: What is Secure cookie flag?

## Answer:
The Secure flag ensures cookies are only sent over HTTPS connections.

## Key Points:
- HTTPS only.
- Prevents transmission over HTTP.
- Essential for sensitive cookies.
- Combined with HttpOnly.

## Interview Tip:
"Secure flag = HTTPS only. Always use it for auth cookies."

---

## Question 87: What is SameSite cookie attribute?

## Answer:
SameSite controls when cookies are sent with cross-site requests.

- **Strict**: Never sent cross-site.
- **Lax**: Sent with top-level navigation.
- **Always sent cross-site (not recommended).

## Key Points:
- Controls cross-site cookie sending.
- Strict: never cross-site.
- Lax: top-level navigation only.
- None: always (requires Secure).

## Interview Tip:
"SameSite=Strict is the most secure; Lax is the practical default."

---

## Question 88: How do cookies help authentication?

## Answer:
Cookies store session IDs or JWT tokens. The browser sends them automatically with every request, maintaining authentication state.

## Key Points:
- Store session IDs or tokens.
- Sent automatically.
- Maintain authentication state.
- HttpOnly + Secure for security.

## Interview Tip:
"Cookies are the standard mechanism for maintaining authentication state."

---

## Question 89: What are cookie security risks?

## Answer:
- **XSS**: JavaScript can access non-HttpOnly cookies.
- **CSRF**: Cookies sent automatically with cross-site requests.
- **Man-in-the-middle**: Cookies intercepted over HTTP.
- **Session hijacking**: Stolen session cookies.

## Key Points:
- XSS: access non-HttpOnly cookies.
- CSRF: automatic cross-site sending.
- MitM: HTTP interception.
- Session hijacking.

## Interview Tip:
"HttpOnly + Secure + SameSite = cookie security."

---

## Question 90: How do you secure authentication cookies?

## Answer:
```javascript
res.cookie("session", sessionId, {
  httpOnly: true,    // No JavaScript access
  secure: true,      // HTTPS only
  sameSite: "strict", // No cross-site
  maxAge: 86400000,  // 1 day
  path: "/"
});
```

## Key Points:
- HttpOnly: prevents XSS access.
- Secure: HTTPS only.
- SameSite: prevents CSRF.
- MaxAge: expiration.
- Path: scope.

## Interview Tip:
"HttpOnly + Secure + SameSite â€” the three essential cookie flags."

---

## Part 10 (91â€“100): CORS

---

## Question 91: What is CORS?

## Answer:
CORS (Cross-Origin Resource Sharing) is a browser security mechanism that controls which origins can access resources from a different origin.

## Key Points:
- Browser security mechanism.
- Controls cross-origin access.
- Uses HTTP headers.
- Preflight requests for complex operations.

## Interview Tip:
"CORS is a browser enforcement â€” servers can allow or deny cross-origin requests."

---

## Question 92: Why does CORS exist?

## Answer:
CORS exists to prevent malicious websites from making unauthorized requests to other domains on behalf of the user.

## Key Points:
- Prevents cross-site unauthorized requests.
- Browser enforcement.
- Protects user data.
- Same-origin policy extension.

## Interview Tip:
"CORS protects users from malicious websites making requests on their behalf."

---

## Question 93: How does the browser enforce CORS?

## Answer:
1. Browser checks if request is cross-origin.
2. For simple requests: sends request, checks response headers.
3. For complex requests: sends preflight OPTIONS request first.
4. Server responds with CORS headers.
5. Browser allows or blocks based on headers.

## Key Points:
- Browser checks origin.
- Preflight for complex requests.
- Server responds with CORS headers.
- Browser enforces.

## Interview Tip:
"CORS is enforced by the browser â€” the server just sets headers."

---

## Question 94: What is a preflight request?

## Answer:
A preflight request is an OPTIONS request sent by the browser before the actual request to check if the server allows the cross-origin request.

## Key Points:
- OPTIONS request before actual request.
- Checks if server allows the request.
- For complex requests (custom headers, methods).
- Server responds with allowed origins/methods.

## Interview Tip:
"Preflight = 'Hey server, is this cross-origin request okay?'"

---

## Question 95: What is an OPTIONS request?

## Answer:
OPTIONS is an HTTP method used in CORS preflight requests to check what methods and headers the server supports.

## Key Points:
- HTTP method for CORS preflight.
- Checks allowed methods and headers.
- Server responds with CORS headers.
- Browser uses response to allow/deny.

## Interview Tip:
"OPTIONS is the CORS handshake â€” it checks permissions before the real request."

---

## Question 96: What are CORS headers?

## Answer:
- **Access-Control-Allow-Origin**: Which origins can access.
- **Access-Control-Allow-Methods**: Which HTTP methods are allowed.
- **Access-Control-Allow-Headers**: Which headers are allowed.
- **Access-Control-Allow-Credentials**: Whether cookies are allowed.

## Key Points:
- Allow-Origin: allowed origins.
- Allow-Methods: allowed HTTP methods.
- Allow-Headers: allowed headers.
- Allow-Credentials: cookie support.

## Interview Tip:
"Access-Control-Allow-Origin is the most important CORS header."

---

## Question 97: How do you configure CORS in Express.js?

## Answer:
```javascript
const cors = require("cors");

app.use(cors({
  origin: "https://myapp.com",
  methods: ["GET", "POST", "PUT", "DELETE"],
  credentials: true
}));
```

## Key Points:
- `cors` middleware for Express.
- Configure origin, methods, credentials.
- Restrict to specific origins.
- Don't use `*` with credentials.

## Interview Tip:
"Never use `origin: '*'` with credentials â€” it's a security risk."

---

## Question 98: What is the difference between CORS and CSRF?

## Answer:
- **CORS**: Controls which origins can access your API.
- **CSRF**: Prevents forged requests from authenticated users.

CORS is about origin access; CSRF is about request authenticity.

## Key Points:
- CORS: origin-based access control.
- CSRF: request authenticity.
- CORS: browser enforcement.
- CSRF: server-side protection.

## Interview Tip:
"CORS controls who can access; CSRF ensures requests are genuine."

---

## Question 99: Why does CORS not protect APIs completely?

## Answer:
CORS only works in browsers â€” non-browser clients (curl, Postman, mobile apps) can ignore CORS. APIs need additional authentication and authorization.

## Key Points:
- Browser-only protection.
- Non-browser clients can bypass.
- Need additional auth.
- CORS is defense in depth, not sole protection.

## Interview Tip:
"CORS protects against browser-based attacks â€” APIs need authentication too."

---

## Question 100: What CORS mistakes do developers commonly make?

## Answer:
1. **Using `origin: '*'`**: Allows any origin.
2. **Allowing credentials with `*`**: Security risk.
3. **Not restricting methods**: Allows all HTTP methods.
4. **Not testing preflight**: Preflight failures are silent.
5. **CORS in production but not development**: Different configs.

## Key Points:
- Don't use `*` with credentials.
- Restrict origins and methods.
- Test preflight requests.
- Consistent config across environments.

## Interview Tip:
"Never use `origin: '*'` in production â€” always restrict to specific origins."

---

## Part 11 (101â€“110): OWASP Top 10 Fundamentals

---

## Question 101: What is OWASP?

## Answer:
OWASP (Open Web Application Security Project) is a nonprofit organization that provides free resources for web application security, including the famous OWASP Top 10.

## Key Points:
- Nonprofit security organization.
- Free security resources.
- OWASP Top 10 vulnerability list.
- Security guidelines and tools.

## Interview Tip:
"OWASP is the industry standard for web security â€” know the Top 10."

---

## Question 102: What is OWASP Top 10?

## Answer:
The OWASP Top 10 is a list of the most critical web application security risks, updated regularly. It includes injection, broken access control, XSS, and more.

## Key Points:
- Most critical web security risks.
- Updated regularly.
- Industry standard reference.
- Guide for security priorities.

## Interview Tip:
"OWASP Top 10 is the security checklist â€” know every item."

---

## Question 103: Why is OWASP important for developers?

## Answer:
- **Awareness**: Know common vulnerabilities.
- **Prevention**: Implement defenses.
- **Standards**: Industry-recognized security baseline.
- **Compliance**: Many regulations reference OWASP.

## Key Points:
- Security awareness.
- Prevention strategies.
- Industry standards.
- Compliance reference.

## Interview Tip:
"OWASP is the security baseline â€” every developer should know the Top 10."

---

## Question 104: What are the most common web application vulnerabilities?

## Answer:
1. **Broken Access Control**
2. **Cryptographic Failures**
3. **Injection** (SQL, NoSQL, Command)
4. **Insecure Design**
5. **Security Misconfiguration**
6. **Vulnerable Components**
7. **Authentication Failures**
8. **Data Integrity Failures**
9. **Logging Failures**
10. **SSRF** (Server-Side Request Forgery)

## Key Points:
- Broken access control is #1.
- Injection and XSS are common.
- Misconfiguration is widespread.
- Authentication failures are critical.

## Interview Tip:
"Broken access control is #1 â€” authorization is the most common vulnerability."

---

## Question 105: How do you use OWASP guidelines in development?

## Answer:
1. **Review OWASP Top 10**: Understand each risk.
2. **Implement defenses**: For each applicable risk.
3. **Security testing**: Include in CI/CD.
4. **Code review**: Check for OWASP vulnerabilities.
5. **Stay updated**: Top 10 changes over time.

## Key Points:
- Review and understand Top 10.
- Implement defenses.
- Include in testing.
- Code review for vulnerabilities.
- Stay current.

## Interview Tip:
"OWASP is a checklist â€” review every item and implement applicable defenses."

---

## Question 106: What is broken access control?

## Answer:
Broken access control is when users can access resources or perform actions they shouldn't be able to. It's the #1 OWASP risk.

## Key Points:
- Unauthorized access to resources.
- #1 OWASP risk.
- Missing or weak authorization.
- Privilege escalation.

## Interview Tip:
"Broken access control = missing or weak authorization. Always enforce server-side."

---

## Question 107: How do you prevent broken access control?

## Answer:
1. **Server-side authorization**: Never trust client-side checks.
2. **RBAC/ABAC**: Implement proper access control.
3. **Least privilege**: Minimum necessary permissions.
4. **Validate ownership**: Users can only access their own resources.
5. **Audit logging**: Track access attempts.

## Key Points:
- Server-side enforcement.
- Proper RBAC/ABAC.
- Least privilege.
- Ownership validation.
- Audit logging.

## Interview Tip:
"Authorization must be server-side â€” client-side checks are easily bypassed."

---

## Question 108: What is security misconfiguration?

## Answer:
Security misconfiguration is when security settings are not properly configured â€” default credentials, unnecessary features enabled, missing security headers, etc.

## Key Points:
- Default credentials.
- Unnecessary features.
- Missing security headers.
- Verbose error messages.
- Common and preventable.

## Interview Tip:
"Security misconfiguration is the easiest vulnerability to prevent â€” check your settings."

---

## Question 109: What is insecure design?

## Answer:
Insecure design is when security isn't considered during the design phase â€” missing threat modeling, insecure patterns, insufficient security controls.

## Key Points:
- Security not in design phase.
- Missing threat modeling.
- Insecure patterns.
- Design-level vulnerabilities.

## Interview Tip:
"Security should be designed in, not bolted on."

---

## Question 110: What is software supply chain security?

## Answer:
Supply chain security protects against vulnerabilities in dependencies â€” malicious packages, outdated libraries, compromised repositories.

## Key Points:
- Dependency vulnerabilities.
- Malicious packages.
- Outdated libraries.
- Package integrity verification.

## Interview Tip:
"npm audit and Snyk scan your dependencies â€” keep them updated."

---

## Part 12 (111â€“120): Cross-Site Scripting (XSS)

---

## Question 111: What is XSS attack?

## Answer:
XSS (Cross-Site Scripting) is an attack where malicious scripts are injected into web pages viewed by other users.

## Key Points:
- Inject malicious scripts.
- Execute in victim's browser.
- Steal cookies, sessions, data.
- Three types: stored, reflected, DOM-based.

## Interview Tip:
"XSS executes malicious code in the victim's browser â€” it's the most common web vulnerability."

---

## Question 112: Why does XSS happen?

## Answer:
XSS happens when user input is rendered as HTML/JavaScript without proper sanitization or encoding.

## Key Points:
- Unsanitized user input.
- Rendered as HTML/JavaScript.
- Missing output encoding.
- Missing input validation.

## Interview Tip:
"XSS = unsanitized input rendered as code."

---

## Question 113: What are the different types of XSS?

## Answer:
1. **Stored XSS**: Malicious script stored in database.
2. **Reflected XSS**: Script in URL reflected in response.
3. **DOM-based XSS**: Client-side JavaScript manipulates DOM.

## Key Points:
- Stored: in database.
- Reflected: in URL.
- DOM-based: client-side.
- All execute malicious scripts.

## Interview Tip:
"Stored is most dangerous â€” the script persists and affects all users."

---

## Question 114: What is stored XSS?

## Answer:
Stored XSS occurs when malicious script is permanently stored in the database and served to all users who view the content.

## Key Points:
- Stored in database.
- Served to all users.
- Most dangerous type.
- Affects all visitors.

## Interview Tip:
"Stored XSS is the most dangerous â€” every user who views the page is affected."

---

## Question 115: What is reflected XSS?

## Answer:
Reflected XSS occurs when user input is reflected in the response without sanitization â€” usually via URL parameters.

## Key Points:
- Input reflected in response.
- Via URL parameters.
- Requires user to click malicious link.
- Not stored permanently.

## Interview Tip:
"Reflected XSS needs the user to click a malicious link â€” social engineering."

---

## Question 116: What is DOM-based XSS?

## Answer:
DOM-based XSS occurs when client-side JavaScript processes untrusted data and updates the DOM unsafely.

## Key Points:
- Client-side JavaScript.
- Processes untrusted data.
- Updates DOM unsafely.
- No server involvement.

## Interview Tip:
"DOM-based XSS happens entirely in the browser â€” the server never sees the attack."

---

## Question 117: How can attackers exploit XSS?

## Answer:
- **Steal cookies**: Access session tokens.
- **Steal credentials**: Fake login forms.
- **Redirect users**: Phishing attacks.
- **Keylogging**: Capture keystrokes.
- **Defacement**: Modify page content.

## Key Points:
- Steal cookies and sessions.
- Phishing and credential theft.
- Keylogging.
- Page defacement.

## Interview Tip:
"XSS gives attackers full control in the victim's browser."

---

## Question 118: How do you prevent XSS attacks?

## Answer:
1. **Output encoding**: Encode user input before rendering.
2. **Content Security Policy (CSP)**: Restrict script sources.
3. **HttpOnly cookies**: Prevent JavaScript access.
4. **Input validation**: Validate and sanitize input.
5. **Framework protection**: React escapes JSX by default.

## Key Points:
- Output encoding.
- CSP headers.
- HttpOnly cookies.
- Input validation.
- Framework auto-escaping.

## Interview Tip:
"Output encoding is the primary defense â€” encode all user input before rendering."

---

## Question 119: What is input sanitization?

## Answer:
Input sanitization removes or escapes potentially dangerous content from user input.

## Key Points:
- Remove dangerous content.
- Escape special characters.
- Allowlists over blocklists.
- DOMPurify for HTML sanitization.

## Interview Tip:
"Sanitize input by removing dangerous content â€” use allowlists."

---

## Question 120: What is output encoding?

## Answer:
Output encoding converts special characters to their safe equivalents before rendering.

```javascript
// HTML encoding
< â†’ &lt;
> â†’ &gt;
" â†’ &quot;
& â†’ &amp;
```

## Key Points:
- Convert special characters.
- Safe equivalents.
- HTML, JavaScript, URL encoding.
- Prevents script execution.

## Interview Tip:
"Output encoding prevents XSS by making user input safe to render."

---

## Part 13 (121â€“130): Cross-Site Request Forgery (CSRF)

---

## Question 121: What is CSRF attack?

## Answer:
CSRF (Cross-Site Request Forgery) tricks a user's browser into making unintended requests to a site where they're authenticated.

## Key Points:
- Forged requests from authenticated users.
- Exploits automatic cookie sending.
- Tricks browser into making requests.
- User is unaware.

## Interview Tip:
"CSRF makes the browser send requests the user didn't intend."

---

## Question 122: How does CSRF work?

## Answer:
1. User is authenticated on site A.
2. User visits malicious site B.
3. Site B sends request to site A.
4. Browser automatically sends site A's cookies.
5. Site A thinks it's a legitimate request.

## Key Points:
- Authenticated user visits malicious site.
- Malicious site sends request to target.
- Browser sends cookies automatically.
- Target processes request as legitimate.

## Interview Tip:
"CSRF exploits automatic cookie sending â€” the browser doesn't know the request is forged."

---

## Question 123: Why are cookies vulnerable to CSRF?

## Answer:
Cookies are sent automatically with every request to the domain, regardless of where the request originates. The browser doesn't distinguish between legitimate and forged requests.

## Key Points:
- Cookies sent automatically.
- Sent with every request to domain.
- No origin checking.
- Browser doesn't distinguish requests.

## Interview Tip:
"Cookies are sent blindly â€” that's why they're vulnerable to CSRF."

---

## Question 124: What is a CSRF token?

## Answer:
A CSRF token is a unique, unpredictable value included in forms and verified on the server. Since the attacker can't know the token, they can't forge valid requests.

## Key Points:
- Unique, unpredictable value.
- Included in forms.
- Verified server-side.
- Attacker can't know the token.

## Interview Tip:
"CSRF tokens prove the request came from your site, not a malicious one."

---

## Question 125: How do CSRF tokens prevent attacks?

## Answer:
1. Server generates unique token per session.
2. Token included in form as hidden field.
3. Server verifies token on submission.
4. Attacker can't know the token.

## Key Points:
- Unique token per session.
- Hidden in form.
- Verified server-side.
- Attacker can't guess.

## Interview Tip:
"CSRF tokens are unpredictable â€” attackers can't forge them."

---

## Question 126: What is SameSite cookie protection?

## Answer:
SameSite cookie attribute prevents cookies from being sent with cross-site requests.

- **Strict**: Never sent cross-site.
- **Lax**: Sent with top-level navigation.
- **None**: Always sent (requires Secure).

## Key Points:
- Prevents cross-site cookie sending.
- Strict: most secure.
- Lax: practical default.
- None: not recommended.

## Interview Tip:
"SameSite=Strict prevents CSRF by blocking cross-site cookie sending."

---

## Question 127: CSRF vs XSS: what is the difference?

## Answer:
- **CSRF**: Forges requests from authenticated users.
- **XSS**: Injects scripts into pages.

CSRF exploits trust; XSS exploits rendering.

## Key Points:
- CSRF: forged requests.
- XSS: injected scripts.
- CSRF: exploits trust.
- XSS: exploits rendering.

## Interview Tip:
"CSRF makes requests; XSS executes code â€” different attacks, different defenses."

---

## Question 128: How do you prevent CSRF in Express.js?

## Answer:
```javascript
const csrf = require("csurf");
const csrfProtection = csrf({ cookie: true });

app.use(csrfProtection);

app.get("/form", (req, res) => {
  res.render("form", { csrfToken: req.csrfToken() });
});

app.post("/process", csrfProtection, (req, res) => {
  // CSRF token verified automatically
});
```

## Key Points:
- `csurf` middleware.
- Generate token per request.
- Include in forms.
- Verify on submission.

## Interview Tip:
"csurf middleware handles CSRF protection â€” generate and verify tokens automatically."

---

## Question 129: Does JWT prevent CSRF?

## Answer:
JWT stored in HttpOnly cookies is still vulnerable to CSRF. JWT in localStorage is not vulnerable to CSRF (but is vulnerable to XSS).

The best approach: JWT in HttpOnly cookies + CSRF tokens.

## Key Points:
- JWT in cookies: vulnerable to CSRF.
- JWT in localStorage: vulnerable to XSS.
- HttpOnly cookies + CSRF tokens: best protection.

## Interview Tip:
"JWT doesn't prevent CSRF â€” you still need CSRF protection with cookies."

---

## Question 130: When is CSRF protection required?

## Answer:
- **Cookie-based authentication**: Always.
- **Form submissions**: Always.
- **State-changing operations**: POST, PUT, DELETE.
- **JWT in cookies**: Always.
- **JWT in localStorage**: Not required (but XSS protection is).

## Key Points:
- Cookie-based auth: always.
- State-changing operations.
- JWT in cookies: required.
- JWT in localStorage: not needed.

## Interview Tip:
"If you use cookies for auth, you need CSRF protection â€” no exceptions."

---

## Part 14 (131â€“140): SQL Injection & Database Security

---

## Question 131: What is SQL Injection?

## Answer:
SQL Injection is an attack where malicious SQL code is inserted into queries through user input, allowing attackers to access, modify, or delete data.

```javascript
// Vulnerable
const query = `SELECT * FROM users WHERE id = ${userId}`;

// Attack: userId = "1 OR 1=1"
// Result: SELECT * FROM users WHERE id = 1 OR 1=1
```

## Key Points:
- Inject malicious SQL through input.
- Access, modify, or delete data.
- Most dangerous web vulnerability.
- Prevent with parameterized queries.

## Interview Tip:
"SQL injection is the most dangerous vulnerability â€” always use parameterized queries."

---

## Question 132: How does SQL Injection happen?

## Answer:
When user input is concatenated directly into SQL queries without sanitization or parameterization.

## Key Points:
- User input in SQL queries.
- String concatenation.
- No sanitization or parameterization.
- Exploits trusted input.

## Interview Tip:
"SQL injection = user input in SQL queries without parameterization."

---

## Question 133: What damage can SQL Injection cause?

## Answer:
- **Data theft**: Access all database data.
- **Data modification**: Change or delete data.
- **Authentication bypass**: Login as any user.
- **Remote code execution**: Execute system commands.
- **Complete system compromise**: Full control.

## Key Points:
- Data theft and modification.
- Authentication bypass.
- Remote code execution.
- Complete compromise.

## Interview Tip:
"SQL injection can give attackers full control of your database â€” and potentially your server."

---

## Question 134: How do you prevent SQL Injection?

## Answer:
1. **Parameterized queries**: Use prepared statements.
2. **ORM**: Use Prisma, TypeORM, Sequelize.
3. **Input validation**: Validate all input.
4. **Least privilege**: Database user with minimal permissions.
5. **WAF**: Web Application Firewall.

## Key Points:
- Parameterized queries (primary defense).
- ORM for safe queries.
- Input validation.
- Least privilege.
- WAF as additional layer.

## Interview Tip:
"Parameterized queries prevent SQL injection â€” never concatenate user input into SQL."

---

## Question 135: What are prepared statements?

## Answer:
Prepared statements separate SQL code from data. The database compiles the query structure first, then binds parameters separately.

```javascript
// Safe: parameterized query
const query = "SELECT * FROM users WHERE id = $1";
const result = await db.query(query, [userId]);
```

## Key Points:
- Separate SQL code from data.
- Database compiles structure first.
- Parameters bound separately.
- Prevents injection.
- Industry standard.

## Interview Tip:
"Prepared statements are the gold standard for preventing SQL injection."

---

## Question 136: How do ORMs prevent SQL Injection?

## Answer:
ORMs like Prisma use parameterized queries internally â€” user input is never concatenated into SQL strings.

```javascript
// Prisma: safe by default
const user = await prisma.user.findUnique({
  where: { id: userId }
});
```

## Key Points:
- ORMs use parameterized queries.
- Input never concatenated into SQL.
- Safe by default.
- Still validate input for business logic.

## Interview Tip:
"ORMs prevent SQL injection by design â€” but still validate input for business logic."

---

## Question 137: Is Prisma completely safe from SQL Injection?

## Answer:
Prisma is safe for normal queries â€” it uses parameterized queries. However, raw queries (`$queryRaw`) can be vulnerable if not parameterized.

```javascript
// Safe: parameterized
await prisma.$queryRaw`SELECT * FROM users WHERE id = ${userId}`;

// Unsafe: string concatenation
await prisma.$queryRaw(`SELECT * FROM users WHERE id = ${userId}`);
```

## Key Points:
- Normal queries: safe.
- Raw queries: parameterize manually.
- Use template literals for parameterization.
- Validate input even with ORMs.

## Interview Tip:
"Prisma is safe by default â€” but raw queries need manual parameterization."

---

## Question 138: What is NoSQL Injection?

## Answer:
NoSQL Injection is similar to SQL Injection but targets NoSQL databases like MongoDB. Attackers inject malicious operators into queries.

```javascript
// Vulnerable
const user = await User.findOne({ username: req.body.username });

// Attack: username = { "$gt": "" }
// Result: matches any user
```

## Key Points:
- Targets NoSQL databases.
- Injects operators ($gt, $ne, etc.).
- Type confusion attacks.
- Prevent with type validation.

## Interview Tip:
"NoSQL injection uses operators â€” validate input types strictly."

---

## Question 139: How do you prevent NoSQL Injection?

## Answer:
1. **Validate input types**: Ensure strings are strings.
2. **Use schema validation**: Mongoose schemas, Joi.
3. **Sanitize queries**: Remove operators from input.
4. **Use parameterized queries**: Where supported.

```javascript
// Validate types
const username = String(req.body.username);
const user = await User.findOne({ username });
```

## Key Points:
- Validate input types.
- Schema validation.
- Sanitize operators.
- Type coercion.

## Interview Tip:
"Validate that input is the expected type â€” strings should be strings, not objects."

---

## Question 140: What database security practices do you follow?

## Answer:
1. **Parameterized queries**: Always.
2. **Least privilege**: Database user with minimal permissions.
3. **Encryption at rest**: Encrypt sensitive data.
4. **Encryption in transit**: TLS connections.
5. **Input validation**: Validate all input.
6. **Audit logging**: Track database access.

## Key Points:
- Parameterized queries.
- Least privilege.
- Encryption at rest and in transit.
- Input validation.
- Audit logging.

## Interview Tip:
"Parameterized queries + least privilege + encryption = database security."

---

## Part 15 (141â€“150): API Security

---

## Question 141: What are common API security threats?

## Answer:
- **Broken authentication**: Weak or missing auth.
- **Broken authorization**: Missing permission checks.
- **Injection**: SQL, NoSQL, command injection.
- **Rate limiting abuse**: Brute force, DDoS.
- **Data exposure**: Excessive data in responses.

## Key Points:
- Broken auth and authorization.
- Injection attacks.
- Rate limiting abuse.
- Data exposure.

## Interview Tip:
"API security = authentication + authorization + validation + rate limiting."

---

## Question 142: How do you secure REST APIs?

## Answer:
1. **HTTPS**: Always.
2. **Authentication**: JWT or API keys.
3. **Authorization**: Check permissions.
4. **Input validation**: Validate all input.
5. **Rate limiting**: Prevent abuse.
6. **CORS**: Restrict origins.
7. **Security headers**: Helmet.js.

## Key Points:
- HTTPS for encryption.
- JWT for authentication.
- Authorization middleware.
- Input validation.
- Rate limiting.
- CORS and security headers.

## Interview Tip:
"HTTPS + JWT + validation + rate limiting + CORS = secure API."

---

## Question 143: What is API authentication?

## Answer:
API authentication verifies the identity of the client making the request â€” usually via JWT, API keys, or OAuth tokens.

## Key Points:
- Verify client identity.
- JWT, API keys, OAuth.
- Sent in Authorization header.
- Stateless verification.

## Interview Tip:
"API authentication proves who's making the request."

---

## Question 144: What is API authorization?

## Answer:
API authorization checks if the authenticated client has permission to perform the requested action.

## Key Points:
- Check permissions.
- After authentication.
- RBAC, ABAC, or resource-level.
- Server-side enforcement.

## Interview Tip:
"API authorization checks if you can do what you're asking."

---

## Question 145: What is API rate limiting?

## Answer:
Rate limiting restricts how many requests a client can make in a time period.

```javascript
const rateLimit = require("express-rate-limit");

const limiter = rateLimit({
  windowMs: 15 * 60 * 1000, // 15 minutes
  max: 100 // 100 requests per window
});

app.use("/api/", limiter);
```

## Key Points:
- Restricts request frequency.
- Per IP or per user.
- Prevents abuse and DDoS.
- 429 Too Many Requests.

## Interview Tip:
"Rate limiting prevents brute force and abuse â€” essential for public APIs."

---

## Question 146: Why is rate limiting important?

## Answer:
- **Prevents brute force**: Login attempts.
- **Prevents DDoS**: Resource exhaustion.
- **Fair usage**: Prevents one user from hogging resources.
- **Cost control**: Limits API costs.

## Key Points:
- Prevents brute force.
- Prevents DDoS.
- Fair usage.
- Cost control.

## Interview Tip:
"Rate limiting protects against abuse and controls costs."

---

## Question 147: What is API throttling?

## Answer:
Throttling is a form of rate limiting that slows down requests instead of blocking them. The server delays responses for excessive requests.

## Key Points:
- Slows down excessive requests.
- Delays instead of blocking.
- Graceful degradation.
- Different from blocking rate limits.

## Interview Tip:
"Throttling degrades gracefully â€” slow down instead of block."

---

## Question 148: How do you prevent API abuse?

## Answer:
1. **Rate limiting**: Restrict request frequency.
2. **Authentication**: Verify identity.
3. **Authorization**: Check permissions.
4. **Input validation**: Prevent malicious input.
5. **Monitoring**: Detect unusual patterns.
6. **API keys**: Track usage per client.

## Key Points:
- Rate limiting.
- Authentication and authorization.
- Input validation.
- Monitoring.
- API keys.

## Interview Tip:
"Rate limiting + authentication + monitoring = abuse prevention."

---

## Question 149: How do you secure API keys?

## Answer:
1. **Never expose in client code**: Server-side only.
2. **Environment variables**: Store in `.env`.
3. **Rotate regularly**: Change keys periodically.
4. **Scope permissions**: Limit what keys can do.
5. **Monitor usage**: Track key usage.

## Key Points:
- Server-side only.
- Environment variables.
- Regular rotation.
- Scoped permissions.
- Usage monitoring.

## Interview Tip:
"API keys are secrets â€” never expose them in client code."

---

## Question 150: What API security practices do you follow in production?

## Answer:
1. **HTTPS everywhere**.
2. **JWT with HttpOnly cookies**.
3. **Input validation with Zod**.
4. **Rate limiting**.
5. **CORS configuration**.
6. **Security headers (Helmet.js)**.
7. **Dependency scanning**.
8. **Audit logging**.

## Key Points:
- HTTPS.
- JWT + HttpOnly cookies.
- Input validation.
- Rate limiting.
- CORS + security headers.
- Dependency scanning.
- Audit logging.

## Interview Tip:
"HTTPS + JWT + validation + rate limiting + CORS + Helmet = production API security."

---

## Part 16 (151â€“160): Encryption & Data Protection

---

## Question 151: What is encryption?

## Answer:
Encryption converts readable data (plaintext) into unreadable data (ciphertext) using an algorithm and key. Only authorized parties with the key can decrypt it.

## Key Points:
- Plaintext â†’ ciphertext.
- Algorithm + key.
- Reversible with key.
- Protects data confidentiality.

## Interview Tip:
"Encryption protects data confidentiality â€” only authorized parties can read it."

---

## Question 152: What is the difference between encryption and hashing?

## Answer:
- **Encryption**: Reversible with key. Used for data protection.
- **Hashing**: One-way, irreversible. Used for passwords.

## Key Points:
- Encryption: reversible.
- Hashing: irreversible.
- Encryption for data.
- Hashing for passwords.

## Interview Tip:
"Encryption for data you need to read; hashing for data you only need to verify."

---

## Question 153: What are symmetric encryption and asymmetric encryption?

## Answer:
- **Symmetric**: Same key for encryption and decryption (AES).
- **Asymmetric**: Public key encrypts, private key decrypts (RSA).

## Key Points:
- Symmetric: one key, fast.
- Asymmetric: key pair, slower.
- Symmetric for bulk data.
- Asymmetric for key exchange.

## Interview Tip:
"Symmetric for speed, asymmetric for key exchange â€” they work together."

---

## Question 154: How does symmetric encryption work?

## Answer:
Same key encrypts and decrypts. Fast but requires secure key sharing.

## Key Points:
- Same key for both operations.
- Fast.
- Key sharing problem.
- AES is the standard.

## Interview Tip:
"Symmetric encryption is fast but requires secure key distribution."

---

## Question 155: How does asymmetric encryption work?

## Answer:
Public key encrypts, private key decrypts. Slower but solves key distribution.

## Key Points:
- Key pair: public and private.
- Public encrypts, private decrypts.
- Slower than symmetric.
- RSA, ECC algorithms.

## Interview Tip:
"Asymmetric encryption solves key distribution â€” public key is safe to share."

---

## Question 156: What is public key encryption?

## Answer:
Public key encryption uses a public key (shared openly) to encrypt data. Only the corresponding private key can decrypt it.

## Key Points:
- Public key: shared openly.
- Private key: kept secret.
- Public encrypts, private decrypts.
- Foundation of HTTPS.

## Interview Tip:
"Public key encryption enables secure communication without pre-shared secrets."

---

## Question 157: What is private key encryption?

## Answer:
Private key encryption uses a single secret key for both encryption and decryption. The key must be kept secret.

## Key Points:
- Single secret key.
- Both encrypt and decrypt.
- Must be kept secret.
- Fast and efficient.

## Interview Tip:
"Private key encryption is fast â€” use it for bulk data after key exchange."

---

## Question 158: What is AES encryption?

## Answer:
AES (Advanced Encryption Standard) is the most widely used symmetric encryption algorithm. It's fast and secure.

## Key Points:
- Symmetric encryption.
- 128, 192, or 256-bit keys.
- Fast and secure.
- Industry standard.

## Interview Tip:
"AES-256 is the gold standard for symmetric encryption."

---

## Question 159: What is RSA encryption?

## Answer:
RSA is an asymmetric encryption algorithm using public/private key pairs. It's used for key exchange and digital signatures.

## Key Points:
- Asymmetric encryption.
- Public/private key pair.
- Used for key exchange.
- Slower than AES.

## Interview Tip:
"RSA for key exchange, AES for bulk data â€” they work together in TLS."

---

## Question 160: When should you use encryption?

## Answer:
- **Data at rest**: Database, files, backups.
- **Data in transit**: HTTPS, TLS.
- **Sensitive data**: PII, financial data, health records.
- **Communication**: Email, messaging.

## Key Points:
- Data at rest and in transit.
- Sensitive data.
- Communication channels.
- Compliance requirements.

## Interview Tip:
"Encrypt sensitive data at rest and in transit â€” always."

---

## Part 17 (161â€“170): HTTPS & TLS

---

## Question 161: What is HTTPS?

## Answer:
HTTPS is HTTP over TLS (Transport Layer Security). It encrypts communication between client and server, preventing eavesdropping and tampering.

## Key Points:
- HTTP + TLS encryption.
- Encrypts communication.
- Prevents eavesdropping.
- Authenticates server.
- Industry standard.

## Interview Tip:
"HTTPS = encrypted HTTP. Always use it in production."

---

## Question 162: How does HTTPS work?

## Answer:
1. Client connects to server.
2. TLS handshake occurs.
3. Server presents certificate.
4. Client verifies certificate.
5. Encrypted communication begins.

## Key Points:
- TLS handshake.
- Certificate verification.
- Encrypted communication.
- Prevents MitM attacks.

## Interview Tip:
"HTTPS establishes trust via certificates and encrypts communication via TLS."

---

## Question 163: What is TLS?

## Answer:
TLS (Transport Layer Security) is the cryptographic protocol that provides encryption, authentication, and integrity for network communication.

## Key Points:
- Cryptographic protocol.
- Encryption, authentication, integrity.
- Successor to SSL.
- Foundation of HTTPS.

## Interview Tip:
"TLS is the security layer â€” it encrypts, authenticates, and ensures integrity."

---

## Question 164: What happens during a TLS handshake?

## Answer:
1. Client sends supported cipher suites.
2. Server selects cipher suite and sends certificate.
3. Client verifies certificate.
4. Key exchange generates shared secret.
5. Encrypted communication begins.

## Key Points:
- Cipher suite negotiation.
- Certificate verification.
- Key exchange.
- Encrypted channel established.

## Interview Tip:
"The TLS handshake establishes trust and creates an encrypted channel."

---

## Question 165: What is an SSL certificate?

## Answer:
An SSL certificate (more accurately, TLS certificate) is a digital document that verifies a server's identity and enables HTTPS.

## Key Points:
- Digital identity document.
- Verifies server identity.
- Enables HTTPS.
- Issued by Certificate Authorities.

## Interview Tip:
"SSL certificates prove the server is who it claims to be."

---

## Question 166: How does certificate validation work?

## Answer:
1. Client checks certificate expiration.
2. Client verifies certificate chain to trusted root CA.
3. Client checks domain matches.
4. Client checks certificate isn't revoked.

## Key Points:
- Check expiration.
- Verify chain to root CA.
- Domain matching.
- Revocation checking.

## Interview Tip:
"Certificate validation ensures you're talking to the real server."

---

## Question 167: Why is HTTPS important?

## Answer:
- **Encryption**: Prevents eavesdropping.
- **Authentication**: Verifies server identity.
- **Integrity**: Prevents tampering.
- **SEO**: Google ranks HTTPS higher.
- **Trust**: Users expect HTTPS.

## Key Points:
- Encryption, authentication, integrity.
- SEO benefits.
- User trust.
- Required for modern web.

## Interview Tip:
"HTTPS is mandatory for any production application â€” it's not optional."

---

## Question 168: What attacks does HTTPS prevent?

## Answer:
- **Eavesdropping**: Encrypted communication.
- **Man-in-the-middle**: Certificate verification.
- **Data tampering**: Integrity checks.
- **Session hijacking**: Encrypted cookies.

## Key Points:
- Eavesdropping prevention.
- MitM prevention.
- Data integrity.
- Session protection.

## Interview Tip:
"HTTPS prevents eavesdropping, MitM, and tampering."

---

## Question 169: What happens if HTTPS is not used?

## Answer:
- **Data exposed**: All communication is readable.
- **MitM attacks**: Attackers can intercept and modify.
- **Credential theft**: Passwords sent in plaintext.
- **Browser warnings**: "Not secure" warning.
- **SEO penalty**: Google ranks HTTP lower.

## Key Points:
- Data exposed.
- MitM attacks.
- Credential theft.
- Browser warnings.
- SEO penalty.

## Interview Tip:
"Without HTTPS, everything is visible â€” passwords, tokens, personal data."

---

## Question 170: How do you configure HTTPS in production?

## Answer:
1. **Get SSL certificate**: Let's Encrypt (free) or commercial CA.
2. **Install certificate**: On your server or CDN.
3. **Configure Nginx/Apache**: SSL settings.
4. **Redirect HTTP to HTTPS**: Force HTTPS.
5. **Auto-renew**: Certbot for Let's Encrypt.

## Key Points:
- SSL certificate.
- Server configuration.
- HTTP to HTTPS redirect.
- Auto-renewal.
- HSTS header.

## Interview Tip:
"Let's Encrypt + Certbot = free, automatic SSL certificates."

---

## Part 18 (171â€“180): Security Headers

---

## Question 171: What are HTTP security headers?

## Answer:
Security headers are HTTP response headers that instruct the browser to enable security features.

## Key Points:
- HTTP response headers.
- Browser security instructions.
- Defense in depth.
- Easy to implement.

## Interview Tip:
"Security headers tell the browser how to protect the user."

---

## Question 172: Why are security headers important?

## Answer:
- **Defense in depth**: Multiple security layers.
- **Browser protection**: Enable built-in browser security.
- **Prevent attacks**: XSS, clickjacking, MIME sniffing.
- **Easy to implement**: Just add headers.

## Key Points:
- Defense in depth.
- Browser-level protection.
- Prevent common attacks.
- Easy implementation.

## Interview Tip:
"Security headers are free protection â€” always configure them."

---

## Question 173: What is Content Security Policy (CSP)?

## Answer:
CSP is a security header that controls which resources the browser is allowed to load â€” preventing XSS by restricting script sources.

```
Content-Security-Policy: script-src 'self' https://trusted.cdn.com
```

## Key Points:
- Controls allowed resource sources.
- Prevents XSS.
- Restricts script sources.
- Configurable per directive.

## Interview Tip:
"CSP is the strongest XSS prevention â€” restrict where scripts can load from."

---

## Question 174: How does CSP prevent XSS?

## Answer:
CSP restricts which scripts can execute. Even if an attacker injects a script, CSP blocks it if the source isn't allowed.

```
Content-Security-Policy: script-src 'self'
```

This blocks all inline scripts and scripts from external domains.

## Key Points:
- Restricts script sources.
- Blocks injected scripts.
- Prevents inline script execution.
- Configurable strictness.

## Interview Tip:
"CSP makes injected scripts harmless â€” they can't execute."

---

## Question 175: What is X-Frame-Options?

## Answer:
X-Frame-Options prevents a page from being embedded in iframes, protecting against clickjacking attacks.

```
X-Frame-Options: DENY
```

## Key Points:
- Prevents iframe embedding.
- Protects against clickjacking.
- DENY or SAMEORIGIN.
- Use CSP frame-ancestors instead (modern).

## Interview Tip:
"X-Frame-Options prevents clickjacking â€” DENY or SAMEORIGIN."

---

## Question 176: What is HSTS?

## Answer:
HSTS (HTTP Strict Transport Security) forces browsers to use HTTPS for all future requests to a domain.

```
Strict-Transport-Security: max-age=31536000; includeSubDomains
```

## Key Points:
- Forces HTTPS.
- Browser remembers.
- Prevents downgrade attacks.
- Include subdomains.

## Interview Tip:
"HSTS forces HTTPS â€” once set, browsers won't use HTTP."

---

## Question 177: What is X-Content-Type-Options?

## Answer:
X-Content-Type-Options prevents MIME type sniffing, ensuring browsers treat files as the declared content type.

```
X-Content-Type-Options: nosniff
```

## Key Points:
- Prevents MIME sniffing.
- Ensures correct content type.
- `nosniff` value.
- Prevents content-type attacks.

## Interview Tip:
"`nosniff` prevents browsers from guessing content types â€” always set it."

---

## Question 178: What is Referrer-Policy?

## Answer:
Referrer-Policy controls how much referrer information is sent with requests.

```
Referrer-Policy: strict-origin-when-cross-origin
```

## Key Points:
- Controls referrer information.
- Protects privacy.
- Configurable strictness.
- `strict-origin-when-cross-origin` recommended.

## Interview Tip:
"Referrer-Policy protects privacy â€” don't leak URLs to external sites."

---

## Question 179: What security headers should every production app have?

## Answer:
```
Content-Security-Policy: script-src 'self'
X-Frame-Options: DENY
X-Content-Type-Options: nosniff
Strict-Transport-Security: max-age=31536000; includeSubDomains
Referrer-Policy: strict-origin-when-cross-origin
Permissions-Policy: camera=(), microphone=()
```

## Key Points:
- CSP for XSS prevention.
- X-Frame-Options for clickjacking.
- HSTS for HTTPS enforcement.
- X-Content-Type-Options for MIME sniffing.
- Referrer-Policy for privacy.

## Interview Tip:
"These six headers should be on every production app â€” use Helmet.js to set them."

---

## Question 180: How do you configure security headers in Node.js?

## Answer:
```javascript
const helmet = require("helmet");

app.use(helmet({
  contentSecurityPolicy: {
    directives: {
      defaultSrc: ["'self'"],
      scriptSrc: ["'self'", "https://trusted.cdn.com"],
    }
  },
  hsts: { maxAge: 31536000, includeSubDomains: true }
}));
```

## Key Points:
- `helmet` middleware for Express.
- Configurable per header.
- Sensible defaults.
- Easy to customize.

## Interview Tip:
"Helmet.js sets all security headers with sensible defaults â€” use it on every Express app."

---

## Part 19 (181â€“190): Secure Application Architecture

---

## Question 181: How do you design a secure full-stack application?

## Answer:
1. **HTTPS everywhere**.
2. **Authentication**: JWT with HttpOnly cookies.
3. **Authorization**: RBAC middleware.
4. **Input validation**: Zod on server.
5. **Security headers**: Helmet.js.
6. **Rate limiting**: Prevent abuse.
7. **Encryption**: At rest and in transit.
8. **Dependency scanning**: npm audit, Snyk.

## Key Points:
- HTTPS.
- Authentication and authorization.
- Input validation.
- Security headers.
- Rate limiting.
- Encryption.
- Dependency scanning.

## Interview Tip:
"Security is defense in depth â€” multiple layers, each catching what others miss."

---

## Question 182: What security layers should a modern application have?

## Answer:
1. **Network**: HTTPS, WAF, DDoS protection.
2. **Application**: Authentication, authorization, validation.
3. **Data**: Encryption, hashing, access control.
4. **Infrastructure**: Firewalls, monitoring, logging.

## Key Points:
- Network layer.
- Application layer.
- Data layer.
- Infrastructure layer.

## Interview Tip:
"Security layers: network â†’ application â†’ data â†’ infrastructure."

---

## Question 183: How do you secure a Next.js application?

## Answer:
1. **Server Components**: Keep sensitive logic server-side.
2. **Middleware**: Auth checks, security headers.
3. **Environment variables**: Never expose secrets.
4. **CSP headers**: Prevent XSS.
5. **CSRF protection**: SameSite cookies.
6. **Input validation**: Zod for all input.

## Key Points:
- Server Components for security.
- Middleware for auth and headers.
- Environment variables for secrets.
- CSP for XSS prevention.
- Input validation.

## Interview Tip:
"Server Components keep secrets server-side â€” that's the security advantage."

---

## Question 184: How do you secure a Node.js API?

## Answer:
1. **HTTPS**: Always.
2. **JWT authentication**: HttpOnly cookies.
3. **Authorization middleware**: Check permissions.
4. **Input validation**: Zod or Joi.
5. **Rate limiting**: Prevent abuse.
6. **Security headers**: Helmet.js.
7. **CORS**: Restrict origins.
8. **Error handling**: Don't expose internals.

## Key Points:
- HTTPS, JWT, authorization.
- Input validation, rate limiting.
- Security headers, CORS.
- Error handling.

## Interview Tip:
"HTTPS + JWT + validation + rate limiting + CORS + Helmet = secure API."

---

## Question 185: How do you implement authentication securely?

## Answer:
1. **Hash passwords**: bcrypt with cost 12+.
2. **HttpOnly cookies**: For token storage.
3. **Short token expiration**: 15-30 minutes.
4. **Refresh token rotation**: Detect stolen tokens.
5. **MFA**: For sensitive accounts.
6. **Rate limiting**: On login endpoints.

## Key Points:
- Hash passwords.
- HttpOnly cookies.
- Short expiration.
- Refresh rotation.
- MFA.
- Rate limiting.

## Interview Tip:
"Hash passwords, use HttpOnly cookies, short expiration, refresh rotation â€” the secure auth stack."

---

## Question 186: How do you design authorization for large applications?

## Answer:
1. **RBAC**: Role-based access for admin panels.
2. **ABAC**: Attribute-based for complex policies.
3. **Resource-level**: Users access only their own data.
4. **Middleware**: Centralized authorization checks.
5. **Database-level**: Row-level security.

## Key Points:
- RBAC for roles.
- ABAC for complex policies.
- Resource-level for data isolation.
- Middleware for centralization.
- Database-level for enforcement.

## Interview Tip:
"Combine RBAC with resource-level permissions for comprehensive authorization."

---

## Question 187: How do you protect sensitive user data?

## Answer:
1. **Encrypt at rest**: Database encryption.
2. **Encrypt in transit**: HTTPS/TLS.
3. **Hash passwords**: bcrypt.
4. **Minimize collection**: Only collect what's needed.
5. **Access control**: Limit who can access.
6. **Audit logging**: Track access.

## Key Points:
- Encrypt at rest and in transit.
- Hash passwords.
- Minimize data collection.
- Access control.
- Audit logging.

## Interview Tip:
"Encrypt, hash, minimize, control, audit â€” the data protection principles."

---

## Question 188: How do you handle secrets in production?

## Answer:
1. **Environment variables**: Never in code.
2. **Secrets manager**: AWS Secrets Manager, HashiCorp Vault.
3. **Rotation**: Regular secret rotation.
4. **Access control**: Limit who can access secrets.
5. **Audit logging**: Track secret access.

## Key Points:
- Environment variables.
- Secrets manager.
- Regular rotation.
- Access control.
- Audit logging.

## Interview Tip:
"Secrets belong in a secrets manager, not in code or environment variables."

---

## Question 189: How do you perform security reviews?

## Answer:
1. **Code review**: Check for vulnerabilities.
2. **Dependency audit**: npm audit, Snyk.
3. **Penetration testing**: Simulate attacks.
4. **Security headers**: Verify configuration.
5. **Authentication review**: Verify implementation.

## Key Points:
- Code review.
- Dependency audit.
- Penetration testing.
- Security headers.
- Auth review.

## Interview Tip:
"Security reviews should be part of every code review â€” check for OWASP Top 10."

---

## Question 190: What security practices do you follow during development?

## Answer:
1. **Never commit secrets**: .gitignore .env files.
2. **Validate all input**: Zod on server.
3. **Use HTTPS**: Even in development.
4. **Dependency scanning**: npm audit.
5. **Security headers**: Helmet.js.
6. **Code review**: Security-focused reviews.

## Key Points:
- Never commit secrets.
- Validate all input.
- HTTPS everywhere.
- Dependency scanning.
- Security headers.
- Security reviews.

## Interview Tip:
"Security starts in development â€” never commit secrets, always validate input."

---

## Part 20 (191â€“200): Production Security & Monitoring

---

## Question 191: How do you detect security attacks in production?

## Answer:
1. **Log monitoring**: Unusual patterns.
2. **Rate limiting alerts**: Spike in requests.
3. **Failed login attempts**: Brute force detection.
4. **Anomaly detection**: Unusual user behavior.
5. **WAF alerts**: Web Application Firewall.

## Key Points:
- Log monitoring.
- Rate limiting alerts.
- Failed login detection.
- Anomaly detection.
- WAF alerts.

## Interview Tip:
"Monitoring is detection â€” you can't stop what you can't see."

---

## Question 192: What is security logging?

## Answer:
Security logging records security-relevant events for auditing, incident response, and compliance.

## Key Points:
- Record security events.
- Authentication attempts.
- Authorization failures.
- Data access.
- Incident response.

## Interview Tip:
"Security logging is the foundation of incident response."

---

## Question 193: What information should not be logged?

## Answer:
- **Passwords**: Never.
- **API keys**: Never.
- **Credit card numbers**: Never.
- **Full request bodies**: May contain sensitive data.
- **Session tokens**: Never.

## Key Points:
- No passwords or API keys.
- No financial data.
- No session tokens.
- Mask sensitive fields.

## Interview Tip:
"If it's sensitive, don't log it â€” mask or exclude."

---

## Question 194: How do you monitor suspicious activities?

## Answer:
1. **Failed login attempts**: Brute force detection.
2. **Unusual IP addresses**: Geographic anomalies.
3. **Rate limiting violations**: Abuse detection.
4. **Privilege escalation attempts**: Unauthorized access.
5. **Data exfiltration**: Unusual data access patterns.

## Key Points:
- Failed logins.
- Unusual IPs.
- Rate limiting violations.
- Privilege escalation.
- Data exfiltration.

## Interview Tip:
"Monitor for patterns, not just events â€” patterns reveal attacks."

---

## Question 195: What is intrusion detection?

## Answer:
Intrusion detection monitors systems for malicious activity or policy violations and alerts when detected.

## Key Points:
- Monitor for malicious activity.
- Detect policy violations.
- Alert on detection.
- IDS/IPS systems.

## Interview Tip:
"Intrusion detection is the alarm system â€” it alerts you to attacks."

---

## Question 196: How do you handle a security breach?

## Answer:
1. **Contain**: Stop the attack.
2. **Assess**: Determine scope.
3. **Notify**: Inform affected users.
4. **Remediate**: Fix the vulnerability.
5. **Document**: Record the incident.
6. **Review**: Post-incident analysis.

## Key Points:
- Contain the breach.
- Assess the scope.
- Notify users.
- Fix vulnerabilities.
- Document and review.

## Interview Tip:
"Contain, assess, notify, remediate, document, review â€” the breach response process."

---

## Question 197: How do you manage dependency vulnerabilities?

## Answer:
1. **npm audit**: Check for known vulnerabilities.
2. **Snyk**: Continuous vulnerability scanning.
3. **Dependabot**: Automated dependency updates.
4. **Regular updates**: Keep dependencies current.
5. **Lock files**: Use package-lock.json.

## Key Points:
- npm audit.
- Snyk for continuous scanning.
- Dependabot for updates.
- Regular updates.
- Lock files.

## Interview Tip:
"npm audit + Snyk + Dependabot = dependency security."

---

## Question 198: What tools can scan applications for vulnerabilities?

## Answer:
- **npm audit**: Dependency vulnerabilities.
- **Snyk**: Comprehensive security scanning.
- **OWASP ZAP**: Web application scanner.
- **SonarQube**: Code quality and security.
- **Snyk Code**: Static analysis.

## Key Points:
- npm audit for dependencies.
- Snyk for comprehensive scanning.
- OWASP ZAP for web apps.
- SonarQube for code analysis.

## Interview Tip:
"npm audit for dependencies, Snyk for comprehensive scanning, OWASP ZAP for web apps."

---

## Question 199: What security mistakes do junior developers commonly make?

## Answer:
1. **Storing secrets in code**.
2. **Not validating input**.
3. **Using HTTP instead of HTTPS**.
4. **Storing passwords in plain text**.
5. **Not using HttpOnly cookies**.
6. **Ignoring CORS configuration**.
7. **Not using security headers**.

## Key Points:
- Secrets in code.
- No input validation.
- HTTP instead of HTTPS.
- Plain text passwords.
- No HttpOnly cookies.
- Ignoring CORS.
- No security headers.

## Interview Tip:
"The biggest mistake is not thinking about security at all."

---

## Question 200: What separates junior, mid-level, and senior developers in web security?

## Answer:
- **Junior**: Implements basic auth, uses HTTPS.
- **Mid-level**: Understands OWASP Top 10, implements security headers, validates input.
- **Senior**: Designs secure architectures, performs security reviews, handles incidents, mentors team.

## Key Points:
- Junior: basic auth and HTTPS.
- Mid-level: OWASP, headers, validation.
- Senior: architecture, reviews, incident response.

## Interview Tip:
"Seniors think about security from design, not just implementation."

---

# End of Web Security Interview Questions & Answers
