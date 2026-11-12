# Cart for One: Ebook Website

The sales page for **Cart for One**, the ebook from the YouTube channel *Cart for One with Bev*. It's a single `index.html` file with images in `assets/`. There's no build step, so it can be hosted anywhere for free.

Live site (GitHub Pages): https://zohaibhassan21.github.io/Opnet-token/
Buy link (Gumroad): https://zohaibh0.gumroad.com/l/cart-for-one

## Change price, buy link or YouTube link

At the bottom of `index.html`:

```js
const BOOK = {
  price: "$12",
  buyUrl: "https://zohaibh0.gumroad.com/l/cart-for-one",
  youtubeUrl: "https://www.youtube.com/..."   // your channel link
};
```

If you change the price on Gumroad, change it here too.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole website |
| `assets/cover.jpg` | Book cover used on the site |
| `assets/page-*.jpg` | Sample pages shown in "Look inside" |
| `assets/gumroad-cover.png` | 1280×720 cover image for the Gumroad product page |
| `assets/gumroad-thumbnail.png` | 600×600 thumbnail for Gumroad |

**The ebook PDF is deliberately not in this repository.** The repo is public, so anyone could download the book here for free. Keep the PDF on your computer and upload it only to Gumroad.

## Hosting

GitHub Pages: Settings → Pages → Deploy from a branch → select this branch and `/ (root)`.

## Originality

All design, code, text and illustrations are original. Fonts are free Google Fonts (Fraunces, Lexend, IBM Plex Mono) under the SIL Open Font License. Bev is a fictional AI presenter, and the site says so.
