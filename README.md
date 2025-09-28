# 🚀 Project Template: Standardized Development & Collaboration

Welcome to the **Lxisoft Standard Project Template**!

This template repository is designed to ensure consistency, high traceability, and maintainability across all our software development projects. By using this template, you automatically inherit:

1. Standardized **Epic, Feature, Story, and Task** issue templates.
2. Mandatory **Conventional Commit** messages with issue ID linking.
3. Automated **Semantic Versioning** and **Changelog** generation.

## 💡 About [LXISOFT](https://www.lxisoft.com): Driving Innovation

[LXISOFT](https://www.lxisoft.com) 

From nurturing a nascent idea to swiftly crafting a prototype, continuously delivering and launching into production, and providing ongoing upgrades, we are dedicated to assisting you every step of the way. Our team comprises internationally certified Java developers who possess the prowess to transform your concepts into fully functional web applications or cross-platform mobile apps for Android, iPhone, iPad, Windows, and more. Additionally, we excel in developing SOA/Microservices-based architectures and Java web portals.

**Our Focus Areas:**

* **Software Development Activities:** We utilize lean, agile methodologies (like the Epic-Feature-Story model) and BDD best practices to deliver robust, scalable, and user-centric software. Our core technology stack is broad and cloud-native, encompassing **Java**, **Python**, and **Flutter** for various development needs. We also leverage **JavaScript/TypeScript** with **Node.js**. Our foundational practices emphasize **AI**, **12 Factor Apps**, **Cloud**, **Container** technologies, **Kubernetes**, and high-throughput **Messaging Middleware** for resilient deployment.

* **Internship Program:** We believe in nurturing the next generation of tech talent. Our comprehensive internship program offers hands-on experience, mentorship, and a direct pathway to full-time roles, fostering a culture of continuous learning and innovation.

**Connect With Us:**

| Platform | Link | 
| ----- | ----- | 
| **Website** | [www.lxisoft.com](http://www.lxisoft.com) | 
| **Facebook** | [@lxisoft](https://www.facebook.com/lxisoft) | 
| **LinkedIn** | [@lxisoft](https://www.linkedin.com/company/lxisoft) | 
| **Twitter/X** | [@lxisoft](https://twitter.com/lxisoft) | 
| **Instagram** | [@lxisoft](https://www.instagram.com/lxisoft) | 

## 🛠️ Developer Setup: Standardization Guide

This template uses **Husky** and **Commitlint** to automatically enforce commit message standards locally, and **Standard-Version** to manage releases.

### 1. Initialize Project Standards (Mandatory)

After cloning your new repository from this template, run the following commands **one time** to install dependencies and activate the Git hooks:


### 1. Install project dependencies (this includes husky, commitlint, and standard-version)

```npm install                                                ```

### 2. The 'prepare' script in package.json automatically runs 'husky install'
 This activates the 'commit-msg' hook on your local machine, enforcing commit rules.

#### 📝 Commit Message Standards & Commitizen

All commits must follow the [Conventional Commits](https://www.conventionalcommits.org/) format and reference an issue ID in the body.

**Standard commit types (`type-enum`):**
- feat
- fix
- docs
- style
- refactor
- perf
- test
- build
- ci
- chore
- revert

**Recommended scopes (`scope-enum`):**
- api, app, auth, build, ci, config, core, docs, deps, devops, feature, infra, model, service, test, ui, util, web, mobile
- Flutter: widget, screen, bloc, provider, theme, assets
- Java: controller, repository, entity, service, dto, spring, jpa
- TS/JS: component, hook, store, redux, context, types, eslint, webpack

**How to create a commit:**
- Use Commitizen for interactive commit messages:

```npx cz                                            ```

#### 🚀 Release Process (Semantic Versioning & Changelog)

This project uses [standard-version](https://github.com/conventional-changelog/standard-version) for automated releases:

1. **Commit your changes** using conventional commit messages.
2. **Run the release command:**
3. ``` npx standard-version                          ```


3. **What happens:**
- The version in `package.json` is bumped (major, minor, or patch).
- A `CHANGELOG.md` is generated or updated.
- A new git commit and tag are created for the release.
4. **Push your changes and tags:**


``` git push --follow-tags                          ```


This automates semantic versioning and changelog management for your project.