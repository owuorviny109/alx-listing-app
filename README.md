#  ALX Listing App – Milestone 1: Scaffolding and Initial Setup

> **Milestone Duration**: June 30, 2025 – July 7, 2025  
> **Level**: Novice | **Weight**: 1  
> **QA Review**:  (Mandatory)  
> **Repository**: [alx-listing-app](https://github.com/owuorviny109/alx-listing-app.git)

---

##  Project Overview

The **ALX Listing App** is a foundational project aimed at scaffolding a modern, scalable, and production-ready clone of an Airbnb-style property listing platform. This milestone focuses on establishing the project's initial codebase using **Next.js**, **TypeScript**, **TailwindCSS**, and **ESLint**. The goal is to build a modular and maintainable front-end architecture that supports responsive UI development, strong type safety, and component reuse.

---

##  Learning Objectives

By completing this milestone, learnt:

- Scaffold a Next.js application tailored for production deployment.
- Implement **TypeScript** to ensure type safety and code consistency.
- Integrate **TailwindCSS** for building responsive and accessible UIs.
- Configure **ESLint** to enforce consistent code quality.
- Create reusable UI components (e.g., `Card`, `Button`).
- Organize assets and structure the application for future scalability.

---

##  Prerequisites

| Requirement                          | Description                                                 |
|--------------------------------------|-------------------------------------------------------------|
| Next.js                              | Version 13+                                                 |
| Node.js                              | Version 16+ (LTS recommended)                               |
| Development Environment              | VS Code with TypeScript and TailwindCSS extensions          |
| Experience Level                     | Basic familiarity with Next.js, React, TypeScript, Tailwind |

---

##  Project Initialization

### 1. Scaffold the Application

Run the following command to bootstrap the project:

```bash
npx create-next-app@latest alx-listing-app \
  --typescript \
  --tailwind \
  --eslint \
  --no-app-router \
  --no-src-dir
```

> Note: This project uses the **Pages Router** and places all files in the root directory—`src/` is not used.

---

### 2. TailwindCSS Configuration

#### `tailwind.config.js`

```js
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
```

#### `styles/globals.css`

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

---

##  Folder and File Structure

```plaintext
alx-listing-app/
├── components/
│   └── common/
│       ├── Card.tsx           # Reusable property listing card
│       └── Button.tsx         # Generic button component
├── interfaces/
│   └── index.ts               # TypeScript interfaces (e.g., CardProps, ButtonProps)
├── constants/
│   └── index.ts               # Static configuration and reusable constants
├── public/
│   └── assets/                # SVGs, images, and other static files
├── pages/
│   └── index.tsx              # Entry point for the listing page UI
├── styles/
│   └── globals.css            # Tailwind base styles
├── tailwind.config.js         # Tailwind configuration file
├── README.md                  # Project documentation
```

---

##  Component Breakdown

| Component           | Description                                                 |
|---------------------|-------------------------------------------------------------|
| `Card.tsx`          | Renders property listing cards using passed props           |
| `Button.tsx`        | Renders styled buttons for actions such as "Book Now", etc. |

All props are strongly typed using interfaces defined in `interfaces/index.ts`.

---

##  TypeScript Interfaces

Centralized in:

```
interfaces/index.ts
```

Initial placeholder interfaces to define:

```ts
export interface CardProps {
  imageUrl: string;
  title: string;
  location: string;
  price: string;
}

export interface ButtonProps {
  label: string;
  onClick: () => void;
  variant?: 'primary' | 'secondary';
}
```

---

##  Constants

The `constants/index.ts` file contains reusable constants for configuration, API routes, UI strings, or static values.

Example:

```ts
export const BASE_API_URL = "https://api.example.com";
export const DEFAULT_IMAGE = "/assets/placeholder.jpg";
```

---

##  Asset Management

Assets such as images and icons should be placed under:

```
public/assets/
```

> Organize files by type (e.g., `/icons`, `/images`) for clarity.

---

##  Local Development Guide

1. **Clone the repository:**

```bash
git clone https://github.com/your-username/alx-listing-app.git
cd alx-listing-app
```

2. **Install dependencies:**

```bash
npm install
```

3. **Run the development server:**

```bash
npm run dev
```

4. **Open in browser:**

```
http://localhost:3000
```

> The application should compile successfully and render the base layout.

---

##  Milestone Completion Checklist

| Task                                             | Status     |
|--------------------------------------------------|------------|
| Next.js app scaffolded with TypeScript & ESLint | ✅          |
| TailwindCSS configured and functional            | ✅          |
| Folder structure established                     | ✅          |
| Reusable components created (`Card`, `Button`)   | ✅          |
| TypeScript interfaces defined                    | ✅          |
| Static assets organized under `public/assets/`   | ✅          |
| README created and project runs locally          | ✅          |

---

##  Tracked Deliverables

- `pages/index.tsx`
- `components/common/Card.tsx`
- `components/common/Button.tsx`
- `interfaces/index.ts`
- `constants/index.ts`
- `public/assets/`
- `README.md`

---

##  Author

> **Name**: Vincent Omondi Owuor  
> **Cohort**: ALX SE 2025  
> **Certification**: AWS Cloud Practitioner  
> **Role**: Cloud-Native Developer, Front-End Engineering Track

---
