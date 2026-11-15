# Arrow Logic: Mind Master — legal pages

Live site: **https://daymonth.github.io/arrow-logic-mind-master-legal/**
Repository: `DayMonth/arrow-logic-mind-master-legal` (public, GitHub Pages from `main` / root).

These pages are the targets of the in-app Settings links (`LEGAL_BASE` in
`src/app/game.gd` of the game repository) and of the App Store Connect
**Privacy Policy URL** and **Support URL** fields, so they must stay publicly
reachable without a login.

| Published page | URL |
| --- | --- |
| `index.html` | `/` |
| `privacy-policy.html` | `/privacy-policy.html` |
| `terms-of-service.html` | `/terms-of-service.html` |
| `technical-support.html` | `/technical-support.html` |

To update: edit the page here, commit, push. GitHub Pages rebuilds
automatically; check `gh api repos/DayMonth/arrow-logic-mind-master-legal/pages --jq .status`
until it reports `built`, then reload the page.

Keep the filenames stable — the app and the store listings hard-code them.

## Notes on content

These pages are written **in English only** for every storefront, per project
decision, even though the app UI ships in English, Simplified Chinese,
Traditional Chinese, Japanese and Korean.

The statements about data practices must stay in sync with the build:

- no advertising SDK, no analytics SDK, no tracking, no account system;
- all progress stored locally in the app sandbox (no cloud save);
- Feedback opens the user's mail app with a `mailto:` draft;
- support address: `PatricioSergio476@gmail.com`.

If a future version adds ads, IAP, analytics or a backend, the Privacy Policy
(sections 1, 2, 10) and the Terms (section 4) must be updated in the same
release.
