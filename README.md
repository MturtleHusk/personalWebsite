# Mitchell Freedman — Personal Website

A hand-built, framework-free personal site. Three files, no build step, no dependencies.

```
index.html    — structure & content (edit your text here)
styles.css    — all styling (edit your colors at the very top)
script.js     — animations, theme toggle, mobile menu
```

## Run it
Just open `index.html` in a browser. That's it — no installs.

## Change the colors  ⭐
Open `styles.css`. The first block (section **1. COLOR PALETTE**) holds every
color as a CSS variable. Change a value and the whole site updates. Example:

```css
--accent: #c0552f;   /* change this one line to re-skin links, buttons, highlights */
```

There's a matching `[data-theme="dark"]` block right below for dark mode.

## Edit your content
Open `index.html` and look for `PLACEHOLDER` comments. Update:
- Hero name, kicker, and one-liner
- About bio + the quick-facts list
- Work items (duplicate a `<li class="work-item">` for each project; set its `href`)
- Experience entries
- Skills chips
- Contact email + social links (set each `href`)

## Make the contact form work
The form is wired to a placeholder. To receive messages:
1. Create a free form endpoint (e.g. [Formspree](https://formspree.io)).
2. In `index.html`, set the form's `action` to your endpoint URL.
3. In `script.js`, delete block **7** (the preview-only handler) so the form submits normally.

## Host it (free options)
Drag the folder into **Netlify Drop**, push to **GitHub Pages**, or deploy with **Vercel** / **Cloudflare Pages**.

---
Built from scratch — no Bootstrap, no templates.
