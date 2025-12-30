# AI-Assisted Code Migration Tool

An AI-assisted code migration tool that helps developers modernize legacy JavaScript codebases by converting them into modern ES6 modules or TypeScript. The tool focuses on improving developer productivity by combining AI-driven code understanding with a clean, interactive editing experience.

---

## 🚀 Project Overview

Modernizing older JavaScript code often involves manual refactoring, adding typings, and restructuring imports. This project simplifies that workflow by allowing users to paste legacy JavaScript code and automatically generate modernized output using an LLM.

The application provides a side-by-side editor experience so developers can review, edit, and validate the migrated code before exporting it.

---

## ✨ Features

- Paste legacy JavaScript code using a Monaco-based editor  
- Convert code to **ES6+ JavaScript** or **TypeScript**
- AI-generated improvements including:
  - Modern imports
  - Cleaner structure
  - TypeScript interfaces and typed imports (when applicable)
- Side-by-side comparison of original and migrated code
- Editable output before export
- Migration session persistence via a backend service
- Modular architecture with a database-agnostic persistence layer

---

## 🛠 Tech Stack

**Frontend**
- React.js
- TypeScript
- Monaco Editor
- Tailwind CSS
- shadcn-ui

**Backend**
- Node.js
- Express.js
- AI API (LLM-based code transformation)

**Persistence**
- Managed backend service (designed to be easily replaceable with MongoDB Atlas)

---

## 🧠 Tech Notes

- TypeScript is used to improve safety and clarity in transformed outputs.
- Some TypeScript warnings may appear depending on the consuming project’s configuration (such as `tsconfig.json` and installed typings), which reflects real-world migration workflows.
- The persistence layer is modular and can be swapped with MongoDB Atlas without affecting the migration or UI logic.

---

## ▶️ Demo

A full walkthrough demonstrating legacy code input, AI-powered migration, and output review is available via the demo video link provided in the submission.

---

## 🧩 Getting Started (Local Setup)

### Prerequisites
- Node.js (v18+ recommended)
- npm

### Installation

```sh
# Clone the repository
git clone <YOUR_GITHUB_REPO_URL>

# Navigate to the project directory
cd ai-code-migration-tool

# Install dependencies
npm install

# Start the development server
npm run dev
