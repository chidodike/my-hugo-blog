# UI polish (branch `ui-polish`) — review before merge

Staged only. Live site stays on `main` until this PR is merged.

## Changes
1. Removed ghost/empty nav item and empty Categories link; nav is Posts · Tags · About (chido.me)
2. Real favicon / apple-touch / header mark (`CD` monogram)
3. Default Open Graph image: `/og-default.png` (from existing `home-2026.png`)
4. Shorter site title: **Chido Dike**
5. Better meta description + keywords
6. Clearer home intro blurb
7. Show post covers on home/list pages
8. Added LinkedIn; kept X + GitHub
9. Removed placeholder Google Analytics (`UA-123-45`) and fake site-verification tags

## How to preview without merging
- Review the diff in this PR
- Optional: check out this branch locally and `hugo server`
- Merge to `main` only when happy — that updates blog.chido.me
