# Email Portfolio

Robert Dorheim, email developer. Portfolio site with hand-coded HTML email templates.

## What this is

A single-page portfolio site: a hero intro, about, experience, a work grid of email projects, a web development section, skills, FAQ, and a contact form.

## Live site

https://robert-dorheim.dev

## What's inside

```
email-portfolio/
├── index.html              Portfolio page (hero, about, work, skills, contact)
├── assets/images/           Site images (headshot, tool/platform icons)
├── assets/css/site.css      Compiled Tailwind CSS (generated, commit it)
├── src/input.css            Tailwind entry file
├── tailwind.config.js       Tailwind config (scans index.html)
├── llms.txt                 Plain-text summary for AI assistants
└── email-projects/          Three standalone HTML email templates
    ├── ecommerce-upsell/    Fungi Perfecti Extracts Email
    ├── newsletter/          Warhammer 40K News
    └── transactional/       MyProtein Order Confirmation
```

Each folder under `email-projects/` is a self-contained HTML email with its own `assets/images/`, built the way real marketing and transactional email has to be built: tables, inline styles, and Outlook conditional markup, not a regular webpage layout.

## Running it locally

The site is static and deploys as-is. The compiled CSS is committed, so you only need Node when you change Tailwind classes in `index.html`:

```
npm install
npm run build   # regenerates assets/css/site.css
```

To view it, either:
- open `index.html` directly in a browser, or
- serve the folder with a simple local server, e.g. `python3 -m http.server` or `npx serve`, then visit the address it prints.

## Tech

Plain HTML, CSS, and JavaScript. No framework.
- Tailwind CSS 3, compiled to a static stylesheet (`npm run build`)
- Lucide icons via CDN
- EmailJS for the contact form

## About the email projects

Each email under `email-projects/` is a personal recreation of a promotional email from my own inbox, built to practice and show my work. Not client work. Not affiliated with or endorsed by the brands shown.
