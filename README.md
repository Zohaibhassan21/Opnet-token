# Ebook Sales Website

A one-page website for selling an ebook. It's a single `index.html` file with no build step and no frameworks, so you can host it anywhere for free.

The page currently uses a sample book, **The Balcony Harvest**, as placeholder content. Replace it with your own book's details.

## Sections

1. Sticky header with a **Buy** button
2. Hero: headline, pitch, drawn book cover, price badge
3. Stats strip (chapters, pages, extras)
4. "Sound familiar?": the problems your book solves
5. "What you'll be able to do": six outcomes
6. Table of contents (expandable parts and chapters)
7. "Look inside": sample pages, scrollable sideways
8. Who it's for / not for
9. Meet the author
10. Get your copy: price card, what's included, refund promise
11. FAQ
12. Free sample chapter signup
13. Footer and a sticky buy bar on phones

## 1. Set price, buy link and email (one place)

At the bottom of `index.html`, edit:

```js
const BOOK = {
  price: "$19",
  buyUrl: "https://gumroad.com/",   // your Gumroad / Payhip / Lemon Squeezy / Amazon link
  email: "hello@example.com",
  signupEndpoint: ""                // optional: Formspree / ConvertKit / Mailchimp form URL
};
```

Every buy button, price and email address on the page updates from these values.

## 2. Replace the text

Search `index.html` for these and change them:

| Find | Replace with |
| --- | --- |
| `The Balcony Harvest` | your book title |
| `R. Linden` / `RL` | your name / initials |
| Hero `<h1>` and the paragraph under it | your headline and pitch |
| `.stats` numbers | your chapter/page counts |
| Chapter lists in `#inside` | your table of contents |
| `#author` section | your bio and social links |
| FAQ answers | your answers |

## 3. Use your real cover and photo (optional)

- **Cover:** replace the `<div class="cover">…</div>` block with
  `<img class="cover" src="cover.jpg" alt="Your book cover">` and add `object-fit:cover` to `.cover` in the CSS.
- **Author photo:** replace `<span>RL</span>` inside `.portrait` with `<img src="me.jpg" alt="Your name">`.

## 4. Change colours

Edit the variables at the top of the `<style>` block (`--marigold` is the button colour and `--ink` is the main text colour, `--band` is the tinted section background). The site always uses the light theme.

## Hosting (free)

- **GitHub Pages:** in the repo, go to Settings → Pages → Deploy from branch, select the branch and `/ (root)`.
- **Netlify / Vercel / Cloudflare Pages:** import the repo. There's no build command, and the publish directory is `/`.
- **Custom domain:** add it in your host's domain settings.

## Originality

All design, layout code, illustrations and text here are original. No text, images, fonts or code from any other site were copied. Fonts are free Google Fonts (Bricolage Grotesque, Figtree, IBM Plex Mono) under the SIL Open Font License.
