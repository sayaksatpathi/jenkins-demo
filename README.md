<div align="center">

# 🧩 Jenkins Demo Pipeline

### A minimal Jenkins Pipeline-as-Code demo: Clone → Build → Test → Deploy.

[![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)](https://www.jenkins.io/)
[![Pipeline](https://img.shields.io/badge/Pipeline_as_Code-Declarative-335061?style=flat-square&logo=jenkins&logoColor=white)](https://www.jenkins.io/doc/book/pipeline/)
[![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)](https://www.gnu.org/software/bash/)

</div>

---

## Overview

A tiny, teaching-focused Jenkins project that demonstrates a **declarative pipeline** running four classic CI/CD stages against a trivial shell app. It's the "hello world" of Jenkins Pipeline-as-Code — the point is the pipeline, not the app.

## 🔄 Pipeline Stages

```
Clone ──► Build ──► Test ──► Deploy
```

| Stage | What happens |
|-------|--------------|
| **Clone** | Confirms the repository is checked out |
| **Build** | Makes `app.sh` executable and runs it |
| **Test** | Placeholder test step |
| **Deploy** | Placeholder deploy step |

`app.sh` simply greets, reports a successful build, and prints the date and hostname — enough to prove each stage executes.

## 🚀 Try It

1. Create a new **Pipeline** job in Jenkins.
2. Point it at this repository (Pipeline script from SCM) so it picks up the [`Jenkinsfile`](Jenkinsfile).
3. **Build Now** and watch the four stages run in the stage view.

Run the app standalone:

```bash
chmod +x app.sh && ./app.sh
```

## 🧱 Files

- **`Jenkinsfile`** — declarative pipeline definition
- **`app.sh`** — the sample build script

> Looking for a production-grade pipeline with real security gates? See **[Jenkins-DevSecOps-Pipeline](https://github.com/sayaksatpathi/Jenkins-DevSecOps-Pipeline)**.

---

<div align="center">

Built by **[Sayak Satpathi](https://github.com/sayaksatpathi)**

</div>
