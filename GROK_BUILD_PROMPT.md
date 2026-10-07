# Grok Build Prompt — Beach Jam 2026 Link Hub (paste this entire document into Grok)

**How to use:** Open Grok → start a new Build / Apps chat → paste everything below the line → publish publicly → copy the live `*.grok.me` URL into your site builder as an iframe.

---

## Build request

Build and publish a single-page public web app titled **Beach Jam 2026 Link Hub** for Stabilize Revitalize Fort Pierce (SRFP).

Preferred live slug: `beach-jam-2026-links.grok.me` (or the closest clear public name).

### Purpose

A clickable sitemap / link hub. Every visitor sees **all fifteen** saved Beach Jam 2026 links as cards/buttons, grouped by category. Embeddable as an **inline iframe** on the nonprofit website. Responsive. No login. No invented links.

### Brand (match SRFP / media kit)

Reference live kit for tone and assets: https://srfp-media-kit.grok.me/

Pull colors/fonts from the Stabilize Revitalize Fort Pierce site / kit. Use this palette if the kit does not expose CSS vars cleanly:

| Token | Hex |
|---|---|
| Navy | `#0c598c` |
| Blue | `#0082ed` |
| Deep blue | `#0050c7` |
| Teal accent | `#26a69a` |
| Mist | `#c0d9d9` |
| Sand background | `#f4f7f8` |
| Ink text | `#212121` |
| Muted text | `#5a6a75` |

Fonts (Google Fonts): **Roboto** for UI, **Lora** for headings.

Look: calm coastal nonprofit — clean cards, generous whitespace, not dark mode, not flashy. Prior SRFP Grok apps for style reference: https://srfp-media-kit.grok.me/ and https://beach-jam-competitor-map-2026.grok.me/field

### Event facts (hero)

- Presenter: Stabilize Revitalize Fort Pierce
- Event: Pick, Paddle & Play Beach Jam 2026 (2nd Annual)
- Date: Saturday, November 14, 2026
- Time: 10 AM – 8 PM
- Place: Causeway Cove Marina, Fort Pierce
- Admission: FREE CONCERT

### Exact fifteen links — do not add, remove, or rewrite URLs

**Press (1)**
1. WQCS News — https://www.wqcs.org/wqcs-news/2026-10-01/free-pick-paddle-play-beach-jam-returns-to-fort-pierce-nov-14

**Community calendars (6)**
2. Treasure Coast Today — https://treasurecoast.today/events/55cf247f6b8c6e353e-free-concert-beach-jam-2nd-annual-pick-paddle-play-beach-jam.html
3. WQCS Community Calendar — https://www.wqcs.org/community-calendar/event/2nd-annual-pick-paddle-amp-play-beach-jam-14-09-2026-14-51-09
4. Palm Beach Illustrated — https://www.palmbeachillustrated.com/community-calendar/#/details/2nd-annual-pick-paddle-play-beach-jam-2026/19507140/2026-11-14T10
5. Fun 4 Space Coast Kids — https://fun4spacecoastkids.com/calendar/eventdetail/125329/364/pick-paddle-and-play-beach-jam-2026
6. Vero Vine — https://verovine.com/events/free-concert-2nd-annual-pick-paddle-play-beach-jam/
7. Indian River Magazine — https://indianrivermagazine.com/events/free-concert-pick-paddle-play-beach-jam-2026/

**Directories (3)**
8. AllEvents — https://allevents.in/fort-pierce/2nd-annual-pick-paddle-and-play-beach-jam-2026/100001994110097983
9. HappeningNext — https://happeningnext.com/event/2nd-annual-pick-paddle-andamp-play-beach-jam-2026-eid1ef0l2kq81wr
10. FestivalNet — https://festivalnet.com/102376/Fort-Pierce-Florida/Festivals/Pick,-Paddle-and-Play-Beach-Jam-2026

**Local (1)**
11. TreasureCoast.com — https://treasurecoast.com/pick-paddle-play-beach-jam/

**Owned (4)**
12. Official Beach Jam page — https://stabilizerevitalizefortpierce.org/pick-paddle-and-play-beach-jam
13. Eventbrite — https://www.eventbrite.com/e/2nd-annual-pick-paddle-play-beach-jam-2026-tickets-1994110097983
14. Facebook Event — https://www.facebook.com/events/1613049523602926
15. SRFP Media Kit — https://srfp-media-kit.grok.me/

### Layout

1. Hero band with presenter, H1 event name, short blurb, chips for date/time/place/FREE CONCERT
2. Category jump nav (Press · Community calendars · Directories · Local · Owned)
3. Five sections with H2 headings; each link is a clickable card (title + one-line description + open cue)
4. Footer: Stabilize Revitalize Fort Pierce · free admission · Causeway Cove Marina

Cards open in a new tab (`target="_blank"` `rel="noopener noreferrer"`).

### SEO / crawlability (required)

- **Pre-rendered / server-rendered static HTML** — all 15 links AND all category headings MUST appear in the initial HTML source (no JavaScript-only rendering of the link list)
- `robots.txt`: `User-agent: *` / `Allow: /` / `Sitemap:` pointing at this app’s `sitemap.xml`
- `sitemap.xml` for the app root URL
- `<title>` and `<meta name="description">` in `<head>` (also set `og:title`, `og:description`, `canonical` to the live URL)
- Semantic HTML: `<main>`, `<header>`, `<nav>`, `<section>`, `<h1>`/`<h2>`, lists (`<ul>`/`<li>`) for cards
- Clean public URL (not a hash-router SPA as the only content path)
- `meta robots` index,follow
- Still iframe-friendly (no frame-busting; works when embedded on stabilizerevitalizefortpierce.org)

Suggested title: `Pick, Paddle & Play Beach Jam 2026 — Link Hub | Stabilize Revitalize Fort Pierce`

Suggested description: `All fifteen live Beach Jam 2026 links: press, community calendars, directories, local pages, Eventbrite, Facebook, and the official Stabilize Revitalize Fort Pierce event page. Free concert Nov 14 at Causeway Cove, Fort Pierce.`

### Deliverable

Publish publicly and return the live hosted URL Roger can paste into his site builder iframe.

---

## Optional: ready-made HTML

If Grok Build can host a static file, use the companion `index.html`, `robots.txt`, and `sitemap.xml` in this same repository (update canonical/sitemap host to the final `*.grok.me` URL after publish).
