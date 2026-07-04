# UK Cities Minicab Service — Links Reference

Reusable list of city names and their `book-a-minicab-in-<city>` landing page URLs.
Use these in "Other Major Cities We Serve" / nearby-cities link sections on future landing pages.

| City | URL |
|---|---|
| Leicester | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-leicester/ |
| Islington | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-islington/ |
| Coventry | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-coventry/ |
| Hull | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-hull/ |
| Wolverhampton | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-wolverhampton/ |
| Newcastle | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-newcastle-upon-tyne/ |
| Preston | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-preston/ |
| Sutton | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-sutton/ |
| Milton Keynes | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-milton-keynes/ |
| Aberdeen | https://ltrminicab.com/uk-cities-minicab-service/book-a-minicab-in-aberdeen/ |

Used in: `luton-airport-to-st-pauls-ec4m-minicab-transfers.html` ("More UK Towns and Cities We Reach From Luton Airport" section).

## Landing page format notes (for future "Airport to Area" pages)

Based on feedback while building the St Paul's EC4M page, apply these rules to every future Luton/Stansted/Heathrow "to area" landing page generated from the standard template:

- Keep the section structure and CSS identical; only rewrite text content per destination.
- Every `<h2>` in every section, including the CTA, must be freshly worded per page. Never reuse a heading verbatim from a previous page.
- FAQs must be reworded and reordered per page, not copy-pasted from the last page.
- Write body copy in plain natural sentences, no em dash or hyphen used as a sentence connector (hyphenated compound words like "door to door" are fine written without the hyphen too).
- Pull the saloon car fare from the SEO comparison price sheet's SEO column for that specific route, then derive the other seven vehicle fares using the same ratios as the reference example (Executive ~1.35x, Estate ~1.15x, MPV5 ~1.47x, MPV6 ~1.74x, MPV7 ~2.0x, Exec MPV7 ~2.41x, MPV8 ~2.71x saloon; return fares use the same pattern off the return saloon price).
- Mention the specific postcodes and small sub-areas that fall under the destination area, not generic City/London copy.
- Vary hyperlink anchor text across pages, do not reuse the same keyword phrase for the same link target every time.
- The day hire section heading and copy should name the specific destination area and reference a different secondary airport (e.g. Stansted) for variety instead of always repeating the primary origin airport.
- "Other Major Cities We Serve" section should use the city list above.
- Ship a companion `<page-name>.json` file alongside every landing page HTML file, containing a `FAQPage` JSON-LD block that mirrors the page's FAQ accordion word for word, plus a `Service`/`LocalBusiness`/`Offer` block listing every vehicle fare (outward and return) from the fixed-price fare table. Keep the filename identical to the HTML file's basename with a `.json` extension.
