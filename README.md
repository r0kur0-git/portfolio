# Arif — Portfolio (static version)

This is a static (no backend) version of the portfolio, built to run on GitHub Pages.

## Files

- `index.html` — Home page
- `work.html` — Work page
- `about.html` — About page
- `contact.html` — Contact page (sends messages via EmailJS)
- `assets/data.js` — Your projects and links live here

## How to add/edit a project

Open `assets/data.js` and add an entry to the `PROJECTS` array:

```js
{
  title: "Project name",
  description: "A short description.",
  medium: "3D · Blender",   // projects with the same medium group into a folder
  year: "2026",
  video: "",                // optional: a YouTube/Vimeo/direct video URL
  image: "images/your-image.jpg"
}
```

Upload the image file into an `/images` folder in this repo and reference it as
shown above (`images/your-image.jpg`), or link directly to an image already
hosted elsewhere.

## How to add/edit a link (shown on Home and Work)

Add an entry to the `LINKS` array in the same file:

```js
{ label: "Instagram", url: "https://instagram.com/yourhandle" }
```

## Changing the contact form's recipient emails

Open `contact.html`, find this block near the bottom, and edit the two values:

```js
var TO_EMAIL = 'arifaqmar10@gmail.com';
var CC_EMAIL = 'arifaqmar1011@gmail.com, theshadowmaster6@gmail.com';
```

## What's different from the AILA version

- No `/admin` page — edit `assets/data.js` / `contact.html` directly instead.
- No login system.
- The contact form still emails you via EmailJS, but submissions are no
  longer also saved to a database as a backup — check your email/spam
  folder if you're not seeing a message you expect.
- The project images currently in `assets/data.js` point to AILA's file
  storage URLs. Those will keep working independently of whether your AILA
  site is published, but consider downloading them and hosting them in an
  `/images` folder in this repo so this site doesn't depend on AILA at all.

## Publishing on GitHub Pages

1. Upload all these files (keeping the folder structure) to the repo.
2. Go to **Settings → Pages**.
3. Under "Source", pick the `main` branch and `/ (root)` folder, then save.
4. GitHub will give you a live URL, usually `https://<username>.github.io/<repo>/`.
