# movienight (legacy host)

Served at `https://sudo-acraciun.github.io/movienight/`.

**Do not delete this repository, and do not turn off GitHub Pages for it.**
Everything here exists only to keep URLs alive that are already out in the
world and cannot be recalled.

## What is still load-bearing

| File | Why it cannot go |
|---|---|
| `index.html` | Deep-link redirector for shared titles. Its URL is baked into every share message sent from older app builds, so those links live on in people's chat histories indefinitely. Newer builds link to `ilikemovies.app/share`. |
| `privacy-policy.html` | Redirect stub. |
| `terms.html` | Redirect stub. |
| `delete-account.html` | Redirect stub. |

## The legal pages moved

The three documents now live on the presentation site:

- https://ilikemovies.app/privacy
- https://ilikemovies.app/terms
- https://ilikemovies.app/delete-account

Source of truth is `movies-agent-static-website/src/pages/`. **Edit them there.**
The files here are stubs and hold no policy text.

They stay because the old addresses are compiled into every app build that has
not taken an over-the-air update, and an install that is never updated never
stops existing. A stub costs nothing; a dead link inside a shipped app is a
Play policy problem.

GitHub Pages serves static files and cannot issue a 301, so each stub uses a
zero-delay `<meta http-equiv="refresh">` for the reader plus `<link
rel="canonical">` to consolidate the address for crawlers.

## If a policy changes

Edit the pages in the website repo. Nothing in here needs touching.
