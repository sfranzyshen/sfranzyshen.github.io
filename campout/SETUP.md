# Campout for Compassion ... Website Setup

This is a working draft, intended for review before publication. The page uses the site's existing Jekyll Minimal layout.

## Preview
Once merged into master and published, the proposed page will be:
https://www.sfranzyshen.org/campout/

## Add the actual event logo
The draft displays a styled text wordmark. Upload the approved PNG logo into this directory as `logo.png`. Then replace the `header.hero` wordmark/city/tag elements with:
`<img src="{{ '/campout/logo.png' | relative_url }}" alt="Chico Campout for Compassion 2026" style="max-width:100%;height:auto;">`
Keep the event date and text below the logo.

## Add the public Google My Maps map
1. Go to https://www.google.com/maps/d/ while signed in as a map editor.
2. Create a map titled "Chico Campout for Compassion 2026 ... Participating Locations".
3. Add confirmed organizations only after they grant permission to list them.
4. You can have layers for "Confirmed Host", "Interested Organization", or "Public Information Site". Never mark private homes or sensitive youth gathering locations.
5. Set map visibility to Public view (but don't allow general public editing).
6. In the map's menu, select "Embed on my site" and copy the iframe.
7. Replace the `<div id="participant-map" ...>...</div>` placeholder with the iframe. Use `class="map-frame"` on the iframe for responsive styling.
Example (illustration only, not a valid active map):
`<iframe class="map-frame" title="Chico participating organizations" src="https://www.google.com/maps/d/embed?mid=YOUR_REAL_MAP_ID" loading="lazy"></iframe>`

Google guide: https://support.google.com/mymaps/answer/3109452

## Community conversation without participant accounts
Version 1: Visitors email their comment, and you publish approved, permission-granted submissions on the site. This is moderated and requires no additional login; it's not a live threaded discussion.

If you want live replies later:
- Hyvor Talk: optional guest commenting with no sign-up, hosted service (paid after trial), moderation.
- Remark42: free/open-source self-hosted service with optional anonymous commenting; requires your own running server separate from GitHub Pages.
- A visitor form service can let guests send submissions without logging in, but it still needs an external form backend. GitHub Pages cannot receive and store form submissions or comments by itself.

Do not choose Giscus or Utterances if you want visitors to comment without GitHub sign-in.

## Publish public resource PDFs
Host packet, age activities, and group invitation exist as completed PDFs outside this repository. Upload the approved PDFs in the `campout/` folder and replace the request-by-email copy with direct links. Do not claim downloads exist until those files are actually hosted.

## Event date
Saturday, November 14, 2026. Verify weather and individual host safety arrangements before promoting overnight participation.
