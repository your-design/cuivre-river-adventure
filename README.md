# Eleven Mile State Park Family Adventure Guide

A comprehensive Jekyll-based travel guide for a multi-generational family camping trip to Eleven Mile State Park, Colorado.

## Overview

This guide covers everything needed for a 7-night RV camping trip in June/July:
- Pre-trip preparation and altitude acclimation
- Packing lists for all family members
- Reservation strategies for multiple sites
- Road trip entertainment for all ages
- Camp setup and cooking guides
- Activities: fishing, hiking, kayaking, backpacking, wildlife watching
- Day trip guides to nearby attractions
- Complete 7-day itinerary

## Quick Start

### Local Development

```bash
# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

### GitHub Pages Deployment

1. Push to a GitHub repository
2. Enable GitHub Pages in repository settings
3. Select the main branch as source
4. Site will be available at `https://yourusername.github.io/repo-name`

## Structure

```
├── _config.yml          # Site configuration
├── index.md             # Home page
├── guides.md            # Guides section index
├── activities.md        # Activities section index
├── day-trips.md         # Day trips section index
├── itinerary.md         # Itinerary section index
├── _guides/             # Pre-trip and camp guides
├── _activities/         # Activity-specific guides
├── _day_trips/          # Day trip destination guides
├── _itinerary/          # Day-by-day schedule
├── _sass/               # Custom styling
└── assets/              # Images, PDFs, etc.
```

## Adding Content

### New Guide

Create a new `.md` file in the appropriate collection folder:

```yaml
---
layout: default
title: "Guide Title"
parent: Guides
nav_order: 8
---

# Guide Title

Content here...
```

### Images

Place images in `assets/images/` and reference them:

```markdown
![Alt text](/assets/images/filename.jpg)
```

## Theme

This site uses [Just the Docs](https://github.com/just-the-docs/just-the-docs), a documentation-focused Jekyll theme.

## License

Content is provided for personal family use. Park information is derived from public sources. Always verify current regulations with Colorado Parks and Wildlife before your trip.

## Contact

- **Eleven Mile State Park:** (719) 748-3401
- **Camping Reservations:** 1-800-244-5613
- **Park Website:** https://cpw.state.co.us/state-parks/eleven-mile-state-park

---

*Safe travels and tight lines!*
