# Campout for Compassion ... Website Setup

This is a working draft, intended for review before publication. The page uses the site's existing Jekyll Minimal layout.

## Preview
Once merged into master and published, the proposed page will be:
https://www.sfranzyshen.org/campout/

## Add the actual event logo
The draft displays a styled text wordmark. Upload the approved PNG logo into this directory as `logo.png`. Then replace the `header.hero` wordmark/city/tag elements with:
`<img src="{{ '/campout/logo.png' | relative_url }}" alt="Chico Campout for Compassion 2026" style="max-width:100%;height:auto;">`
Keep the event date and text below the logo.

## Public Google My Maps map

The website draft now embeds the provided map ID `14GtfNekVDUJ-1zj6plsSn1u6gdLKca4` from Google My Maps.
- Editor: https://www.google.com/maps/d/edit?mid=14GtfNekVDUJ-1zj6plsSn1u6gdLKca4
- Visitor: https://www.google.com/maps/d/viewer?mid=14GtfNekVDUJ-1zj6plsSn1u6gdLKca4
- Embedded: https://www.google.com/maps/d/embed?mid=14GtfNekVDUJ-1zj6plsSn1u6gdLKca4

Important: the map could not be independently viewed using a web fetch. Make sure the My Maps sharing settings allow public VIEWING, and test in a private/incognito browser window without signing in. Do NOT enable public editing.

To start the map in Chico, pan/zoom to the Chico region and choose `Set default view` from the map menu. This sets the initial extent but cannot confine visitors to city limits.

Add only confirmed, consenting organizations as pins. Do not publish private houses or exact youth overnight gathering sites without explicit permission.

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
