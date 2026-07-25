# Docker Interview Questions (150 Total)

---

# Docker Fundamentals

1. What is Docker?
2. Why was Docker created?
3. What problems does Docker solve?
4. What are the advantages of Docker?
5. What are the disadvantages of Docker?
6. What is containerization?
7. How is Docker different from virtual machines?
8. What is the difference between containers and VMs?
9. Why are Docker containers lightweight?
10. What are the main components of Docker?

---

# Docker Architecture

11. What is Docker Engine?
12. What is Docker Client?
13. What is Docker Daemon?
14. How does Docker architecture work?
15. What happens when you run a Docker command?
16. What is Docker Hub?
17. What are Docker registries?
18. What is the difference between public and private registries?
19. What is Docker Desktop?
20. What Docker components have you used?

---

# Images

21. What is a Docker image?
22. How are Docker images created?
23. What is an image layer?
24. Why are Docker images layered?
25. What is the difference between an image and a container?
26. How do you create a Docker image?
27. What is a Docker image tag?
28. What is the latest tag?
29. How do you list Docker images?
30. How do you remove Docker images?

---

# Containers

31. What is a Docker container?
32. How is a container created from an image?
33. How do you run a Docker container?
34. What happens when a container starts?
35. How do you stop a container?
36. How do you restart a container?
37. How do you remove a container?
38. How do you list running containers?
39. What is the difference between running and stopped containers?
40. How do containers communicate?

---

# Basic Docker Commands

41. What does `docker run` do?
42. What does `docker ps` do?
43. What does `docker ps -a` do?
44. What does `docker start` do?
45. What does `docker stop` do?
46. What does `docker restart` do?
47. What does `docker exec` do?
48. What does `docker logs` do?
49. What does `docker inspect` do?
50. What Docker commands do you use regularly?

---

# Dockerfile

51. What is a Dockerfile?
52. Why do we use Dockerfiles?
53. How does a Dockerfile create an image?
54. What is the difference between Dockerfile and Docker image?
55. What is the `FROM` instruction?
56. What is the `RUN` instruction?
57. What is the `COPY` instruction?
58. What is the `ADD` instruction?
59. What is the difference between COPY and ADD?
60. What is the `WORKDIR` instruction?

---

# Dockerfile Instructions

61. What is the `CMD` instruction?
62. What is the `ENTRYPOINT` instruction?
63. What is the difference between CMD and ENTRYPOINT?
64. What is the `EXPOSE` instruction?
65. What is the `ENV` instruction?
66. What is the `ARG` instruction?
67. What is the difference between ARG and ENV?
68. What is the `LABEL` instruction?
69. What is the `USER` instruction?
70. What Dockerfile best practices do you follow?

---

# Image Optimization

71. How do you reduce Docker image size?
72. What are multi-stage builds?
73. Why are multi-stage builds useful?
74. How do you optimize Node.js Docker images?
75. How do you optimize Next.js Docker images?
76. Why should you avoid installing unnecessary packages?
77. What is `.dockerignore`?
78. Why is `.dockerignore` important?
79. How do Docker image layers affect caching?
80. How do you improve Docker build performance?

---

# Docker Compose

81. What is Docker Compose?
82. Why do we use Docker Compose?
83. What is a `docker-compose.yml` file?
84. What are services in Docker Compose?
85. How do you define multiple containers using Compose?
86. How do you start Docker Compose services?
87. How do you stop Docker Compose services?
88. What is the difference between Docker run and Docker Compose?
89. How do containers communicate in Docker Compose?
90. What Docker Compose best practices do you follow?

---

# Networking & Storage

91. What is Docker networking?
92. What are Docker network types?
93. What is the bridge network?
94. What is the host network?
95. What is the none network?
96. How do containers communicate with each other?
97. What is port mapping?
98. What is a Docker volume?
99. Why are Docker volumes needed?
100. What is the difference between volumes and bind mounts?

---

# Production Docker Management

101. How do you deploy Docker containers to production?
102. What challenges occur when running Docker in production?
103. How do you manage Docker containers in production?
104. What is container orchestration?
105. Why is orchestration needed?
106. What tools are used for container orchestration?
107. What is Kubernetes?
108. What is the difference between Docker and Kubernetes?
109. When should you use Kubernetes?
110. What production Docker best practices do you follow?

---

# Container Security

111. How do you secure Docker containers?
112. Why should containers not run as root?
113. How do you run containers with non-root users?
114. What are Docker security risks?
115. How do you scan Docker images for vulnerabilities?
116. What are Docker image vulnerabilities?
117. How do you keep Docker images secure?
118. How do you manage secrets in Docker?
119. Why should secrets not be stored inside Docker images?
120. What Docker security practices do you follow?

---

# Resource Management & Monitoring

121. How do you limit Docker container resources?
122. What are CPU limits in Docker?
123. What are memory limits in Docker?
124. What happens when a container exceeds memory limits?
125. How do you monitor Docker containers?
126. What Docker metrics should you monitor?
127. How do you check container logs?
128. How do you debug a failing container?
129. How do you troubleshoot Docker performance issues?
130. What Docker monitoring tools have you used?

---

# CI/CD Integration

131. How is Docker used in CI/CD pipelines?
132. How do you build Docker images automatically?
133. How do you push images to Docker Hub or private registries?
134. How do you deploy Docker images automatically?
135. How do GitHub Actions and Docker work together?
136. How do you handle Docker image versioning?
137. What is a Docker image registry?
138. How do you rollback Docker deployments?
139. What deployment strategies work with Docker?
140. What Docker CI/CD best practices do you follow?

---

# Senior Real-World Interview Questions

141. Describe the largest Docker-based application you have worked on.
142. What was the most difficult Docker issue you solved?
143. How do you debug a container that keeps crashing?
144. How would you Dockerize a Next.js + Node.js + PostgreSQL application?
145. How would you design a Docker architecture for a SaaS application?
146. How would you optimize Docker builds in a large team?
147. How do you manage Docker images across development, staging, and production?
148. What Docker mistakes do junior developers commonly make?
149. What Docker features do you use most frequently in production?
150. In your opinion, what separates a junior, mid-level, and senior Docker user?

---

# ANSWERS


---

## Part 1 (1â€“10): Docker Fundamentals

---

## Question 1: What is Docker?

## Answer:
Docker is a platform for building, shipping, and running applications in containers. Containers package an application with all its dependencies (libraries, runtime, configuration) into a single unit that runs consistently across any environment.

```bash
docker run nginx  # Runs Nginx in a container
```

## Key Points:
- Platform for containerization.
- Packages applications with dependencies.
- Runs consistently across environments.
- Lightweight alternative to virtual machines.
- Industry standard for containerization.

## Interview Tip:
"Docker solves the 'works on my machine' problem â€” containers run the same everywhere."

---

## Question 2: Why was Docker created?

## Answer:
Docker was created to solve environment inconsistency problems. Before Docker:
- Applications behaved differently across environments.
- Setting up development environments was time-consuming.
- Deploying required manual configuration on each server.
- Scaling required provisioning new servers manually.

Docker containers package everything the app needs, ensuring consistency.

## Key Points:
- Environment inconsistency.
- Complex setup processes.
- Manual deployment configuration.
- Difficult scaling.
- Docker ensures consistency.

## Interview Tip:
"Docker was created because 'it works on my machine' isn't acceptable in production."

---

## Question 3: What problems does Docker solve?

## Answer:
1. **Environment consistency**: Same behavior everywhere.
2. **Dependency conflicts**: Isolated environments per app.
3. **Deployment complexity**: Package once, deploy anywhere.
4. **Scaling**: Spin up containers in seconds.
5. **Resource efficiency**: Lightweight compared to VMs.
6. **Microservices**: Easy service isolation.

## Key Points:
- Environment consistency.
- Dependency isolation.
- Simplified deployment.
- Fast scaling.
- Resource efficiency.
- Microservices support.

## Interview Tip:
"Docker solves environment consistency, dependency isolation, and deployment complexity."

---

## Question 4: What are the advantages of Docker?

## Answer:
- **Consistency**: Same behavior across environments.
- **Isolation**: Each container is independent.
- **Lightweight**: Shares host OS kernel.
- **Fast startup**: Containers start in seconds.
- **Portable**: Run anywhere Docker is installed.
- **Version control**: Image versioning and rollback.
- **Scalability**: Easy horizontal scaling.

## Key Points:
- Consistent environments.
- Isolated containers.
- Lightweight and fast.
- Portable across platforms.
- Easy scaling.

## Interview Tip:
"Docker containers are lightweight, fast, and consistent â€” that's the triple advantage."

---

## Question 5: What are the disadvantages of Docker?

## Answer:
- **Learning curve**: Docker concepts take time.
- **Complexity**: Networking, volumes, orchestration.
- **Security**: Shared kernel risks.
- **Stateful apps**: Databases need careful volume management.
- **GUI apps**: Not ideal for desktop applications.
- **Performance**: Slight overhead vs native.
- **Debugging**: Harder than debugging locally.

## Key Points:
- Learning curve.
- Networking complexity.
- Security considerations.
- Stateful app challenges.
- Slight performance overhead.

## Interview Tip:
"Docker's main challenge is networking and stateful apps â€” databases need volumes."

---

## Question 6: What is containerization?

## Answer:
Containerization is a lightweight form of virtualization where applications run in isolated user-space instances called containers. Containers share the host OS kernel but have their own filesystem, processes, and network.

## Key Points:
- Lightweight virtualization.
- Shared host OS kernel.
- Isolated user-space instances.
- Own filesystem and processes.
- Faster than VMs.

## Interview Tip:
"Containers share the host kernel â€” that's why they're lighter than VMs."

---

## Question 7: How is Docker different from virtual machines?

## Answer:
| Feature | Docker Containers | Virtual Machines |
|---------|-------------------|------------------|
| OS | Shares host kernel | Full OS per VM |
| Size | MBs | GBs |
| Startup | Seconds | Minutes |
| Performance | Near-native | Overhead |
| Isolation | Process-level | Hardware-level |

## Key Points:
- Containers share host kernel.
- VMs have full OS per instance.
- Containers are MBs; VMs are GBs.
- Containers start in seconds.
- Containers have less overhead.

## Interview Tip:
"Containers share the kernel, VMs don't â€” that's the fundamental difference."

---

## Question 8: What is the difference between containers and VMs?

## Answer:
- **Containers**: Share host OS kernel, lightweight, fast startup, process-level isolation.
- **VMs**: Full OS per instance, heavyweight, slow startup, hardware-level isolation.

## Key Points:
- Containers: lightweight, fast, shared kernel.
- VMs: heavyweight, slow, full OS.
- Containers for apps; VMs for full OS isolation.
- Containers are more resource-efficient.
- VMs provide stronger isolation.

## Interview Tip:
"Use containers for app isolation; VMs when you need full OS isolation."

---

## Question 9: Why are Docker containers lightweight?

## Answer:
Containers are lightweight because:
1. **Shared kernel**: No separate OS per container.
2. **Layered filesystem**: Shared base layers.
3. **No hardware virtualization**: Direct access to host resources.
4. **Minimal overhead**: Only application and dependencies.

## Key Points:
- Shared host kernel.
- Layered filesystem.
- No hardware virtualization.
- Minimal overhead.
- MBs instead of GBs.

## Interview Tip:
"Containers share the kernel and use layered filesystems â€” that's why they're lightweight."

---

## Question 10: What are the main components of Docker?

## Answer:
1. **Docker Engine**: Core runtime.
2. **Docker Images**: Read-only templates.
3. **Docker Containers**: Running instances.
4. **Docker Registry**: Image storage (Docker Hub).
5. **Docker Compose**: Multi-container orchestration.
6. **Dockerfile**: Image build instructions.

## Key Points:
- Docker Engine: runtime.
- Images: templates.
- Containers: running instances.
- Registry: image storage.
- Compose: multi-container.
- Dockerfile: build instructions.

## Interview Tip:
"Engine, Images, Containers, Registry, Compose â€” the five Docker components."

---

## Part 2 (11â€“20): Docker Architecture

---

## Question 11: What is Docker Engine?

## Answer:
Docker Engine is the core runtime that builds and runs containers. It consists of:
- **Docker Daemon** (`dockerd`): Background service.
- **REST API**: Interface for daemon communication.
- **CLI** (`docker`): Command-line interface.

## Key Points:
- Core Docker runtime.
- Daemon, API, and CLI.
- Builds and runs containers.
- Background service.
- Client-server architecture.

## Interview Tip:
"Docker Engine is the daemon + API + CLI â€” it's the core of Docker."

---

## Question 12: What is Docker Client?

## Answer:
The Docker Client is the CLI tool (`docker`) that sends commands to the Docker Daemon via the REST API.

```bash
docker run nginx  # Client sends to daemon
```

## Key Points:
- CLI tool (`docker`).
- Sends commands to daemon.
- Communicates via REST API.
- Can connect to remote daemons.
- User interface for Docker.

## Interview Tip:
"The Docker Client is what you type commands into â€” it talks to the daemon."

---

## Question 13: What is Docker Daemon?

## Answer:
The Docker Daemon (`dockerd`) is a background service that manages Docker objects: images, containers, networks, and volumes.

## Key Points:
- Background service.
- Manages Docker objects.
- Listens for API requests.
- Builds and runs containers.
- Manages images, networks, volumes.

## Interview Tip:
"The daemon does the heavy lifting â€” building images, running containers, managing networks."

---

## Question 14: How does Docker architecture work?

## Answer:
```
Docker Client â†’ REST API â†’ Docker Daemon â†’ Containers
                                      â†“
                                  Images, Networks, Volumes
```

1. Client sends command to daemon.
2. Daemon processes command.
3. Daemon manages containers, images, etc.
4. Results returned to client.

## Key Points:
- Client-server architecture.
- REST API communication.
- Daemon manages everything.
- Can connect to remote daemons.
- Centralized management.

## Interview Tip:
"Docker is client-server â€” the client sends commands, the daemon executes them."

---

## Question 15: What happens when you run a Docker command?

## Answer:
```bash
docker run nginx
```

1. Client sends `run` command to daemon.
2. Daemon checks local images for `nginx`.
3. If not found, pulls from Docker Hub.
4. Creates a container from the image.
5. Starts the container.
6. Returns container ID to client.

## Key Points:
- Client sends to daemon.
- Daemon checks local images.
- Pulls from registry if needed.
- Creates and starts container.
- Returns container ID.

## Interview Tip:
"`docker run` = pull + create + start â€” all in one command."

---

## Question 16: What is Docker Hub?

## Answer:
Docker Hub is the default public registry for Docker images. It hosts official images (nginx, node, postgres) and user-published images.

```bash
docker pull nginx  # Pulls from Docker Hub
```

## Key Points:
- Default public registry.
- Official and user images.
- Free for public images.
- Private repositories available.
- `docker pull` and `docker push`.

## Interview Tip:
"Docker Hub is like GitHub for Docker images â€” it's the default registry."

---

## Question 17: What are Docker registries?

## Answer:
Registries store and distribute Docker images. Docker Hub is the default, but you can use private registries (AWS ECR, GitHub Container Registry, Azure ACR).

## Key Points:
- Store and distribute images.
- Docker Hub: default public.
- Private registries for organizations.
- Push and pull images.
- Version management.

## Interview Tip:
"Use private registries for proprietary code â€” never push secrets to Docker Hub."

---

## Question 18: What is the difference between public and private registries?

## Answer:
| Feature | Public Registry | Private Registry |
|---------|----------------|------------------|
| Access | Anyone | Authorized only |
| Examples | Docker Hub (public) | AWS ECR, GitHub CR |
| Use case | Open source | Proprietary code |
| Security | Low | High |

## Key Points:
- Public: open access.
- Private: authorized only.
- Public for open source.
- Private for proprietary code.
- Security consideration.

## Interview Tip:
"Use private registries for production images â€” never expose proprietary code."

---

## Question 19: What is Docker Desktop?

## Answer:
Docker Desktop is a GUI application for Mac, Windows, and Linux that includes Docker Engine, CLI, Compose, and Kubernetes.

## Key Points:
- GUI for Docker.
- Includes Engine, CLI, Compose, Kubernetes.
- Available for Mac, Windows, Linux.
- Easy installation.
- Development-focused.

## Interview Tip:
"Docker Desktop is the easiest way to get started with Docker on Mac/Windows."

---

## Question 20: What Docker components have you used?

## Answer:
- **Docker Engine**: Running containers.
- **Dockerfile**: Building images.
- **Docker Compose**: Multi-container apps.
- **Docker Hub**: Pulling and pushing images.
- **Docker Volumes**: Persistent storage.
- **Docker Networks**: Container communication.

## Key Points:
- Engine for runtime.
- Dockerfile for building.
- Compose for multi-container.
- Hub for registry.
- Volumes for storage.
- Networks for communication.

## Interview Tip:
"Name the components you've actually used â€” be specific about your experience."

---

## Part 3 (21â€“30): Images

---

## Question 21: What is a Docker image?

## Answer:
A Docker image is a read-only template containing everything needed to run an application: code, runtime, libraries, environment variables, and configuration.

```bash
docker pull node:20  # Pull Node.js image
```

## Key Points:
- Read-only template.
- Contains code, runtime, libraries.
- Used to create containers.
- Stored in registries.
- Versioned with tags.

## Interview Tip:
"An image is a blueprint; a container is a running instance of that blueprint."

---

## Question 22: How are Docker images created?

## Answer:
1. **Dockerfile**: Build instructions.
2. **docker build**: Build from Dockerfile.
3. **docker commit**: Save container as image.
4. **Pull**: Download from registry.

```bash
docker build -t my-app .  # Build from Dockerfile
```

## Key Points:
- Dockerfile for build instructions.
- `docker build` to create.
- `docker commit` from container.
- Pull from registry.
- Layered approach.

## Interview Tip:
"Most images are built from Dockerfiles â€” `docker build` is the standard way."

---

## Question 23: What is an image layer?

## Answer:
Each instruction in a Dockerfile creates a layer. Layers are cached and shared between images.

```dockerfile
FROM node:20        # Layer 1
COPY package.json . # Layer 2
RUN npm install     # Layer 3
COPY . .            # Layer 4
```

## Key Points:
- Each instruction creates a layer.
- Layers are cached.
- Shared between images.
- Stacked on top of each other.
- Immutable once created.

## Interview Tip:
"Layers are cached â€” if nothing changes, Docker reuses the cached layer."

---

## Question 24: Why are Docker images layered?

## Answer:
Layering enables:
1. **Caching**: Unchanged layers are reused.
2. **Sharing**: Common layers shared between images.
3. **Efficiency**: Only changed layers are rebuilt.
4. **Smaller downloads**: Only pull missing layers.

## Key Points:
- Caching for faster builds.
- Sharing between images.
- Efficient rebuilds.
- Smaller downloads.
- Immutable layers.

## Interview Tip:
"Layering is why Docker builds are fast â€” unchanged layers are cached."

---

## Question 25: What is the difference between an image and a container?

## Answer:
| Feature | Image | Container |
|---------|-------|-----------|
| State | Read-only | Running instance |
| Mutability | Immutable | Mutable (changes in layer) |
| Analogy | Blueprint | House |
| Storage | Registry | Local |

## Key Points:
- Image: read-only template.
- Container: running instance.
- Image is the blueprint.
- Container is the house.
- Multiple containers from one image.

## Interview Tip:
"An image is a blueprint; a container is a running instance of it."

---

## Question 26: How do you create a Docker image?

## Answer:
```bash
# From Dockerfile
docker build -t my-app:1.0 .

# From running container
docker commit container-id my-app:1.0
```

## Key Points:
- `docker build` from Dockerfile.
- `docker commit` from container.
- Tag with name and version.
- `-t` for tag.
- `.` for build context.

## Interview Tip:
"`docker build -t name:tag .` is the standard way to create images."

---

## Question 27: What is a Docker image tag?

## Answer:
Tags identify specific versions of an image.

```bash
docker pull node:20      # Version 20
docker pull node:20-alpine  # Version 20, Alpine variant
docker pull node:latest   # Latest version
```

## Key Points:
- Identify image versions.
- `name:tag` format.
- Default tag is `latest`.
- Use specific versions in production.
- Semantic versioning common.

## Interview Tip:
"Always use specific tags in production â€” `latest` is unpredictable."

---

## Question 28: What is the latest tag?

## Answer:
The `latest` tag is the default tag when none is specified. It points to the most recently pushed version.

```bash
docker pull node  # Same as docker pull node:latest
```

## Key Points:
- Default tag.
- Points to most recent version.
- Can change unexpectedly.
- Don't use in production.
- Specify explicit versions.

## Interview Tip:
"Never use `latest` in production â€” it can change unexpectedly and break things."

---

## Question 29: How do you list Docker images?

## Answer:
```bash
docker images          # List all images
docker image ls        # Same as above
docker images -a       # Include intermediate images
docker images --filter "dangling=true"  # Dangling images
```

## Key Points:
- `docker images` lists all images.
- `-a` includes intermediate images.
- Filter by name, tag, or status.
- Shows size and creation date.

## Interview Tip:
"`docker images` shows all local images â€” use `-a` to see intermediate layers."

---

## Question 30: How do you remove Docker images?

## Answer:
```bash
docker rmi image-id        # Remove by ID
docker rmi name:tag        # Remove by name:tag
docker image prune         # Remove dangling images
docker image prune -a      # Remove all unused images
```

## Key Points:
- `docker rmi` removes specific images.
- `docker image prune` removes unused.
- `-a` removes all unused.
- Cannot remove images used by containers.
- Clean up regularly.

## Interview Tip:
"`docker image prune -a` cleans up all unused images â€” run it regularly."

---

## Part 4 (31â€“40): Containers

---

## Question 31: What is a Docker container?

## Answer:
A container is a running instance of a Docker image. It has its own filesystem, processes, and network, but shares the host OS kernel.

## Key Points:
- Running instance of an image.
- Own filesystem and processes.
- Shares host kernel.
- Isolated from other containers.
- Lightweight and fast.

## Interview Tip:
"A container is a running image â€” it's the live instance."

---

## Question 32: How is a container created from an image?

## Answer:
```bash
docker run nginx
# Creates and starts a container from the nginx image
```

`docker run` = `docker create` + `docker start`.

## Key Points:
- `docker run` creates and starts.
- `docker create` only creates.
- `docker start` starts a stopped container.
- Container gets writable layer on top of image.

## Interview Tip:
"`docker run` is the most common command â€” it creates and starts in one step."

---

## Question 33: How do you run a Docker container?

## Answer:
```bash
docker run nginx                    # Run in foreground
docker run -d nginx                 # Run in background (detached)
docker run -d --name my-nginx nginx # With custom name
docker run -p 8080:80 nginx         # With port mapping
```

## Key Points:
- `docker run` to start.
- `-d` for detached (background).
- `--name` for custom name.
- `-p` for port mapping.
- Many options available.

## Interview Tip:
"`docker run -d -p 8080:80 nginx` â€” detached with port mapping, the most common pattern."

---

## Question 34: What happens when a container starts?

## Answer:
1. Docker creates a writable layer on top of the image.
2. Docker sets up networking (IP, ports).
3. Docker configures storage (volumes).
4. Container runs the CMD/ENTRYPOINT command.
5. Container runs until the command exits.

## Key Points:
- Writable layer added.
- Networking configured.
- Storage configured.
- CMD/ENTRYPOINT executed.
- Runs until command exits.

## Interview Tip:
"A container runs the CMD/ENTRYPOINT command â€” when it exits, the container stops."

---

## Question 35: How do you stop a container?

## Answer:
```bash
docker stop container-id    # Graceful stop (SIGTERM)
docker stop -t 0 container  # Force stop (SIGKILL)
docker kill container-id    # Immediate kill (SIGKILL)
```

## Key Points:
- `docker stop`: graceful (SIGTERM).
- `docker kill`: immediate (SIGKILL).
- `-t 0`: skip grace period.
- Always try `stop` before `kill`.
- Stopped containers still exist.

## Interview Tip:
"`docker stop` is graceful; `docker kill` is immediate â€” use stop first."

---

## Question 36: How do you restart a container?

## Answer:
```bash
docker restart container-id
```

Stops and starts the container.

## Key Points:
- Stops and starts.
- Same container (not new).
- Preserves configuration.
- Useful for applying changes.
- Can set restart policy.

## Interview Tip:
"`docker restart` is useful for applying configuration changes."

---

## Question 37: How do you remove a container?

## Answer:
```bash
docker rm container-id          # Remove stopped container
docker rm -f container-id       # Force remove running container
docker container prune          # Remove all stopped containers
```

## Key Points:
- `docker rm` removes stopped containers.
- `-f` force removes running containers.
- `docker container prune` removes all stopped.
- Cannot remove running containers without `-f`.
- Clean up regularly.

## Interview Tip:
"`docker container prune` cleans up all stopped containers â€” run it regularly."

---

## Question 38: How do you list running containers?

## Answer:
```bash
docker ps              # Running containers
docker ps -a           # All containers (including stopped)
docker ps -q           # Only container IDs
docker ps --filter "status=exited"  # Filter by status
```

## Key Points:
- `docker ps` for running.
- `-a` for all (including stopped).
- `-q` for IDs only.
- Filter by status, name, etc.
- Most used Docker command.

## Interview Tip:
"`docker ps` is the most used Docker command â€” learn its filters."

---

## Question 39: What is the difference between running and stopped containers?

## Answer:
- **Running**: Active, consuming resources, executing processes.
- **Stopped**: Exited, not consuming resources, still exists.

Stopped containers can be restarted without losing data (unless volumes are removed).

## Key Points:
- Running: active, consuming resources.
- Stopped: exited, not consuming resources.
- Stopped containers still exist.
- Can restart stopped containers.
- Remove stopped containers to free disk space.

## Interview Tip:
"Stopped containers still exist â€” remove them with `docker rm` or `docker container prune`."

---

## Question 40: How do containers communicate?

## Answer:
1. **Docker networks**: Containers on the same network can communicate.
2. **Port mapping**: Expose container ports to host.
3. **DNS**: Containers can resolve each other by name.
4. **Shared volumes**: Share data via volumes.

## Key Points:
- Docker networks for container communication.
- Port mapping for host access.
- DNS for name resolution.
- Shared volumes for data sharing.
- Bridge network by default.

## Interview Tip:
"Containers on the same Docker network can communicate by name â€” that's DNS-based discovery."

---

## Part 5 (41â€“50): Basic Docker Commands

---

## Question 41: What does `docker run` do?

## Answer:
`docker run` creates and starts a container from an image.

```bash
docker run [OPTIONS] IMAGE [COMMAND]
docker run -d -p 8080:80 --name web nginx
```

## Key Points:
- Creates and starts a container.
- Many options (-d, -p, --name, -v).
- Can specify command to run.
- Most commonly used Docker command.
- Equivalent to create + start.

## Interview Tip:
"`docker run` is the Swiss Army knife of Docker â€” learn its options."

---

## Question 42: What does `docker ps` do?

## Answer:
Lists running containers.

```bash
docker ps
# CONTAINER ID  IMAGE  COMMAND  CREATED  STATUS  PORTS  NAMES
```

## Key Points:
- Lists running containers.
- Shows ID, image, status, ports.
- `-a` for all containers.
- `-q` for IDs only.
- Most used monitoring command.

## Interview Tip:
"`docker ps` is your go-to for checking what's running."

---

## Question 43: What does `docker ps -a` do?

## Answer:
Lists all containers, including stopped ones.

```bash
docker ps -a
# Shows running + stopped + exited containers
```

## Key Points:
- Shows all containers.
- Includes stopped and exited.
- Useful for debugging.
- Shows container history.
- `-q` for just IDs.

## Interview Tip:
"`docker ps -a` shows everything â€” useful for finding stopped containers."

---

## Question 44: What does `docker start` do?

## Answer:
Starts a stopped container.

```bash
docker start container-id
docker start -a container-id  # Attach to output
```

## Key Points:
- Starts stopped containers.
- Same container (not new).
- Preserves configuration.
- `-a` to attach to output.
- Different from `docker run`.

## Interview Tip:
"`docker start` restarts a stopped container; `docker run` creates a new one."

---

## Question 45: What does `docker stop` do?

## Answer:
Gracefully stops a running container by sending SIGTERM, then SIGKILL after timeout.

```bash
docker stop container-id
docker stop -t 30 container-id  # 30 second timeout
```

## Key Points:
- Graceful stop (SIGTERM).
- Timeout before SIGKILL.
- Default timeout: 10 seconds.
- Container still exists after stop.
- Use before `docker rm`.

## Interview Tip:
"`docker stop` is graceful â€” give your app time to shut down cleanly."

---

## Question 46: What does `docker restart` do?

## Answer:
Stops and starts a container.

```bash
docker restart container-id
```

## Key Points:
- Stops and starts.
- Same container.
- Preserves configuration.
- Useful for applying changes.
- Can set restart policy.

## Interview Tip:
"`docker restart` is useful for configuration changes."

---

## Question 47: What does `docker exec` do?

## Answer:
Runs a command inside a running container.

```bash
docker exec -it container-id bash  # Interactive shell
docker exec container-id ls /app   # Run command
```

## Key Points:
- Runs command in running container.
- `-it` for interactive terminal.
- `bash` for shell access.
- Useful for debugging.
- Doesn't stop the container.

## Interview Tip:
"`docker exec -it container-id bash` gives you a shell inside the container."

---

## Question 48: What does `docker logs` do?

## Answer:
Shows container logs (stdout/stderr).

```bash
docker logs container-id
docker logs -f container-id    # Follow (tail -f)
docker logs --tail 100 container-id  # Last 100 lines
```

## Key Points:
- Shows container stdout/stderr.
- `-f` to follow logs.
- `--tail` for recent lines.
- `--since` for time-based filtering.
- Primary debugging tool.

## Interview Tip:
"`docker logs -f` is your best friend for debugging â€” follow the logs in real-time."

---

## Question 49: What does `docker inspect` do?

## Answer:
Shows detailed JSON metadata about a container, image, network, or volume.

```bash
docker inspect container-id
docker inspect --format '{{.NetworkSettings.IPAddress}}' container-id
```

## Key Points:
- Shows detailed metadata.
- JSON format.
- Can filter with `--format`.
- Shows IP, ports, volumes, env vars.
- Useful for debugging.

## Interview Tip:
"`docker inspect` gives you everything about a container â€” IP, ports, volumes, environment."

---

## Question 50: What Docker commands do you use regularly?

## Answer:
- `docker run`: Start containers.
- `docker ps`: List running containers.
- `docker logs`: Check container logs.
- `docker exec`: Access container shell.
- `docker compose up`: Start multi-container apps.
- `docker build`: Build images.
- `docker system prune`: Clean up.

## Key Points:
- `run`, `ps`, `logs`, `exec`: daily use.
- `compose up` for multi-container.
- `build` for images.
- `prune` for cleanup.

## Interview Tip:
"Know the essential commands: run, ps, logs, exec, compose up, build, prune."

---

## Part 6 (51â€“60): Dockerfile

---

## Question 51: What is a Dockerfile?

## Answer:
A Dockerfile is a text file containing instructions to build a Docker image.

```dockerfile
FROM node:20
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD ["node", "server.js"]
```

## Key Points:
- Text file with build instructions.
- Each instruction creates a layer.
- Builds an image.
- Version controlled.
- Declarative approach.

## Interview Tip:
"A Dockerfile is the blueprint for your Docker image â€” version control it."

---

## Question 52: Why do we use Dockerfiles?

## Answer:
- **Reproducibility**: Same image every time.
- **Automation**: No manual setup.
- **Version control**: Track changes.
- **Documentation**: Self-documenting setup.
- **CI/CD**: Automated builds.

## Key Points:
- Reproducible builds.
- Automated image creation.
- Version controlled.
- Self-documenting.
- CI/CD integration.

## Interview Tip:
"Dockerfiles make builds reproducible and automatable â€” no manual setup."

---

## Question 53: How does a Dockerfile create an image?

## Answer:
```bash
docker build -t my-app .
```

Docker reads the Dockerfile, executes each instruction, and creates layers. Each layer is cached.

## Key Points:
- `docker build` reads Dockerfile.
- Each instruction creates a layer.
- Layers are cached.
- Final layer is the image.
- Build context is the directory.

## Interview Tip:
"`docker build` processes instructions top-to-bottom, creating cached layers."

---

## Question 54: What is the difference between Dockerfile and Docker image?

## Answer:
- **Dockerfile**: Text file with build instructions.
- **Docker Image**: Built artifact from Dockerfile.

Dockerfile is the recipe; image is the cake.

## Key Points:
- Dockerfile: source code.
- Image: built artifact.
- Dockerfile is version controlled.
- Image is stored in registry.
- One Dockerfile can create many images.

## Interview Tip:
"Dockerfile is the recipe; image is the cake."

---

## Question 55: What is the `FROM` instruction?

## Answer:
`FROM` sets the base image for the Dockerfile.

```dockerfile
FROM node:20
FROM nginx:alpine
FROM python:3.11-slim
```

## Key Points:
- Sets the base image.
- First instruction in Dockerfile.
- Can use multiple FROM (multi-stage).
- Use official images when possible.
- Use specific versions, not `latest`.

## Interview Tip:
"Always specify a version in `FROM` â€” `FROM node:20` not `FROM node:latest`."

---

## Question 56: What is the `RUN` instruction?

## Answer:
`RUN` executes commands during image build.

```dockerfile
RUN npm install
RUN apt-get update && apt-get install -y curl
```

## Key Points:
- Executes during build.
- Creates a new layer.
- Can run any command.
- Chain commands to reduce layers.
- Results are committed to image.

## Interview Tip:
"Chain RUN commands with `&&` to reduce layers â€” `RUN apt-get update && apt-get install -y curl`."

---

## Question 57: What is the `COPY` instruction?

## Answer:
`COPY` copies files from the build context into the image.

```dockerfile
COPY package*.json ./
COPY . .
COPY --from=builder /app/dist ./dist  # Multi-stage
```

## Key Points:
- Copies files into image.
- From build context to container.
- Can copy from previous stage.
- Most commonly used instruction.
- Better than ADD for simple copies.

## Interview Tip:
"Use `COPY` over `ADD` â€” it's clearer and more predictable."

---

## Question 58: What is the `ADD` instruction?

## Answer:
`ADD` copies files like COPY, but with extra features:
- Auto-extracts tar files.
- Supports URLs.

```dockerfile
ADD archive.tar.gz /app/
ADD https://example.com/file.txt /app/
```

## Key Points:
- Copies files like COPY.
- Auto-extracts tar files.
- Supports URLs.
- Less predictable than COPY.
- Use COPY when possible.

## Interview Tip:
"Prefer `COPY` over `ADD` â€” `ADD` has hidden behavior (auto-extraction)."

---

## Question 59: What is the difference between COPY and ADD?

## Answer:
| Feature | COPY | ADD |
|---------|------|-----|
| Copy files | Yes | Yes |
| Auto-extract tar | No | Yes |
| URLs | No | Yes |
| Predictability | High | Lower |

Use COPY for simple file copies; ADD only when you need auto-extraction.

## Key Points:
- COPY: simple, predictable.
- ADD: auto-extraction, URL support.
- COPY is preferred.
- ADD has hidden behavior.
- Use COPY unless you need ADD features.

## Interview Tip:
"Default to `COPY` â€” use `ADD` only for tar extraction or URLs."

---

## Question 60: What is the `WORKDIR` instruction?

## Answer:
`WORKDIR` sets the working directory for subsequent instructions.

```dockerfile
WORKDIR /app
COPY . .  # Copies to /app
RUN npm install  # Runs in /app
```

## Key Points:
- Sets working directory.
- Creates directory if it doesn't exist.
- Affects subsequent instructions.
- Can be used multiple times.
- Best practice: set early.

## Interview Tip:
"Set `WORKDIR /app` early â€” it makes subsequent instructions cleaner."

---

## Part 7 (61â€“70): Dockerfile Instructions

---

## Question 61: What is the `CMD` instruction?

## Answer:
`CMD` sets the default command to run when the container starts.

```dockerfile
CMD ["node", "server.js"]
CMD ["npm", "start"]
```

Can be overridden at runtime: `docker run my-app python app.py`.

## Key Points:
- Default command for container.
- Can be overridden at runtime.
- Only one CMD per Dockerfile.
- JSON array format preferred.
- Exec form vs shell form.

## Interview Tip:
"`CMD` is the default â€” it can be overridden. Use JSON array format."

---

## Question 62: What is the `ENTRYPOINT` instruction?

## Answer:
`ENTRYPOINT` configures the container to run as an executable. It's not easily overridden.

```dockerfile
ENTRYPOINT ["node", "server.js"]
```

## Key Points:
- Configures container as executable.
- Not easily overridden.
- CMD provides default arguments.
- ENTRYPOINT + CMD pattern.
- Use for fixed commands.

## Interview Tip:
"Use `ENTRYPOINT` for the main command; `CMD` for default arguments."

---

## Question 63: What is the difference between CMD and ENTRYPOINT?

## Answer:
| Feature | CMD | ENTRYPOINT |
|---------|-----|------------|
| Override | Easily | Not easily |
| Purpose | Default command | Fixed executable |
| Runtime | `docker run args` replaces CMD | `docker run args` appends to ENTRYPOINT |

```dockerfile
ENTRYPOINT ["node"]
CMD ["server.js"]
# docker run my-app â†’ node server.js
# docker run my-app app.js â†’ node app.js
```

## Key Points:
- CMD: easily overridden.
- ENTRYPOINT: fixed executable.
- Together: ENTRYPOINT + default CMD args.
- Use ENTRYPOINT for the main binary.
- Use CMD for default arguments.

## Interview Tip:
"ENTRYPOINT for the binary, CMD for defaults â€” they work together."

---

## Question 64: What is the `EXPOSE` instruction?

## Answer:
`EXPOSE` documents which ports the container uses. It doesn't actually publish the port.

```dockerfile
EXPOSE 3000
EXPOSE 8080 8443
```

## Key Points:
- Documents port usage.
- Doesn't publish ports.
- Documentation only.
- Use `-p` to actually publish.
- Good practice to include.

## Interview Tip:
"`EXPOSE` is documentation â€” use `-p` to actually publish ports."

---

## Question 65: What is the `ENV` instruction?

## Answer:
`ENV` sets environment variables in the image.

```dockerfile
ENV NODE_ENV=production
ENV PORT=3000
```

## Key Points:
- Sets environment variables.
- Available during build and runtime.
- Can be overridden at runtime.
- Use for configuration.
- Multiple ENV instructions allowed.

## Interview Tip:
"Use `ENV` for default configuration â€” override at runtime with `-e`."

---

## Question 66: What is the `ARG` instruction?

## Answer:
`ARG` defines build-time variables.

```dockerfile
ARG NODE_VERSION=20
FROM node:${NODE_VERSION}
```

```bash
docker build --build-arg NODE_VERSION=18 .
```

## Key Points:
- Build-time only.
- Not available at runtime.
- Can be passed with `--build-arg`.
- Use for build configuration.
- Different from ENV.

## Interview Tip:
"`ARG` is build-time only; `ENV` is runtime. Don't confuse them."

---

## Question 67: What is the difference between ARG and ENV?

## Answer:
| Feature | ARG | ENV |
|---------|-----|-----|
| Availability | Build-time only | Build and runtime |
| Override | `--build-arg` | `-e` at runtime |
| In image | No | Yes |
| Use case | Build config | Runtime config |

## Key Points:
- ARG: build-time only.
- ENV: build and runtime.
- ARG not in final image.
- ENV persists in image.
- Use ARG for build config.

## Interview Tip:
"ARG for build configuration; ENV for runtime configuration."

---

## Question 68: What is the `LABEL` instruction?

## Answer:
`LABEL` adds metadata to the image.

```dockerfile
LABEL maintainer="alice@example.com"
LABEL version="1.0"
LABEL description="My application"
```

## Key Points:
- Adds metadata.
- Key-value pairs.
- Multiple labels allowed.
- Use for documentation.
- Can be queried with `docker inspect`.

## Interview Tip:
"Use `LABEL` to document image metadata â€” maintainer, version, description."

---

## Question 69: What is the `USER` instruction?

## Answer:
`USER` sets the user for subsequent instructions and runtime.

```dockerfile
RUN addgroup -S appgroup && adduser -S appuser -G appgroup
USER appuser
```

## Key Points:
- Sets the user for commands.
- Don't run as root.
- Create a non-root user.
- Security best practice.
- Apply after installing dependencies.

## Interview Tip:
"Never run containers as root â€” use `USER` to set a non-root user."

---

## Question 70: What Dockerfile best practices do you follow?

## Answer:
1. **Use specific versions**: `FROM node:20`, not `node:latest`.
2. **Order instructions wisely**: Cache dependencies.
3. **Minimize layers**: Chain RUN commands.
4. **Use `.dockerignore`**: Exclude unnecessary files.
5. **Non-root user**: Don't run as root.
6. **Multi-stage builds**: Reduce final image size.
7. **Use COPY over ADD**: More predictable.

## Key Points:
- Specific versions for reproducibility.
- Order for caching.
- Minimize layers.
- `.dockerignore` for efficiency.
- Non-root for security.
- Multi-stage for smaller images.

## Interview Tip:
"Order matters for caching â€” put rarely-changing instructions first."

---

## Part 8 (71â€“80): Image Optimization

---

## Question 71: How do you reduce Docker image size?

## Answer:
1. **Use slim/alpine base images**: `node:20-alpine`.
2. **Multi-stage builds**: Build in one stage, copy to another.
3. **Remove unnecessary files**: `.dockerignore`, cleanup.
4. **Chain RUN commands**: Reduce layers.
5. **Use COPY over ADD**: More predictable.
6. **Don't install dev dependencies**: Production only.

## Key Points:
- Alpine/slim base images.
- Multi-stage builds.
- `.dockerignore`.
- Chain RUN commands.
- Production dependencies only.

## Interview Tip:
"Alpine images + multi-stage builds = smallest possible images."

---

## Question 72: What are multi-stage builds?

## Answer:
Multi-stage builds use multiple FROM instructions to separate build and runtime stages.

```dockerfile
# Build stage
FROM node:20 AS builder
WORKDIR /app
COPY . .
RUN npm ci && npm run build

# Runtime stage
FROM node:20-alpine
WORKDIR /app
COPY --from=builder /app/dist ./dist
COPY --from=builder /app/node_modules ./node_modules
CMD ["node", "dist/server.js"]
```

## Key Points:
- Multiple FROM instructions.
- Separate build and runtime.
- Copy only needed artifacts.
- Dramatically smaller images.
- Build tools not in final image.

## Interview Tip:
"Multi-stage builds separate build tools from the final image â€” use them for production."

---

## Question 73: Why are multi-stage builds useful?

## Answer:
- **Smaller images**: Build tools not included in final image.
- **Security**: Fewer packages = fewer vulnerabilities.
- **Faster deployments**: Smaller images transfer faster.
- **Clean separation**: Build vs runtime concerns.

## Key Points:
- Smaller final images.
- Fewer vulnerabilities.
- Faster deployments.
- Clean separation.
- Industry standard.

## Interview Tip:
"Multi-stage builds are essential for production â€” they reduce image size by 50-90%."

---

## Question 74: How do you optimize Node.js Docker images?

## Answer:
```dockerfile
FROM node:20-alpine AS builder
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build

FROM node:20-alpine
WORKDIR /app
COPY --from=builder /app/dist ./dist
COPY --from=builder /app/node_modules ./node_modules
COPY --from=builder /app/package.json ./
USER node
CMD ["node", "dist/server.js"]
```

## Key Points:
- Alpine base image.
- Multi-stage build.
- Copy only production artifacts.
- Non-root user.
- Production dependencies only.

## Interview Tip:
"Alpine + multi-stage + non-root user â€” the Node.js Docker optimization pattern."

---

## Question 75: How do you optimize Next.js Docker images?

## Answer:
```dockerfile
FROM node:20-alpine AS builder
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build

FROM node:20-alpine
WORKDIR /app
COPY --from=builder /app/.next/standalone ./
COPY --from=builder /app/.next/static ./.next/static
COPY --from=builder /app/public ./public
EXPOSE 3000
CMD ["node", "server.js"]
```

Use `output: "standalone"` in `next.config.js`.

## Key Points:
- Standalone output for minimal size.
- Multi-stage build.
- Copy only standalone output.
- Alpine base image.
- Non-root user.

## Interview Tip:
"Next.js standalone output + multi-stage build = optimized Docker image."

---

## Question 76: Why should you avoid installing unnecessary packages?

## Answer:
- **Image size**: More packages = larger image.
- **Security**: More packages = more vulnerabilities.
- **Build time**: More packages = longer builds.
- **Attack surface**: Fewer packages = fewer entry points.

## Key Points:
- Larger image size.
- More vulnerabilities.
- Longer builds.
- Larger attack surface.
- Install only what's needed.

## Interview Tip:
"Every unnecessary package increases size and vulnerability â€” install only what's needed."

---

## Question 77: What is `.dockerignore`?

## Answer:
`.dockerignore` excludes files from the build context, similar to `.gitignore`.

```
node_modules
.git
.env
*.md
dist
coverage
```

## Key Points:
- Excludes files from build context.
- Similar to `.gitignore`.
- Reduces build context size.
- Speeds up builds.
- Prevents copying secrets.

## Interview Tip:
"Always have a `.dockerignore` â€” exclude node_modules, .git, .env, and dist."

---

## Question 78: Why is `.dockerignore` important?

## Answer:
- **Faster builds**: Smaller build context.
- **Smaller images**: Unnecessary files excluded.
- **Security**: Secrets not copied into image.
- **Cache efficiency**: Fewer files = better caching.

## Key Points:
- Faster builds.
- Smaller images.
- Security (no secrets).
- Better caching.
- Essential for production.

## Interview Tip:
"Without `.dockerignore`, Docker copies everything â€” including .git and node_modules."

---

## Question 79: How do Docker image layers affect caching?

## Answer:
Docker caches layers. If a layer hasn't changed, Docker uses the cached version.

```dockerfile
COPY package*.json ./   # Layer 1 (cached if unchanged)
RUN npm install          # Layer 2 (cached if Layer 1 unchanged)
COPY . .                 # Layer 3 (changes often)
```

Order: put rarely-changing instructions first.

## Key Points:
- Layers are cached.
- Unchanged layers reused.
- Order matters for caching.
- Put dependencies before code.
- Speeds up rebuilds.

## Interview Tip:
"Order your Dockerfile for optimal caching â€” dependencies before code."

---

## Question 80: How do you improve Docker build performance?

## Answer:
1. **Use `.dockerignore`**: Smaller build context.
2. **Order for caching**: Dependencies before code.
3. **Chain RUN commands**: Fewer layers.
4. **Use BuildKit**: Faster builds.
5. **Multi-stage builds**: Parallel stages.

## Key Points:
- `.dockerignore` for smaller context.
- Order for caching.
- Chain RUN commands.
- BuildKit for speed.
- Multi-stage for parallelism.

## Interview Tip:
"BuildKit + `.dockerignore` + proper ordering = fast builds."

---

## Part 9 (81â€“90): Docker Compose

---

## Question 81: What is Docker Compose?

## Answer:
Docker Compose is a tool for defining and running multi-container applications using a YAML file.

```yaml
services:
  web:
    build: .
    ports:
      - "3000:3000"
  db:
    image: postgres:15
    environment:
      POSTGRES_PASSWORD: secret
```

```bash
docker compose up
```

## Key Points:
- Multi-container orchestration.
- YAML configuration.
- `docker compose up` to start.
- Defines services, networks, volumes.
- Development-focused.

## Interview Tip:
"Docker Compose is for multi-container apps â€” define everything in YAML."

---

## Question 82: Why do we use Docker Compose?

## Answer:
- **Multi-container apps**: Define multiple services.
- **Reproducibility**: Same setup every time.
- **Simplicity**: One command to start everything.
- **Networking**: Automatic service discovery.
- **Development**: Easy local development setup.

## Key Points:
- Multi-container management.
- Reproducible environments.
- Simple commands.
- Automatic networking.
- Development-focused.

## Interview Tip:
"Docker Compose simplifies multi-container development â€” one YAML file, one command."

---

## Question 83: What is a `docker-compose.yml` file?

## Answer:
A YAML file that defines services, networks, and volumes for a multi-container application.

```yaml
services:
  app:
    build: .
    ports:
      - "3000:3000"
    depends_on:
      - db
  db:
    image: postgres:15
    volumes:
      - db-data:/var/lib/postgresql/data

volumes:
  db-data:
```

## Key Points:
- Defines services, networks, volumes.
- YAML format.
- Version controlled.
- Reproducible setup.
- Single source of truth.

## Interview Tip:
"`docker-compose.yml` is the single source of truth for your multi-container setup."

---

## Question 84: What are services in Docker Compose?

## Answer:
Services are container definitions in `docker-compose.yml`. Each service runs one container.

```yaml
services:
  web:     # Service name
    image: nginx
  api:     # Another service
    build: .
  db:      # Another service
    image: postgres:15
```

## Key Points:
- Container definitions.
- Each service = one container.
- Can use image or build.
- Named for DNS resolution.
- Can depend on other services.

## Interview Tip:
"Services are container definitions â€” they communicate by name via DNS."

---

## Question 85: How do you define multiple containers using Compose?

## Answer:
```yaml
services:
  frontend:
    build: ./frontend
    ports:
      - "3000:3000"
  backend:
    build: ./backend
    ports:
      - "4000:4000"
  database:
    image: postgres:15
    environment:
      POSTGRES_PASSWORD: secret
```

## Key Points:
- Multiple services in one file.
- Each with own configuration.
- Automatic networking between services.
- Shared volumes possible.
- Single command to start all.

## Interview Tip:
"Define all services in one `docker-compose.yml` â€” they communicate automatically."

---

## Question 86: How do you start Docker Compose services?

## Answer:
```bash
docker compose up          # Start in foreground
docker compose up -d       # Start in background
docker compose up --build  # Rebuild and start
```

## Key Points:
- `docker compose up` to start.
- `-d` for detached.
- `--build` to rebuild images.
- Starts all services.
- Creates networks and volumes.

## Interview Tip:
"`docker compose up -d --build` â€” start everything in background with fresh builds."

---

## Question 87: How do you stop Docker Compose services?

## Answer:
```bash
docker compose down         # Stop and remove containers
docker compose down -v      # Also remove volumes
docker compose stop         # Stop without removing
```

## Key Points:
- `down`: stop and remove.
- `down -v`: also remove volumes.
- `stop`: stop only.
- Clean up resources.
- Preserve data with volumes.

## Interview Tip:
"`docker compose down -v` removes everything including volumes â€” use carefully."

---

## Question 88: What is the difference between Docker run and Docker Compose?

## Answer:
| Feature | Docker Run | Docker Compose |
|---------|-----------|----------------|
| Containers | Single | Multiple |
| Configuration | CLI args | YAML file |
| Networking | Manual | Automatic |
| Use case | Single container | Multi-container |

## Key Points:
- Docker Run: single container.
- Docker Compose: multiple containers.
- Docker Run: CLI arguments.
- Docker Compose: YAML configuration.
- Compose for complex setups.

## Interview Tip:
"Docker Run for single containers; Docker Compose for multi-container apps."

---

## Question 89: How do containers communicate in Docker Compose?

## Answer:
Containers communicate by service name via automatic DNS resolution.

```yaml
services:
  api:
    build: .
  db:
    image: postgres:15
```

```javascript
// In API container
const db = await connect("db:5432"); // "db" resolves to container IP
```

## Key Points:
- Automatic DNS resolution.
- Service name = hostname.
- No manual networking needed.
- Default bridge network.
- Internal communication.

## Interview Tip:
"Use service names as hostnames â€” Docker Compose handles DNS automatically."

---

## Question 90: What Docker Compose best practices do you follow?

## Answer:
1. **Version control**: Commit `docker-compose.yml`.
2. **Environment variables**: Use `.env` file.
3. **Named volumes**: For persistent data.
4. **Health checks**: Ensure services are ready.
5. **depends_on**: Control startup order.
6. **Restart policies**: `restart: unless-stopped`.

## Key Points:
- Version control the YAML.
- `.env` for configuration.
- Named volumes for data.
- Health checks for readiness.
- Restart policies for reliability.

## Interview Tip:
"Version control your `docker-compose.yml` â€” it's your infrastructure as code."

---

## Part 10 (91â€“100): Networking & Storage

---

## Question 91: What is Docker networking?

## Answer:
Docker networking enables communication between containers and between containers and the outside world.

## Key Points:
- Container communication.
- Isolated networks.
- Automatic DNS resolution.
- Port mapping for external access.
- Multiple network types.

## Interview Tip:
"Docker networking is how containers talk to each other and the outside world."

---

## Question 92: What are Docker network types?

## Answer:
1. **Bridge**: Default, isolated network.
2. **Host**: Uses host's network directly.
3. **None**: No networking.
4. **Overlay**: Multi-host networking.
5. **Macvlan**: Assigns MAC addresses.

## Key Points:
- Bridge: default, isolated.
- Host: shares host network.
- None: no networking.
- Overlay: multi-host.
- Macvlan: direct network access.

## Interview Tip:
"Bridge for most cases; host for performance; overlay for multi-host."

---

## Question 93: What is the bridge network?

## Answer:
The default network for containers. Containers on the same bridge can communicate, but are isolated from other networks.

```bash
docker network ls
docker run --network bridge nginx
```

## Key Points:
- Default network.
- Containers can communicate.
- Isolated from other networks.
- Port mapping for external access.
- Automatic DNS.

## Interview Tip:
"Bridge is the default â€” containers on the same bridge communicate automatically."

---

## Question 94: What is the host network?

## Answer:
The container shares the host's network directly â€” no isolation.

```bash
docker run --network host nginx
```

## Key Points:
- Shares host network.
- No port mapping needed.
- No network isolation.
- Better performance.
- Linux only.

## Interview Tip:
"Host network is faster but no isolation â€” use for performance-critical apps."

---

## Question 95: What is the none network?

## Answer:
The container has no network access â€” completely isolated.

```bash
docker run --network none alpine
```

## Key Points:
- No network access.
- Completely isolated.
- Use for security.
- No external communication.
- Uncommon.

## Interview Tip:
"None network for complete isolation â€” useful for security-sensitive containers."

---

## Question 96: How do containers communicate with each other?

## Answer:
1. **Same network**: Automatic DNS resolution.
2. **Port mapping**: Via host ports.
3. **Shared volumes**: File-based communication.
4. **Docker Compose**: Automatic service discovery.

## Key Points:
- Same network = automatic DNS.
- Port mapping for host access.
- Shared volumes for data.
- Compose for service discovery.
- Bridge network by default.

## Interview Tip:
"Containers on the same network communicate by service name â€” Docker handles DNS."

---

## Question 97: What is port mapping?

## Answer:
Port mapping exposes container ports to the host.

```bash
docker run -p 8080:80 nginx
# Host:8080 â†’ Container:80
```

## Key Points:
- `-p host:container`.
- Exposes container ports.
- Multiple ports supported.
- Required for external access.
- `-P` for all exposed ports.

## Interview Tip:
"`-p 8080:80` maps host port 8080 to container port 80."

---

## Question 98: What is a Docker volume?

## Answer:
A volume is persistent storage that exists outside the container lifecycle. Data in volumes survives container removal.

```bash
docker volume create my-data
docker run -v my-data:/app/data nginx
```

## Key Points:
- Persistent storage.
- Survives container removal.
- Managed by Docker.
- Shared between containers.
- Better than bind mounts for production.

## Interview Tip:
"Volumes persist data beyond container lifecycle â€” essential for databases."

---

## Question 99: Why are Docker volumes needed?

## Answer:
Without volumes, data in containers is lost when the container is removed. Volumes provide:
- **Persistence**: Data survives container removal.
- **Sharing**: Multiple containers can share data.
- **Performance**: Faster than bind mounts.
- **Backup**: Easy to backup and restore.

## Key Points:
- Data persistence.
- Container-independent.
- Shared between containers.
- Better performance.
- Easy backup.

## Interview Tip:
"Without volumes, container data is ephemeral â€” volumes make it persistent."

---

## Question 100: What is the difference between volumes and bind mounts?

## Answer:
| Feature | Volumes | Bind Mounts |
|---------|---------|-------------|
| Location | Docker-managed | Host directory |
| Portability | High | Low |
| Performance | Better | Slightly slower |
| Use case | Production | Development |

## Key Points:
- Volumes: Docker-managed, portable.
- Bind mounts: host directory, less portable.
- Volumes for production.
- Bind mounts for development.
- Volumes have better performance.

## Interview Tip:
"Volumes for production; bind mounts for development (live reload)."

---

## Part 11 (101â€“110): Production Docker Management

---

## Question 101: How do you deploy Docker containers to production?

## Answer:
1. **Build optimized images**: Multi-stage, Alpine.
2. **Push to registry**: Docker Hub, AWS ECR.
3. **Deploy with orchestration**: Docker Compose, Kubernetes.
4. **Configure networking**: Load balancer, SSL.
5. **Set up monitoring**: Logs, metrics.
6. **Health checks**: Ensure containers are healthy.

## Key Points:
- Optimized images.
- Push to registry.
- Orchestration.
- Networking and SSL.
- Monitoring.
- Health checks.

## Interview Tip:
"Build, push, deploy, monitor â€” the production Docker workflow."

---

## Question 102: What challenges occur when running Docker in production?

## Answer:
1. **Networking**: Service discovery, load balancing.
2. **Storage**: Persistent data management.
3. **Security**: Image vulnerabilities, secrets.
4. **Monitoring**: Container health, logs.
5. **Scaling**: Auto-scaling containers.
6. **Updates**: Zero-downtime deployments.

## Key Points:
- Networking complexity.
- Storage management.
- Security concerns.
- Monitoring challenges.
- Scaling requirements.
- Update strategies.

## Interview Tip:
"Production Docker challenges: networking, storage, security, monitoring, and scaling."

---

## Question 103: How do you manage Docker containers in production?

## Answer:
1. **Orchestration**: Kubernetes, Docker Swarm.
2. **Health checks**: Automatic restart on failure.
3. **Logging**: Centralized logging.
4. **Monitoring**: Container metrics.
5. **Restart policies**: `restart: unless-stopped`.

## Key Points:
- Orchestration for management.
- Health checks for reliability.
- Centralized logging.
- Container monitoring.
- Restart policies.

## Interview Tip:
"Orchestration + health checks + monitoring = production-ready Docker."

---

## Question 104: What is container orchestration?

## Answer:
Container orchestration automates deployment, scaling, and management of containers. It handles:
- Scheduling containers on hosts.
- Load balancing.
- Health checks.
- Auto-scaling.
- Rolling updates.

## Key Points:
- Automated deployment.
- Scaling management.
- Health monitoring.
- Load balancing.
- Rolling updates.

## Interview Tip:
"Orchestration automates container management at scale â€” it's essential for production."

---

## Question 105: Why is orchestration needed?

## Answer:
- **Scale**: Manage hundreds of containers.
- **Reliability**: Auto-restart failed containers.
- **Load balancing**: Distribute traffic.
- **Updates**: Zero-downtime deployments.
- **Resource management**: Efficient resource usage.

## Key Points:
- Scale management.
- Reliability.
- Load balancing.
- Zero-downtime updates.
- Resource efficiency.

## Interview Tip:
"Orchestration is needed when you have more containers than you can manage manually."

---

## Question 106: What tools are used for container orchestration?

## Answer:
- **Kubernetes**: Industry standard.
- **Docker Swarm**: Simple, Docker-native.
- **Amazon ECS**: AWS-managed.
- **Azure AKS**: Azure-managed.
- **Google GKE**: Google-managed.

## Key Points:
- Kubernetes: industry standard.
- Docker Swarm: simple alternative.
- Cloud-managed: ECS, AKS, GKE.
- Choose based on needs.
- Kubernetes for complex; Swarm for simple.

## Interview Tip:
"Kubernetes is the industry standard; Docker Swarm is simpler but less powerful."

---

## Question 107: What is Kubernetes?

## Answer:
Kubernetes (K8s) is an open-source container orchestration platform that automates deployment, scaling, and management of containerized applications.

## Key Points:
- Container orchestration platform.
- Automated deployment and scaling.
- Self-healing containers.
- Service discovery and load balancing.
- Industry standard.

## Interview Tip:
"Kubernetes is the industry standard for container orchestration â€” it handles scaling, healing, and networking."

---

## Question 108: What is the difference between Docker and Kubernetes?

## Answer:
| Feature | Docker | Kubernetes |
|---------|--------|------------|
| Purpose | Build and run containers | Orchestrate containers |
| Scope | Single host | Multi-host |
| Scaling | Manual | Automatic |
| Complexity | Simple | Complex |

Docker builds and runs; Kubernetes orchestrates at scale.

## Key Points:
- Docker: build and run.
- Kubernetes: orchestrate at scale.
- Docker for development.
- Kubernetes for production.
- They complement each other.

## Interview Tip:
"Docker builds containers; Kubernetes orchestrates them at scale."

---

## Question 109: When should you use Kubernetes?

## Answer:
- **Large scale**: Hundreds of containers.
- **Auto-scaling**: Dynamic resource allocation.
- **Multi-host**: Containers across servers.
- **High availability**: Self-healing, redundancy.
- **Complex deployments**: Canary, blue-green.

## Key Points:
- Large-scale deployments.
- Auto-scaling.
- Multi-host networking.
- High availability.
- Complex deployment strategies.

## Interview Tip:
"Use Kubernetes when you need auto-scaling, multi-host, and high availability."

---

## Question 110: What production Docker best practices do you follow?

## Answer:
1. **Optimized images**: Multi-stage, Alpine.
2. **Non-root user**: Security.
3. **Health checks**: Automatic monitoring.
4. **Resource limits**: CPU and memory.
5. **Restart policies**: `restart: unless-stopped`.
6. **Logging**: Centralized logging.
7. **Secrets management**: Don't hardcode.

## Key Points:
- Optimized images.
- Non-root user.
- Health checks.
- Resource limits.
- Restart policies.
- Logging.
- Secrets management.

## Interview Tip:
"Production Docker = optimized images + non-root + health checks + resource limits."

---

## Part 12 (111â€“120): Container Security

---

## Question 111: How do you secure Docker containers?

## Answer:
1. **Non-root user**: Don't run as root.
2. **Scan images**: Check for vulnerabilities.
3. **Minimal base images**: Alpine, distroless.
4. **No secrets in images**: Use environment variables.
5. **Read-only filesystem**: Prevent modifications.
6. **Resource limits**: Prevent resource exhaustion.

## Key Points:
- Non-root user.
- Image scanning.
- Minimal base images.
- No secrets in images.
- Read-only filesystem.
- Resource limits.

## Interview Tip:
"Non-root user + minimal images + image scanning = secure containers."

---

## Question 112: Why should containers not run as root?

## Answer:
- **Privilege escalation**: Root in container = root on host (potential).
- **Security**: Minimize attack surface.
- **Compliance**: Security policies require non-root.
- **Best practice**: Principle of least privilege.

## Key Points:
- Privilege escalation risk.
- Minimize attack surface.
- Compliance requirements.
- Least privilege principle.
- Use `USER` instruction.

## Interview Tip:
"Running as root is a security risk â€” always use a non-root user."

---

## Question 113: How do you run containers with non-root users?

## Answer:
```dockerfile
FROM node:20-alpine
RUN addgroup -S appgroup && adduser -S appuser -G appgroup
WORKDIR /app
COPY --chown=appuser:appgroup . .
USER appuser
CMD ["node", "server.js"]
```

## Key Points:
- Create user in Dockerfile.
- `COPY --chown` for file ownership.
- `USER` instruction to switch.
- Apply after installing dependencies.
- Test as non-root.

## Interview Tip:
"Create a user, copy files with correct ownership, then switch to that user."

---

## Question 114: What are Docker security risks?

## Answer:
1. **Root containers**: Privilege escalation.
2. **Vulnerable images**: Known CVEs.
3. **Secrets in images**: Exposed credentials.
4. **Unnecessary packages**: Larger attack surface.
5. **Network exposure**: Unprotected ports.

## Key Points:
- Root containers.
- Vulnerable images.
- Exposed secrets.
- Unnecessary packages.
- Network exposure.

## Interview Tip:
"The biggest risks: root containers, vulnerable images, and exposed secrets."

---

## Question 115: How do you scan Docker images for vulnerabilities?

## Answer:
```bash
# Docker Scout
docker scout cves my-image:latest

# Trivy
trivy image my-image:latest

# Snyk
snyk container test my-image:latest
```

## Key Points:
- Docker Scout: built-in.
- Trivy: open-source scanner.
- Snyk: commercial scanner.
- Scan in CI/CD pipeline.
- Fix critical vulnerabilities.

## Interview Tip:
"Scan images in CI/CD â€” don't deploy images with critical vulnerabilities."

---

## Question 116: What are Docker image vulnerabilities?

## Answer:
Vulnerabilities are security flaws in packages within the image:
- Outdated libraries.
- Known CVEs.
- Insecure configurations.
- Exposed secrets.

## Key Points:
- Outdated libraries.
- Known CVEs.
- Insecure configurations.
- Exposed secrets.
- Regular scanning needed.

## Interview Tip:
"Regular image scanning catches vulnerabilities before deployment."

---

## Question 117: How do you keep Docker images secure?

## Answer:
1. **Use official images**: Verified and maintained.
2. **Update regularly**: Patch vulnerabilities.
3. **Scan images**: Automated scanning.
4. **Minimal images**: Fewer packages = fewer vulnerabilities.
5. **Non-root user**: Reduce attack surface.

## Key Points:
- Official images.
- Regular updates.
- Automated scanning.
- Minimal packages.
- Non-root user.

## Interview Tip:
"Official images + regular updates + scanning = secure images."

---

## Question 118: How do you manage secrets in Docker?

## Answer:
1. **Environment variables**: Pass at runtime.
2. **Docker secrets**: Swarm/Kubernetes secrets.
3. **External vaults**: HashiCorp Vault, AWS Secrets Manager.
4. **Never in images**: Don't bake secrets into images.

## Key Points:
- Environment variables.
- Docker secrets.
- External vaults.
- Never in images.
- Rotate regularly.

## Interview Tip:
"Never store secrets in images â€” use environment variables or external vaults."

---

## Question 119: Why should secrets not be stored inside Docker images?

## Answer:
- **Exposure**: Anyone with the image can extract secrets.
- **Version control**: Images are shared and stored.
- **Layers**: Secrets persist in image layers.
- **Security**: Violates least privilege.

## Key Points:
- Anyone can extract secrets.
- Images are shared.
- Secrets persist in layers.
- Security violation.
- Use runtime injection.

## Interview Tip:
"Secrets in images are visible to anyone who pulls the image â€” never do it."

---

## Question 120: What Docker security practices do you follow?

## Answer:
1. **Non-root user**: Always.
2. **Scan images**: In CI/CD.
3. **Minimal base**: Alpine, distroless.
4. **No secrets**: Runtime injection only.
5. **Resource limits**: CPU and memory.
6. **Read-only filesystem**: When possible.

## Key Points:
- Non-root user.
- Image scanning.
- Minimal base.
- No secrets in images.
- Resource limits.
- Read-only filesystem.

## Interview Tip:
"Non-root + scan + minimal + no secrets = secure Docker."

---

## Part 13 (121â€“130): Resource Management & Monitoring

---

## Question 121: How do you limit Docker container resources?

## Answer:
```bash
docker run --cpus="1.5" --memory="512m" nginx
```

```yaml
# Docker Compose
services:
  app:
    deploy:
      resources:
        limits:
          cpus: "1.5"
          memory: 512M
```

## Key Points:
- `--cpus` for CPU limits.
- `--memory` for memory limits.
- Deploy resources in Compose.
- Prevent resource exhaustion.
- Essential for production.

## Interview Tip:
"Always set resource limits in production â€” prevent one container from consuming all resources."

---

## Question 122: What are CPU limits in Docker?

## Answer:
CPU limits control how much CPU a container can use.

```bash
docker run --cpus="1.5" nginx  # Max 1.5 CPU cores
docker run --cpu-shares="512" nginx  # Relative weight
```

## Key Points:
- `--cpus`: absolute limit.
- `--cpu-shares`: relative weight.
- Prevents CPU exhaustion.
- Essential for multi-tenant.
- Default: no limit.

## Interview Tip:
"`--cpus` for hard limits; `--cpu-shares` for relative priority."

---

## Question 123: What are memory limits in Docker?

## Answer:
Memory limits control how much RAM a container can use.

```bash
docker run --memory="512m" nginx
docker run --memory="512m" --memory-swap="1g" nginx
```

## Key Points:
- `--memory`: hard limit.
- `--memory-swap`: total (RAM + swap).
- Prevents memory exhaustion.
- Container killed if exceeded.
- Essential for production.

## Interview Tip:
"Set memory limits to prevent OOM kills from affecting other containers."

---

## Question 124: What happens when a container exceeds memory limits?

## Answer:
The container is killed by the OOM (Out of Memory) killer. The container exits with code 137.

## Key Points:
- Container killed (OOM).
- Exit code 137.
- Other containers unaffected.
- Restart policy can restart it.
- Monitor for OOM kills.

## Interview Tip:
"Exit code 137 = OOM kill â€” increase memory limits or optimize the app."

---

## Question 125: How do you monitor Docker containers?

## Answer:
```bash
docker stats                    # Real-time stats
docker stats container-id       # Specific container
docker inspect container-id     # Detailed info
docker logs container-id        # Container logs
```

## Key Points:
- `docker stats` for real-time metrics.
- `docker inspect` for details.
- `docker logs` for logs.
- External tools for production.
- Monitor CPU, memory, network.

## Interview Tip:
"`docker stats` for quick monitoring; external tools for production."

---

## Question 126: What Docker metrics should you monitor?

## Answer:
- **CPU usage**: Percentage of CPU used.
- **Memory usage**: RAM consumed.
- **Network I/O**: Bytes in/out.
- **Disk I/O**: Read/write operations.
- **Container status**: Running, stopped, restarting.
- **Restart count**: Frequent restarts indicate issues.

## Key Points:
- CPU and memory usage.
- Network and disk I/O.
- Container status.
- Restart count.
- Set up alerts.

## Interview Tip:
"Monitor CPU, memory, and restart count â€” they indicate container health."

---

## Question 127: How do you check container logs?

## Answer:
```bash
docker logs container-id
docker logs -f container-id      # Follow
docker logs --tail 100 container-id  # Last 100 lines
docker logs --since 1h container-id  # Last hour
```

## Key Points:
- `docker logs` for stdout/stderr.
- `-f` to follow.
- `--tail` for recent lines.
- `--since` for time-based.
- Centralized logging for production.

## Interview Tip:
"`docker logs -f` for real-time debugging; centralized logging for production."

---

## Question 128: How do you debug a failing container?

## Answer:
1. **Check logs**: `docker logs container-id`.
2. **Inspect container**: `docker inspect container-id`.
3. **Exec into container**: `docker exec -it container-id sh`.
4. **Check exit code**: `docker ps -a`.
5. **Check events**: `docker events`.

## Key Points:
- Logs for errors.
- Inspect for configuration.
- Exec for shell access.
- Exit code for failure reason.
- Events for lifecycle.

## Interview Tip:
"Start with logs, then inspect, then exec â€” the debugging progression."

---

## Question 129: How do you troubleshoot Docker performance issues?

## Answer:
1. **Check resource usage**: `docker stats`.
2. **Check limits**: Are limits too restrictive?
3. **Check logs**: Application-level issues.
4. **Check networking**: Latency, DNS issues.
5. **Check storage**: Volume performance.

## Key Points:
- Resource stats.
- Resource limits.
- Application logs.
- Network issues.
- Storage performance.

## Interview Tip:
"Start with `docker stats` â€” most performance issues are resource-related."

---

## Question 130: What Docker monitoring tools have you used?

## Answer:
- **Docker stats**: Built-in monitoring.
- **Prometheus + Grafana**: Metrics and dashboards.
- **Datadog**: Full-stack monitoring.
- **cAdvisor**: Container metrics.
- **ELK Stack**: Log aggregation.

## Key Points:
- Docker stats for basic monitoring.
- Prometheus + Grafana for metrics.
- Datadog for full-stack.
- cAdvisor for container metrics.
- ELK for logs.

## Interview Tip:
"Prometheus + Grafana for metrics; ELK for logs â€” the standard monitoring stack."

---

## Part 14 (131â€“140): CI/CD Integration

---

## Question 131: How is Docker used in CI/CD pipelines?

## Answer:
1. **Build**: Build Docker image in CI.
2. **Test**: Run tests in container.
3. **Push**: Push image to registry.
4. **Deploy**: Deploy container to production.

## Key Points:
- Build in CI.
- Test in containers.
- Push to registry.
- Deploy containers.
- Consistent environments.

## Interview Tip:
"Docker ensures CI/CD environments match production â€” no more 'works in CI, fails in production.'"

---

## Question 132: How do you build Docker images automatically?

## Answer:
```yaml
# GitHub Actions
- name: Build and push
  run: |
    docker build -t my-app:${{ github.sha }} .
    docker push my-app:${{ github.sha }}
```

## Key Points:
- Build in CI/CD.
- Tag with commit SHA.
- Push to registry.
- Automated on push.
- Consistent builds.

## Interview Tip:
"Tag images with commit SHA for traceability â€” `my-app:abc123`."

---

## Question 133: How do you push images to Docker Hub or private registries?

## Answer:
```bash
# Docker Hub
docker tag my-app:1.0 username/my-app:1.0
docker push username/my-app:1.0

# AWS ECR
docker tag my-app:1.0 123456789.dkr.ecr.us-east-1.amazonaws.com/my-app:1.0
docker push 123456789.dkr.ecr.us-east-1.amazonaws.com/my-app:1.0
```

## Key Points:
- Tag with registry URL.
- `docker push` to upload.
- Authenticate first.
- Use specific tags.
- Automate in CI/CD.

## Interview Tip:
"Tag, authenticate, push â€” the three steps to publish images."

---

## Question 134: How do you deploy Docker images automatically?

## Answer:
1. **Push triggers webhook**: Registry notifies deployment system.
2. **Pull new image**: Deployment system pulls latest.
3. **Restart containers**: With new image.
4. **Health check**: Verify deployment.

## Key Points:
- Push triggers deployment.
- Pull new image.
- Restart containers.
- Health check.
- Rollback on failure.

## Interview Tip:
"Push â†’ webhook â†’ pull â†’ restart â†’ health check â€” the automated deployment flow."

---

## Question 135: How do GitHub Actions and Docker work together?

## Answer:
```yaml
name: CI/CD
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Build
        run: docker build -t my-app:${{ github.sha }} .
      - name: Push
        run: docker push my-app:${{ github.sha }}
```

## Key Points:
- Build in GitHub Actions.
- Tag with commit SHA.
- Push to registry.
- Deploy on merge to main.
- Secrets for credentials.

## Interview Tip:
"GitHub Actions + Docker = automated CI/CD â€” build, test, push, deploy."

---

## Question 136: How do you handle Docker image versioning?

## Answer:
- **Semantic versioning**: `v1.0.0`, `v1.1.0`.
- **Git SHA**: `my-app:abc123`.
- **Latest**: `my-app:latest` (avoid in production).
- **Environment**: `my-app:staging`, `my-app:production`.

## Key Points:
- Semantic versioning for releases.
- Git SHA for traceability.
- Avoid `latest` in production.
- Environment tags for stages.
- Consistent tagging strategy.

## Interview Tip:
"Use semantic versioning for releases; Git SHA for traceability."

---

## Question 137: What is a Docker image registry?

## Answer:
A registry stores and distributes Docker images. Docker Hub is the default public registry.

## Key Points:
- Stores Docker images.
- Docker Hub: default public.
- Private registries for organizations.
- Push and pull images.
- Version management.

## Interview Tip:
"Docker Hub for public; private registries for proprietary images."

---

## Question 138: How do you rollback Docker deployments?

## Answer:
```bash
# Pull previous version
docker pull my-app:v1.0.0

# Restart with previous version
docker run -d my-app:v1.0.0
```

Or with orchestration tools, rollback is automated.

## Key Points:
- Pull previous version.
- Restart with old image.
- Orchestration tools automate rollback.
- Keep previous versions available.
- Test rollback process.

## Interview Tip:
"Keep previous image versions â€” rollback is just running the old version."

---

## Question 139: What deployment strategies work with Docker?

## Answer:
- **Rolling update**: Gradually replace containers.
- **Blue-green**: Two environments, switch traffic.
- **Canary**: Gradually shift traffic to new version.
- **Recreate**: Stop all, start new.

## Key Points:
- Rolling: gradual replacement.
- Blue-green: two environments.
- Canary: gradual traffic shift.
- Recreate: stop and start.
- Choose based on needs.

## Interview Tip:
"Rolling updates for most cases; blue-green for zero-downtime."

---

## Question 140: What Docker CI/CD best practices do you follow?

## Answer:
1. **Build in CI**: Automated builds.
2. **Scan images**: Security scanning.
3. **Tag with SHA**: Traceability.
4. **Push to registry**: Central storage.
5. **Automate deployment**: Push to deploy.
6. **Health checks**: Verify deployment.
7. **Rollback plan**: Keep previous versions.

## Key Points:
- Automated builds.
- Security scanning.
- SHA tagging.
- Registry storage.
- Automated deployment.
- Health checks.
- Rollback plan.

## Interview Tip:
"Build, scan, tag, push, deploy, verify â€” the CI/CD pipeline."

---

## Part 15 (141â€“150): Senior Real-World Interview Questions

---

## Question 141: Describe the largest Docker-based application you have worked on.

## Answer:
Pick a real project and describe:
- **Scale**: Number of containers, services.
- **Architecture**: Microservices, databases.
- **Challenges**: What was hard and how you solved it.
- **Your role**: What you specifically contributed.
- **Results**: Performance improvements, reliability.

## Key Points:
- Quantify the scale.
- Describe the architecture.
- Highlight challenges and solutions.
- Explain your contributions.
- Show impact.

## Interview Tip:
"Tell a story with a beginning (problem), middle (solution), and end (result)."

---

## Question 142: What was the most difficult Docker issue you solved?

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

## Question 143: How do you debug a container that keeps crashing?

## Answer:
1. **Check logs**: `docker logs container-id`.
2. **Check exit code**: `docker ps -a`.
3. **Inspect container**: `docker inspect container-id`.
4. **Exec into container**: `docker exec -it container-id sh`.
5. **Check resources**: `docker stats`.
6. **Check events**: `docker events`.

## Key Points:
- Logs for errors.
- Exit code for failure reason.
- Inspect for configuration.
- Exec for shell access.
- Stats for resource issues.
- Events for lifecycle.

## Interview Tip:
"Exit code 137 = OOM; exit code 1 = application error â€” check the exit code first."

---

## Question 144: How would you Dockerize a Next.js + Node.js + PostgreSQL application?

## Answer:
```yaml
services:
  frontend:
    build: ./frontend
    ports:
      - "3000:3000"
  backend:
    build: ./backend
    ports:
      - "4000:4000"
    environment:
      DATABASE_URL: postgres://user:pass@db:5432/mydb
  db:
    image: postgres:15
    volumes:
      - db-data:/var/lib/postgresql/data
    environment:
      POSTGRES_PASSWORD: secret

volumes:
  db-data:
```

## Key Points:
- Separate services for frontend, backend, database.
- Multi-stage builds for frontend and backend.
- Named volumes for database.
- Environment variables for configuration.
- Health checks for all services.

## Interview Tip:
"One service per container â€” frontend, backend, database as separate services."

---

## Question 145: How would you design a Docker architecture for a SaaS application?

## Answer:
- **Load balancer**: Nginx or Traefik.
- **API servers**: Multiple Node.js containers.
- **Database**: PostgreSQL with volumes.
- **Cache**: Redis container.
- **Background jobs**: Worker containers.
- **Monitoring**: Prometheus + Grafana.

## Key Points:
- Load balancer for distribution.
- Multiple API servers for scaling.
- Database with persistent storage.
- Redis for caching.
- Workers for background jobs.
- Monitoring for observability.

## Interview Tip:
"Load balancer + multiple API servers + database + cache + workers â€” the SaaS architecture."

---

## Question 146: How would you optimize Docker builds in a large team?

## Answer:
1. **Build cache**: Use BuildKit cache.
2. **Multi-stage builds**: Parallel stages.
3. **`.dockerignore`**: Smaller context.
4. **Base image registry**: Mirror frequently used images.
5. **CI cache**: Cache layers in CI.

## Key Points:
- BuildKit for caching.
- Multi-stage for parallelism.
- `.dockerignore` for smaller context.
- Image registry mirroring.
- CI layer caching.

## Interview Tip:
"BuildKit caching + `.dockerignore` + CI caching = fast team builds."

---

## Question 147: How do you manage Docker images across development, staging, and production?

## Answer:
- **Development**: Local builds, docker-compose.
- **Staging**: CI-built images, staging registry.
- **Production**: Tested images, production registry.
- **Tagging**: Semantic versioning + environment tags.

## Key Points:
- Local builds for dev.
- CI builds for staging/production.
- Separate registries per environment.
- Consistent tagging strategy.
- Same image across environments.

## Interview Tip:
"Build once, deploy everywhere â€” same image across staging and production."

---

## Question 148: What Docker mistakes do junior developers commonly make?

## Answer:
1. **Running as root**: Security risk.
2. **Using `latest` tag**: Unpredictable.
3. **No `.dockerignore`**: Large build context.
4. **Secrets in images**: Security exposure.
5. **No resource limits**: Resource exhaustion.
6. **No health checks**: Unreliable deployments.
7. **Single-stage builds**: Large images.

## Key Points:
- Running as root.
- Using `latest` tag.
- No `.dockerignore`.
- Secrets in images.
- No resource limits.
- No health checks.
- Single-stage builds.

## Interview Tip:
"The biggest mistake is running as root â€” always use a non-root user."

---

## Question 149: What Docker features do you use most frequently in production?

## Answer:
- **Multi-stage builds**: For optimized images.
- **Docker Compose**: For multi-container apps.
- **Volumes**: For persistent data.
- **Networks**: For container communication.
- **Health checks**: For reliability.
- **Resource limits**: For stability.

## Key Points:
- Multi-stage builds.
- Docker Compose.
- Volumes for data.
- Networks for communication.
- Health checks.
- Resource limits.

## Interview Tip:
"Multi-stage builds, volumes, health checks, and resource limits â€” the production essentials."

---

## Question 150: In your opinion, what separates a junior, mid-level, and senior Docker user?

## Answer:
- **Junior**: Knows basic commands (run, ps, logs). Can containerize simple apps.
- **Mid-level**: Understands Dockerfile optimization, Compose, networking. Can build production-ready images.
- **Senior**: Designs container architecture, handles orchestration, manages security and monitoring. Can debug any container issue.

The biggest differentiator: a senior understands production concerns â€” security, monitoring, and scalability.

## Key Points:
- Junior: basic commands, simple containerization.
- Mid-level: optimization, Compose, networking.
- Senior: architecture, orchestration, security, monitoring.
- Senior thinks about production from day one.
- Senior can debug any container issue.

## Interview Tip:
"The best answer shows self-awareness. Pick your level and explain what you're doing to grow."

---

# End of Docker Interview Questions & Answers
