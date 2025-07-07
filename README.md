# ALX Listing App

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
│   └── globals.css          # Global styles with Tailwind directives
├── tailwind.config.js       # TailwindCSS configuration
├── tsconfig.json            # TypeScript configuration
├── .eslintrc.json           # ESLint rules
└── README.md                # Project documentation
