# Visual fidelity

Overall match: **33/100** — fonts, type sizes, spacing and each section measured in a browser on both sites, and how alike the pages look as pictures, each counted from what two unrelated pages score (0) to identical (100); the weaker of the two counts double, and so do the weakest page and device. How it's scored: docs/qa/import-fidelity.md.

**Next step:** The automatic move is rough (33/100): the words and pictures came across, but most of the design didn't. That's normal for custom-built sites. Claude can make it match closely: in Claude with the OpenSpace connector, use the finish-a-move prompt (or Studio's "Finish it with Claude"). It compares the old and new pages side by side and rebuilds what didn't come across, keeping every word and picture editable.

Scored two ways, side by side: **33/100 corrected**, 33/100 by the strict v3 scorer. The corrected score reads three things the strict one gets wrong (navigation in a header themed "brand", off-screen slides counted as columns, a picture-only band on a phone); the pages below list where it did.

Before auto-tuning: 39/100. What it changed:

- /contact: 2 sections joined into one, as on the original
- background on light sections #e9e6d2, as on the original (12 of 14 sections)
- /approach: "What meeting people where they are looks like.": 2 cards per row, as on the original
- /contact: "Find us, or reach us.": its background #15261a, as on the original
- /give: "Help us keep showing up.": its background #15261a, as on the original
- /approach: "Person first" set at the h3 size, as on the original
- /: section 1 "Meeting people where they are." recreated as a custom component
- /: section 5 "Small steps add up." recreated as a custom component
- /about: section 1 recreated as a custom component
- /about: section 2 "The team." recreated as a custom component
- /about: section 3 "We work with." recreated as a custom component
- /contact: section 1 "Find us, or reach us." recreated as a custom component
- /about: 3 section(s) at the content width, as on the original

Without custom components: 31/100; with the sections recreated as components: 33/100.

## / at 1440px — 68/100

Checks passed: 88% · screenshots 83% alike (two unrelated pages compare at about 55%).

Original: https://boulderfeetforward.org/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Newsreader Variable 88px | not found | **differs** |
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 2 size | 59.2px | 59.2px | same |
| Heading 3 size | 32px | 32px | same |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 18px | 18px | same |
| Lead text size | 41.6px | 41.6px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 16.3px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Navigation size | 16.3px | 16.3px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Content width | 992px | 992px | same |
| Section padding | 91px | 91px | same |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Meeting people where they are. | 88 | Heading: Newsreader Variable 88px → Playfair Display 88px; Image placement: center, 100% wide → none |
| 2 | When systems fail, people fall through the gaps. | 77 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Columns: 2 → 1 |
| 3 | We meet people where they are. Then we keep showing up. | 97 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px |
| 4 | There is no single pathway out of homelessness. | 79 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Image placement: left, 37% wide → none; Height: 1145px → 703px |
| 5 | Small steps add up. | 94 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Text: Newsreader Variable 41.6px → Playfair Display 41.6px |
| 6 | (no heading) | 80 | Height: 182px → 246px |
| 7 | Help us keep showing up. | 77 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Text: Newsreader Variable 36.8px → Playfair Display 41.6px |
| 8 | Hear from the park. | 97 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Adjust the stack column spans (image column) or the image's side.
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## / at 390px — 49/100

Checks passed: 86% · screenshots 79% alike (two unrelated pages compare at about 65%).

Original: https://boulderfeetforward.org/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Newsreader Variable 46.4px | not found | **differs** |
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 2 size | 33.6px | 34.3px | same |
| Heading 3 size | 23.2px | 23.4px | same |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 18px | 18px | same |
| Lead text size | 24.8px | 22px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 16.3px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 53px | 54px | same |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Meeting people where they are. | 73 | Heading: Newsreader Variable 46.4px → Playfair Display 70px; Image placement: center, 100% wide → none |
| 2 | When systems fail, people fall through the gaps. | 97 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px |
| 3 | We meet people where they are. Then we keep showing up. | 97 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px |
| 4 | There is no single pathway out of homelessness. | 79 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px; Image placement: center, 81% wide → none; Height: 1539px → 856px |
| 5 | Small steps add up. | 60 | Heading: Newsreader Variable 33.6px → Playfair Display 47px; Text: Newsreader Variable 24.8px → Playfair Display 33px |
| 6 | (no heading) | 80 | Height: 105px → 182px |
| 7 | Help us keep showing up. | 94 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px; Text: Newsreader Variable 24px → Playfair Display 22px |
| 8 | Hear from the park. | 97 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Adjust the stack column spans (image column) or the image's side.

## /about at 1440px — 73/100

Checks passed: 87% · screenshots 86% alike (two unrelated pages compare at about 55%).

Original: https://boulderfeetforward.org/about/  
Imported: /about (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Newsreader Variable 83.2px | not found | **differs** |
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 2 size | 59.2px | 59.2px | same |
| Heading 3 size | 32px | 32px | same |
| Body font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Body text size | 29.6px | 29.6px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 15.2px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Navigation size | 16.3px | 16.3px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Content width | 992px | 992px | same |
| Section padding | 75.5px | 122px | **differs** |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 96 | Text: Newsreader Variable 29.6px → Playfair Display 29.6px |
| 2 | The team. | 72 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Text color: #3f4f3b → #242018; Image placement: left, 24% wide → right, 23% wide; Image crop: 0.55:1 → 0.98:1 |
| 3 | We work with. | 97 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPadding = 76
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).

## /about at 390px — 45/100

Checks passed: 69% · screenshots 80% alike (two unrelated pages compare at about 65%).

Original: https://boulderfeetforward.org/about/  
Imported: /about (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Newsreader Variable 41.6px | not found | **differs** |
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 2 size | 33.6px | 47px | **differs** |
| Heading 3 size | 23.2px | 26px | **differs** |
| Body font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Body text size | 21.6px | 24px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 15.2px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 44.5px | 54.5px | same |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 96 | Text: Newsreader Variable 21.6px → Playfair Display 24px |
| 2 | The team. | 50 | Heading: Newsreader Variable 33.6px → Playfair Display 47px; Text: Atkinson Hyperlegible 18px → Atkinson Hyperlegible 14px; Text color: #3f4f3b → #242018; Image crop: 0.49:1 → 0.98:1 |
| 3 | We work with. | 60 | Heading: Newsreader Variable 33.6px → Playfair Display 47px; Text: Atkinson Hyperlegible 18px → Atkinson Hyperlegible 14px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h2.sizeMobile = 34
- choices.typography.scale.h3.sizeMobile = 23
- Site Styles → choices.typography.body = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Use the original's image proportions (the block's aspect ratio).

## /approach at 1440px — 63/100

Checks passed: 83% · screenshots 81% alike (two unrelated pages compare at about 55%).

Original: https://boulderfeetforward.org/approach/  
Imported: /approach (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 1 size | 83.2px | 88px | same |
| Heading 2 size | 59.2px | 59.2px | same |
| Heading 3 size | 32px | 25.7px | **differs** |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 18px | 18px | same |
| Lead text size | 21.6px | 25.7px | **differs** |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 16.3px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Navigation size | 16.3px | 16.3px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Content width | 992px | 992px | same |
| Section padding | 91px | 91px | same |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Person first | 77 | Heading: Newsreader Variable 32px → Playfair Display 32px; Text color: #3f4f3b → #242018; Height: 307px → 456px |
| 2 | Eight dimensions of wellness. | 79 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Image placement: left, 37% wide → none; Height: 993px → 546px |
| 3 | Small steps build stability. | 77 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Text: Atkinson Hyperlegible 18px → Playfair Display 41.6px |
| 4 | What meeting people where they are looks like. | 87 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Text color: #3f4f3b → #242018 |
| 5 | We stick around for the long haul. | 77 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Text: Atkinson Hyperlegible 18px → Playfair Display 41.6px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h3.size = 32
- choices.typography.scale.lead.size = 22
- Adjust the stack column spans (image column) or the image's side.

## /approach at 390px — 49/100

Checks passed: 86% · screenshots 79% alike (two unrelated pages compare at about 65%).

Original: https://boulderfeetforward.org/approach/  
Imported: /approach (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 1 size | 41.6px | 40.9px | same |
| Heading 2 size | 33.6px | 34.3px | same |
| Heading 3 size | 23.2px | 21px | same |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 18px | 18px | same |
| Lead text size | 21.6px | 22px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 16.3px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 53px | 54px | same |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Person first | 87 | Heading: Newsreader Variable 23.2px → Playfair Display 23.4px; Text color: #3f4f3b → #242018 |
| 2 | Eight dimensions of wellness. | 79 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px; Image placement: center, 81% wide → none; Height: 1385px → 730px |
| 3 | Small steps build stability. | 77 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px; Text: Atkinson Hyperlegible 18px → Playfair Display 22px |
| 4 | What meeting people where they are looks like. | 87 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px; Text color: #3f4f3b → #242018 |
| 5 | We stick around for the long haul. | 77 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px; Text: Atkinson Hyperlegible 18px → Playfair Display 22px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Adjust the stack column spans (image column) or the image's side.

## /contact at 1440px — 17/100

Checks passed: 77% · screenshots 48% alike (two unrelated pages compare at about 55%).

Original: https://boulderfeetforward.org/contact/  
Imported: /contact (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Newsreader Variable 83.2px | not found | **differs** |
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 2 size | 25.6px | 83.2px | **differs** |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 15.2px | 15.2px | same |
| Lead text size | 36.8px | 18px | **differs** |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 15.2px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Navigation size | 16.3px | 16.3px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Content width | 992px | 970px | same |
| Section padding | 217px | 307px | **differs** |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Find us, or reach us. | 79 | Heading: Newsreader Variable 83.2px → Playfair Display 83.2px; Text color: #3f4f3b → #37342b; Image placement: left, 6% wide → none |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h2.size = 26
- choices.typography.scale.lead.size = 37
- choices.layout.sectionPadding = 217
- Adjust the stack column spans (image column) or the image's side.

## /contact at 390px — 25/100

Checks passed: 71% · screenshots 70% alike (two unrelated pages compare at about 65%).

Original: https://boulderfeetforward.org/contact/  
Imported: /contact (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 1: present | Newsreader Variable 41.6px | not found | **differs** |
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 2 size | 25.6px | 67px | **differs** |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 15.2px | 14px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 15.2px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 169px | 93px | **differs** |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Find us, or reach us. | 64 | Heading: Newsreader Variable 41.6px → Playfair Display 67px; Text color: #3f4f3b → #242018; Image placement: left, 10% wide → none |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h2.sizeMobile = 26
- choices.layout.sectionPaddingMobile = 169
- Adjust the stack column spans (image column) or the image's side.

## /give at 1440px — 51/100

Checks passed: 72% · screenshots 77% alike (two unrelated pages compare at about 55%).

Original: https://boulderfeetforward.org/give/  
Imported: /give (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 1 size | 83.2px | 88px | same |
| Heading 2 size | 35.2px | 59.2px | **differs** |
| Heading 3 size | 20px | 25.7px | **differs** |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 18px | 18px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 16.3px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Navigation size | 16.3px | 16.3px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Content width | 992px | 992px | same |
| Section padding | 217px | 91px | **differs** |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Help us keep showing up. | 52 | Heading: Newsreader Variable 83.2px → Playfair Display 88px; Text color: #3f4f3b → #f5f2ec; Columns: 2 → 1; Image placement: left, 6% wide → none; Height: 2529px → 341px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h2.size = 35
- choices.typography.scale.h3.size = 20
- choices.layout.sectionPadding = 217
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.

## /give at 390px — 53/100

Checks passed: 79% · screenshots 82% alike (two unrelated pages compare at about 65%).

Original: https://boulderfeetforward.org/give/  
Imported: /give (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 1 size | 41.6px | 40.9px | same |
| Heading 2 size | 25.6px | 34.3px | **differs** |
| Heading 3 size | 20px | 21px | same |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 18px | 18px | same |
| Lead text size | 24px | 22px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 16.3px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 169px | 54px | **differs** |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Help us keep showing up. | 70 | Heading: Newsreader Variable 41.6px → Playfair Display 40.9px; Text color: #3f4f3b → #f5f2ec; Image placement: left, 10% wide → none; Height: 3418px → 291px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.h2.sizeMobile = 26
- choices.layout.sectionPaddingMobile = 169
- Adjust the stack column spans (image column) or the image's side.

## /impact at 1440px — 60/100

Checks passed: 82% · screenshots 80% alike (two unrelated pages compare at about 55%).

Original: https://boulderfeetforward.org/impact/  
Imported: /impact (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 1 size | 83.2px | 88px | same |
| Heading 2 size | 59.2px | 59.2px | same |
| Heading 3 size | 32px | 32px | same |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 16.3px | 18px | same |
| Lead text size | 41.6px | 41.6px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 16.3px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Navigation size | 16.3px | 16.3px | same |
| Navigation letter spacing and case | 0em, none | 0em, none | same |
| Content width | 992px | 992px | same |
| Section padding | 106px | 91px | same |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 38 | Text: Newsreader Variable 41.6px → Atkinson Hyperlegible 18px; Columns: 3 → 1; Height: 1681px → 832px |
| 2 | In their words. | 96 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px |
| 3 | How your donation helps us keep showing up. | 67 | Heading: Newsreader Variable 59.2px → Playfair Display 59.2px; Text color: #3f4f3b → #242018; Columns: 3 → 1 |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## /impact at 390px — 53/100

Checks passed: 91% · screenshots 80% alike (two unrelated pages compare at about 65%).

Original: https://boulderfeetforward.org/impact/  
Imported: /impact (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Newsreader Variable | Playfair Display (close stand-in) | close (85%) |
| Heading 1 size | 41.6px | 40.9px | same |
| Heading 2 size | 33.6px | 34.3px | same |
| Heading 3 size | 23.2px | 23.4px | same |
| Body font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Body text size | 16.3px | 18px | same |
| Lead text size | 24.8px | 22px | same |
| Label font | Atkinson Hyperlegible | Atkinson Hyperlegible | same |
| Buttons size | 16.3px | 16.3px | same |
| Buttons letter spacing and case | 0em, none | 0em, none | same |
| Section padding | 61.5px | 54px | same |
| Button corners | 999px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 75 | Text: Newsreader Variable 24.8px → Atkinson Hyperlegible 18px |
| 2 | In their words. | 96 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px |
| 3 | How your donation helps us keep showing up. | 87 | Heading: Newsreader Variable 33.6px → Playfair Display 34.3px; Text color: #3f4f3b → #242018 |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "Newsreader Variable" } (Google Fonts), or upload it in Site Styles → Your fonts.

