# LTR Minicab Landing Page Instructions

## What This Repo Is

Each HTML file is a self-contained set of WordPress shortcode-style page sections for an LTR Minicab landing page targeting a specific London area or station. The file `liverpool-street-station-minicab-transfers.html` is the canonical structure reference.

## Rules for Every New Page

### Structure
- Never change the section order or CSS class names.
- Sections in order: home-testimonials, home-why-choose-us, way-it-operates, home-prebook (with iframe map), ideal-rides, travel-options-comparison, home-fleet, home-personalized-rides, minicab-fare (fare table), home-london-airport (Meet & Greet), based-near (hotels), based-near (london areas), major-cities, landing-cta, home-faqs.
- `[theme_img ...]` and `[trustindex ...]` shortcodes stay exactly as-is.
- All booking links stay as `https://book.ltrminicab.com/`.

### Content
- Replace every mention of "Liverpool Street" / "Liverpool" with the new place name.
- All text must read as naturally written by a human. No em-dashes, no bullet-point lists that look like AI output, no repetitive sentence starters, no phrases like "In conclusion" or "It is worth noting".
- Vary sentence length. Mix short punchy sentences with longer descriptive ones.
- Pull real local detail: nearby landmarks, transport links, business districts, travel context specific to that area.

### Prices
- Look up real approximate fares on minicabit.com, minicabride.co.uk, and uber.com for the route from the new place to Heathrow Airport.
- Use those as the Saloon base price. Scale other vehicle types using these fixed uplifts from Saloon:
  - Executive: +£20
  - Estate: +£10
  - MPV 5: +£30
  - MPV 6: +£45
  - MPV 7: +£60
  - Executive MPV 7: +£85
  - MPV 8: +£100
- Return journey (Heathrow to the place) add £5 to every vehicle price.
- Round all prices to the nearest £5.

### FAQs
- Write 10 FAQs each time. Source question ideas from Google's "People also ask" for that area + Heathrow transfers, TripAdvisor threads, Reddit r/london, and Trustpilot reviews of minicab services.
- Never reuse the same FAQ questions from a previous page.
- Answers must be 2-3 sentences, conversational, no lists inside answers.

### Map iframe
- Update the Google Maps embed query to reflect the new place to Heathrow Airport, e.g.:
  `https://www.google.com/maps?q=PLACE+NAME+to+Heathrow+Airport&output=embed`

### Hotels section
- List 10 real hotels near the new area with real LTR Minicab hotel transfer URLs if they exist, otherwise use `https://ltrminicab.com/london-hotel-transfers/` as the href.

### London areas buttons
- Choose 10 London areas that are geographically relevant to the new place (nearby boroughs, common destinations from that area).

### File naming
- Use the pattern: `PLACE-NAME-minicab-transfers.html` (lowercase, hyphens, no spaces).

## SEO Keywords

Every page must weave these keywords in naturally. Never stuff them — use each one once or twice across the whole page where it fits the sentence. Do not italicise, bold, or mark them in any way that looks forced.

### Secondary Keywords (body copy and H2s)
Use the actual area name in place of {Area}:
- {Area} minicab service
- {Area} taxi service
- cheap minicab in {Area}
- affordable taxi in {Area}
- local minicab {Area}
- 24/7 minicab {Area}
- minicab near me {Area}
- book a minicab in {Area}
- pre-booked taxi {Area}
- fixed fare minicab {Area}
- reliable taxi {Area}

Spread these across the why-choose-us section, the ideal-rides section, the home-personalized-rides intro, and the landing-cta paragraph. Do not drop all of them into one section.

### Long Tail Keywords (FAQs and body paragraphs)
At least 6 of these must appear somewhere in the page, worked into natural sentences or FAQ answers:
- how much is a minicab in {Area}
- cheapest minicab in {Area}
- minicab from {Area} to London
- {Area} to Heathrow minicab
- {Area} to Gatwick minicab
- airport transfer from {Area}
- minicab from {Area} to city centre
- late night minicab {Area}
- minicab {Area} fixed price

### Trust and Intent Keywords (CTAs, meta copy, button labels, intro lines)
Use all of these at least once across the page:
- fixed fare
- no hidden charges
- meet and greet
- flight tracking
- 24/7 available
- pre-book online
- instant confirmation

These fit naturally in the way-it-operates section, the home-london-airport Meet & Greet section, the landing-cta, and inside FAQ answers.

### Keyword rotation rule
Each new page must use the keywords in different sentences and different sections compared to the previous page. Never copy a sentence from a previous page and just swap the place name. The surrounding phrasing must change every time.

## Simple Query to Use Every Time

When the user provides a place name, follow all the rules above and write the complete HTML file using the Liverpool Street file as the structural template. Commit and push to the active feature branch.
