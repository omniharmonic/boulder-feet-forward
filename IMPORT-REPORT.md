# Import report: Boulder Feet Forward

Imported from https://boulderfeetforward.org on 2026-11-05 with `openspace import url`.
Sources: page HTML. 18 requests.

## Summary

- **11** pages, **0** collection items in 0 collection(s)
- **3** media files (0.3 MB) downloaded into `media/`
- **0** redirects so old addresses keep working
- **3** item(s) need your attention (below)

## Pages

| Old address | OpenSpace | Title | Sections | Blocks |
| --- | --- | --- | ---: | ---: |
| `/` | `/` | Home | 8 | 22 |
| `/approach` | `/approach` | Approach | 6 | 12 |
| `/work` | `/work` | Work | 3 | 6 |
| `/impact` | `/impact` | Impact | 4 | 8 |
| `/volunteer` | `/volunteer` | Volunteer | 4 | 5 |
| `/about` | `/about` | About | 3 | 8 |
| `/contact` | `/contact` | Need help? | 2 | 2 |
| `/give` | `/give` | Help us keep showing up. | 5 | 12 |
| `/work/weekly-outreach` | `/work/weekly-outreach` | All are welcome. | 4 | 6 |
| `/work/peer-support` | `/work/peer-support` | Support from someone who has been there. | 3 | 5 |
| `/work/case-management` | `/work/case-management` | The long game, at your pace. | 4 | 9 |

## Design

The look was recreated with OpenSpace's own design system (Site Styles tokens, section color themes, layouts and section presets), not by copying the original site's CSS or code.

- Brand color #a7c25a (the site's accent color).
- Fonts on the original site: Newsreader Variable / Atkinson Hyperlegible → pairing "Fraunces & Hanken Grotesk" (Fraunces / Hanken Grotesk), the closest curated match. Licensed fonts can be uploaded in Site Styles → Fonts.
- Type scale on the original site: Heading 1 is 4.9× body text (very large; OpenSpace's display preset is the nearest). Density "comfortable" from the section heights.
- Fonts on the original site kept as they are (Atkinson Hyperlegible): free on Google Fonts, self-hosted with the site.
- Newsreader Variable (a licensed font) can't be copied, so Playfair Display — the closest measured shape (x-height, width) among free fonts — stands in. With a web licence, upload the real font in Site Styles → Your fonts.
- Type scale on the original site (the live site, measured in a browser) kept: display 88px/46.4px, heading 1 88px/46.4px, heading 2 59.2px/33.6px, body 18px/18px.
- Page rhythm on the original site (the live site, measured in a browser): content 992px wide, sections padded 91px (53px on phones) — kept in Site Styles.
- The contrast solver adjusted 3 color pairing(s) so every section theme meets WCAG AA (e.g. light accent, light accent-hover).
- Page background #e9e6d2 on the original site → #fcfaf5 (text contrast 15.5:1).

Design check: 0 error(s), 9 warning(s).

- warning (/): Four sections in a row use the light color theme, so the page reads as one long block.
- warning (/approach): Service description is 52 words; this layout is designed for 8–40.
- warning (/approach): Service description is 58 words; this layout is designed for 8–40.
- warning (/approach): Service description is 48 words; this layout is designed for 8–40.
- warning (/approach): Four sections in a row use the light color theme, so the page reads as one long block.
- warning (/give): Four sections in a row use the light color theme, so the page reads as one long block.
- warning (/work/case-management): “Housing assessments and Coordinated Entry” jumps from Heading 1 to Heading 3, skipping a level.
- warning (site): Your menu links to “find-us” on Need help?, but no section there is called that.
- warning (/): A button on Home links to “give-things” on Help us keep showing up., but no section there is called that.

## Needs attention

### Forms and newsletter

- Newsletter signup recreated. The old site didn't keep a subscriber list itself: if its form sent sign-ups to an email service, export the list there and import it in the Hub. _(/, footer)_

### Pages that couldn't be read

- No sitemap; pages were found by following the site's own links. _(/sitemap.xml)_

### Design

- Layout: "Meeting people where they are.": its background #e9e6d2, as on the original. _(/)_
- Layout: "When systems fail, people fall through the gaps.": its background #e9e6d2, as on the original. _(/)_
- Layout: "We meet people where they are. Then we keep showing up.": its background #e9e6d2, as on the original. _(/)_
- Layout: "There is no single pathway out of homelessness.": its background #e9e6d2, as on the original. _(/)_
- Layout: "Small steps add up.": its background #e9e6d2, as on the original. _(/)_
- Layout: "Help us keep showing up.": its background #e9e6d2, as on the original. _(/)_
- Layout: "Hear from the park.": its background #e9e6d2, as on the original. _(/)_

## Not moved by the importer

- Scripts, animations and anything rendered only by JavaScript (try `--render` for script-built pages).
- Server-side features: shops, logins, search, comments.
- Form submissions, newsletter subscribers, member accounts and comments.
- Analytics and SEO history (search engines follow the redirects).

## Next steps

1. `npm install`, then `npx openspace check` (it should report no errors) and `npx openspace dev` to look around.
2. Bring it to visual parity with Claude: in this folder run `claude`, then `/openspace:migrate https://boulderfeetforward.org` (or ask Claude to compare each page with the original). It screenshots both sites at desktop and mobile and adjusts presets, Site Styles and sections — never raw HTML.
3. Fix the items under **Needs attention**, then publish (push to GitHub, or `publish` with Claude).
4. Move the domain only after the new site is live and checked:
   - add the custom domain in OpenSpace (`deploy.customDomain` in `openspace.json`, or the Hub);
   - at your DNS provider (your registrar or elsewhere), point the records at the new host as the domain guide says (GitHub Pages: `A`/`CNAME` records; Cloudflare: the Pages project's records);
   - keep the old hosting until the new site serves your domain over HTTPS and the redirects work; then cancel it (and transfer the domain if you like).

