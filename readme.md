# Pro #1 Inspections — consolidated website review

This is a complete replacement for the current Netlify deployment. All eight HTML pages use the same shared `styles.css`, `script.js`, header, navigation, and footer.

## Publish without changing your Wix embed
1. Extract this ZIP file.
2. Open your **existing** Netlify project `radiant-tanuki-b48c58`.
3. Open **Deploys** and manually deploy the extracted folder that contains `index.html` at its top level.
4. Wait for the deploy to publish.
5. Visit `https://radiant-tanuki-b48c58.netlify.app/` and hard refresh.
6. Check the Wix embed in both desktop and mobile preview. Wix controls the outer iframe height.

## Included pages
Home, Services, About Us, Contact Us, Pricing, Get a Quote, FAQ, Sample Report.

## Consolidated improvements
- Centered desktop navigation, larger 16px menu text, direct single-click menu links.
- Shared sticky header, mobile menu, and footer across all eight pages.
- Consistent hero, section headings, cards, spacing, and call-to-action treatments.
- Additional practical information on every page, including inspection selection, preparation, scope, and next steps.
- More useful FAQ coverage, with insurance and report caveats.
- Keyboard skip-to-content link and clear focus styling.
- Internal relative links checked against included HTML files.

## Important factual and technical limitations
- Uses the owner's requested **Certified Home Inspector** wording; does not claim Certified Master Inspector.
- Confirm actual certification, insurance, inspection services, and coverage areas before publication.
- No invented pricing, customer reviews, years of experience, or turnaround guarantees.
- No sample report PDF was provided; the page explains how to request one.
- External Spectora scheduling and request URLs are configured but their booking flow has not been end-to-end tested.
- The live Netlify site returned 401 to the remote checker, so a real-browser QA pass remains necessary.
- Wix's Embed a Site iframe can create nested scrolling. The sticky header is sticky within the embedded document, not the parent Wix page.
- Static HTML is intentionally used: no backend forms or fake form submissions.

## Suggested manual acceptance tests
1. Desktop: verify menu is visually centered and sticky while scrolling the embedded content.
2. Mobile: open and close the hamburger menu; check no horizontal clipping.
3. On every page: click Home, Services, About Us, Contact Us.
4. Open Pricing, FAQ, Sample Report, and Get a Quote from the footer.
5. Verify phone tap-to-call, Schedule Now, and Request Inspection destinations.
6. Verify no extra scrollbar or blank area in the Wix desktop/mobile embeds.
