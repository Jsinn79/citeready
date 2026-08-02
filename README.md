# CiteReady site — what to fill in before you launch

Seven files. Open each in any text editor (or GitHub's web editor on your phone) and replace the
ALL-CAPS placeholders. Nothing else needs touching.

## Files
- `index.html` — sales page
- `mini-check.html` — free 3-prompt check (your lead engine)
- `sample-audit.html` — the real sample audit (your credibility)
- `about.html` — you
- `thank-you.html` — post-payment page (Stripe redirects here)
- `legal.html` — Privacy / Terms / Refund, linked as `legal.html#privacy`, `#terms`, `#refund`
- `style.css` — shared styling; edit `--brand` to change the accent color

## Find-and-replace, every file
| Placeholder | Replace with |
|---|---|
| `YOUR_EMAIL@gmail.com` | your real support email |
| `[Your Name]` / `[Your Legal Name]` | your name |
| `STRIPE_LINK_FOUNDING` | Stripe Payment Link for the $147 founding audit |
| `STRIPE_LINK_AUDIT` | Stripe Payment Link for the $197 audit |
| `TALLY_FORM_URL_MINI_CHECK` | Tally embed URL for the free-check form |
| `TALLY_FORM_URL_INTAKE` | Tally embed URL for the post-purchase intake form |
| `SAMPLE_AUDIT_PDF_EMBED_URL` | Google Drive `/preview` link for your redacted sample audit |
| `SAMPLE_AUDIT_PDF_DOWNLOAD_URL` | Drive download link for the same PDF |
| `[DATE]`, `[City, State, Country]`, `[Your State/Country]`, `[Your County/State]` | in `legal.html` |

## Real content to add (do not launch without these)
1. **Hero screenshot** — replace the striped placeholder in `index.html` with a real screenshot of an
   AI assistant naming competitors. Save it in this folder as `proof.png` and swap the `<div class="placeholder">`
   block for `<img src="proof.png" alt="...">`. Keep the prompt visible in the image.
2. **Your photo** — replace the `PHOTO:` circles in `index.html` and `about.html` with a real headshot.
3. **Sample audit scores** — fill the real numbers into the pillar table in `sample-audit.html`. Placeholder
   numbers there cancel out every other trust signal on the site.
4. **Loom embed** — swap the video placeholder in `sample-audit.html` for your Loom or unlisted YouTube embed.
5. **Testimonial** — one real line from your volunteer client, or delete the blockquote entirely.
6. **Cloudflare Web Analytics** — paste the snippet where each file says `ANALYTICS:` (all 6 HTML files).

## Publishing free on GitHub Pages
1. Create a GitHub account (username becomes your web address).
2. New public repository named `<username>.github.io`.
3. Upload all seven files to the repo root (the web upload works fine from a phone).
4. Settings → Pages → Source: `main`, folder `/ (root)` → Save.
5. Live at `https://<username>.github.io` in about two minutes.
6. In Stripe, set each payment link's post-payment redirect to `https://<username>.github.io/thank-you.html`.

Test on your phone before sending a single DM — that's where your buyers will open it.
