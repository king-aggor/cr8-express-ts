# cr8-express-ts

[![npm version](https://img.shields.io/npm/v/cr8-express-ts)](https://www.npmjs.com/package/cr8-express-ts)
[![npm downloads](https://img.shields.io/npm/dt/cr8-express-ts.svg)](https://www.npmjs.com/package/cr8-express-ts)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**`cr8-express-ts`** is a simple CLI tool that scaffolds a ready-to-use **Express.js + TypeScript** project with a clean folder structure, configured TypeScript compiler, CORS support, error handling and basic server setup.

---

## 📚 Table of Contents

- [🚀 Features](#-features)
- [📦 Installation](#-installation)
- [🧱 Usage](#-usage)
- [📁 Generated Folder Structure](#-generated-folder-structure)
- [📝 NPM Scripts](#-npm-scripts)
- [📜 Included Middleware](#-included-middleware)
- [🤝 Contributing](#-contributing)

---

## 🚀 Features

- 🔧 TypeScript configuration (`tsconfig.json`)
- ⚙️ Express.js + dotenv + CORS installed
- 🛠 Auto-generated folder structure
- 🔄 Nodemon + ts-node setup for development
- 🌐 CORS support enabled by default
- 🧩 Built-in error handling middleware
- 📁 Includes `routes/`, `controllers/`, `middlewares/`, `utils/`
- ⚡ Ready to run with `npm run dev`

---

## 📦 Installation

```bash
npm install -g cr8-express-ts
```

---

## 🧱 Usage

```bash
cr8-express-ts <project-name>
```

Or use without installing globally:

```bash
npx cr8-express-ts <project-name>
```

To scaffold the project in your current directory:

```bash
npx cr8-express-ts .
```

### Example

```bash
npx cr8-express-ts awesome-api
```

This will:

- Create a new folder `awesome-api`
- Initialize `package.json`
- Install dependencies (`express`, `dotenv`, `cors`, `typescript`, etc.)
- Set up TypeScript compiler config
- Create folder structure and starter files
- Generate `.gitignore`, `.env` and scripts

### 📁 Generated Folder Structure

```
awesome-api/
├── src/
│ ├── controllers/
│ ├── middlewares/
│ │ └── errorHandler.ts
│ ├── routes/
│ ├── utils/
│ ├── app.ts
│ └── server.ts
├── public/
├── .env
├── .gitignore
├── tsconfig.json
├── package.json
```

---

## 📝 NPM Scripts

```json
"scripts": {
"start": "node dist/server.js",
"dev": "nodemon src/server.ts",
"build": "tsc"
}
```

---

## 📜 Included Middleware

- `cors` - Enabled by default for crosss-origin requests
- `express.json()` – Parses incoming JSON requests.
- Custom error handler (`middlewares/errorHandler.ts`) – Catches and handles application errors.

---

## 🤝 Contributing

Pull requests are welcome! If you find a bug or have a feature request, feel free to open an issue or submit a PR.
