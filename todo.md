---
layout: default
title: Todo
published: false
---

# Site Improvements

## High Priority

- [x] **Delete `photos/featured/feature-01-original.jpg`** — the 8.5MB backup should not be committed to git; keep the original in Lightroom/Dropbox instead
- [x] **Add `feature-01-original.jpg` to `.gitignore`** — or add a blanket rule like `photos/featured/*-original.jpg` to protect against accidental commits of large originals
- [x] **Add `og:image` meta tag** — set `feature-01.jpg` as the Open Graph image in `_config.yml` so it shows as a preview card when the site is shared on social media or iMessage
- [x] **Fill out About page equipment** — add your camera body and primary lens to `about.md` so clients know what they're getting

## Content

- [ ] **Add client testimonials** — even 2–3 short quotes with first name and graduation year go a long way on the home page or packages page
- [ ] **Add a "How it works" section** to the home page or packages page: Book → Session → Delivery → Gallery. Sets clear expectations for first-time clients
- [ ] **Expand the gallery** — portrait section only has 3 images; aim for at least 6–8 to match graduation and lifestyle
- [x] **Add Instagram embed or link prominently** — currently only in the footer; consider a line in the gallery or home page pointing clients to recent work
- [ ] **Add turnaround time info** — clients often want to know when they'll receive their photos; add to FAQ or packages

## SEO & Performance

- [x] **Add `loading="lazy"` to all gallery `<img>` tags** in `gallery.md` — defers offscreen images and improves initial page load
- [ ] **Add structured data (JSON-LD)** — a `LocalBusiness` or `Photographer` schema block in `default.html` helps Google understand the business and surface it in local search
- [ ] **Add a sitemap** — enable the `jekyll-sitemap` plugin in `_config.yml` and `Gemfile` so Google can index all pages
- [ ] **Add `alt` text to all gallery images** — currently `alt="Graduation photo 1"` etc.; more descriptive text like `alt="UF graduation photo at Century Tower"` helps SEO and accessibility

## Booking & Contact

- [ ] **Add a Calendly or booking link** — the contact page currently has no inline booking; even a Calendly embed or button removes friction for ready-to-book clients
- [ ] **Add a response time note** to the contact page — e.g. "I typically respond within 24 hours" so clients know what to expect

## Housekeeping

- [x] **Add `_-original.jpg` pattern to `.gitignore`** to prevent future accidental commits of uncompressed originals
- [x] **Compress new photos before adding** — run `sips -Z 2400 --setProperty formatOptions 82 filename.jpg` on any new images before committing
