# Internet2 Homepage Concept

A design concept for the Internet2 homepage, with an interactive national
backbone map and a scroll-driven motion system.

## Running it

Open `index.html` in any browser. That's it — no build step, no server, no
dependencies. The file is fully self-contained: the logo is an embedded data
URI, the map is inline SVG, and all CSS and JavaScript are inline. Nothing is
fetched from a CDN or any third-party host.

## What's on the page

| Section | Contents |
|---|---|
| Hero | Headline, three calls to action, interactive network map |
| 01 Services | Ten services as hairline-ruled rows, filterable from the nav search |
| 02 Get engaged | Community Engagement and Impact, Research Engagement, Events, Training, MS-CC |
| 03 Our purpose | Mission statement and four strategic values |
| 04 News | Three current stories from internet2.edu/news |
| CTA + footer | Contact prompt and site links |

An announcement ribbon for the 2027 Global Summit sits above the navigation.

## The map

The hero map is interactive, not decorative:

- Light pulses travel each of the 36 fiber segments. Travel time is scaled to
  segment length, so the whole network moves at one believable pace.
- All 24 nodes resolve to cities. Hovering or focusing one lights its own
  paths, dims the rest, and shows the city, its role and its path count.
- Philadelphia doubles as the 2027 Global Summit marker: white fill, its own
  beacon, and event details in place of the usual node label. It is a real
  link.
- A **Pause Motion** control sits on the map itself.

Node labels are illustrative. The city positions are plotted from real
coordinates, but "core node" and "regional connector" are concept copy, not
published topology, and the path counts simply describe the drawing.

## Accessibility

- Map nodes are keyboard-reachable, with labels and a polite live region.
- `prefers-reduced-motion` drops the light, beacons, parallax and scroll
  reveals, while leaving hover and focus exploration intact.
- Below 760px the map becomes decorative: no tab stops, no horizontal
  overflow.
- Verified in Chromium at 1680, 1440, 1280, 1100, 1080 and 900px, on iPhone
  SE, iPhone 13 and Pixel 7, under reduced motion, and by keyboard.

## Before this goes anywhere real

1. **Confirm the Summit hotel cut-off.** Internet2's own hotel page gives two
   different dates (March 1 and March 8, 2027). Neither is on this page, so
   nothing here is wrong — but the source should be fixed.
2. **Registration wording.** Every Summit call to action says *Save the date*,
   because the event site still reads "Register Coming Soon." These become
   *Register* once registration opens.
3. **Two links point at pages with no dedicated landing page.** Community
   Engagement and Impact goes to `/community/`, and Training goes to the
   training page linked from Research Engagement. Both should be repointed if
   dedicated pages exist.
4. **News categories.** The news listing doesn't expose a per-story category,
   so the eyebrows carry publication dates instead of topic labels.
5. **News stories go stale.** The three stories were current as of
   November 13, 2026.
6. **The Summit map marker needs ≥1100px.** Below that the hero map is already
   cropped and Philadelphia falls off the right edge. The ribbon carries the
   message at every width.

## Status

This is a design concept for review, not approved external copy. The strategic
messaging is drawn from draft material, and the structure is inspired by
Mozilla's editorial, product-first layout.
