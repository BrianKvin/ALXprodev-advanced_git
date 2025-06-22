
---

````markdown
# Git-Flows Project

**Level:** Novice  
**Weight:** 1  
**Project Duration:** June 16, 2025 – June 23, 2025  
**Manual QA Review Required**

---

## 📖 Overview

Git-Flow is a powerful Git branching model introduced by Vincent Driessen to streamline collaborative development. It standardizes how features, releases, and fixes are managed in code repositories — especially for large-scale or team-driven projects.

Git-Flow revolves around five key branch types:

- `main` – production-ready code  
- `develop` – ongoing development  
- `feature/*` – new feature development  
- `release/*` – preparing code for production  
- `hotfix/*` – emergency fixes to production  

---

## 🎯 Relevance in the Development Process

Git-Flow enables:

- **Code Organization:** Clear separation between development and production.
- **Team Collaboration:** Efficient workflows using structured branching.
- **Stability:** Safe integration of new features and fixes.
- **Release Management:** Easy handling of versioned and stable releases.

---

## 📚 Learning Objectives

By the end of this project, learners will:

- Understand the Git-Flow structure and its purpose.
- Identify and use different Git-Flow branch types.
- Manage features, hotfixes, and releases using Git best practices.
- Apply Git-Flow in CI/CD pipelines.

---

## ✅ Learning Outcomes

Learners will be able to:

- Explain how Git-Flow benefits large, collaborative development.
- Create and manage branches following the Git-Flow model.
- Use Git commands to handle feature, release, and hotfix branches.
- Integrate Git-Flow into automated testing and deployment pipelines.

---

## 🚀 Git-Flow Best Practices

| Best Practice | Description |
|---------------|-------------|
| Start with `develop` | Always branch from `develop` for new features. |
| Feature Isolation | Keep each feature in its own branch. |
| Merge via Pull Requests | Use PRs to ensure code review before merging. |
| Keep `main` Clean | Only production-ready, tested code should be on `main`. |
| Tag Releases | Use Git tags on `main` to mark release points. |
| Use `hotfix/*` for urgent bugs | Urgent fixes should be done directly on `main`, and merged back into `develop`. |
| Document Your Workflow | Always keep clear documentation of your branching model. |

---

## 🛠 Common Git-Flow Commands

```bash
git flow init                    # Initialize Git-Flow
git flow feature start <name>   # Start a feature branch
git flow feature finish <name>  # Finish feature and merge into develop
git flow release start <x.x.x>  # Start a release branch
git flow release finish <x.x.x> # Merge release into main and develop
git flow hotfix start <x.x.x>   # Start a hotfix branch
git flow hotfix finish <x.x.x>  # Merge hotfix into main and develop
````

---

## 📝 Project Tasks

### 0. Setting up GitFlow

* Create a repo: `ALXprodev-advanced_git`
* Clone it locally
* Create and push a `develop` branch
* Initialize Git-Flow with default settings (`git flow init -d`)
* Create an empty `README.md` and push

---

### 1. Creating a Feature Branch

* Create `feature/implement-login` from `develop`
* Inside it, create `login-page/README.md` with:
  *"Login Feature Coming soon"*
* Commit with message:
  `feat: scaffolding login page`
* Push the branch

---

### 2. Creating a Release Branch

* Create `feature/implement-signup` and add `signup-page/README.md` with:
  *"feature coming soon"*
* Merge both features into `develop`
* Create a release branch `release/1.0.0`
* Edit `signup-page/README.md` to include:
  *"data requirements: email, firstName, lastName, profilePic"*
* Merge `release/1.0.0` to `main` and `develop`
* Tag release as `v1.0.0` and push the tag

---

### 3. Git Hooks and Automation

* Create a **pre-commit hook** (`.git/hooks/pre-commit`) to ensure each directory has a `README.md`
* Create a **post-merge hook** to log merges into `main`

---

## 🔍 Manual Review

This project requires a **manual QA review**. Once all tasks are complete, submit for manual checking.

---

## 📁 Repository Structure

```
ALXprodev-advanced_git/
├── login-page/
│   └── README.md
├── signup-page/
│   └── README.md
└── README.md
```

---

## 🏁 End of Project

Congratulations on reaching the end of the Git-Flow Project! You've learned essential collaborative Git practices, and you're ready to apply them in real-world scenarios.

---

```

Let me know if you’d like this broken into separate sections or included with a `.md` file download.
```
