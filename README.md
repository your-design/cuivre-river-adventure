# Cuivre River Adventure — Family Camping Guide

A Jekyll-based guide for a four-family summer camping trip to **Cuivre River State
Park** near Troy, Missouri — **July 1–7, 2026**.

Built with the [Just the Docs](https://just-the-docs.com/) theme. The site source
lives in [`docs/`](docs/) and deploys to **GitHub Pages** via GitHub Actions.

## What's inside

- **Park Info** — Lake Lincoln, campgrounds, trails, fishing, rules, contacts
- **Plan & Prepare** — game plan, reservations, the drive from Columbia, packing
  lists, camp setup, camp cooking, and savvy camper / RV tips
- **Things to Do** — kayaking, biking, fishing, swimming, hiking, wildlife
- **Food Plan** — meal schedule, make-ahead prep, master shopping list, and each
  family's preferences (from the idea book)
- **Daily Itinerary** — a loose day-by-day plan for July 1–7 (incl. a July 4 feast)
- **Kids at Camp** — boredom-busters plus **printable** activity sheets
- **Day Trips** — Troy, Winfield (Mississippi River), St. Charles, Hannibal, St. Louis

## Run it locally

Requires Ruby (3.x) and Bundler.

```bash
cd docs
bundle install
bundle exec jekyll serve --livereload
```

Then open <http://localhost:4000>. (On Windows, the `Gemfile` already includes
`tzinfo-data` and `wdm` so this works out of the box.)

Build a production copy without serving:

```bash
cd docs
bundle exec jekyll build       # outputs to docs/_site
```

## Deploy to GitHub Pages

Deployment is automated by [`.github/workflows/pages.yml`](.github/workflows/pages.yml):

1. Push to the **`main`** branch of the GitHub repo
   (`git@github.com:your-design/cuivre-river-adventure.git`).
2. In the repo: **Settings → Pages → Build and deployment → Source = GitHub Actions**.
3. The workflow builds `docs/` and publishes the site.

**Custom domain:** [`docs/CNAME`](docs/CNAME) is set to
`cuivre-river-adventure.your-design.app`. Point that DNS record at GitHub Pages, or
delete the file to use the default `*.github.io` URL. If you use a project URL
(no custom domain), the workflow injects the correct base path automatically.

## Project structure

```
.github/workflows/pages.yml   # GitHub Pages build & deploy
docs/
├── _config.yml               # Site configuration
├── Gemfile                   # Ruby dependencies (theme + plugins)
├── CNAME                     # Custom domain
├── index.md                  # Home
├── park-info.md              # Park overview
├── guides.md  + _guides/     # Plan & Prepare
├── activities.md + _activities/
├── meals.md   + _meals/      # Food plan
├── itinerary.md + _itinerary/
├── day-trips.md + _day_trips/
├── kids.md                   # Kids at Camp
├── _sass/                    # Custom colors & styles
└── assets/
    ├── images/               # Logo, hero, park photo
    └── printables/           # Print-ready kids' activity sheets (HTML)
```

## Printables

The kid activity sheets in `docs/assets/printables/` are self-contained HTML. Open one
in a browser and use **Print** (or **Save as PDF**). They're linked from the
**Kids at Camp** page.

## Credits & sources

- Park details from [Missouri State Parks](https://mostateparks.com/park/cuivre-river-state-park)
  and the Missouri Department of Conservation. **Verify current rules, fees, hours, and
  reservations before the trip.**
- Lake Lincoln photo: Wikimedia Commons (CC BY-SA). Logo and hero banner: custom illustrations.

---

*Park office: (636) 528-7247 · Reservations: [Missouri State Parks](https://icampmo1.usedirect.com/MoStateParksWeb/) · Tight lines and happy trails!*
