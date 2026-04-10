---
name: create-website
description: Scaffold and build a personal website project. Use when the user wants to create a personal website, portfolio, blog, or landing page.
user-invocable: true
allowed-tools: Bash(*) Write Read Edit Glob Grep
argument-hint: [project-name]
effort: high
---

# Create Personal Website

Help the user create a personal website project.

## Step 1: Gather Requirements

Ask the user the following (skip any they've already answered):

1. **Website type**: blog, portfolio, resume/CV, landing page, or hybrid?
2. **Theme**: dark mode, light mode, or auto-switch?
3. **Content sections**: e.g., About, Projects, Blog, Contact, Skills
4. **Tech stack preference**: or recommend one based on their experience level
5. **Deployment target**: Vercel, GitHub Pages, Netlify, or other?

## Step 2: Recommend Stack

Based on user's experience, suggest one of:

- **Beginner**: Astro + Tailwind CSS (simple, fast, markdown-friendly)
- **Intermediate**: Next.js + Tailwind CSS (React-based, flexible)
- **Advanced**: Nuxt / SvelteKit + Tailwind CSS

Default to **Astro + Tailwind CSS** if the user has no preference.

## Step 3: Scaffold Project

1. Create the project using the chosen framework's CLI
2. Set up dark mode with Tailwind CSS `darkMode: 'class'`
3. Create the requested content sections as pages/components
4. Add responsive design (mobile-first)
5. Include basic SEO meta tags
6. Set up a clean project structure

## Step 4: Add Content Placeholders

- Add placeholder text and sections the user can easily customize
- Include comments marking where to add personal info
- Set up any blog/markdown support if requested

## Step 5: Verify & Run

1. Install dependencies
2. Run dev server to verify it works
3. Show the user how to access and customize it

## Style Guidelines

- Default to dark mode with a modern, minimal aesthetic
- Use a consistent color palette (e.g., slate/zinc backgrounds, accent color)
- Smooth transitions and subtle animations
- Clean typography with good readability
- Responsive across all screen sizes

## Project Structure Example (Astro)

```
$ARGUMENTS/
├── src/
│   ├── components/
│   ├── layouts/
│   ├── pages/
│   └── styles/
├── public/
├── astro.config.mjs
├── tailwind.config.mjs
└── package.json
```
