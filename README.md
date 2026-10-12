# Precision & Recall: The Angler's Dilemma

A self-contained, zero-dependency HTML teaching game about the precision vs. recall
tradeoff, built for a non-technical audience. The entire game is `index.html` — open
it in any browser, no build step.

**Play it:** https://tim-marlowe-snapdocs.github.io/the-anglers-dilemma/

## Editing

`index.html` is the single source of truth. GitHub Pages serves it from the root of
`main`, so **merging to `main` publishes automatically** (first build takes a minute).

Work on branches, not directly on `main`:

```sh
git switch -c tweak-bass-round      # new branch
# edit index.html, test by opening it locally in a browser
git commit -am "Rebalance Trophy Bass round"
git push -u origin tweak-bass-round
gh pr create --fill                 # open a PR
# merge the PR -> main -> site redeploys
```

To preview locally just open the file (`open index.html`) — it needs no server.
