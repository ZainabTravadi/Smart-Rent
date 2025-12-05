# 🌟 **Contributing to Smart-Rent**

Welcome, developer! 👋
We’re thrilled that you’re interested in contributing to **Smart-Rent**, a modern, full-stack MERN rental platform built with scalability, UX finesse, and real-time interactions in mind.

This guide will walk you through everything—from setup to submitting PRs—so your contributions land smoothly and make an impact.

<div align="center">

💡 *Whether you're fixing bugs, improving UI, writing docs, or shipping new features — thank you for helping Smart-Rent grow.*

</div>

---

# 📚 **Table of Contents**

* [🚀 How to Contribute](#-how-to-contribute)
* [🛠️ Project Setup](#️-project-setup)
* [🧹 Coding Standards](#-coding-standards)
* [🔀 Pull Request Guidelines](#-pull-request-guidelines)
* [🐞 Issue Reporting](#-issue-reporting)
* [🌱 Good First Issues](#-good-first-issues)
* [💬 Communication](#-communication)
* [🤝 Code of Conduct](#-code-of-conduct)
* [🔄 Development Workflow Summary](#-development-workflow-summary)
* [📘 Resources](#-resources)

---

<a id="how-to-contribute"></a>
## 🚀 How to Contribute

## 1️⃣ **Fork the Repository**

* Navigate to the repo:
  👉 [https://github.com/hitesh-kumar123/Smart-Rent](https://github.com/hitesh-kumar123/Smart-Rent)
* Click **Fork** in the top-right corner.
* You now have your personal copy.

---

## 2️⃣ **Clone Your Fork**

```bash
git clone https://github.com/YOUR_USERNAME/Smart-Rent.git
cd Smart-Rent

git remote add upstream https://github.com/hitesh-kumar123/Smart-Rent.git
```

This connects your fork to the main repo for syncing updates.

---

## 3️⃣ **Create a Feature Branch**

Never work on `main` directly.

```bash
git fetch upstream
git checkout -b feature/my-awesome-feature upstream/main
```

### 🌿 Branch Naming Rules

| Type     | Format              | Example                          |
| -------- | ------------------- | -------------------------------- |
| Feature  | `feature/<name>`    | `feature/add-wishlist`           |
| Bugfix   | `fix/<issue>`       | `fix/booking-overlap-validation` |
| Docs     | `docs/<name>`       | `docs/improve-api-guide`         |
| Refactor | `refactor/<module>` | `refactor/user-controller`       |
| Tests    | `test/<purpose>`    | `test/property-endpoints`        |

❌ Avoid names like:
`stuff`, `wip`, `update`, `bug`, `changes`.

---

<a id="project-setup"></a>
## 🛠️ Project Setup

## Backend Setup

```bash
cd backend
npm install
cp .env.example .env
npm run dev
```

Backend runs on:
👉 `http://localhost:8000`

---

## Frontend Setup

```bash
cd frontend
npm install
npm start
```

Frontend runs on:
👉 `http://localhost:3000`

---

### 🌍 Required Environment Variables

```env
MONGODB_URI=
JWT_SECRET=
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=
EMAIL_USER=
EMAIL_PASS=
PORT=8000
NODE_ENV=development
```

---

<a id="coding-standards"></a>
## 🧹 Coding Standards

We follow clean, modular, readable JavaScript.
Be kind to the next developer. Write code they’ll thank you for.

---

### 🧠 General Rules

✔ Write self-explanatory variable names
✔ Use React functional components + hooks
✔ Follow existing file/folder conventions
✔ Comment only where logic is non-obvious
✔ Delete unused imports & console.logs
✔ Keep functions small & focused

---

### 🟦 **Node.js Best Practices**

```js
// GOOD
const getUser = async (id) => {
  const user = await User.findById(id);
  if (!user) throw new Error("User not found");
  return user;
};

// BAD
async function g(id){
 let u = await User.findById(id)
 return u
}
```

---

### 🟩 **React Standards**

```jsx
// GOOD
const PropertyCard = ({ property }) => (
  <div className="card">
    <h3>{property.title}</h3>
    <p>${property.price}/night</p>
  </div>
);

// BAD
function Card(props){
 return <div>{props.data}</div>
}
```

---

# 🧾 **Commit Message Rules (Conventional Commits)**

Format:

```
<type>(scope): subject
```

### Allowed Types

| Type       | Use Case                               |
| ---------- | -------------------------------------- |
| `feat`     | Add a feature                          |
| `fix`      | Fix a bug                              |
| `docs`     | Update docs                            |
| `refactor` | Improve code without changing behavior |
| `test`     | Add/update tests                       |
| `style`    | Formatting only                        |
| `perf`     | Performance improvement                |
| `chore`    | Tooling, configs                       |

### Examples

```bash
feat(property): add category-based filtering

fix(booking): prevent double booking overlaps

docs(api): update booking endpoint documentation

refactor(auth): simplify token verification
```

---

<a id="pull-request-guidelines"></a>
## 🔀 Pull Request Guidelines

Before opening a PR:

✔ Code builds without errors
✔ No debug logs
✔ Linting passes
✔ Tests updated (if applicable)
✔ Screenshots included for UI changes
✔ Documentation updated if needed

---

### 📝 PR Template

Your PR description **should** follow this structure:

```markdown
## 🚀 Summary
Short explanation of what this PR does.

## 🧩 Type of Change
- [ ] Feature
- [ ] Bug Fix
- [ ] Refactor
- [ ] Documentation
- [ ] Performance

## 🔗 Related Issues
Fixes #123  
Closes #456  

## 🛠️ Changes Made
- Change 1  
- Change 2  
- Change 3  

## 🧪 How to Test
1. Step one  
2. Step two  
3. Expected result  

## 📸 Screenshots (UI changes)
[Attach images]

## ✅ Checklist
- [ ] Code follows standards  
- [ ] No unused variables/logs  
- [ ] Tested on mobile + desktop  
- [ ] All docs updated  
```

---

<a id="issue-reporting"></a>
## 🐞 Issue Reporting

### Before reporting:

✔ Search existing issues
✔ Test on the latest branch
✔ Include browser, OS, Node version

---

### 🐛 Bug Report Template

```markdown
## Description
Describe the bug clearly.

## Steps to Reproduce
1. Step one
2. Step two

## Expected Behavior
What should have happened?

## Actual Behavior
What happened instead?

## Environment
OS:  
Browser:  
Node version:  

## Screenshots / Logs
Attach if applicable.
```

---

<a id="good-first-issues"></a>
## 🌱 Good First Issues

Start with issues labeled:

* `good-first-issue`
* `help-wanted`
* `documentation`

These are beginner-friendly, safe, and well-scoped.

---

<a id="communication"></a>
## 💬 Communication

* Ask questions in **GitHub Issues**
* Discuss ideas in **GitHub Discussions**
* Tag maintainers when stuck

⏱ **Response Time Goals**

* Issues: 3–5 days
* PR reviews: 5–7 days

---

<a id="code-of-conduct"></a>
## 🤝 Code of Conduct

Smart-Rent follows the **Contributor Covenant**.
We expect contributors to:

💙 Be respectful
💛 Give constructive feedback
💜 Be inclusive
🧡 Support beginners

Harassment, discrimination, or hostility = 🚫 **not tolerated**.

Report violations privately to maintainers.

---

<a id="development-workflow-summary"></a>
## 🔄 Development Workflow Summary

```
1. Fork repo
     ↓
2. Clone fork
     ↓
3. Create feature branch
     ↓
4. Write clean, tested code
     ↓
5. Commit using Conventional Commits
     ↓
6. Push branch to your fork
     ↓
7. Open a Pull Request
     ↓
8. Address review comments
     ↓
9. Merge & celebrate 🎉
```

---

<a id="resources"></a>
## 📘 Resources

### Project Docs

* README.md
* API.md
* FEATURES.md
* UI-UX.md
* BACKEND.md
* FRONTEND.md

### Developer Learning

* [https://nodejs.org](https://nodejs.org)
* [https://react.dev](https://react.dev)
* [https://expressjs.com](https://expressjs.com)
* [https://mongodb.com](https://mongodb.com)

---

# ❤️ **Thank You for Contributing!**

Every PR, every comment, every line of documentation pushes Smart-Rent forward.

<div align="center">

✨ *Your contribution matters.*
✨ *Your effort is appreciated.*
✨ *Your code makes this project better.*

</div>
