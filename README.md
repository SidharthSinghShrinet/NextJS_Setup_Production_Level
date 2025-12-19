# 🛠️ NextJS Setup — Production Level

A **production-ready Next.js starter template** configured with industry-standard tools and best practices, including:

- ESLint + Prettier integration
- lint-staged + Husky for pre-commit automation
- Tailored for Next.js 15/16 projects
- Best code quality and formatting workflows

---

## 🚀 Features

A polished starter configuration for building scalable Next.js applications:

✔ ESLint configured with Next.js recommended rules  
✔ Prettier formatting with Tailwind (if used)  
✔ lint-staged + Husky pre-commit hooks for auto-fixing on staged files  
✔ Automatic formatting + linting on save  
✔ Path quoting support for Windows environments  
✔ Structured setup to encourage team collaboration

---

## 📁 Project Structure

├── .husky/ # Git hooks for pre-commit
├── app/ # Next.js app folder
├── public/ # Static assets
├── .lintstagedrc.js # lint-staged configuration
├── .prettierignore # Files to ignore for prettier
├── .prettierrc # Prettier configuration
├── eslint.config.mjs # ESLint flat config
├── jsconfig.json # Path aliases (optional)
├── next.config.mjs # Next.js configuration
├── package.json # Project dependencies & scripts
└── README.md # You are here!

yaml
Copy code

---

## 🧩 Getting Started

### 📌 Prerequisites

Make sure you have:

- **Node.js v16+** installed
- Package manager: `npm`, `pnpm`, or `yarn`

---

### 🛠️ Installation

Clone the repository:

```bash
git clone https://github.com/SidharthSinghShrinet/NextJS_Setup_Production_Level.git
cd NextJS_Setup_Production_Level
Install dependencies:

bash
Copy code
npm install
# or
yarn install
# or
pnpm install
🚀 Development
Run the local development server:

bash
Copy code
npm run dev
# or
yarn dev
# or
pnpm dev
Open in browser:

arduino
Copy code
http://localhost:3000
🧹 Linting & Formatting
🔍 Lint (check code quality)
bash
Copy code
npm run lint
🛠 Auto-fix lint issues
bash
Copy code
npm run lint:fix
📐 Format files
bash
Copy code
npm run format
📑 Pre-commit (lint-staged)
Staged files are automatically linted and formatted on git commit via Husky:

bash
Copy code
git add .
git commit -m "feat: your message"
This ensures:

ESLint runs with --fix

Prettier formats staged files

Only valid code is committed

🧠 How It Works
ESLint
Configured using a flat config with Next.js and Prettier integration. Rules enforce:

No unused vars

Hook rules

Best practices

ESLint auto-fixes what it can and reports the rest.

Prettier
Handles formatting tidily. With prettier-plugin-tailwindcss (if Tailwind is used), classes are automatically sorted. Formatting is safe and consistent across the codebase.

lint-staged + Husky
Ensures quality gates before commits:

lint-staged only runs on staged files

ESLint + Prettier run together without conflicts

Integration is safe on Windows (paths are correctly quoted)

📦 Scripts
Script	Description
dev	Start development server
build	Build production version
start	Start production server
lint	Run ESLint
lint:fix	Fix lint issues
format	Run Prettier formatting
lint:staged	Run pre-commit tasks manually

📌 Production and Optimizations
Before deploying:

Run npm run build

Ensure no lint errors remain (very useful in CI pipelines)

Use performance profiling tools

Keep dependencies up to date

Learn more in the official Next.js Production Checklist:
👉 https://nextjs.org/docs/app/guides/production-checklist 
Next.js

📚 Next.js Resources
Documentation: https://nextjs.org/docs

App Router Guides: Routing, layouts, caching, data fetching 
Next.js

💡 Contributing
Contributions are welcome! Please:

Fork the repository

Create a new branch

Make your changes

Submit a pull request

Follow coding conventions and keep commits clean.

📝 License
This project is open source — feel free to use
