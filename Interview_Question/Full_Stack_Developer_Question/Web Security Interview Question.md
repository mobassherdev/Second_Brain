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

