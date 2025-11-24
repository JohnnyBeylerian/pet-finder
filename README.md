# PetFinder

A modern web application that helps pet owners register pets, generate unique QR codes for collars/tags, and reunite with their pets faster when they go missing.

## Features
- Secure authentication for pet owners
- Pet profiles: add, edit, delete, and manage multiple pets
- Automatic QR code generation for each pet profile
- Public “Found Pet” page via QR scan with owner contact workflow
- Responsive UI built with modern component library

## Tech Stack
- React + Vite + TypeScript
- Tailwind CSS + shadcn/ui
- React Router
- React Query
- Supabase (auth/storage) [if configured]

## Getting Started

Prerequisites:
- Node.js (LTS) and npm. We recommend installing via nvm: https://github.com/nvm-sh/nvm#installing-and-updating

Install and run:
```sh
# Clone
git clone https://github.com/bigshabs13/pet-finder.git
cd pet-finder

# Install dependencies
npm install

# Start dev server
npm run dev
```

Common scripts:
```sh
npm run dev       # start local dev server
npm run build     # production build
npm run preview   # preview built app
npm run lint      # run eslint
```

## Configuration
Create a `.env` file in the project root as needed (example keys):
```env
VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=
```
Do not commit secrets. Use environment variables for local development and CI.

## Project Structure
- `src/` – application source (components, routes, hooks, lib)
- `public/` – static assets
- `index.html` – Vite entry

## Contributing
Issues and PRs are welcome. Please run `npm run lint` and ensure builds pass before submitting.

## License
This project is licensed under the MIT License. See `LICENSE` for details.
