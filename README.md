# lusomaniac-games.xyz

The website for Lusomaniac Games: plain files, no build step. Put the **contents of this folder** at the root
of a GitHub repository and publish it with GitHub Pages.

| Address | File |
|---|---|
| https://lusomaniac-games.xyz/ | `index.html` |
| https://lusomaniac-games.xyz/app-ads.txt | `app-ads.txt` (AdMob) |
| https://lusomaniac-games.xyz/cosus/ | `cosus/index.html` |
| https://lusomaniac-games.xyz/cosus/privacy/ | `cosus/privacy/index.html` (Play Console privacy policy URL) |
| https://lusomaniac-games.xyz/cosus/privacidade/ | `cosus/privacidade/index.html` (Portuguese) |

`CNAME` tells GitHub Pages the domain; `.nojekyll` makes it serve the files as they are.

**Before publishing:** replace `[YOUR FULL NAME]` / `[O TEU NOME COMPLETO]` in both privacy pages (the GDPR asks
for the name of whoever is responsible for the data). When the app is on Google Play, swap the "Coming soon" box
in `cosus/index.html` for the store link.

## Publish with GitHub Pages

1. GitHub → New repository (public), e.g. `lusomaniac-games.xyz`. Upload everything in this folder, including
   `CNAME` and `.nojekyll` (in the upload page, drag the files; hidden files may need "Add file › Create new file").
2. Repository → Settings → Pages: Source "Deploy from a branch", branch `main`, folder `/ (root)`.
   Custom domain: `lusomaniac-games.xyz` → Save.
3. Namecheap → Domain List → Manage → Advanced DNS:
   - A Record, Host `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153` (four records)
   - CNAME Record, Host `www`: `<your-github-username>.github.io.`
   - remove any "URL Redirect" or parking records for `@` / `www`. **Keep the Google MX records** (e-mail).
4. When GitHub shows the domain check as successful (minutes to a few hours), tick **Enforce HTTPS**.
5. Check https://lusomaniac-games.xyz/app-ads.txt shows the one line, and the privacy page opens.

In Play Console use `https://lusomaniac-games.xyz` as the developer website (it must match the app-ads.txt
domain) and `https://lusomaniac-games.xyz/cosus/privacy/` as the privacy policy.
