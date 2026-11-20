# Persona

A Pinterest-style gallery for AI characters and brands, made by human creators.
Front-end MVP: static HTML/CSS/JS, no build step.

## Pages
- `#home`: masonry feed of every pin, filter by Characters / Brands
- `#noor`, `#kai`, `#maison`: profiles (AI badge, creator credit, stats, Created / Boards tabs)
- Click any pin to open the detail view (prompt, tags, link to profile)

## Content
All data lives in the `characters` array at the top of the `<script>` in `index.html`.
Images are Unsplash photos (free Unsplash license), loaded from `images.unsplash.com`.
To use your own images, replace the photo IDs, or change the `U()` helper to point at your own CDN.

## Run locally
Open `index.html` in a browser, or:

    npx serve .

## Deploy
    gh repo create persona --private --source . --push
    npx vercel --prod

Or import the GitHub repo at vercel.com/new (framework preset: Other, no build command).
