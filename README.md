# Monterey Bay Region Web Review

An independent review of **mby.pca.org**, the website of the Monterey Bay Region of the
Porsche Club of America, prepared for the region board in August 2026, together with a
working prototype of the recommended redesign.

**Live pages**

| Page | What it is |
|---|---|
| `index.html` | Overview and entry point |
| `report.html` | The review: 11-area audit, 8-club benchmark, three costed options, 30/60/90 plan |
| `prototype.html` | Eleven working screens of the proposed site, mobile first, plus a design rationale and a WordPress template map |

## Headline recommendation

Keep WordPress, keep the pca.org address, keep the existing on-site booking system, and
fix what is already there. Do not rebuild and do not replatform. PCA National hosts the
site free of charge, so there is no annual bill to reduce by moving, only one to create.
The region's on-site event registration is better than all eight benchmarked peer clubs,
and both a rebuild and a replatform put it at risk.

## Two things to know before reading

**1. The review here is the public edition.** Three findings that named specific unpatched
software on a live site that takes card payments have been generalised, because these pages
are public. Every score, figure, cost and recommendation is unchanged. The board holds the
full version. Once the first 30 days of updates in the roadmap are applied, the distinction
stops mattering.

**2. The prototype is a mockup.** Nothing on it submits, charges, or connects to anything.
The forms are inert. The screen switcher and width buttons in the grey bar at the top are
review scaffolding and are not part of the design.

## Images and assets

- The region crest in `assets/` was supplied by the board and converted to transparent PNG.
- Every photograph in the prototype is **hot-linked from the region's own media library** at
  `mby.pca.org/wp-content/uploads/`, credited to the member who took it. Nothing is copied
  into this repository. If a photo is renamed or moved on the live site, that slot will break.
  To make the prototype fully self-contained, download the images and change the `src`
  attributes to local paths.
- Sponsor logos are the sponsors' own marks, shown to credit them, exactly as the live site does.
- Three slots remain labelled placeholders because no real asset exists yet: the four board
  portraits, the meeting-point map, and a webstore product shot.
- Photograph-to-article pairing on the news screen is illustrative in one case (the SLO Coastal
  Escape card uses a coastal tour photograph from a different date).

## Can this be pushed into WordPress?

Not as-is. These are static HTML pages, not a WordPress theme. The prototype is a **design
specification**, and the build note at the foot of `prototype.html` maps every screen to the
WordPress template that would produce it inside the site's existing bootscore child theme,
with Events Manager Pro left exactly where it is. Two things change on the way in:
the `@container` queries become ordinary `@media` queries, and the status rail on each event
reads live booking data instead of fixed values.

## Trademarks

Monterey Bay Region is a chartered region of the Porsche Club of America and is not affiliated
with, endorsed by, or connected to Dr. Ing. h.c. F. Porsche AG or Porsche Cars North America.
Porsche and the Porsche Crest are trademarks of Dr. Ing. h.c. F. Porsche AG and are not used on
these pages. Photographs and sponsor logos remain the property of their owners and appear here
for review purposes.

---

`robots.txt` disallows crawling and every page carries a `noindex` tag, so these pages are
reachable by link but should not appear in search results.
