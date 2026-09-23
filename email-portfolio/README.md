# Email Portfolio

Robert Dorheim, email developer. Portfolio site with hand-coded HTML email templates.

## What this is

A single-page portfolio site: a hero intro, an about section, a work grid of email projects, a skills summary, and a contact form.

## Live site

https://robert-dorheim.dev

## What's inside

```
email-portfolio/
├── index.html              Portfolio page (hero, about, work, skills, contact)
├── assets/images/           Site images (headshot, tool/platform icons)
└── email-projects/          Three standalone HTML email templates
    ├── ecommerce-upsell/    Fungi Perfecti Extracts Email
    ├── newsletter/          Warhammer 40K News
    └── transactional/       MyProtein Order Confirmation
```

Each folder under `email-projects/` is a self-contained HTML email with its own `assets/images/`, built the way real marketing and transactional email has to be built: tables, inline styles, and Outlook conditional markup, not a regular webpage layout.

## Running it locally

This is a static site with no build step. Either:
- open `index.html` directly in a browser, or
- serve the folder with a simple local server, e.g. `python3 -m http.server` or `npx serve`, then visit the address it prints.

## Tech

Plain HTML, CSS, and JavaScript. No framework, no build step.
- Tailwind CSS via CDN
- Lucide icons via CDN
- EmailJS for the contact form

## About the email projects

Each email under `email-projects/` is a personal recreation of a promotional email from my own inbox, built to practice and show my work. Not client work. Not affiliated with or endorsed by the brands shown.
