# Git & GitHub Interview Questions (150 Total)

---

# Git Fundamentals

1. What is Git?
2. Why was Git created?
3. What problems does Git solve?
4. What are the advantages of Git?
5. What is the difference between Git and GitHub?
6. What is a version control system?
7. What are centralized and distributed version control systems?
8. Why is Git called a distributed version control system?
9. What happens when you initialize a Git repository?
10. What is the `.git` folder?

---

# Basic Git Concepts

11. What is a repository in Git?
12. What is the working directory?
13. What is the staging area?
14. What is a commit?
15. What information does a commit contain?
16. What is a commit hash?
17. What is HEAD in Git?
18. What is a branch?
19. What is the default branch?
20. What is the difference between local and remote repositories?

---

# Basic Commands

21. What does `git init` do?
22. What does `git clone` do?
23. What does `git status` show?
24. What does `git add` do?
25. What is the difference between `git add .` and `git add -A`?
26. What does `git commit` do?
27. What does `git push` do?
28. What does `git pull` do?
29. What does `git fetch` do?
30. What is the difference between `git pull` and `git fetch`?

---

# Commit Management

31. What makes a good Git commit message?
32. What is a conventional commit?
33. What is the difference between `git commit` and `git commit --amend`?
34. How do you change the last commit message?
35. How do you undo the last commit?
36. What is `git revert`?
37. What is `git reset`?
38. What is the difference between reset and revert?
39. What are the types of `git reset`?
40. When should you use revert instead of reset?

---

# Remote Repository

41. What is a Git remote?
42. What is origin in Git?
43. How do you add a remote repository?
44. How do you remove a remote repository?
45. How do you check remote URLs?
46. What is upstream tracking?
47. How do you connect a local branch to a remote branch?
48. How do you rename a branch?
49. How do you delete a branch?
50. What Git workflow do you follow in your projects?

---

# Branching

51. What is a Git branch?
52. Why are branches useful?
53. How does Git store branches?
54. How do you create a new branch?
55. How do you switch branches?
56. What is the difference between `git checkout` and `git switch`?
57. How do you create and switch to a branch in one command?
58. How do you list all branches?
59. How do you delete a branch?
60. What branching strategy do you follow?

---

# Merge

61. What is Git merge?
62. How does Git merge work?
63. What is a fast-forward merge?
64. What is a three-way merge?
65. What happens during a merge conflict?
66. How do you resolve merge conflicts?
67. How do you abort a merge?
68. What causes frequent merge conflicts?
69. How do you prevent merge conflicts in a team?
70. What are merge best practices?

---

# Rebase

71. What is Git rebase?
72. How does rebase differ from merge?
73. When should you use rebase?
74. When should you avoid rebase?
75. What is interactive rebase?
76. What does `git rebase -i` do?
77. How do you squash commits?
78. What is rewriting Git history?
79. Why is rebasing shared branches dangerous?
80. What Git history management practices do you follow?

---

# Stashing & Temporary Changes

81. What is Git stash?
82. Why would you use Git stash?
83. How do you create a stash?
84. How do you view stash history?
85. How do you apply a stash?
86. How do you remove a stash?
87. What is the difference between `git stash apply` and `git stash pop`?
88. How do you stash specific files?
89. When should you use stash?
90. What are alternatives to using stash?

---

# Collaboration & GitHub Workflow

91. What is a Pull Request (PR)?
92. Why are pull requests important?
93. What happens during code review?
94. What is a fork in GitHub?
95. What is the difference between clone and fork?
96. What is GitHub Flow?
97. What is Git Flow?
98. What branching strategy is best for teams?
99. How do you handle code reviews?
100. What GitHub collaboration best practices do you follow?

---

# Git Internals

101. How does Git work internally?
102. What are Git objects?
103. What are the four types of Git objects?
104. What is a blob object?
105. What is a tree object?
106. What is a commit object?
107. What is a tag object?
108. How does Git store file changes?
109. Why is Git fast compared to other version control systems?
110. What is the Git object database?

---

# Git History & Recovery

111. How do you view Git history?
112. What does `git log` do?
113. What is `git log --oneline`?
114. What is `git diff`?
115. How do you compare two commits?
116. How do you find who changed a specific line?
117. What is `git blame`?
118. How do you find a bug introduced in a commit?
119. What is `git bisect`?
120. How do you recover deleted commits?

---

# Tags & Releases

121. What is a Git tag?
122. Why are Git tags used?
123. What is the difference between lightweight and annotated tags?
124. How do you create a tag?
125. How do you push tags to GitHub?
126. How do you delete a tag?
127. What is semantic versioning?
128. How do Git tags relate to releases?
129. How do you manage production releases using Git?
130. What release management practices do you follow?

---

# Git Hooks & Automation

131. What are Git hooks?
132. What are client-side Git hooks?
133. What are server-side Git hooks?
134. What is a pre-commit hook?
135. What is a pre-push hook?
136. How do you automate code checks with Git hooks?
137. What tools are commonly used with Git hooks?
138. What are Husky and lint-staged?
139. How do Git hooks improve code quality?
140. What Git automation practices do you follow?

---

# GitHub Actions & Senior Workflow

141. What is GitHub Actions?
142. How does GitHub Actions work?
143. What are workflows in GitHub Actions?
144. What are jobs and steps?
145. How do you run tests automatically on every push?
146. How do you deploy applications using GitHub Actions?
147. How do you manage secrets in GitHub Actions?
148. How do you handle large-scale Git workflows in a team?
149. What Git mistakes do junior developers commonly make?
150. In your opinion, what separates a junior, mid-level, and senior Git user?

---

# ANSWERS


---

## Part 1 (1â€“10): Git Fundamentals

---

## Question 1: What is Git?

## Answer:
Git is a distributed version control system (DVCS) that tracks changes in source code over time. It allows multiple developers to work on the same project simultaneously, maintain a complete history of changes, and collaborate efficiently.

Created by Linus Torvalds in 2005 for Linux kernel development, Git is now the most widely used version control system in the world.

## Key Points:
- Distributed version control system.
- Tracks changes in source code.
- Allows parallel development.
- Maintains complete history.
- Created by Linus Torvalds in 2005.

## Interview Tip:
"Git is distributed â€” every developer has a full copy of the repository, including history."

---

## Question 2: Why was Git created?

## Answer:
Git was created in 2005 by Linus Torvalds because the Linux kernel community lost access to BitKeeper (a proprietary VCS). He needed a system that was:
- **Fast**: Handle large projects like the Linux kernel.
- **Distributed**: No central server dependency.
- **Non-linear**: Support thousands of parallel branches.
- **Efficient**: Handle millions of commits.

## Key Points:
- Created for Linux kernel development.
- Needed a fast, distributed system.
- BitKeeper license revoked.
- Designed for large-scale projects.
- Non-linear development support.

## Interview Tip:
"Git was born out of necessity â€” the Linux kernel needed a fast, distributed VCS."

---

## Question 3: What problems does Git solve?

## Answer:
1. **Version tracking**: Track every change to code.
2. **Collaboration**: Multiple developers work simultaneously.
3. **History**: Maintain complete change history.
4. **Branching**: Work on features without affecting main code.
5. **Backup**: Distributed copies across developers.
6. **Rollback**: Undo changes to any point in history.
7. **Conflict resolution**: Handle simultaneous changes.

## Key Points:
- Version tracking.
- Parallel collaboration.
- Complete history.
- Safe branching.
- Distributed backup.
- Easy rollback.
- Conflict resolution.

## Interview Tip:
"Git solves the fundamental problem of coordinating multiple developers working on the same codebase."

---

## Question 4: What are the advantages of Git?

## Answer:
- **Distributed**: Every clone is a full backup.
- **Fast**: Local operations are lightning fast.
- **Branching**: Cheap, instant branches.
- **Merging**: Powerful merge algorithms.
- **Staging area**: Review before committing.
- **History**: Complete audit trail.
- **Open source**: Free and actively maintained.

## Key Points:
- Distributed architecture.
- Fast local operations.
- Cheap branching.
- Powerful merging.
- Staging area.
- Complete history.
- Open source.

## Interview Tip:
"Git's biggest advantage is that it's distributed â€” every clone is a full repository with complete history."

---

## Question 5: What is the difference between Git and GitHub?

## Answer:
| Feature | Git | GitHub |
|---------|-----|--------|
| Type | Version control system | Hosting platform |
| Location | Local machine | Cloud (web) |
| Purpose | Track code changes | Collaborate, share, host repos |
| Features | Branching, merging, history | PRs, issues, actions, reviews |
| Usage | Command line / GUI | Web interface / API |

Git is the tool; GitHub is the platform. Git works without GitHub; GitHub uses Git.

## Key Points:
- Git: local version control.
- GitHub: cloud hosting platform.
- Git tracks changes; GitHub enables collaboration.
- Git works independently; GitHub uses Git.
- Alternatives: GitLab, Bitbucket.

## Interview Tip:
"Git is the engine; GitHub is the garage. You can have Git without GitHub, but not the other way around."

---

## Question 6: What is a version control system?

## Answer:
A version control system (VCS) records changes to files over time so you can recall specific versions later. It tracks who made what change and when, enabling collaboration and history.

## Key Points:
- Records changes over time.
- Tracks who, what, and when.
- Enables collaboration.
- Maintains history.
- Allows rollback.

## Interview Tip:
"A VCS is a time machine for your code â€” you can go back to any point in history."

---

## Question 7: What are centralized and distributed version control systems?

## Answer:
- **Centralized (CVCS)**: Single central server stores all versions. Clients check out files from the server. Examples: SVN, CVS.
- **Distributed (DVCS)**: Every client has a full copy of the repository. No central server dependency. Examples: Git, Mercurial.

## Key Points:
- CVCS: single central server.
- DVCS: every client has full copy.
- CVCS: single point of failure.
- DVCS: works offline.
- Git is distributed.

## Interview Tip:
"Distributed means every clone is a full repository â€” no single point of failure."

---

## Question 8: Why is Git called a distributed version control system?

## Answer:
Because every developer has a complete copy of the repository, including the full history. There's no single central server â€” each clone is a full repository.

This means:
- You can work offline.
- You have a full backup.
- You can commit locally before pushing.
- No single point of failure.

## Key Points:
- Every clone is a full repository.
- Full history in every copy.
- Works offline.
- No single point of failure.
- Multiple backups.

## Interview Tip:
"Distributed means every clone is a full repository â€” you can work offline and have a complete backup."

---

## Question 9: What happens when you initialize a Git repository?

## Answer:
Running `git init` creates a `.git` directory in the current folder. This directory contains all the metadata and object database for the repository.

```bash
git init
# Creates: .git/ folder
```

## Key Points:
- Creates `.git` directory.
- Initializes empty repository.
- Tracks all changes from this point.
- `.git` contains all repository data.
- Run once per project.

## Interview Tip:
"`git init` creates the `.git` folder â€” that's where Git stores everything."

---

## Question 10: What is the `.git` folder?

## Answer:
The `.git` folder contains all Git metadata and the object database:
- **objects/**: All content (blobs, trees, commits).
- **refs/**: Branch and tag references.
- **HEAD**: Points to current branch.
- **config**: Repository configuration.
- **hooks/**: Git hook scripts.

## Key Points:
- Contains all Git data.
- `objects/` for content.
- `refs/` for branches and tags.
- `HEAD` for current branch.
- `config` for settings.
- `hooks/` for automation.

## Interview Tip:
"The `.git` folder IS the repository â€” delete it and you lose all Git history."

---

## Part 2 (11â€“20): Basic Git Concepts

---

## Question 11: What is a repository in Git?

## Answer:
A repository (repo) is a directory that contains your project files and the `.git` folder with all version history. It can be local (on your machine) or remote (on GitHub).

## Key Points:
- Contains project files and `.git` folder.
- Tracks all changes and history.
- Can be local or remote.
- Created with `git init` or `git clone`.

## Interview Tip:
"A repository is your project plus its entire history â€” stored in the `.git` folder."

---

## Question 12: What is the working directory?

## Answer:
The working directory is the directory where your project files live. It's the current state of files on your filesystem. Changes in the working directory are either staged or unstaged.

```
Working Directory â†’ Staging Area â†’ Repository
```

## Key Points:
- Current state of files on disk.
- Where you edit files.
- Changes are tracked or untracked.
- Files can be staged from here.

## Interview Tip:
"The working directory is where you edit files â€” it's your current workspace."

---

## Question 13: What is the staging area?

## Answer:
The staging area (index) is an intermediate area where you prepare changes before committing. You explicitly add changes to the staging area with `git add`.

```
Working Directory â†’ Staging Area â†’ Repository
                   (git add)      (git commit)
```

## Key Points:
- Intermediate area before commit.
- `git add` adds changes to staging.
- Review changes before committing.
- Partial commits possible.
- Also called the "index."

## Interview Tip:
"The staging area lets you review and organize changes before committing â€” it's like a draft."

---

## Question 14: What is a commit?

## Answer:
A commit is a snapshot of your staged changes at a specific point in time. It records what changed, who changed it, and when.

```bash
git commit -m "Add user authentication"
```

## Key Points:
- Snapshot of staged changes.
- Records author, timestamp, and message.
- Immutable once created.
- Linked to parent commit(s).
- Forms the project history.

## Interview Tip:
"A commit is a snapshot â€” it captures the state of your code at a specific moment."

---

## Question 15: What information does a commit contain?

## Answer:
- **Hash**: Unique SHA-1 identifier.
- **Author**: Who made the commit.
- **Timestamp**: When the commit was made.
- **Message**: Description of changes.
- **Parent**: Reference to previous commit(s).
- **Tree**: Snapshot of the file structure.

## Key Points:
- SHA-1 hash for identification.
- Author and timestamp.
- Commit message.
- Parent commit reference.
- Tree object for file snapshot.

## Interview Tip:
"A commit contains who, when, what, and why â€” plus a reference to the previous commit."

---

## Question 16: What is a commit hash?

## Answer:
A commit hash is a unique 40-character SHA-1 identifier for each commit. It's generated from the commit's content, author, timestamp, and parent.

```
commit 7a8b9c0d1e2f3a4b5c6d7e8f9a0b1c2d3e4f5a6b
```

You can use short hashes (first 7+ characters) for convenience.

## Key Points:
- 40-character SHA-1 hash.
- Unique identifier for each commit.
- Generated from commit content.
- Short hashes (7+ chars) work too.
- Used for referencing commits.

## Interview Tip:
"The commit hash is the unique ID â€” use the short version (7+ characters) for convenience."

---

## Question 17: What is HEAD in Git?

## Answer:
HEAD is a pointer to the current branch reference, which in turn points to the latest commit on that branch.

```bash
git log --oneline -1
# HEAD -> main -> commit abc123
```

When you make a commit, HEAD moves forward. When you checkout a different branch, HEAD moves to that branch.

## Key Points:
- Pointer to current branch.
- Points to latest commit on current branch.
- Moves with commits and checkouts.
- Can be "detached" (pointing directly to a commit).
- Central to understanding Git state.

## Interview Tip:
"HEAD is 'where you are' in Git â€” it points to the current branch's latest commit."

---

## Question 18: What is a branch?

## Answer:
A branch is a lightweight, movable pointer to a commit. It allows you to work on features or fixes without affecting the main code.

```bash
git branch feature-login
# Creates a new branch pointing to current commit
```

## Key Points:
- Pointer to a commit.
- Enables parallel development.
- Cheap to create and delete.
- Independent line of development.
- Default branch is usually `main`.

## Interview Tip:
"A branch is just a pointer to a commit â€” creating one is instant and cheap."

---

## Question 19: What is the default branch?

## Answer:
The default branch is the primary branch in a repository. Traditionally called `master`, it's now commonly `main` (GitHub default since 2020).

It's the branch that:
- Is created when you initialize a repo.
- Is the base for pull requests.
- Represents production-ready code.

## Key Points:
- Primary branch in the repository.
- Usually `main` (previously `master`).
- Created on `git init`.
- Base for PRs and deployments.
- Represents production code.

## Interview Tip:
"The default branch (`main`) is the source of truth â€” it should always be deployable."

---

## Question 20: What is the difference between local and remote repositories?

## Answer:
- **Local**: On your machine. You work directly with it.
- **Remote**: On a server (GitHub, GitLab). You push/pull to/from it.

```
Local Repository â†” Remote Repository
  (git commit)      (git push/pull)
```

## Key Points:
- Local: your machine.
- Remote: server (GitHub, GitLab).
- Work locally, share via remote.
- `git push` uploads to remote.
- `git pull` downloads from remote.

## Interview Tip:
"Work locally, share remotely â€” push when ready, pull to stay updated."

---

## Part 3 (21â€“30): Basic Commands

---

## Question 21: What does `git init` do?

## Answer:
`git init` creates a new Git repository in the current directory by adding a `.git` folder.

```bash
git init
# Creates .git/ directory
```

Run it once per project to start tracking changes.

## Key Points:
- Creates a new repository.
- Adds `.git` folder.
- Run once per project.
- Can initialize existing projects.
- `git init --bare` for server repos.

## Interview Tip:
"`git init` is the first command â€” it creates the repository."

---

## Question 22: What does `git clone` do?

## Answer:
`git clone` creates a local copy of a remote repository, including all history and branches.

```bash
git clone https://github.com/user/repo.git
```

## Key Points:
- Copies remote repository locally.
- Includes all history and branches.
- Sets up remote tracking.
- Creates a new directory.
- `origin` remote is set automatically.

## Interview Tip:
"`git clone` downloads the entire repository â€” history, branches, and all."

---

## Question 23: What does `git status` show?

## Answer:
`git status` shows the current state of the working directory and staging area:
- Untracked files (new).
- Modified files (changed).
- Staged files (ready to commit).
- Branch information.

## Key Points:
- Shows working directory state.
- Lists untracked, modified, staged files.
- Shows current branch.
- Most frequently used command.
- Run before every commit.

## Interview Tip:
"`git status` is your best friend â€” run it constantly to understand the current state."

---

## Question 24: What does `git add` do?

## Answer:
`git add` adds changes from the working directory to the staging area.

```bash
git add file.js      # Add specific file
git add .            # Add all changes
git add *.js         # Add all JS files
```

## Key Points:
- Moves changes to staging area.
- Prepares for commit.
- Can add specific files or all.
- `git add .` adds all changes.
- Review with `git status` before adding.

## Interview Tip:
"`git add` prepares changes for commit â€” use it to organize what goes into each commit."

---

## Question 25: What is the difference between `git add .` and `git add -A`?

## Answer:
- **`git add .`**: Adds all changes in the current directory and subdirectories.
- **`git add -A`**: Adds all changes in the entire repository (including deleted files).

In practice, they're similar, but `-A` is more comprehensive.

## Key Points:
- `git add .`: current directory and below.
- `git add -A`: entire repository.
- Both stage new, modified, and deleted files.
- `-A` includes deleted files from anywhere.
- Use `-A` for completeness.

## Interview Tip:
"`git add -A` is safer â€” it catches everything including deletions."

---

## Question 26: What does `git commit` do?

## Answer:
`git commit` saves staged changes to the repository as a new commit.

```bash
git commit -m "Add user authentication"
```

Creates a snapshot of the staged changes with a message.

## Key Points:
- Saves staged changes.
- Creates a new commit.
- Requires a message (`-m`).
- Only commits staged changes.
- Triggers pre-commit hooks.

## Interview Tip:
"Commit often with clear messages â€” each commit should represent one logical change."

---

## Question 27: What does `git push` do?

## Answer:
`git push` uploads local commits to a remote repository.

```bash
git push origin main
# Pushes main branch to origin remote
```

## Key Points:
- Uploads commits to remote.
- Updates remote branch.
- Requires remote access (authentication).
- Fails if remote has newer commits.
- `git push -u` sets upstream tracking.

## Interview Tip:
"`git push` shares your work â€” push regularly to backup and collaborate."

---

## Question 28: What does `git pull` do?

## Answer:
`git pull` fetches changes from a remote repository and merges them into the current branch.

```bash
git pull origin main
```

It's equivalent to `git fetch` + `git merge`.

## Key Points:
- Fetches and merges remote changes.
- Equivalent to `fetch` + `merge`.
- Updates local branch.
- May cause merge conflicts.
- Use `--rebase` for cleaner history.

## Interview Tip:
"`git pull` is `fetch + merge` â€” use `pull --rebase` for a cleaner history."

---

## Question 29: What does `git fetch` do?

## Answer:
`git fetch` downloads changes from a remote repository without merging them into your working branch.

```bash
git fetch origin
```

You can then review changes before merging.

## Key Points:
- Downloads remote changes.
- Doesn't merge into working branch.
- Safe way to check for updates.
- Use before merging or rebasing.
- Updates remote tracking branches.

## Interview Tip:
"`git fetch` is safe â€” it downloads changes without modifying your work."

---

## Question 30: What is the difference between `git pull` and `git fetch`?

## Answer:
| Feature | git fetch | git pull |
|---------|-----------|----------|
| Downloads | Yes | Yes |
| Merges | No | Yes |
| Safe | Yes | May cause conflicts |
| Use case | Review before merge | Quick update |

`fetch` = download only. `pull` = download + merge.

## Key Points:
- `fetch`: download only, safe.
- `pull`: download + merge, may conflict.
- `fetch` for review; `pull` for quick updates.
- `pull --rebase` for cleaner history.

## Interview Tip:
"`fetch` to review; `pull` to update. Know the difference."

---

## Part 4 (31â€“40): Commit Management

---

## Question 31: What makes a good Git commit message?

## Answer:
A good commit message:
- **Subject line**: Short (50 chars), imperative mood ("Add feature" not "Added feature").
- **Body**: Explain what and why, not how.
- **Reference**: Link to issue/ticket if applicable.

```
Add user authentication

- Implement JWT-based authentication
- Add login and register endpoints
- Include password hashing with bcrypt

Closes #123
```

## Key Points:
- Short subject (50 chars).
- Imperative mood.
- Explain what and why.
- Reference issues.
- Separate subject from body with blank line.

## Interview Tip:
"Write commit messages for your future self â€” explain WHY, not WHAT."

---

## Question 32: What is a conventional commit?

## Answer:
Conventional commits use a standardized format:

```
<type>(<scope>): <description>

feat(auth): add JWT authentication
fix(api): handle null user response
docs(readme): update installation steps
refactor(utils): simplify date formatting
```

Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`.

## Key Points:
- Standardized commit format.
- `<type>(<scope>): <description>`.
- Enables automated changelogs.
- Enables semantic versioning.
- Used with tools like commitlint.

## Interview Tip:
"Conventional commits enable automated changelogs and semantic versioning."

---

## Question 33: What is the difference between `git commit` and `git commit --amend`?

## Answer:
- **`git commit`**: Creates a new commit.
- **`git commit --amend`**: Modifies the last commit (message or content).

```bash
git commit -m "Add feature"
git commit --amend -m "Add feature with tests"
# Modifies the last commit
```

## Key Points:
- `commit`: new commit.
- `--amend`: modifies last commit.
- Changes commit hash.
- Don't amend pushed commits.
- Use for quick fixes.

## Interview Tip:
"`--amend` modifies the last commit â€” use it before pushing, never after."

---

## Question 34: How do you change the last commit message?

## Answer:
```bash
git commit --amend -m "New commit message"
```

This changes the message of the most recent commit. The commit hash changes.

## Key Points:
- `--amend -m` changes last message.
- Changes commit hash.
- Only works on last commit.
- Don't amend pushed commits.
- Use `--no-edit` to keep message.

## Interview Tip:
"`git commit --amend -m` changes the last commit message â€” safe if not pushed."

---

## Question 35: How do you undo the last commit?

## Answer:
```bash
# Keep changes staged
git reset --soft HEAD~1

# Keep changes unstaged
git reset --mixed HEAD~1

# Discard changes completely
git reset --hard HEAD~1
```

`HEAD~1` means "one commit before HEAD."

## Key Points:
- `--soft`: keeps changes staged.
- `--mixed`: keeps changes unstaged.
- `--hard`: discards changes.
- `HEAD~1` = previous commit.
- Use with caution (`--hard` is destructive).

## Interview Tip:
"`git reset --soft HEAD~1` undoes the commit but keeps changes staged â€” safest option."

---

## Question 36: What is `git revert`?

## Answer:
`git revert` creates a new commit that undoes the changes of a specified commit. It doesn't modify history â€” it adds a new commit.

```bash
git revert abc123
# Creates a new commit that undoes abc123
```

## Key Points:
- Creates a new commit.
- Undoes changes of specified commit.
- Doesn't modify history.
- Safe for shared branches.
- Preserves the original commit.

## Interview Tip:
"`git revert` is safe for shared branches â€” it adds a new commit instead of modifying history."

---

## Question 37: What is `git reset`?

## Answer:
`git reset` moves HEAD to a specified commit, optionally modifying the staging area and working directory.

```bash
git reset --soft HEAD~1   # Keep changes staged
git reset --mixed HEAD~1  # Keep changes unstaged
git reset --hard HEAD~1   # Discard changes
```

## Key Points:
- Moves HEAD to specified commit.
- Three modes: soft, mixed, hard.
- Modifies history.
- Dangerous for shared branches.
- Use with caution.

## Interview Tip:
"`git reset` modifies history â€” never use on shared branches unless you know what you're doing."

---

## Question 38: What is the difference between reset and revert?

## Answer:
| Feature | reset | revert |
|---------|-------|--------|
| History | Modifies | Preserves |
| New commit | No | Yes |
| Safe for sharing | No | Yes |
| Use case | Local cleanup | Undo shared commits |

## Key Points:
- `reset`: modifies history, dangerous.
- `revert`: preserves history, safe.
- Use `reset` for local cleanup.
- Use `revert` for shared branches.

## Interview Tip:
"`revert` for shared branches; `reset` for local cleanup. Never `reset` pushed commits."

---

## Question 39: What are the types of `git reset`?

## Answer:
- **`--soft`**: Moves HEAD, keeps changes staged.
- **`--mixed`**: Moves HEAD, keeps changes unstaged (default).
- **`--hard`**: Moves HEAD, discards all changes.

## Key Points:
- `--soft`: changes stay staged.
- `--mixed`: changes stay unstaged.
- `--hard`: changes are lost.
- Default is `--mixed`.
- `--hard` is destructive.

## Interview Tip:
"`--soft` for staged changes, `--mixed` for unstaged, `--hard` to discard everything."

---

## Question 40: When should you use revert instead of reset?

## Answer:
Use `revert` when:
- The commit has been pushed to a shared branch.
- You want to preserve history.
- You need to undo a specific commit (not the latest).

Use `reset` when:
- The commit is local only.
- You want to clean up before pushing.
- You need to restructure commits.

## Key Points:
- `revert` for shared branches.
- `reset` for local cleanup.
- `revert` preserves history.
- `reset` modifies history.
- Choose based on whether commits are shared.

## Interview Tip:
"If the commit is pushed, use `revert`. If it's local, use `reset`."

---

## Part 5 (41â€“50): Remote Repository

---

## Question 41: What is a Git remote?

## Answer:
A remote is a version of your repository hosted on a server (GitHub, GitLab). You can have multiple remotes.

```bash
git remote -v
# origin  https://github.com/user/repo.git (fetch)
# origin  https://github.com/user/repo.git (push)
```

## Key Points:
- Server-hosted repository.
- Usually GitHub, GitLab, or Bitbucket.
- Can have multiple remotes.
- `origin` is the default remote.
- Push/pull to/from remotes.

## Interview Tip:
"A remote is a server-hosted copy of your repository â€” `origin` is the default."

---

## Question 42: What is origin in Git?

## Answer:
`origin` is the default name for the remote repository you cloned from. It's a convention, not a special keyword.

```bash
git remote -v
# origin  https://github.com/user/repo.git
```

## Key Points:
- Default remote name.
- Convention, not required.
- Set automatically on `git clone`.
- Can be renamed or removed.
- Most projects use `origin`.

## Interview Tip:
"`origin` is just a name â€” it's the convention for the primary remote."

---

## Question 43: How do you add a remote repository?

## Answer:
```bash
git remote add origin https://github.com/user/repo.git
```

Adds a new remote named `origin` pointing to the URL.

## Key Points:
- `git remote add <name> <url>`.
- `origin` is the conventional name.
- Multiple remotes allowed.
- Use HTTPS or SSH URLs.
- Verify with `git remote -v`.

## Interview Tip:
"`git remote add origin <url>` connects your local repo to GitHub."

---

## Question 44: How do you remove a remote repository?

## Answer:
```bash
git remote remove origin
```

Removes the remote named `origin`.

## Key Points:
- `git remote remove <name>`.
- Removes remote tracking.
- Doesn't affect local repository.
- Verify with `git remote -v`.

## Interview Tip:
"`git remote remove` disconnects from the remote â€” local repo is unaffected."

---

## Question 45: How do you check remote URLs?

## Answer:
```bash
git remote -v
# origin  https://github.com/user/repo.git (fetch)
# origin  https://github.com/user/repo.git (push)
```

Shows all remotes with their URLs.

## Key Points:
- `git remote -v` shows URLs.
- Shows fetch and push URLs.
- Verify remote configuration.
- Check before pushing.

## Interview Tip:
"`git remote -v` is the quick way to check where your repo is connected."

---

## Question 46: What is upstream tracking?

## Answer:
Uptracking connects a local branch to a remote branch, so `git push` and `git pull` know where to go.

```bash
git push -u origin main
# Sets upstream tracking for main â†’ origin/main
```

After setting upstream, you can just `git push` without specifying the remote.

## Key Points:
- Connects local to remote branch.
- `-u` flag sets upstream.
- Enables `git push` and `git pull` without arguments.
- Configured per branch.
- Verify with `git branch -vv`.

## Interview Tip:
"`git push -u origin main` sets upstream â€” then you can just `git push`."

---

## Question 47: How do you connect a local branch to a remote branch?

## Answer:
```bash
git branch --set-upstream-to=origin/main main
```

Or when pushing for the first time:
```bash
git push -u origin main
```

## Key Points:
- `--set-upstream-to` connects branches.
- `-u` flag on push sets upstream.
- Enables simplified push/pull.
- Per-branch configuration.

## Interview Tip:
"Use `-u` when pushing for the first time â€” it sets upstream tracking."

---

## Question 48: How do you rename a branch?

## Answer:
```bash
git branch -m old-name new-name

# Rename current branch
git branch -m new-name
```

## Key Points:
- `git branch -m <old> <new>`.
- `-m` for rename.
- Updates local branch name.
- Remote branch needs separate rename.

## Interview Tip:
"`git branch -m` renames the local branch â€” update remote separately if needed."

---

## Question 49: How do you delete a branch?

## Answer:
```bash
# Delete local branch
git branch -d branch-name

# Force delete local branch
git branch -D branch-name

# Delete remote branch
git push origin --delete branch-name
```

## Key Points:
- `-d` for safe delete (merged only).
- `-D` for force delete.
- `--delete` on push for remote.
- Cannot delete current branch.
- Clean up after merging.

## Interview Tip:
"`-d` for safe delete; `-D` for force. Clean up branches after merging."

---

## Question 50: What Git workflow do you follow in your projects?

## Answer:
I follow a simplified Git Flow:
1. **`main`**: Production-ready code.
2. **`develop`**: Integration branch.
3. **Feature branches**: `feature/xxx` for new features.
4. **Release branches**: `release/v1.0` for releases.
5. **Hotfix branches**: `hotfix/xxx` for urgent fixes.

For smaller teams, GitHub Flow is simpler: `main` + feature branches + PRs.

## Key Points:
- `main` for production.
- Feature branches for development.
- PRs for code review.
- Merge to `main` when ready.
- Adapt based on team size.

## Interview Tip:
"Adapt the workflow to the team â€” Git Flow for large teams, GitHub Flow for small teams."

---

## Part 6 (51â€“60): Branching

---

## Question 51: What is a Git branch?

## Answer:
A branch is a lightweight, movable pointer to a commit. It enables parallel development without affecting the main code.

```bash
git branch feature-login
```

## Key Points:
- Pointer to a commit.
- Enables parallel development.
- Cheap to create and delete.
- Independent line of development.
- Default branch is `main`.

## Interview Tip:
"A branch is just a pointer â€” creating one is instant and cheap."

---

## Question 52: Why are branches useful?

## Answer:
- **Isolation**: Work on features without affecting main code.
- **Parallel development**: Multiple developers work simultaneously.
- **Experimentation**: Try ideas safely.
- **Code review**: Review before merging.
- **Release management**: Manage releases separately.

## Key Points:
- Isolation from main code.
- Parallel development.
- Safe experimentation.
- Code review workflow.
- Release management.

## Interview Tip:
"Branches enable safe, parallel development â€” every feature gets its own branch."

---

## Question 53: How does Git store branches?

## Answer:
Branches are stored as files in `.git/refs/heads/`. Each file contains the commit hash the branch points to.

```
.git/refs/heads/main â†’ abc123
.git/refs/heads/feature â†’ def456
```

## Key Points:
- Stored as files in `.git/refs/heads/`.
- Each file contains a commit hash.
- Lightweight (just a pointer).
- Updated on new commits.
- Remote branches in `.git/refs/remotes/`.

## Interview Tip:
"Branches are just files containing commit hashes â€” that's why they're so lightweight."

---

## Question 54: How do you create a new branch?

## Answer:
```bash
git branch feature-login
```

Creates a new branch pointing to the current commit.

## Key Points:
- `git branch <name>` creates a branch.
- Points to current commit.
- Doesn't switch to it.
- Use `-b` to create and switch.
- Convention: lowercase with hyphens.

## Interview Tip:
"`git branch` creates; `git switch` switches. Use `git switch -c` to do both."

---

## Question 55: How do you switch branches?

## Answer:
```bash
git switch feature-login
# or
git checkout feature-login
```

Moves HEAD to the specified branch and updates the working directory.

## Key Points:
- `git switch <branch>` (modern).
- `git checkout <branch>` (legacy).
- Updates working directory.
- Must commit or stash changes first.
- HEAD moves to new branch.

## Interview Tip:
"`git switch` is the modern way â€” `git checkout` is legacy but still works."

---

## Question 56: What is the difference between `git checkout` and `git switch`?

## Answer:
- **`git checkout`**: Does many things (switch branches, restore files, create branches).
- **`git switch`**: Only switches branches (clearer intent).

```bash
git switch feature       # Switch branch
git switch -c feature    # Create and switch
```

`git switch` was introduced to clarify intent.

## Key Points:
- `checkout`: overloaded (branches, files, detach).
- `switch`: only branch operations.
- `switch` is clearer and safer.
- Both work for branch switching.
- Use `switch` for modern workflows.

## Interview Tip:
"`git switch` is clearer â€” it only does branch operations."

---

## Question 57: How do you create and switch to a branch in one command?

## Answer:
```bash
git switch -c feature-login
# or
git checkout -b feature-login
```

Creates the branch and switches to it.

## Key Points:
- `git switch -c <name>` (modern).
- `git checkout -b <name>` (legacy).
- Creates and switches in one step.
- Most common way to create branches.

## Interview Tip:
"`git switch -c` is the one-step way to create and switch."

---

## Question 58: How do you list all branches?

## Answer:
```bash
git branch            # Local branches
git branch -r         # Remote branches
git branch -a         # All branches (local + remote)
```

The current branch is marked with `*`.

## Key Points:
- `git branch`: local branches.
- `-r`: remote branches.
- `-a`: all branches.
- `*` marks current branch.
- `-vv` shows upstream tracking.

## Interview Tip:
"`git branch -a` shows everything â€” local and remote branches."

---

## Question 59: How do you delete a branch?

## Answer:
```bash
git branch -d feature-login    # Safe delete (merged only)
git branch -D feature-login    # Force delete
git push origin --delete feature-login  # Delete remote
```

## Key Points:
- `-d`: safe delete (merged only).
- `-D`: force delete.
- `--delete` on push for remote.
- Cannot delete current branch.
- Clean up after merging.

## Interview Tip:
"`-d` for safe delete; `-D` for force. Clean up after merging."

---

## Question 60: What branching strategy do you follow?

## Answer:
- **Feature branches**: `feature/xxx` for new features.
- **Bug fixes**: `fix/xxx` for bug fixes.
- **Releases**: `release/v1.0` for releases.
- **Hotfixes**: `hotfix/xxx` for urgent fixes.
- **Main branch**: Always deployable.

Naming convention: `type/description` (e.g., `feature/user-auth`).

## Key Points:
- Feature branches for development.
- Main branch for production.
- Naming conventions for clarity.
- Delete after merging.
- Keep main always deployable.

## Interview Tip:
"Consistent naming and deletion â€” `feature/`, `fix/`, `release/`, `hotfix/`."

---

## Part 7 (61â€“70): Merge

---

## Question 61: What is Git merge?

## Answer:
Git merge combines changes from one branch into another.

```bash
git switch main
git merge feature-login
```

## Key Points:
- Combines changes from one branch to another.
- Creates a merge commit (usually).
- Preserves branch history.
- May cause conflicts.
- Fast-forward when possible.

## Interview Tip:
"Merge combines branches â€” it preserves the history of both branches."

---

## Question 62: How does Git merge work?

## Answer:
Git merge finds the common ancestor, compares changes, and combines them. If both branches modified the same lines, a conflict occurs.

## Key Points:
- Finds common ancestor.
- Compares changes from both branches.
- Combines non-conflicting changes.
- Reports conflicts for resolution.
- Creates merge commit.

## Interview Tip:
"Merge finds the common ancestor and combines changes â€” conflicts occur when both modify the same lines."

---

## Question 63: What is a fast-forward merge?

## Answer:
A fast-forward merge happens when the target branch has no new commits since the source branched. Git simply moves the pointer forward.

```
Before: main â†’ A â† B â† C (feature)
After:  main â†’ A â†’ B â†’ C
```

No merge commit is created.

## Key Points:
- No new commits on target branch.
- Git moves pointer forward.
- No merge commit created.
- Linear history.
- Happens when possible by default.

## Interview Tip:
"Fast-forward merge is just moving the pointer â€” no merge commit needed."

---

## Question 64: What is a three-way merge?

## Answer:
A three-way merge combines changes from two branches that have diverged. Git uses three commits: the common ancestor, and the tips of both branches.

```
main:    A â†’ B â†’ C
feature: A â†’ D â†’ E
Result:  A â†’ B â†’ C â†’ D â†’ E â†’ M (merge commit)
```

## Key Points:
- Branches have diverged.
- Uses common ancestor + both tips.
- Creates a merge commit.
- Preserves both histories.
- Default when branches diverge.

## Interview Tip:
"Three-way merge creates a merge commit â€” it preserves both branch histories."

---

## Question 65: What happens during a merge conflict?

## Answer:
A merge conflict occurs when both branches modify the same lines. Git marks the conflicting sections:

```
<<<<<<< HEAD
Changes from current branch
=======
Changes from incoming branch
>>>>>>> feature-branch
```

You must manually resolve the conflict.

## Key Points:
- Both branches modify same lines.
- Git marks conflicts with `<<<<<<<`, `=======`, `>>>>>>>`.
- Manual resolution required.
- Edit the file, then `git add` and `git commit`.
- Common in team environments.

## Interview Tip:
"Conflicts happen when both branches modify the same lines â€” resolve manually."

---

## Question 66: How do you resolve merge conflicts?

## Answer:
1. Open the conflicting file.
2. Find conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`).
3. Choose or combine changes.
4. Remove conflict markers.
5. `git add <file>`.
6. `git commit` (creates merge commit).

## Key Points:
- Edit the file manually.
- Remove conflict markers.
- Choose or combine changes.
- `git add` the resolved file.
- `git commit` to complete merge.

## Interview Tip:
"Resolve conflicts by editing the file, removing markers, and committing."

---

## Question 67: How do you abort a merge?

## Answer:
```bash
git merge --abort
```

Aborts the merge and returns to the state before the merge started.

## Key Points:
- `git merge --abort` cancels the merge.
- Returns to pre-merge state.
- Use when conflicts are too complex.
- Safe operation.

## Interview Tip:
"`git merge --abort` is your escape hatch â€” it cancels the merge."

---

## Question 68: What causes frequent merge conflicts?

## Answer:
- **Long-lived branches**: Large divergence over time.
- **Same files modified**: Multiple developers editing same files.
- **Infrequent merging**: Not merging main regularly.
- **Large PRs**: Too many changes at once.
- **Poor file organization**: Too much in one file.

## Key Points:
- Long-lived branches.
- Same file modifications.
- Infrequent merging.
- Large PRs.
- Poor file organization.

## Interview Tip:
"Merge frequently and keep PRs small â€” that's how you prevent conflicts."

---

## Question 69: How do you prevent merge conflicts in a team?

## Answer:
1. **Merge frequently**: Pull from main regularly.
2. **Small PRs**: Smaller changes, fewer conflicts.
3. **Communicate**: Talk about who's working on what.
4. **Modular code**: Separate concerns into different files.
5. **Feature flags**: Avoid touching the same code.

## Key Points:
- Merge frequently.
- Small PRs.
- Communicate with team.
- Modular code structure.
- Feature flags.

## Interview Tip:
"Merge frequently, communicate, and keep PRs small â€” that prevents most conflicts."

---

## Question 70: What are merge best practices?

## Answer:
1. **Pull before merging**: Get latest changes.
2. **Test after merging**: Verify nothing broke.
3. **Resolve conflicts carefully**: Don't rush.
4. **Use merge commits**: Preserve history.
5. **Clean up branches**: Delete after merging.

## Key Points:
- Pull before merging.
- Test after merging.
- Careful conflict resolution.
- Merge commits for history.
- Clean up branches.

## Interview Tip:
"Pull, merge, test, clean up â€” the merge best practice cycle."

---

## Part 8 (71â€“80): Rebase

---

## Question 71: What is Git rebase?

## Answer:
Git rebase moves or reapplies commits from one branch onto another. It creates a linear history by replaying commits.

```bash
git switch feature
git rebase main
```

## Key Points:
- Moves commits to a new base.
- Creates linear history.
- No merge commit.
- Rewrites commit history.
- Cleaner than merge for some workflows.

## Interview Tip:
"Rebase creates linear history â€” it's cleaner but rewrites commits."

---

## Question 72: How does rebase differ from merge?

## Answer:
| Feature | Merge | Rebase |
|---------|-------|--------|
| History | Preserves branch history | Linear history |
| Merge commit | Yes | No |
| Rewrites history | No | Yes |
| Safe for sharing | Yes | No |
| Use case | Shared branches | Local cleanup |

## Key Points:
- Merge: preserves history, merge commit.
- Rebase: linear history, no merge commit.
- Rebase rewrites history.
- Rebase is not safe for shared branches.
- Use rebase for local cleanup.

## Interview Tip:
"Merge preserves history; rebase linearizes it. Use rebase only on local branches."

---

## Question 73: When should you use rebase?

## Answer:
- **Before merging**: Clean up local commits before merge.
- **Keeping branches updated**: Rebase feature branch on main.
- **Linear history preference**: When you want clean history.
- **Local branches only**: Never rebase shared branches.

## Key Points:
- Before merging to main.
- Updating feature branches.
- Linear history preference.
- Local branches only.

## Interview Tip:
"Rebase before merging to main â€” it creates a clean, linear history."

---

## Question 74: When should you avoid rebase?

## Answer:
- **Shared branches**: Never rebase branches others are working on.
- **Public history**: Don't rebase commits that have been pushed.
- **Complex conflicts**: Merge is easier for complex conflicts.
- **Team policy**: Some teams prefer merge commits.

## Key Points:
- Never rebase shared branches.
- Don't rebase pushed commits.
- Merge for complex conflicts.
- Follow team conventions.

## Interview Tip:
"The golden rule: never rebase commits that exist on someone else's machine."

---

## Question 75: What is interactive rebase?

## Answer:
Interactive rebase lets you modify commits: reorder, squash, edit, or delete them.

```bash
git rebase -i HEAD~3
# Opens editor with last 3 commits
```

## Key Points:
- Modify commits interactively.
- Reorder, squash, edit, delete.
- `-i` flag for interactive mode.
- Powerful history rewriting tool.
- Use before pushing.

## Interview Tip:
"Interactive rebase is the power tool â€” squash, reorder, and clean up commits."

---

## Question 76: What does `git rebase -i` do?

## Answer:
Opens an interactive editor where you can choose actions for each commit:

```
pick abc123 Add feature
pick def456 Fix bug
pick ghi789 Add tests
```

Actions: `pick`, `squash`, `edit`, `reword`, `drop`.

## Key Points:
- Opens interactive editor.
- Choose action per commit.
- `pick`, `squash`, `edit`, `reword`, `drop`.
- Modify history before pushing.
- Powerful cleanup tool.

## Interview Tip:
"`pick`, `squash`, `reword`, `drop` â€” the interactive rebase actions."

---

## Question 77: How do you squash commits?

## Answer:
```bash
git rebase -i HEAD~3
# Change "pick" to "squash" for commits to squash
pick abc123 First commit
squash def456 Second commit  # Squashed into first
squash ghi789 Third commit   # Squashed into first
```

## Key Points:
- Use interactive rebase.
- Change `pick` to `squash`.
- Combines multiple commits into one.
- Edit commit message.
- Use before pushing.

## Interview Tip:
"Squash commits before merging to main â€” it creates a cleaner history."

---

## Question 78: What is rewriting Git history?

## Answer:
Rewriting history changes existing commits â€” their content, order, or messages. Operations that rewrite history:
- `git commit --amend`
- `git rebase`
- `git reset`

## Key Points:
- Changes existing commits.
- Creates new commit hashes.
- Dangerous for shared branches.
- Safe for local branches.
- Use before pushing.

## Interview Tip:
"Rewriting history is powerful but dangerous â€” only do it on local branches."

---

## Question 79: Why is rebasing shared branches dangerous?

## Answer:
Rebasing rewrites commit hashes. If others have the old commits, they'll have conflicts when they pull. This creates duplicate commits and confusion.

## Key Points:
- Rewrites commit hashes.
- Creates conflicts for collaborators.
- Duplicate commits.
- Confusion and lost work.
- Never rebase shared branches.

## Interview Tip:
"The golden rule: never rebase commits that exist on someone else's machine."

---

## Question 80: What Git history management practices do you follow?

## Answer:
1. **Rebase before merging**: Clean up local commits.
2. **Squash related commits**: Combine related changes.
3. **Clear commit messages**: Every commit should be meaningful.
4. **Linear history preferred**: Easier to read and debug.
5. **Merge commits for shared branches**: Preserve history.

## Key Points:
- Rebase for local cleanup.
- Squash related commits.
- Clear messages.
- Linear history preferred.
- Merge for shared branches.

## Interview Tip:
"Rebase locally, merge for shared branches â€” that's the best of both worlds."

---

## Part 9 (81â€“90): Stashing & Temporary Changes

---

## Question 81: What is Git stash?

## Answer:
Git stash temporarily saves uncommitted changes so you can switch branches or work on something else.

```bash
git stash
# Saves changes, reverts to clean state
```

## Key Points:
- Temporarily saves changes.
- Reverts to clean state.
- Stack-based (multiple stashes).
- Use before switching branches.
- Restore with `stash pop` or `stash apply`.

## Interview Tip:
"Stash is a temporary storage â€” save your work without committing."

---

## Question 82: Why would you use Git stash?

## Answer:
- **Switch branches**: Save work before switching.
- **Pull latest**: Stash changes before pulling.
- **Quick fix**: Save work to fix something urgent.
- **Clean working directory**: Start fresh temporarily.

## Key Points:
- Save work before switching branches.
- Stash before pulling.
- Quick fixes.
- Clean working directory temporarily.

## Interview Tip:
"Stash when you need to switch context but aren't ready to commit."

---

## Question 83: How do you create a stash?

## Answer:
```bash
git stash                    # Stash all changes
git stash push -m "message"  # Stash with message
git stash -u                 # Include untracked files
```

## Key Points:
- `git stash` for basic stash.
- `-m` for descriptive message.
- `-u` includes untracked files.
- Stack-based storage.

## Interview Tip:
"Always add a message with `-m` â€” it helps you remember what each stash contains."

---

## Question 84: How do you view stash history?

## Answer:
```bash
git stash list
# stash@{0}: WIP on main: abc123 Add feature
# stash@{1}: WIP on main: def456 Fix bug
```

## Key Points:
- `git stash list` shows all stashes.
- Stack-based (newest first).
- Descriptive messages help.
- `stash@{0}` is the most recent.

## Interview Tip:
"`git stash list` shows your stash stack â€” use descriptive messages."

---

## Question 85: How do you apply a stash?

## Answer:
```bash
git stash apply         # Apply most recent (keep stash)
git stash pop           # Apply most recent (remove stash)
git stash apply stash@{1}  # Apply specific stash
```

## Key Points:
- `apply` keeps the stash.
- `pop` removes the stash.
- Specify stash with `stash@{n}`.
- Apply specific stash.

## Interview Tip:
"`pop` for one-time use; `apply` when you want to keep the stash."

---

## Question 86: How do you remove a stash?

## Answer:
```bash
git stash drop stash@{0}   # Remove specific stash
git stash clear             # Remove all stashes
```

## Key Points:
- `drop` removes specific stash.
- `clear` removes all stashes.
- Use after applying.
- Keep stash list clean.

## Interview Tip:
"Clean up stashes regularly â€” don't let them pile up."

---

## Question 87: What is the difference between `git stash apply` and `git stash pop`?

## Answer:
- **`apply`**: Applies stash, keeps it in the list.
- **`pop`**: Applies stash, removes it from the list.

## Key Points:
- `apply`: keeps stash.
- `pop`: removes stash.
- `pop` for one-time use.
- `apply` for reusing stash.

## Interview Tip:
"`pop` for one-time use; `apply` when you might need it again."

---

## Question 88: How do you stash specific files?

## Answer:
```bash
git stash push -m "message" -- file1.js file2.js
git stash push -m "message" -- src/*.js
```

## Key Points:
- Specify files after `--`.
- Stash only specific changes.
- Useful for partial stashing.
- More granular control.

## Interview Tip:
"Stash specific files with `git stash push -- file.js`."

---

## Question 89: When should you use stash?

## Answer:
- **Context switching**: Save work before switching branches.
- **Pulling updates**: Stash before pulling.
- **Quick fixes**: Save work for urgent fixes.
- **Clean slate**: Start fresh temporarily.

## Key Points:
- Context switching.
- Before pulling.
- Quick fixes.
- Temporary clean state.

## Interview Tip:
"Stash for temporary storage â€” commit when you're ready."

---

## Question 90: What are alternatives to using stash?

## Answer:
1. **Commit**: Make a WIP commit, reset later.
2. **Worktree**: Separate working directory for another branch.
3. **New branch**: Commit to a new branch.
4. **WIP commits**: `git commit -m "WIP"`.

## Key Points:
- WIP commit for temporary work.
- Worktree for parallel work.
- New branch for isolated work.
- Each has trade-offs.

## Interview Tip:
"WIP commits are simpler than stash â€” just reset later."

---

## Part 10 (91â€“100): Collaboration & GitHub Workflow

---

## Question 91: What is a Pull Request (PR)?

## Answer:
A Pull Request is a request to merge changes from one branch into another. It's the primary way to propose changes and request code review on GitHub.

## Key Points:
- Request to merge branches.
- Primary collaboration mechanism.
- Enables code review.
- Discussion and feedback.
- Merge when approved.

## Interview Tip:
"PRs are the heart of GitHub collaboration â€” they enable code review and discussion."

---

## Question 92: Why are pull requests important?

## Answer:
- **Code review**: Others review your code before merging.
- **Discussion**: Questions and feedback on changes.
- **Quality gate**: Tests and checks must pass.
- **Documentation**: PR description explains changes.
- **History**: Record of why changes were made.

## Key Points:
- Code review.
- Discussion and feedback.
- Quality gates (CI/CD).
- Documentation.
- Historical record.

## Interview Tip:
"PRs ensure quality â€” code review, tests, and discussion before merging."

---

## Question 93: What happens during code review?

## Answer:
1. **Reviewer reads code**: Understands changes and context.
2. **Feedback**: Comments on improvements or issues.
3. **Discussion**: Back-and-forth on approach.
4. **Approval**: Reviewer approves the PR.
5. **Merge**: PR is merged into the target branch.

## Key Points:
- Read and understand changes.
- Provide feedback.
- Discuss approach.
- Approve when satisfied.
- Merge after approval.

## Interview Tip:
"Code review is about quality and knowledge sharing â€” be constructive in feedback."

---

## Question 94: What is a fork in GitHub?

## Answer:
A fork is a personal copy of someone else's repository. It allows you to make changes without affecting the original.

## Key Points:
- Personal copy of a repository.
- Independent from original.
- Make changes freely.
- Create PRs to contribute back.
- Common in open source.

## Interview Tip:
"Forks are for contributing to open source â€” make changes in your fork, then create a PR."

---

## Question 95: What is the difference between clone and fork?

## Answer:
| Feature | Clone | Fork |
|---------|-------|------|
| Location | Local copy | GitHub copy |
| Ownership | Same repo | Your copy |
| Purpose | Local development | Contribution |
| Updates | Pull from original | Sync with original |

## Key Points:
- Clone: local copy, same repo.
- Fork: GitHub copy, your ownership.
- Clone for development; fork for contribution.
- Forks need manual syncing.

## Interview Tip:
"Clone for local work; fork for contributing to others' repositories."

---

## Question 96: What is GitHub Flow?

## Answer:
GitHub Flow is a simple workflow:
1. Create a branch from `main`.
2. Make changes and commit.
3. Open a Pull Request.
4. Review and discuss.
5. Merge into `main`.
6. Deploy.

## Key Points:
- Simple workflow.
- `main` + feature branches.
- PRs for code review.
- Deploy from `main`.
- Great for small teams.

## Interview Tip:
"GitHub Flow is simple: branch, commit, PR, review, merge, deploy."

---

## Question 97: What is Git Flow?

## Answer:
Git Flow is a branching model with multiple branch types:
- **`main`**: Production code.
- **`develop`**: Integration branch.
- **`feature/*`**: New features.
- **`release/*`**: Release preparation.
- **`hotfix/*`**: Urgent fixes.

## Key Points:
- Multiple branch types.
- `main` for production.
- `develop` for integration.
- Feature, release, hotfix branches.
- More complex than GitHub Flow.

## Interview Tip:
"Git Flow for complex release cycles; GitHub Flow for simple deployments."

---

## Question 98: What branching strategy is best for teams?

## Answer:
- **Small teams, continuous deployment**: GitHub Flow.
- **Large teams, scheduled releases**: Git Flow.
- **Open source**: Fork + PR.
- **Monorepos**: Trunk-based development.

Choose based on team size, release cadence, and complexity.

## Key Points:
- GitHub Flow for small teams.
- Git Flow for large teams.
- Fork + PR for open source.
- Trunk-based for monorepos.

## Interview Tip:
"Choose based on team size and release cadence â€” simpler is usually better."

---

## Question 99: How do you handle code reviews?

## Answer:
1. **Review promptly**: Don't block teammates.
2. **Be constructive**: Suggest improvements, not just criticism.
3. **Focus on important things**: Architecture, logic, security.
4. **Approve when satisfied**: Don't nitpick endlessly.
5. **Learn from feedback**: Apply lessons to future code.

## Key Points:
- Review promptly.
- Constructive feedback.
- Focus on important issues.
- Approve when ready.
- Learn from reviews.

## Interview Tip:
"Good code reviews are about quality and learning â€” be constructive and timely."

---

## Question 100: What GitHub collaboration best practices do you follow?

## Answer:
1. **PR templates**: Standardize PR descriptions.
2. **Code owners**: Assign reviewers automatically.
3. **Branch protection**: Require reviews and CI passing.
4. **Issue templates**: Standardize bug reports.
5. **Labels**: Organize issues and PRs.
6. **Milestones**: Track progress toward goals.

## Key Points:
- PR templates for consistency.
- Code owners for automatic review.
- Branch protection for quality.
- Issue templates for bug reports.
- Labels and milestones for organization.

## Interview Tip:
"Templates, protection rules, and automation â€” they make collaboration smoother."

---

## Part 11 (101â€“110): Git Internals

---

## Question 101: How does Git work internally?

## Answer:
Git stores content as objects in `.git/objects/`. Each object is identified by its SHA-1 hash. Git uses four object types: blobs, trees, commits, and tags.

## Key Points:
- Content-addressable storage.
- SHA-1 hashes for identification.
- Four object types.
- Snapshots, not diffs.
- Local operations are fast.

## Interview Tip:
"Git stores snapshots, not diffs â€” that's why it's fast."

---

## Question 102: What are Git objects?

## Answer:
Git objects are the fundamental data structures stored in `.git/objects/`. Each object has a type, content, and SHA-1 hash.

## Key Points:
- Stored in `.git/objects/`.
- Identified by SHA-1 hash.
- Four types: blob, tree, commit, tag.
- Immutable once created.
- Content-addressable.

## Interview Tip:
"Everything in Git is an object â€” blobs, trees, commits, and tags."

---

## Question 103: What are the four types of Git objects?

## Answer:
1. **Blob**: File content.
2. **Tree**: Directory structure (maps names to blobs/trees).
3. **Commit**: Snapshot with metadata (author, message, parent).
4. **Tag**: Named reference to a commit.

## Key Points:
- Blob: file content.
- Tree: directory structure.
- Commit: snapshot + metadata.
- Tag: named reference.
- All identified by SHA-1.

## Interview Tip:
"Blob for files, tree for directories, commit for snapshots, tag for labels."

---

## Question 104: What is a blob object?

## Answer:
A blob stores the content of a file. It doesn't contain the filename â€” that's stored in the tree object.

## Key Points:
- Stores file content.
- No filename (that's in the tree).
- Content-addressable.
- Same content = same blob (shared).
- Binary storage.

## Interview Tip:
"Blobs store content; trees store names. Together they represent files."

---

## Question 105: What is a tree object?

## Answer:
A tree maps filenames to blobs and other trees. It represents the directory structure at a point in time.

## Key Points:
- Maps names to blobs/trees.
- Represents directory structure.
- Points to blobs (files) and trees (subdirectories).
- Recursive structure.
- Part of commit snapshot.

## Interview Tip:
"Trees are directories â€” they map filenames to blobs and other trees."

---

## Question 106: What is a commit object?

## Answer:
A commit stores a snapshot of the project at a point in time, with metadata:
- Author and timestamp.
- Commit message.
- Parent commit(s).
- Tree (root directory snapshot).

## Key Points:
- Snapshot of project.
- Author, timestamp, message.
- Parent commit reference.
- Tree reference.
- Immutable once created.

## Interview Tip:
"A commit is a snapshot plus metadata â€” it points to a tree and its parent commit."

---

## Question 107: What is a tag object?

## Answer:
A tag is a named reference to a specific commit, typically used for releases.

- **Lightweight tag**: Just a pointer to a commit.
- **Annotated tag**: Full object with metadata (tagger, message).

## Key Points:
- Named reference to a commit.
- Lightweight: just a pointer.
- Annotated: full object with metadata.
- Used for releases.
- `v1.0.0`, `v2.0.0` naming convention.

## Interview Tip:
"Annotated tags for releases; lightweight tags for quick labels."

---

## Question 108: How does Git store file changes?

## Answer:
Git stores complete snapshots (not diffs). Each commit stores the entire file tree. Unchanged files are referenced by the same blob hash.

## Key Points:
- Complete snapshots, not diffs.
- Unchanged files share blobs.
- Efficient storage via compression.
- Fast checkout (no reconstruction).
- Content-addressable storage.

## Interview Tip:
"Git stores snapshots, not diffs â€” unchanged files are shared, not duplicated."

---

## Question 109: Why is Git fast compared to other version control systems?

## Answer:
- **Local operations**: Most operations are local (no server round-trips).
- **Snapshots**: No need to reconstruct files from diffs.
- **Compression**: Objects are compressed with zlib.
- **Hash-based**: Fast lookups via SHA-1.

## Key Points:
- Local operations.
- Snapshots, not diffs.
- Compressed objects.
- Hash-based lookups.
- No server dependency for most operations.

## Interview Tip:
"Git is fast because it's local â€” most operations don't need a server."

---

## Question 110: What is the Git object database?

## Answer:
The object database stores all Git objects in `.git/objects/`. Objects are stored as files named by their SHA-1 hash.

```
.git/objects/ab/cdef1234567890...
```

## Key Points:
- Stores all Git objects.
- File-based storage.
- Named by SHA-1 hash.
- Compressed with zlib.
- Content-addressable.

## Interview Tip:
"The object database is Git's storage â€” everything lives in `.git/objects/`."

---

## Part 12 (111â€“120): Git History & Recovery

---

## Question 111: How do you view Git history?

## Answer:
```bash
git log                    # Full history
git log --oneline          # Compact
git log --graph            # Visual graph
git log -n 5               # Last 5 commits
git log --author="Alice"   # By author
```

## Key Points:
- `git log` for full history.
- `--oneline` for compact view.
- `--graph` for visual branches.
- `-n` for limiting results.
- `--author` for filtering.

## Interview Tip:
"`git log --oneline --graph` gives you a clean, visual history."

---

## Question 112: What does `git log` do?

## Answer:
`git log` shows the commit history of the current branch, including author, date, and message.

## Key Points:
- Shows commit history.
- Author, date, message.
- Many formatting options.
- Filter by author, date, etc.
- Most used history command.

## Interview Tip:
"`git log` is the history browser â€” learn its options for efficient debugging."

---

## Question 113: What is `git log --oneline`?

## Answer:
Shows each commit on one line with abbreviated hash and message.

```bash
git log --oneline
# abc123 Add feature
# def456 Fix bug
# ghi789 Initial commit
```

## Key Points:
- One line per commit.
- Abbreviated hash.
- First line of message only.
- Compact and readable.
- Most common log format.

## Interview Tip:
"`git log --oneline` is the most useful format â€” compact and readable."

---

## Question 114: What is `git diff`?

## Answer:
`git diff` shows differences between:
- Working directory and staging area.
- Staging area and last commit.
- Two commits.

```bash
git diff              # Working vs staging
git diff --staged     # Staging vs last commit
git diff main..feature  # Between branches
```

## Key Points:
- Shows differences.
- Working vs staging.
- Staging vs commit.
- Between commits or branches.
- Essential for code review.

## Interview Tip:
"`git diff --staged` shows what you're about to commit â€” always check before committing."

---

## Question 115: How do you compare two commits?

## Answer:
```bash
git diff abc123..def456      # Between two commits
git diff abc123..HEAD        # Between commit and HEAD
git diff main..feature       # Between branches
```

## Key Points:
- `git diff <commit1>..<commit2>`.
- Shows all differences.
- Works with branches too.
- Useful for code review.

## Interview Tip:
"`git diff main..feature` shows everything that changed in the feature branch."

---

## Question 116: How do you find who changed a specific line?

## Answer:
```bash
git blame file.js
```

Shows the author and commit for each line in a file.

## Key Points:
- Shows author per line.
- Shows commit hash per line.
- Useful for finding who changed what.
- Helps with debugging.
- Can filter by date or range.

## Interview Tip:
"`git blame` is your detective tool â€” find who changed a specific line and why."

---

## Question 117: What is `git blame`?

## Answer:
`git blame` annotates each line of a file with the commit hash, author, and date of the last change.

```bash
git blame file.js
# abc123 (Alice 2024-01-15) function login() {
```

## Key Points:
- Annotates lines with commit info.
- Shows author, hash, date.
- Helps find who changed what.
- Useful for debugging.
- Can filter by range.

## Interview Tip:
"`git blame` answers 'who wrote this and when' â€” essential for debugging."

---

## Question 118: How do you find a bug introduced in a commit?

## Answer:
Use `git bisect` to binary search through commits:

```bash
git bisect start
git bisect bad          # Current commit has bug
git bisect good abc123  # This commit was fine
# Git checks out a middle commit
# Test it, then mark as good or bad
# Repeat until found
```

## Key Points:
- Binary search through commits.
- Mark commits as good or bad.
- Efficiently finds the problematic commit.
- Can automate with scripts.
- Powerful debugging tool.

## Interview Tip:
"`git bisect` is the bug-finding power tool â€” binary search through commit history."

---

## Question 119: What is `git bisect`?

## Answer:
`git bisect` uses binary search to find the commit that introduced a bug. You mark commits as "good" or "bad," and Git narrows down the culprit.

## Key Points:
- Binary search through history.
- Mark good/bad commits.
- Efficiently finds bug source.
- Can be automated.
- Powerful for debugging.

## Interview Tip:
"`git bisect` finds the exact commit that introduced a bug â€” it's incredibly efficient."

---

## Question 120: How do you recover deleted commits?

## Answer:
```bash
git reflog
# Shows all HEAD movements
# Find the commit hash
git checkout abc123
# or
git branch recovery-branch abc123
```

`git reflog` shows all HEAD movements, including deleted commits.

## Key Points:
- `git reflog` shows all HEAD movements.
- Find deleted commit hash.
- Create a branch from it.
- Commits aren't truly deleted immediately.
- Last resort recovery tool.

## Interview Tip:
"`git reflog` is your safety net â€” it shows all HEAD movements, including 'deleted' commits."

---

## Part 13 (121â€“130): Tags & Releases

---

## Question 121: What is a Git tag?

## Answer:
A tag is a named reference to a specific commit, typically used for releases.

```bash
git tag v1.0.0
```

## Key Points:
- Named reference to a commit.
- Used for releases.
- Lightweight or annotated.
- Immutable (usually).
- `v1.0.0` naming convention.

## Interview Tip:
"Tags mark specific commits â€” usually for releases like `v1.0.0`."

---

## Question 122: Why are Git tags used?

## Answer:
- **Release marking**: Tag releases for easy reference.
- **Versioning**: Track versions (v1.0.0, v2.0.0).
- **Deployment**: Deploy specific tagged versions.
- **Rollback**: Easy rollback to tagged versions.
- **Documentation**: Mark important milestones.

## Key Points:
- Release marking.
- Versioning.
- Deployment.
- Rollback.
- Documentation.

## Interview Tip:
"Tags are bookmarks for releases â€” they make it easy to find and deploy specific versions."

---

## Question 123: What is the difference between lightweight and annotated tags?

## Answer:
| Feature | Lightweight | Annotated |
|---------|------------|-----------|
| Object | Pointer only | Full object |
| Metadata | None | Author, message, date |
| Use case | Quick labels | Releases |
| Signing | No | Yes |

## Key Points:
- Lightweight: just a pointer.
- Annotated: full object with metadata.
- Annotated for releases.
- Lightweight for quick labels.
- Annotated can be signed.

## Interview Tip:
"Annotated tags for releases; lightweight tags for quick labels."

---

## Question 124: How do you create a tag?

## Answer:
```bash
git tag v1.0.0                    # Lightweight
git tag -a v1.0.0 -m "Release"    # Annotated
git tag -a v1.0.0 abc123          # Tag specific commit
```

## Key Points:
- `-a` for annotated.
- `-m` for message.
- Tag specific commit with hash.
- Default: tags HEAD.

## Interview Tip:
"Always use annotated tags for releases â€” they contain metadata."

---

## Question 125: How do you push tags to GitHub?

## Answer:
```bash
git push origin v1.0.0     # Push specific tag
git push origin --tags      # Push all tags
```

Tags aren't pushed by default â€” you must push them explicitly.

## Key Points:
- Tags aren't pushed by default.
- `git push origin <tag>` for specific.
- `git push origin --tags` for all.
- Push tags for releases.

## Interview Tip:
"Tags aren't pushed by default â€” `git push origin --tags` to share them."

---

## Question 126: How do you delete a tag?

## Answer:
```bash
git tag -d v1.0.0                    # Delete local
git push origin --delete v1.0.0      # Delete remote
```

## Key Points:
- `-d` for local deletion.
- `--delete` on push for remote.
- Delete both local and remote.

## Interview Tip:
"Delete both local and remote tags when cleaning up."

---

## Question 127: What is semantic versioning?

## Answer:
Semantic versioning uses `MAJOR.MINOR.PATCH`:
- **MAJOR**: Breaking changes.
- **MINOR**: New features (backward-compatible).
- **PATCH**: Bug fixes.

Example: `1.2.3` = MAJOR 1, MINOR 2, PATCH 3.

## Key Points:
- MAJOR.MINOR.PATCH format.
- MAJOR: breaking changes.
- MINOR: new features.
- PATCH: bug fixes.
- Industry standard.

## Interview Tip:
"`MAJOR.MINOR.PATCH` â€” breaking, features, fixes."

---

## Question 128: How do Git tags relate to releases?

## Answer:
Tags mark specific commits for releases. On GitHub, you can create a release from a tag, which includes release notes and downloadable assets.

## Key Points:
- Tags mark release commits.
- GitHub releases from tags.
- Include release notes.
- Downloadable assets.
- Easy rollback to tagged versions.

## Interview Tip:
"Create a GitHub release from a tag â€” it adds release notes and download links."

---

## Question 129: How do you manage production releases using Git?

## Answer:
1. **Tag the release**: `git tag -a v1.0.0 -m "Release 1.0.0"`.
2. **Push the tag**: `git push origin v1.0.0`.
3. **Create GitHub release**: Add release notes.
4. **Deploy**: Deploy the tagged version.
5. **Hotfix if needed**: Create hotfix branch from tag.

## Key Points:
- Tag releases.
- Push tags to remote.
- Create GitHub releases.
- Deploy tagged versions.
- Hotfix from tags.

## Interview Tip:
"Tag, push, release, deploy â€” the release workflow."

---

## Question 130: What release management practices do you follow?

## Answer:
1. **Semantic versioning**: Use MAJOR.MINOR.PATCH.
2. **Annotated tags**: For all releases.
3. **Release notes**: Document changes.
4. **Automated CI/CD**: Deploy on tag push.
5. **Hotfix process**: Quick fixes for production.

## Key Points:
- Semantic versioning.
- Annotated tags.
- Release notes.
- Automated deployment.
- Hotfix process.

## Interview Tip:
"Semantic versioning, annotated tags, and automated deployment â€” the release trifecta."

---

## Part 14 (131â€“140): Git Hooks & Automation

---

## Question 131: What are Git hooks?

## Answer:
Git hooks are scripts that run automatically at specific points in the Git workflow (pre-commit, pre-push, etc.).

Located in `.git/hooks/` or configured with tools like Husky.

## Key Points:
- Scripts that run automatically.
- Triggered by Git events.
- Located in `.git/hooks/`.
- Client-side and server-side.
- Used for automation.

## Interview Tip:
"Git hooks automate checks â€” lint before commit, test before push."

---

## Question 132: What are client-side Git hooks?

## Answer:
Client-side hooks run on the developer's machine:
- **pre-commit**: Before commit.
- **prepare-commit-msg**: Before editor opens.
- **commit-msg**: After commit message.
- **pre-push**: Before push.

## Key Points:
- Run locally.
- Pre-commit for linting.
- Commit-msg for message validation.
- Pre-push for tests.
- Not shared by default.

## Interview Tip:
"Client-side hooks run on your machine â€” use them for quality checks."

---

## Question 133: What are server-side Git hooks?

## Answer:
Server-side hooks run on the Git server:
- **pre-receive**: Before accepting push.
- **update**: Before updating refs.
- **post-receive**: After push is accepted.

## Key Points:
- Run on server.
- Pre-receive for validation.
- Post-receive for notifications.
- Enforce server-side policies.
- Managed by server admin.

## Interview Tip:
"Server-side hooks enforce policies â€” use them for access control and notifications."

---

## Question 134: What is a pre-commit hook?

## Answer:
A pre-commit hook runs before a commit is created. It's commonly used for:
- Linting code.
- Running tests.
- Checking formatting.
- Validating commit messages.

## Key Points:
- Runs before commit.
- Linting, testing, formatting.
- Can prevent commit if check fails.
- Most common Git hook.
- Use with Husky.

## Interview Tip:
"Pre-commit hooks catch issues before they're committed â€” lint, format, and test."

---

## Question 135: What is a pre-push hook?

## Answer:
A pre-push hook runs before pushing to a remote. It's commonly used for:
- Running full test suite.
- Checking for secrets.
- Validating branch names.

## Key Points:
- Runs before push.
- Full test suite.
- Secret detection.
- Branch validation.
- Last line of defense.

## Interview Tip:
"Pre-push hooks are the last check â€” run tests before pushing."

---

## Question 136: How do you automate code checks with Git hooks?

## Answer:
```bash
#!/bin/sh
# .git/hooks/pre-commit
npm run lint
npm run test
```

Or with Husky:
```json
// package.json
{
  "husky": {
    "hooks": {
      "pre-commit": "npm run lint",
      "pre-push": "npm run test"
    }
  }
}
```

## Key Points:
- Shell scripts in `.git/hooks/`.
- Husky for npm projects.
- Lint, test, format checks.
- Prevent commit on failure.
- Automate quality checks.

## Interview Tip:
"Husky makes Git hooks easy â€” configure in package.json."

---

## Question 137: What tools are commonly used with Git hooks?

## Answer:
- **Husky**: Git hooks manager for npm.
- **lint-staged**: Run linters on staged files.
- **commitlint**: Validate commit messages.
- **prettier**: Auto-format code.
- **eslint**: Lint JavaScript/TypeScript.

## Key Points:
- Husky for hook management.
- lint-staged for staged files.
- commitlint for messages.
- prettier for formatting.
- eslint for linting.

## Interview Tip:
"Husky + lint-staged + commitlint = automated code quality."

---

## Question 138: What are Husky and lint-staged?

## Answer:
- **Husky**: Manages Git hooks in npm projects.
- **lint-staged**: Runs linters only on staged files (faster).

```json
{
  "husky": {
    "hooks": {
      "pre-commit": "lint-staged"
    }
  },
  "lint-staged": {
    "*.js": "eslint --fix",
    "*.md": "prettier --write"
  }
}
```

## Key Points:
- Husky: manages Git hooks.
- lint-staged: runs on staged files only.
- Faster than linting all files.
- Common in modern projects.
- Configured in package.json.

## Interview Tip:
"lint-staged only lints changed files â€” it's much faster than linting everything."

---

## Question 139: How do Git hooks improve code quality?

## Answer:
- **Pre-commit**: Catch linting errors before commit.
- **Commit-msg**: Enforce commit message format.
- **Pre-push**: Run tests before sharing code.
- **Automated formatting**: Consistent code style.

## Key Points:
- Catch errors early.
- Enforce standards.
- Consistent formatting.
- Prevent bad commits.
- Automate quality checks.

## Interview Tip:
"Git hooks catch issues before they reach the repository â€” that's quality at the source."

---

## Question 140: What Git automation practices do you follow?

## Answer:
1. **Pre-commit hooks**: Lint and format.
2. **Commit-msg hooks**: Validate messages.
3. **Pre-push hooks**: Run tests.
4. **CI/CD**: Automated testing and deployment.
5. **GitHub Actions**: Automated workflows.

## Key Points:
- Pre-commit for linting.
- Commit-msg for format.
- Pre-push for tests.
- CI/CD for automation.
- GitHub Actions for workflows.

## Interview Tip:
"Automate everything: linting, testing, formatting, and deployment."

---

## Part 15 (141â€“150): GitHub Actions & Senior Workflow

---

## Question 141: What is GitHub Actions?

## Answer:
GitHub Actions is a CI/CD platform built into GitHub. It automates workflows like testing, building, and deploying based on Git events.

```yaml
# .github/workflows/ci.yml
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm test
```

## Key Points:
- CI/CD platform built into GitHub.
- Automates workflows.
- Triggered by Git events.
- YAML configuration.
- Free for public repos.

## Interview Tip:
"GitHub Actions is CI/CD built into GitHub â€” automate testing, building, and deployment."

---

## Question 142: How does GitHub Actions work?

## Answer:
1. **Event triggers**: Push, PR, schedule, etc.
2. **Workflow runs**: GitHub starts a runner.
3. **Jobs execute**: Steps run in sequence or parallel.
4. **Artifacts**: Output files, reports.
5. **Status**: Pass/fail feedback on PR.

## Key Points:
- Event triggers.
- Runner execution.
- Jobs and steps.
- Artifacts.
- Status feedback.

## Interview Tip:
"GitHub Actions is event-driven â€” trigger on push, PR, or schedule."

---

## Question 143: What are workflows in GitHub Actions?

## Answer:
Workflows are automated processes defined in YAML files. They're triggered by events and contain jobs.

```yaml
name: CI
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm ci
      - run: npm test
```

## Key Points:
- YAML configuration files.
- Triggered by events.
- Contain jobs and steps.
- Stored in `.github/workflows/`.
- Multiple workflows per repo.

## Interview Tip:
"Workflows are YAML files in `.github/workflows/` â€” they define your CI/CD pipeline."

---

## Question 144: What are jobs and steps?

## Answer:
- **Jobs**: Groups of steps that run on a runner.
- **Steps**: Individual commands or actions within a job.

```yaml
jobs:
  test:                    # Job
    runs-on: ubuntu-latest
    steps:                 # Steps
      - uses: actions/checkout@v4
      - run: npm test
```

## Key Points:
- Jobs run on runners.
- Steps run sequentially within jobs.
- Jobs can run in parallel.
- Steps can use actions or commands.

## Interview Tip:
"Jobs are groups of steps â€” steps are individual commands. Jobs can run in parallel."

---

## Question 145: How do you run tests automatically on every push?

## Answer:
```yaml
name: Tests
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
      - run: npm ci
      - run: npm test
```

## Key Points:
- Trigger on push and PR.
- Checkout code.
- Setup environment.
- Install dependencies.
- Run tests.

## Interview Tip:
"Trigger on push and PR â€” that's the standard CI setup."

---

## Question 146: How do you deploy applications using GitHub Actions?

## Answer:
```yaml
name: Deploy
on:
  push:
    branches: [main]
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm ci
      - run: npm run build
      - uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./dist
```

## Key Points:
- Trigger on main branch push.
- Build the application.
- Deploy to hosting.
- Use secrets for credentials.
- Many deployment actions available.

## Interview Tip:
"Deploy on push to main â€” that's the standard CD setup."

---

## Question 147: How do you manage secrets in GitHub Actions?

## Answer:
1. Go to repo Settings â†’ Secrets.
2. Add secrets (API keys, tokens).
3. Use in workflows: `${{ secrets.MY_SECRET }}`.

```yaml
steps:
  - run: echo ${{ secrets.API_KEY }}
  - env:
      API_KEY: ${{ secrets.API_KEY }}
```

## Key Points:
- Settings â†’ Secrets.
- `${{ secrets.NAME }}` syntax.
- Encrypted at rest.
- Not visible in logs.
- Essential for credentials.

## Interview Tip:
"Store credentials as secrets â€” never hardcode them in workflows."

---

## Question 148: How do you handle large-scale Git workflows in a team?

## Answer:
1. **Branch protection**: Require reviews and CI passing.
2. **CODEOWNERS**: Automatic reviewer assignment.
3. **Templates**: PR and issue templates.
4. **Automation**: GitHub Actions for CI/CD.
5. **Documentation**: Contributing guidelines.

## Key Points:
- Branch protection rules.
- CODEOWNERS for reviewers.
- Templates for consistency.
- Automation for quality.
- Documentation for onboarding.

## Interview Tip:
"Branch protection, CODEOWNERS, and automation â€” the large team essentials."

---

## Question 149: What Git mistakes do junior developers commonly make?

## Answer:
1. **Committing to main**: Always use feature branches.
2. **No commit messages**: Write meaningful messages.
3. **Force pushing shared branches**: Never force push shared branches.
4. **Not pulling before pushing**: Pull first to avoid conflicts.
5. **Committing secrets**: Never commit API keys or passwords.
6. **Giant commits**: Make small, focused commits.
7. **Not using .gitignore**: Commit unnecessary files.

## Key Points:
- Use feature branches.
- Write meaningful messages.
- Don't force push shared branches.
- Pull before pushing.
- Never commit secrets.
- Small, focused commits.
- Use .gitignore.

## Interview Tip:
"The biggest mistake is committing to main â€” always use feature branches."

---

## Question 150: In your opinion, what separates a junior, mid-level, and senior Git user?

## Answer:
- **Junior**: Knows basic commands (add, commit, push, pull). Can create branches and resolve simple conflicts.
- **Mid-level**: Understands branching strategies, rebasing, and stashing. Can handle merge conflicts and code reviews.
- **Senior**: Masters Git internals, interactive rebase, and complex workflows. Can recover from any Git disaster and mentor others.

The biggest differentiator: a senior understands Git's internal model and can recover from any situation.

## Key Points:
- Junior: basic commands, simple workflows.
- Mid-level: branching, rebasing, stashing, code review.
- Senior: internals, complex workflows, disaster recovery.
- Senior understands the "why" behind Git's design.
- Senior can mentor and recover from any Git issue.

## Interview Tip:
"The best answer shows self-awareness. Pick your level and explain what you're doing to grow."

---

# End of Git & GitHub Interview Questions & Answers
