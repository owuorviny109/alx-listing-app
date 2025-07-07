

#  ALX Listing App – Milestone 1: Scaffolding and Initial Setup

## Overview

The **ALX Listing App** is a foundational Airbnb clone built with **Next.js**, **TypeScript**, **TailwindCSS**, and **ESLint**. This project scaffolds the initial listing page for property displays using reusable components, a scalable folder structure, and modern development standards.

This milestone establishes a robust, production-ready codebase for subsequent features including property listings, filtering, and bookings.

---

## Project Goals

- Implement a clean, maintainable Next.js project using **Pages Router** (not App Router)
- Ensure strong **type safety** using TypeScript interfaces
- Design reusable, accessible **UI components** with TailwindCSS
- Apply **industry-standard** project structuring and linting with ESLint

---

## Folder Structure

```txt
alx-listing-app/
├── components/
│   └── common/
│       ├── Button.tsx       # Reusable button component
│       └── Card.tsx         # Reusable property card component
├── constants/
│   └── index.ts             # Application-wide constants
├── interfaces/
│   └── index.ts             # Shared TypeScript interfaces
├── public/
│   └── assets/              # Static images and SVGs
├── pages/
│   └── index.tsx            # Entry page
├── styles/
<<<<<<< HEAD
│   └── globals.css          # Global styles with Tailwind directives
├── tailwind.config.js       # TailwindCSS configuration
├── tsconfig.json            # TypeScript configuration
├── .eslintrc.json           # ESLint rules
└── README.md                # Project documentation
=======
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

Assets such as images and icons are placed under:

```
public/assets/
```

> Organize files by type (e.g., `/icons`, `/images`) for clarity.

---

##  Local Development Guide

1. **Clone the repository:**

```bash
git clone https://github.com/owuorviny109/alx-listing-app.git
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
 

