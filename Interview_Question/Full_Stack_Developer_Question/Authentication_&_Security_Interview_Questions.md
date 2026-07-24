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

