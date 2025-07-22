# 🛠️ General Tech Stack Template

This document outlines a flexible and modern technology stack template for web applications, featuring Vue 3 as the default frontend framework. It is designed to support scalable, maintainable, and accessible apps, with a clean separation of frontend and backend concerns.

---

## 🧩 Architecture Overview

The app is structured into separate frontend and backend layers. The frontend communicates with the backend exclusively via API calls, allowing independent development and deployment.

---

## 🌐 Frontend

| Layer          | Technology           | Notes |
|----------------|----------------------|-------|
| Framework      | **Vue 3**            | Using `<script setup>` and Composition API by default |
| Build Tool     | **Vite**             | Fast build times and hot module replacement |
| State Mgmt     | **Pinia**            | Lightweight and modular global state management |
| UI Components  | **Custom or UI Library** | Optionally build base components manually or integrate popular UI libraries |
| Component Dev  | **Storybook**         | Recommended for isolated component development and documentation |
| Accessibility  | **WAI-ARIA Best Practices** | Follow accessibility patterns and guidelines for inclusive UI |
| Routing       | **Vue Router**         | Declarative routing with nested views and guards |
| Testing        | **Vitest + Testing Library** | Unit, integration, and component testing |
| Linting/Format | **ESLint + Prettier** | Code quality and consistent formatting |

---

## 🔧 Backend (Pluggable / Replaceable)

| Layer        | Common Options           | Notes                  |
|--------------|--------------------------|------------------------|
| Hosting      | Node.js, Firebase, Supabase | Depending on app scale |
| Auth         | Firebase Auth, Auth.js, Clerk | User authentication and authorization |
| Database     | PostgreSQL, Firestore, MongoDB | SQL or NoSQL options  |
| File Storage | AWS S3, Firebase Storage   | For media and assets   |
| API Layer    | REST, GraphQL, RPC        | API design choice      |
| DevOps       | Docker, CI/CD pipelines   | For automation         |

---

## ♿ Accessibility & UI Patterns

Accessibility is critical for all apps. Follow these general guidelines:

- Use semantic HTML elements whenever possible
- Follow [WAI-ARIA Authoring Practices](https://www.w3.org/WAI/ARIA/apg/)
- Make components keyboard accessible and screen reader friendly
- Use automated tools (axe, Lighthouse) and manual testing

---

## 🎯 Development Principles

- 🧱 **Modularity:** Keep code and UI components decoupled and reusable  
- 🔁 **API-first:** Design backend APIs independently of frontend implementation  
- 🧠 **Context-aware:** Use context engineering for AI-assisted development (optional)  
- 📚 **Documentation:** Use tools like Storybook and markdown docs for clarity  

---

## 📁 Example File Structure

src/
├── components/ # UI components
├── views/ # Route views / pages
├── stores/ # Pinia stores
├── services/ # API calls, utils
├── router/ # Vue Router setup
└── assets/ # Images, styles, fonts

