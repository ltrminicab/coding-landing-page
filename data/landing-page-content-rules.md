# Rules for generating airport-to-area minicab landing pages

Reference: `luton-airport-to-hoxton-n1-minicab-transfers.html` and `mercure-london-heathrow-minicab-transfers.html` for structural examples. `data/uk-cities-minicab-links.json` holds reusable city links for the "Other UK Cities" section.

## Structure
Keep the same section order and CSS structure as the reference pages: review strip, fixed-price table (first section after the banner), six feature cards, route overview + map, transport comparison table, day hire / hourly booking, corporate and group travel, fleet carousel, baby and child seat section, personalized rides icon grid, full fares table, nearby hotels, other UK cities served, nearby postcodes/areas, landing CTA, FAQs.

## Pricing
- Use the saloon car fare for the route as the base figure.
- Derive other vehicle prices from the saloon fare using these ratios: Executive x1.35, Estate x1.15, MPV5 x1.47, MPV6 x1.74, MPV7 x2.0, Exec MPV7 x2.4, MPV8 x2.7.
- The return-direction saloon fare is the forward fare plus roughly £10; scale the other vehicles the same way for the return row.
- If an actual SEO comparison price sheet figure is supplied for the saloon car, always use that figure instead of estimating.

## Content rules
- Write unique, area- and postcode-specific content each time (mention the actual postcode, nearby streets, stations, and landmarks). Do not just swap the area name into identical sentences.
- Do not increase content length beyond what the reference pages use for each section.
- Write in a natural, human style. Do not use en dashes or em dashes in headings or body text.
- Vary section headings on every page. Never reuse the exact heading wording from a previous page.
- Vary FAQ questions and wording every time; do not repeat the same FAQ set across pages.
- Vary the anchor text/keywords used for hyperlinks across pages instead of reusing the same button labels every time.
- The day hire section heading and description must name both the real airport for that route and the specific area/postcode being served, not a different airport.
- Add any new UK city name + link the user provides to `data/uk-cities-minicab-links.json` so it can be reused in future "Other UK Cities We Serve" sections.
