# Paws and Effect

A one-page timeline of a dog's first two years. It shows brain stages, body
limits, normal bad behavior, where the dog can safely go, and what to train. A
red line marks today.

The chart is a schedule, not an advice column. An entry gets a bar only if it
can say when it becomes true and when it stops being true. That allows three
shapes: a window that opens and closes, a restriction that lifts at a given
week, and a single dated event. Titles name the window, so you can say it out
loud: "she is in her fear period", "he started teething".

Advice that is true at every age is not a schedule, so it is not here at all.

All 53 bars cite the source they came from. The citation is in the detail
panel, under the description.

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
- **A prompt to start.** On the first visit a dialog asks for the date of birth,
  already filled in with the default. It is the only place the page says
  "start here", and it does not come back after you answer it or skip it.
- **Sources on every entry.** Open any bar to see where its dates come from.

## The six sections

| Section | What it holds |
|---|---|
| Brain & stages | Windows in brain development, such as socialization and adolescence. |
| Body & vet | Vaccines, parasites, teeth, growth plates, weight, and neutering. |
| What you will see | Normal, unwelcome behavior, and when to expect it. |
| Body limits & safety | How much the growing body can take, week by week. |
| Places & other dogs | Where the dog can go, and which dogs it can meet. |
| Training & household | The window in which to establish each skill. |

## Files

| File | What it is |
|---|---|
| `index.html` | The whole site. All the CSS and JavaScript are inline. |
| `favicon.svg` | The tab icon. It has two palettes and changes with the browser theme. |
| `favicon-32.png`, `apple-touch-icon.png` | Raster copies of the icon, rendered from `favicon.svg`, for browsers that do not accept an SVG icon. |
| `.nojekyll` | Tells GitHub Pages to copy the files as they are. |
| `sitemap.xml` | One entry, for search engines. |
| `social-card.png` | The 1200x630 preview image for links shared on social sites. |

The timeline data is the `GROUPS` array near the top of the script in
`index.html`. Each entry has a title, a start week, an end week, a description,
optional shape flags, and one or two sources.

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

## Search engines

The page declares a canonical URL, a description, Open Graph and Twitter card
tags, and `WebApplication` structured data. `sitemap.xml` holds the one URL.

Two things live outside this repository:

- `robots.txt` is served from the root of `grantwilk.com`, which is a different
  repository. It already permits crawling.
- The root sitemap does not list this page, so submit
  `https://grantwilk.com/paws-and-effect/sitemap.xml` in Google Search Console,
  and add a link to this page from the portfolio site. A link from a page
  Google already crawls is the fastest way to get indexed.

## Where the dates come from

Each entry cites one or two sources, and the page links to all of them. The
sources are of three kinds:

- **Veterinary guidelines**, for medical timing. AAHA, WSAVA, AVMA, AVSAB, the
  Companion Animal Parasite Council, and the American Heartworm Society.
- **Peer-reviewed studies**, for behavior and for growth.
- **Named, experienced trainers and certifying bodies**, for training timing.
  Training research often does not give a week number, and good trainers do.

Content marketing from pet retailers and pet food companies is not used.

These ages are typical ranges, not deadlines. Small breeds mature near the early
end of each range, and giant breeds near the late end. Vaccination dates, spay
or neuter dates, and joint readiness are veterinary decisions. Use those bars as
questions for your vet, not as instructions.
