 ALX Listing App
Milestone 1: Scaffolding and Initial Setup for Listing Page
Level: Novice
Weight: 1
Project Duration: Jun 30, 2025 – Jul 7, 2025

📌 Overview
The ALX Listing App project scaffolds the foundational structure for a modern Airbnb-style property listing page. It is built using Next.js, TypeScript, TailwindCSS, and ESLint, with a clean and scalable folder structure. This milestone establishes best practices and modular design to enable the development of a dynamic, responsive, and production-grade frontend.

🎯 Learning Objectives
Scaffold a Next.js project suitable for production.
Enforce type safety with TypeScript and reusable interfaces.
Configure TailwindCSS for responsive, accessible UI development.
Apply best practices in project structure and component reuse.
Manage static assets effectively for real-world applications.

✅ Prerequisites
Proficiency with Next.js, React, and TypeScript
Familiarity with TailwindCSS
Understanding of ESLint for code quality
Knowledge of scalable folder structuring and modular development

🛠️ Technical Requirements
Next.js version 13+
Node.js version 16+
VS Code or equivalent editor with TypeScript and TailwindCSS extensions

🔧 Setup Instructions
1. Scaffold the Project
Use the following CLI to generate the project:

npx create-next-app@latest alx-listing-app \
  --typescript \
  --tailwind \
  --eslint \
  --no-app-router \
  --no-src-dir

2. Configure TailwindCSS
In tailwind.config.js:

module.exports = {
  content: [
    './pages/**/*.{ts,tsx}',
    './components/**/*.{js,ts,jsx,tsx}',
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}

In styles/globals.css:

@tailwind base;
@tailwind components;
@tailwind utilities;

📁 Folder Structure

alx-listing-app/
├── components/
│   └── common/
│       ├── Button.tsx
│       └── Card.tsx
├── constants/
│   └── index.ts
├── interfaces/
│   └── index.ts
├── pages/
│   └── index.tsx
├── public/
│   └── assets/
│       └── [images and SVGs]
├── styles/
│   └── globals.css
├── tailwind.config.js
└── README.md

🔁 Reusable Components
components/common/Card.tsx: Generic listing card
components/common/Button.tsx: Themed button for interaction

🧩 TypeScript Interfaces
interfaces/index.ts: Centralized declaration of CardProps, ButtonProps, etc.

🧭 Constants
constants/index.ts: Placeholder for configuration values, API URLs, and text constants

🖼️ Assets
Images, icons, and SVGs reside in public/assets/
Assets follow a flat or nested structure based on usage context

📘 How to Run the Project
Step-by-step:
Clone the repository:

git clone https://github.com/owuorviny109/alx-listing-app.git
cd alx-listing-app

Install dependencies:

npm install

Run development server:

npm run dev

Access app at:
http://localhost:3000

✅ Verification Checklist
- Project compiles without error
- Tailwind styles are applied correctly
- Card and Button components render without issue
- Folders follow required structure
- Static assets load properly

🔗 GitHub Repository
URL: https://github.com/owuorviny109/alx-listing-app

Tracked Files:
- pages/index.tsx
- components/common/Card.tsx
- components/common/Button.tsx
- interfaces/index.ts

ALX Listing App
Milestone 1: Scaffolding and Initial Setup for Listing Page
Level: Novice
Weight: 1
Project Duration: Jun 30, 2025 – Jul 7, 2025

📌 Overview
The ALX Listing App project scaffolds the foundational structure for a modern Airbnb-style property listing page. It is built using Next.js, TypeScript, TailwindCSS, and ESLint, with a clean and scalable folder structure. This milestone establishes best practices and modular design to enable the development of a dynamic, responsive, and production-grade frontend.

🎯 Learning Objectives

Scaffold a Next.js project suitable for production.

Enforce type safety with TypeScript and reusable interfaces.

Configure TailwindCSS for responsive, accessible UI development.

Apply best practices in project structure and component reuse.

Manage static assets effectively for real-world applications.

✅ Prerequisites

Proficiency with Next.js, React, and TypeScript

Familiarity with TailwindCSS

Understanding of ESLint for code quality

Knowledge of scalable folder structuring and modular development

🛠️ Technical Requirements

Next.js version 13+

Node.js version 16+

VS Code or equivalent editor with TypeScript and TailwindCSS extensions

🔧 Setup Instructions

1. Scaffold the Project
Use the following CLI to generate the project:

bash
Copy
Edit
npx create-next-app@latest alx-listing-app \
  --typescript \
  --tailwind \
  --eslint \
  --no-app-router \
  --no-src-dir
2. Configure TailwindCSS
In tailwind.config.js:

js
Copy
Edit
module.exports = {
  content: [
    './pages/**/*.{ts,tsx}',
    './components/**/*.{js,ts,jsx,tsx}',
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
In styles/globals.css:

css
Copy
Edit
@tailwind base;
@tailwind components;
@tailwind utilities;
📁 Folder Structure

pgsql
Copy
Edit
alx-listing-app/
├── components/
│   └── common/
│       ├── Button.tsx
│       └── Card.tsx
├── constants/
│   └── index.ts
├── interfaces/
│   └── index.ts
├── pages/
│   └── index.tsx
├── public/
│   └── assets/
│       └── [images and SVGs]
├── styles/
│   └── globals.css
├── tailwind.config.js
└── README.md
🔁 Reusable Components

components/common/Card.tsx: Generic listing card

components/common/Button.tsx: Themed button for interaction

🧩 TypeScript Interfaces

interfaces/index.ts: Centralized declaration of CardProps, ButtonProps, etc.

🧭 Constants

constants/index.ts: Placeholder for configuration values, API URLs, and text constants

🖼️ Assets

Images, icons, and SVGs reside in public/assets/

Assets follow a flat or nested structure based on usage context

📘 How to Run the Project

Step-by-step:

1. Clone the repository:

bash
Copy
Edit
git clone https://github.com/owuorviny109/alx-listing-app.git
cd alx-listing-app
2. Install dependencies:

bash
Copy
Edit
npm install
3. Run development server:

bash
Copy
Edit
npm run dev
4. Access app at:
http://localhost:3000

✅ Verification Checklist

 Project compiles without error

 Tailwind styles are applied correctly

 Card and Button components render without issue

 Folders follow required structure

 Static assets load properly

🔗 GitHub Repository
URL: https://github.com/owuorviny109/alx-listing-app

Tracked Files:

pages/index.tsx

components/common/Card.tsx

components/common/Button.tsx

interfaces/index.ts

constants/index.ts

public/assets/

README.md


- constants/index.ts
- public/assets/
- README.md
