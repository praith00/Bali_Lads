# Bali_Lads

Hello guys Welcom to Bali lads, an app to connect and create via doodles

Bali_Lads is a web app built with **Vite**, **React**, **TypeScript**, **Tailwind CSS**, **shadcn/ui**, and **Supabase**.

This README explains how to set up and run the project locally so others can try it out.

---

## 🚀 Features

* Modern frontend using React + Vite
* TailwindCSS for styling with shadcn/ui components
* Supabase backend for authentication and database
* Hot-reloading development server

---

## 📦 Prerequisites

Before running this project, install:

* [Node.js](https://nodejs.org/) (latest LTS recommended)
* [npm](https://www.npmjs.com/) (comes with Node.js)
* A [Supabase](https://supabase.com/) account

Optional but recommended:

* [nvm](https://github.com/nvm-sh/nvm) to manage Node.js versions

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/praith00/Bali_Lads.git
cd Bali_Lads
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure Supabase

1. Go to [Supabase](https://supabase.com/), create a free project.
2. Copy your **Project URL** and **Anon Public Key** from **Project Settings > API**.
3. In your project root, create a `.env` file (based on `.env.example` if available).

Example:

```env
VITE_SUPABASE_URL=https://your-project.supabase.co
VITE_SUPABASE_ANON_KEY=your-anon-public-key
```

4. Set up your database tables and authentication according to your project needs (if migrations or SQL schema are included in the repo, run them).

---

## 🖥️ Run the Project

### Development

```bash
npm run dev
```

The app will be available at:
👉 `http://localhost:5173`

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

---

## 📂 Project Structure

```bash
Bali_Lads/
│── src/          # React components, pages, hooks, utils
│── public/       # Static assets
│── .env          # Environment variables (not committed)
│── package.json  # Project scripts & dependencies
│── vite.config.ts # Vite configuration
│── tailwind.config.js # Tailwind configuration
```

---

## 🛠️ Scripts Overview

| Script            | Description                              |
| ----------------- | ---------------------------------------- |
| `npm run dev`     | Start development server with hot reload |
| `npm run build`   | Build optimized production output        |
| `npm run preview` | Preview the production build locally     |

---

## ☁️ Deployment

Once built (`npm run build`), deploy the `dist/` folder to any static hosting provider such as:

* [Vercel](https://vercel.com/)
* [Netlify](https://www.netlify.com/)
* [GitHub Pages](https://pages.github.com/)

Make sure your Supabase environment variables are configured in the hosting provider’s dashboard.
