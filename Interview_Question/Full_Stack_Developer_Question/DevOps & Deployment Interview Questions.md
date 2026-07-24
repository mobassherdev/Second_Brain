# DevOps & Deployment Interview Questions (200 Total)

---

# Linux Fundamentals

1. What is Linux?
2. Why is Linux commonly used for servers?
3. What are the advantages of Linux for backend systems?
4. What is a Linux distribution?
5. What is the difference between Ubuntu, Debian, and CentOS?
6. What is a Linux shell?
7. What is Bash?
8. What happens when you execute a Linux command?
9. What is the Linux filesystem structure?
10. What are root and user accounts?

---

# Linux Commands

11. How do you navigate directories in Linux?
12. What does `ls` command do?
13. What does `cd` command do?
14. What does `pwd` command do?
15. What does `mkdir` command do?
16. What does `rm` command do?
17. What does `cp` command do?
18. What does `mv` command do?
19. What does `cat` command do?
20. What does `grep` command do?

---

# File Permissions & Users

21. What are Linux file permissions?
22. What do read, write, and execute permissions mean?
23. What is chmod?
24. What is chown?
25. What are Linux users and groups?
26. Why are permissions important on servers?
27. How do you secure Linux servers?
28. What is sudo?
29. Why should applications not run as root?
30. How do you manage server users?

---

# Processes & Services

31. What is a Linux process?
32. How do you check running processes?
33. What is the difference between process and thread?
34. What is PID?
35. What is a daemon process?
36. What is systemd?
37. How do you manage services in Linux?
38. What is systemctl?
39. How do you restart a service?
40. How do you check server logs?

---

# Server Deployment Basics

41. What happens when you deploy an application?
42. What are the steps to deploy a web application?
43. What is a production environment?
44. Development vs staging vs production: what is the difference?
45. What are environment variables?
46. Why should secrets not be stored in code?
47. How do you manage application configuration?
48. What is a reverse proxy?
49. Why is Nginx used in production?
50. How do you deploy a Node.js application on a Linux server?

---

# Docker Fundamentals

51. What is Docker?
52. Why do we use Docker?
53. What problems does Docker solve?
54. What is a container?
55. What is the difference between containers and virtual machines?
56. How does Docker work internally?
57. What is Docker Engine?
58. What is Docker CLI?
59. What is Docker Hub?
60. What are Docker images?

---

# Docker Images & Containers

61. What is a Docker image?
62. How are Docker images created?
63. What is a Dockerfile?
64. What are Dockerfile instructions?
65. What is the difference between CMD and ENTRYPOINT?
66. What is a Docker layer?
67. Why are Docker layers useful?
68. How do you reduce Docker image size?
69. What is a multi-stage Docker build?
70. How do you optimize Docker builds?

---

# Docker Commands

71. How do you create a Docker container?
72. How do you start and stop containers?
73. How do you list running containers?
74. How do you view container logs?
75. How do you access a running container?
76. How do you remove containers?
77. How do you remove images?
78. What is Docker volume?
79. Why are Docker volumes needed?
80. What is Docker networking?

---

# Docker Compose

81. What is Docker Compose?
82. Why use Docker Compose?
83. What is docker-compose.yml?
84. How do you run multiple services using Docker Compose?
85. How would you containerize a Node.js application?
86. How would you containerize PostgreSQL with Node.js?
87. How do containers communicate with each other?
88. What are Docker environment variables?
89. Docker Compose vs Kubernetes: what is the difference?
90. When should you use Docker Compose?

---

# CI/CD Fundamentals

91. What is CI/CD?
92. Why is CI/CD important?
93. What is Continuous Integration?
94. What is Continuous Delivery?
95. What is Continuous Deployment?
96. What are the benefits of CI/CD?
97. What are CI/CD pipeline stages?
98. What happens during a build pipeline?
99. What happens during a deployment pipeline?
100. What CI/CD tools have you used?

---

# GitHub Actions & CI/CD Automation

101. What is GitHub Actions?
102. Why use GitHub Actions?
103. What is a workflow in GitHub Actions?
104. What is a GitHub Actions runner?
105. What are GitHub Actions events/triggers?
106. What are GitHub Actions jobs?
107. What are GitHub Actions steps?
108. How do you create a CI pipeline using GitHub Actions?
109. How do you deploy a Next.js application using GitHub Actions?
110. How do you manage secrets in GitHub Actions?

---

# Jenkins & Other CI/CD Tools

111. What is Jenkins?
112. Why is Jenkins used?
113. Jenkins vs GitHub Actions: what is the difference?
114. What is a Jenkins pipeline?
115. What is a Jenkinsfile?
116. How do you configure automated deployments?
117. What is a build artifact?
118. How do you rollback failed deployments?
119. What CI/CD tools have you worked with?
120. How do you improve CI/CD pipeline performance?

---

# Kubernetes Fundamentals

121. What is Kubernetes?
122. Why do we need Kubernetes?
123. What problems does Kubernetes solve?
124. What is container orchestration?
125. What is a Kubernetes cluster?
126. What are Kubernetes nodes?
127. What is a Kubernetes pod?
128. What is a Kubernetes deployment?
129. What is a Kubernetes service?
130. What is Kubernetes architecture?

---

# Kubernetes Components

131. What is the Kubernetes control plane?
132. What is kube-apiserver?
133. What is etcd?
134. What is kube-scheduler?
135. What is kube-controller-manager?
136. What is kubelet?
137. What is kube-proxy?
138. What happens when you deploy an application to Kubernetes?
139. How does Kubernetes manage failed containers?
140. How does Kubernetes achieve high availability?

---

# Monitoring & Logging

141. Why is monitoring important?
142. What application metrics should be monitored?
143. What is infrastructure monitoring?
144. What is log aggregation?
145. What is centralized logging?
146. What tools are used for monitoring?
147. What is Prometheus?
148. What is Grafana?
149. What is the ELK Stack?
150. How do you debug production issues using logs and metrics?

---

# Nginx & Reverse Proxy

151. What is Nginx?
152. Why is Nginx used in production?
153. What is a reverse proxy?
154. Reverse proxy vs forward proxy: what is the difference?
155. How does Nginx handle incoming requests?
156. How do you configure Nginx for a Node.js application?
157. How do you configure Nginx for a Next.js application?
158. How does Nginx perform load balancing?
159. How do you configure SSL with Nginx?
160. What are common Nginx configuration mistakes?

---

# SSL & HTTPS Deployment

161. What is an SSL certificate?
162. How does HTTPS work?
163. What is TLS handshake?
164. How do you install SSL certificates on a server?
165. What is Let's Encrypt?
166. How do you automate SSL renewal?
167. What happens if an SSL certificate expires?
168. How do you redirect HTTP traffic to HTTPS?
169. Why is HTTPS mandatory for production applications?
170. How do you troubleshoot SSL issues?

---

# Deployment Strategies

171. What is a deployment strategy?
172. What is blue-green deployment?
173. What is canary deployment?
174. What is rolling deployment?
175. Blue-green vs canary deployment: what is the difference?
176. How do you minimize downtime during deployment?
177. How do you rollback a failed deployment?
178. What is zero-downtime deployment?
179. How do you deploy database changes safely?
180. What deployment strategy do you prefer and why?

---

# Application Scaling

181. What is application scaling?
182. Vertical scaling vs horizontal scaling: what is the difference?
183. When should you scale vertically?
184. When should you scale horizontally?
185. How do you scale a Node.js application?
186. How do you handle high traffic?
187. How does load balancing help scaling?
188. What is auto scaling?
189. How do you scale database systems?
190. How do you identify scaling bottlenecks?

---

# Production Engineering & Senior DevOps

191. How do you design a production-ready application?
192. How do you manage multiple environments?
193. How do you handle production incidents?
194. What is disaster recovery?
195. What backup strategies do you follow?
196. How do you secure production servers?
197. How do you manage application secrets?
198. What DevOps practices improve developer productivity?
199. What mistakes do junior developers make in deployment?
200. What separates junior, mid-level, and senior DevOps engineers?

---
