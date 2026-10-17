# In the Balance — XR Leadership Simulation

A short, browser-only branching case about academic technology leadership at a fictional university. Participants make four consequential decisions; the later situations depend on earlier choices. The ending offers narrative consequences and reflection, not a score.

## Publish on GitHub Pages

1. Create a new GitHub repository, for example `xr-leadership-lab`.
2. Upload `index.html`, `style.css`, and `app.js` to the repository root.
3. Open **Settings → Pages**, set **Build and deployment** to **Deploy from a branch**, and select `main` / `/ (root)`.
4. Open the GitHub Pages URL once deployment completes.

You can also preview it locally by opening `index.html` in a browser. No build step is necessary.

## Privacy / architecture

No network calls, database, authentication, analytics, third-party scripts, cookies, localStorage, or LLM calls. Decisions are held in memory for the current playthrough only and cleared on replay or page refresh.

## Edit the story

In `app.js`, edit `first` (opening decision), `nodes` (conditional scenes), `chooseNext()` (routing), and `finish()` (endings/debrief). Each playthrough has four decisions. If the participant declines to own the XR initiative, the story follows the leader into institutional consequences rather than stopping.

This is a fictionalized teaching scenario, not a compliance guide. Review campus legal/security/accessibility procedures before using any implementation claim as operational advice.

## Revision 2 notes

- Fixed literal quotation tags in stakeholder messages, including inline quotations.
- Added clearer speaker panels and an inline sender identity immediately above each communication.
- Added a permanent provost transition on eligible paths; the interim provost's limited funding authority is explicit.
- Reworked concluding outcomes to reflect all four decisions. Outcomes include a collapsed program, a stalled initiative, deliberate closure, a limited program, provisional renewal, and other consequences.
- Removed named cohort-speaker attribution from the participant-facing debrief.

The ending logic uses narrative flags to select plausible trajectories. It is intentionally not a validated predictive model.

## Typography

The site loads Fraunces (headings) and Source Sans 3 (interface and body text) from Google Fonts. It retains local system serif/sans-serif fallbacks if those resources are blocked or the visitor is offline. These font requests go to Google; no simulation decisions are sent or stored.


Typography v2: Fraunces is used on headings, questions and pull quotes; Source Sans 3 on body and controls. Fonts are fetched from Google Fonts when online. If deployed over an older version, hard-refresh the page to clear browser cache; `style.css?v=typography-2` is included to refresh the stylesheet.

## Opening illustration

The introductory scene uses `vr-headset1.jpeg` as a locally bundled, feathered background image (no third-party image request). Keep this file alongside `index.html` and `style.css` when publishing to GitHub Pages. The image is decorative; its context is supplied by adjacent text. Confirm you have appropriate rights to publish the image.


## Version 6 narrative revision
The permanent provost now explicitly prioritizes curriculum-wide AI integration over XR. The decision offers evidence-based advocacy, a 12–18 month off-ramp, or semester-end closure; each has a distinct consequence and ending, including doubts about independent judgment after a quick reversal.

## Version 7 narrative change
The permanent-provost scene now presents opposing staff perspectives (Rafael and Morgan) and replaces the extended off-ramp with a conditional faculty grant-funding path. The provost may permit a faculty-led application with strict support limits or refuse a proposal that requires institutional commitments.

## Version 9 narrative consistency pass

- CISO is Dr. Priya Nair; Morgan Chen remains the Academic Technology Specialist.
- Early failure remains a failed initiative, but the leader’s final response changes the aftermath.
- A reachable XR PROGRAM THRIVING ending now follows demonstrated instructional adoption, accessible design or shared faculty ownership, and a funded operating proposal.
- The end-of-year review clarifies interim provost limits; the reporting line remains directly to the provost.
- No scoring, accounts, data collection, or changes to the four-decision structure.
