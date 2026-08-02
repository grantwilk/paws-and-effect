# Paws and Effect

What your dog can handle, week by week.

This is a one-page timeline of a dog's first two years. It shows brain stages,
body limits, normal bad behavior, what is safe to do, and what to train. A red
line marks today.

Live site: https://grantwilk.com/paws-and-effect/

## Features

- **Live today line.** The page reads the real clock and moves the today marker.
  It also reads the date again when you return to the tab, so a page left open
  overnight is correct in the morning.
- **Your own birth date.** Enter any date of birth. The page saves the date in
  your browser, so it is still there when you return. The default is
  May 18, 2026.
- **Light and dark themes.** The page follows your system setting. You can also
  select light or dark with the button in the header.
- **Phone and desktop layouts.** Wide screens get the full scrolling timeline.
  Phones get a stacked view with the same bars, the same today line, and the
  same detail text.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole site. All the CSS and JavaScript are inline. |
| `favicon.svg` | The tab icon. It has two palettes and changes with the browser theme. |
| `favicon-32.png`, `apple-touch-icon.png` | Raster copies of the icon, rendered from `favicon.svg`, for browsers that do not accept an SVG icon. |
| `.nojekyll` | Tells GitHub Pages to copy the files as they are. |

## Running it locally

The site has no build step. Open `index.html` in a browser, or serve the
folder:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000/.

## Deployment

GitHub Pages serves the `main` branch from the repository root. A push to `main`
publishes the site. The `.nojekyll` file tells Pages to copy the files as they
are, without a Jekyll build.

This repository is a project site. It inherits the custom domain of the user
site at `grantwilk.github.io`, so it is published under `grantwilk.com` and not
under `github.io`. The `github.io` address still works and redirects.

## Writing style

The text of the page follows ASD-STE100 Simplified Technical English. The rules
that matter most here:

- Maximum 20 words in an instruction, and 25 words in a description.
- One instruction per sentence, and the condition before the command.
- Active voice. The only modal verbs are "can", "will", and "must".
- One word for one meaning. The page says "make sure" and never "check",
  "verify", or "confirm".
- No names, and no pronouns for the dog. The text says "the dog" or
  "the puppy", so any reader can use the page for any dog.

## A note on the content

These ages are typical ranges, not deadlines. Vaccination dates, spay or neuter
dates, and joint readiness are veterinary decisions. Use those bars as questions
for your vet, not as instructions.
