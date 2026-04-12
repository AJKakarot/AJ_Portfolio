# AJ Portfolio

Personal developer portfolio by Ajeet Gupta. It is a Next.js application with TypeScript, focused on clear presentation of projects, experience, and writing.

## Features

- Next.js App Router with server and client components where appropriate
- TypeScript across the codebase
- Tailwind CSS and shadcn-style UI primitives for layout and components
- Blog section backed by MDX-style content and markdown processing
- Theme switching (light and dark) via `next-themes`
- Motion-based UI polish using Framer Motion / Motion
- ESLint for code quality

## Tech stack

| Area | Choice |
|------|--------|
| Framework | [Next.js](https://nextjs.org/) 14 (App Router) |
| Language | [TypeScript](https://www.typescriptlang.org/) |
| Styling | [Tailwind CSS](https://tailwindcss.com/), Radix primitives, `class-variance-authority`, `tailwind-merge` |
| Content | MDX-related pipeline (`react-markdown`, `remark`, `rehype`, `gray-matter`) |
| Animation | [Framer Motion](https://www.framer.com/motion/), Motion |
| Icons | [Lucide React](https://lucide.dev/) |

Deployment is typically done on [Vercel](https://vercel.com/) or any Node host that supports Next.js.

## Repository layout

```
AJ_Portfolio/
├── public/                 # Static assets (images, media, SVGs)
├── content/                # Markdown / MDX content for the blog
├── src/
│   ├── app/                # App Router: layout, home, blog routes
│   ├── components/         # Shared UI (cards, navbar, MDX, magicui, ui)
│   ├── data/               # Structured data (for example resume content)
│   └── lib/                # Utilities
├── next.config.mjs
├── tailwind.config.ts
├── tsconfig.json
└── package.json
```

## Getting started

Prerequisites: Node.js 18 or newer and npm, pnpm, or yarn.

```bash
git clone https://github.com/AJKakarot/AJ__Portfolio.git
cd AJ__Portfolio
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in the browser.

Other scripts:

- `npm run build` – production build
- `npm run start` – run the production server (after `build`)
- `npm run lint` – run ESLint

## Environment

If you add API keys or service credentials, use `.env.local` and keep them out of version control. Files matching `.env*.local` are ignored by Git per `.gitignore`.

## Author

**Ajeet Gupta** — full-stack developer with emphasis on Next.js, TypeScript, and modern web applications.

## License

This project is released under the terms of the [MIT License](LICENSE). You may use and modify it for personal or commercial work according to that license.
