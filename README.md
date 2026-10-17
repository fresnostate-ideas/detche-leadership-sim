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
