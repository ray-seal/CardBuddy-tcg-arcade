# CardBuddy TCG Arcade

A static prototype for testing a virtual card-collecting mini-game alongside CardBuddy. Built with plain HTML, CSS and JavaScript so it runs on GitHub Pages without a framework or build process.

## Prototype features

- CardBuddy-inspired booster art and pack-opening animation.
- Loads the English Pokémon 151 card pool from the public TCGdex API.
- Five-card pack opening, with rarity-weighted demo selection.
- Virtual collection, duplicate counts, search and sorting.
- Earnable coins with a daily mission cap.
- Local browser save and a reset that affects only this prototype.

## Publish on GitHub Pages

1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch `main` and folder `/(root)`, then click **Save**.
4. Wait for GitHub to publish the site. The expected project URL is `https://ray-seal.github.io/CardBuddy-tcg-arcade/`.

GitHub's guide: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Testing checklist

- [ ] Open the Pages URL on a phone.
- [ ] Confirm the TCGdex status reports a loaded card pool.
- [ ] Open a pack and confirm five cards reveal.
- [ ] Check new cards and duplicate counts.
- [ ] Refresh and confirm the local collection persists.
- [ ] Claim missions and verify the daily cap.
- [ ] Reset the test save and confirm physical binders are unaffected.
- [ ] Try opening a pack while offline; failed pulls should refund the coins.

## Known limitations

- **Local-only save:** coins and virtual collection are stored in this browser's local storage. They do not sync across devices or accounts.
- **Prototype odds:** rarity weighting is invented for testing and is not official booster collation or pack odds.
- **API dependency:** the pack pool requires internet access and the public TCGdex API. If it is unavailable, pack opening is blocked until the catalogue loads.
- **No trading or battles yet:** first validate the pack → reveal → collection loop.
- **Not a secure economy:** browser storage and client-side random selection must not be reused for multiplayer trading, battles, leaderboards, or coin stakes.
- **IP and asset review:** Pokémon names, card data and images belong to their respective rights holders. Review the TCGdex terms and relevant Pokémon IP requirements before broader publication or any commercial use.

This is an unofficial fan-made experiment and is not affiliated with or endorsed by Nintendo, Creatures, GAME FREAK, or The Pokémon Company.
