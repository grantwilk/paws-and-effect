# Paws and Effect

A one-page timeline of a puppy's first two years. It shows brain stages, body
limits, normal bad behavior, what is physically safe to do, and what to train,
week by week. A red line marks today.

Live site: https://grantwilk.github.io/paws-and-effect/

## Features

- **Live today line.** The page reads the real clock and moves the today marker.
  It also re-checks the date when you return to the tab, so a page left open
  overnight is correct in the morning.
- **Your own birth date.** Enter any date of birth. The page saves it in your
  browser, so it is still there when you come back. The default is May 18, 2026.
- **Light and dark themes.** The page follows your system setting. You can also
  force light or dark with the toggle in the header.
- **Phone and desktop layouts.** Wide screens get the full scrolling timeline.
  Phones get a stacked view with the same bars, the same today line, and the
  same detail text.

## Running it locally

The site is one static HTML file with no build step. Open `index.html` in a
browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000/.

## Deployment

GitHub Pages serves the `main` branch from the repository root. A push to `main`
publishes the site. The `.nojekyll` file tells Pages to copy the files as they
are, without a Jekyll build.

To use a custom domain:

1. Add a `CNAME` DNS record at your DNS provider. Point it at
   `grantwilk.github.io`.
2. In Settings, then Pages, enter the domain in the "Custom domain" field.
3. When the certificate is ready, turn on "Enforce HTTPS".

## A note on the content

The ages are typical ranges, not deadlines. Vaccination timing, spay or neuter
timing, and joint readiness are veterinary decisions. Treat those bars as
questions for your vet, not as instructions.
