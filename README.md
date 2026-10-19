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

### Version 10 narrative change
The permanent-provost AI pivot offers a conditional choice to ask Dr. Brooks to advocate for XR when prior decisions established her as a faculty champion. She respectfully declines due to upcoming tenure review. The President's award is referenced only if it occurred earlier on that path. The path leads to a distinct faculty-advocate-withdrawal outcome, without an additional decision or any change to privacy settings.


## Brand and accessibility (Version 11)

The fictional Ash Creek University uses burgundy `#714b55` and blue `#084aae` as brand accents. Both are used with appropriate contrasting text; muted foreground text was darkened. Focus moves to the new scene heading, consequence heading, or outcome heading as the interface changes. The progress indicator includes a text equivalent.

This version is designed toward WCAG 2.1 AA and includes accessibility-oriented corrections. Automated source and contrast checking is **not a conformance certification**. Before public deployment, test all branches in a browser with keyboard only, screen readers (VoiceOver + Safari and NVDA + Firefox or Chrome), zoom/reflow at 200% and 400%, and automated tools such as axe DevTools. In particular, verify focus movement and announcements when dynamic content changes, and verify each branch's text and contrast. The ADA Title II rule uses WCAG 2.1 AA; see https://www.ada.gov/resources/2024-03-08-web-rule/.


## Version 12 interface update
- Start Over control in the header during play and on the ending. Confirmation clears the current local session and returns to the opening. No individual decision can be undone.
- Reduced redundant masthead, intro and footer copy. Existing narrative, branching, local-only behavior and typography remain unchanged.


## Version 13 visual layer

- Scene-specific documentary photography is loaded from `images/`. The opening image now also reads from `images/vr-headset1.jpeg`; an unchanged root copy remains for compatibility.
- Narratives and all decision logic are preserved from Version 12. The new visual mapping only chooses photographs and the correspondence/in-person appearance of existing scenes.
- Photographs are atmospheric/decorative and intentionally have empty alternative text. Speaker names, roles, and decisions remain text.
- External Google Fonts remain the only externally loaded site resource. No analytics or other network calls were introduced.


### V14 interface and scenario changes
- Removed duplicate case labels, small scene numbers, and confusing message-medium tags in the narrative pane.
- Reduced photography to three context-setting moments; the opening and conclusion retain their visuals.
- Added a fourth, defensive response to Rafael's post-failure conversation with a distinct leadership consequence.

### Version 15
- Added a fourth, intentionally self-protective option to Dr. Simone Vale's Faculty Senate scene. It routes to a fourth decision with Dr. Park about a misrepresented Senate/provost conversation, followed by distinct outcomes.
- Restyled the post-choice consequence as a bordered, high-contrast result panel to prevent it disappearing visually before Continue.

### Version 16 narrative routing fix
- When the director recommends against taking over XR and does not reverse course into a limited pilot, the third decision now involves faculty learning of the recommendation, rather than an unrelated Senate mandate concern.
- Deflecting blame onto Dr. Park triggers a fourth decision about correcting, hedging, or doubling down on the funding story, with distinct ending consequences.
- Senate governance dilemmas remain available on active XR initiative paths.


## Version 17 opening copy

The opening briefing now foregrounds leadership purpose, competing priorities, and uncertainty, and no longer introduces Dr. Park before the story. All decision logic, styling, and other content remain unchanged from Version 16.


## Version 18 — Introductory framing and campus identity
The introduction now separates the leadership reflection from the fictional XR case using a divider and the Ash Creek University logo (`images/ash-creek-logo-nobg-2.png`). No simulation logic changed.

## Version 19 opening attribution

The opening screen includes a project credit linking to the Fresno State Office of IDEAS. The credit is contained within the opening `#intro` section and is not displayed during play or on the ending screen.

## Version 20 opening composition
The XR photograph now accompanies the Ash Creek scenario introduction, below the university logo, rather than the general leadership philosophy. The rest of the narrative and branching are unchanged.
