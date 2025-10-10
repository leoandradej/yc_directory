# 🚀 YC Directory

> A platform for founders to share and explore startup ideas — built with Next.js, Sanity, and GitHub Auth.

[🌐 Live Demo](https://yc-directory-nine-beige.vercel.app/)  
[🧠 Author](https://github.com/leoandradej)

---

## 📘 Overview

**YC Directory** is a modern web app inspired by Y Combinator’s startup listings.  
It allows users to:

- Sign in with **GitHub**
- Submit their **startup ideas**
- **Browse, filter, and explore** pitches from others
- Manage content seamlessly with **Sanity CMS**
- Enjoy a smooth, **responsive** UI built with **TailwindCSS + ShadCN**

---

## ✨ Features

✅ GitHub OAuth authentication via **NextAuth**  
✅ **Sanity CMS** integration for content management  
✅ **Server Actions** for form submissions  
✅ Real-time startup directory feed  
✅ Category filters and search functionality  
✅ Fully responsive UI (mobile + desktop)  
✅ Error tracking with **Sentry**  
✅ Deployed easily on **Vercel**

---

## 🛠 Tech Stack

| Layer      | Technology                                                                     |
| ---------- | ------------------------------------------------------------------------------ |
| Framework  | [Next.js 15 (App Router)](https://nextjs.org/)                                 |
| Language   | [TypeScript](https://www.typescriptlang.org/)                                  |
| Styling    | [Tailwind CSS](https://tailwindcss.com/) + [ShadCN/UI](https://ui.shadcn.com/) |
| CMS        | [Sanity.io](https://www.sanity.io/)                                            |
| Auth       | [NextAuth.js (GitHub Provider)](https://next-auth.js.org/)                     |
| Monitoring | [Sentry](https://sentry.io/)                                                   |
| Deployment | [Vercel](https://vercel.com/)                                                  |

---

## ⚙️ Getting Started

### 1️⃣ Clone & Install

```bash
git clone https://github.com/leoandradej/yc_directory.git
cd yc_directory
npm install
```

### 2️⃣ Set Up Environment Variables

Create a `.env.local` file in the root:

```env
# Auth
AUTH_SECRET=your_secret
AUTH_GITHUB_ID=your_github_client_id
AUTH_GITHUB_SECRET=your_github_client_secret

# Sanity
NEXT_PUBLIC_SANITY_PROJECT_ID=your_project_id
NEXT_PUBLIC_SANITY_DATASET=production
SANITY_WRITE_TOKEN=your_sanity_write_token

# Optional
SENTRY_AUTH_TOKEN=your_sentry_token
```

### 3️⃣ Run Locally

```bash
npm run dev
```

Then open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 🗂 Folder Structure

```
yc_directory/
├── app/                  # Next.js app router (routes, layouts, pages)
├── components/            # UI components (cards, buttons, etc.)
├── lib/                   # Utilities, configs, queries
├── sanity/                # Sanity schemas and client setup
├── public/                # Static assets
├── styles/                # Global and Tailwind styles
├── .env.local.example
├── next.config.js
├── package.json
└── README.md
```

---

## 🧩 Usage Guide

1. **Sign in** with your GitHub account.
2. **Create a new startup pitch** using the “Create” button.
3. **Browse existing ideas**, filter by category, and explore.
4. **Sign out** or manage your profile from the navbar.

---

## 🧪 Development Tips

- Use TypeScript strictly for type safety.
- Keep your Sanity schema synced between local and production.
- Handle `null` session cases carefully when using `auth()` calls.
- Use `sonner` for toast notifications (replacement for deprecated `toast` API).

---

## 🧱 Deployment

### Deploy with Vercel (Recommended)

1. Push your code to GitHub.
2. Go to [Vercel](https://vercel.com/) and import the project.
3. Add your environment variables in the dashboard.
4. Click **Deploy** — that’s it! 🎉

Ensure your **Sanity project** is deployed and accessible publicly.

---

## 🤝 Contributing

1. Fork this repo
2. Create a new branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m "feat: add new feature"`)
4. Push and open a Pull Request 🎉

---

## 📄 License

This project is licensed under the **MIT License** — feel free to use and modify.

---

## ❤️ Acknowledgments

- Based on the YC Directory concept by [JavaScript Mastery](https://github.com/adrianhajdin/yc_directory)
- Built and improved by [Leonardo Andrade](https://github.com/leoandradej)
- Icons by [Lucide](https://lucide.dev)
- Components by [shadcn/ui](https://ui.shadcn.com)

---

## 🖼 Bonus: Shields (Badges)

![Next.js](https://img.shields.io/badge/Next.js-black?style=flat&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Sanity](https://img.shields.io/badge/Sanity-F03E2F?style=flat&logo=sanity&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)
