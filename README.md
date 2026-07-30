# Arif — Portfolio

## Site link

```js
  https://r0kur0-git.github.io/portfolio/index.html
```

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

## Publishing on GitHub Pages

1. Upload all these files (keeping the folder structure) to the repo.
2. Go to **Settings → Pages**.
3. Under "Source", pick the `main` branch and `/ (root)` folder, then save.
4. GitHub will give you a live URL, usually `https://<username>.github.io/<repo>/`.
