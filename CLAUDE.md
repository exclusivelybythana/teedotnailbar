# Tee (DOT) Nail Bar — Website Editing Context
> Business info, pricing, T&Cs → memory files. This file = website context only.
---
<!-- ============================================ -->
<!-- DO NOT REMOVE OR EDIT: Shortcuts block below -->
<!-- ============================================ -->
## ⚡ Shortcuts
### /tidy
Tidy up ALL memory files in this session:
1. **CLAUDE.md** — fix formatting, remove redundancy, improve clarity, preserve all shortcuts
2. **memory.md** — consolidate entries, remove duplicates, group into sub-categories based on actual content
3. Show a **summary of what changed** (before/after diff in plain English)
4. Offer both files as **downloadable outputs**
> Rules: No clarifying questions. Execute immediately. Never remove the Shortcuts block.
---
### /tidy claude
Tidy up `CLAUDE.md` only:
- Fix formatting and structure
- Remove redundant or outdated entries
- Preserve all shortcuts exactly as written
- Offer as downloadable file
---
### /tidy memory
Tidy up `memory.md` only:
- Consolidate duplicate entries
- Suggest and apply sub-categories based on content
- Sort entries within each sub-category
- Offer as downloadable file
---
### /summary
Summarize this conversation into a compact `session-notes.md`:
- Key changes made to which files
- Design decisions made
- Open items / next steps
- Output as downloadable file for use as context next session
> Rules: Keep it under 20 lines. No prose, bullet points only.
---
### /status
Show current working state:
- Active project
- Last files edited
- Open tasks
- Any broken links or missing images spotted
> Rules: Output as a clean table. No prose.
---
### /new-page [pagename]
Scaffold a new HTML page for teedotnailbar:
1. Use the same nav structure as all existing pages
2. Apply fonts: Playfair Display (headings) + Inter (body)
3. Apply CSS vars: `--cream` `--gold` `--text` `--text-mid` `--cream-mid` `--white` `--gold-dark` `--text-light`
4. Add responsive breakpoints at 900px and 640px
5. No CSS frameworks. No emoji.
6. Output as a downloadable `.html` file named `[pagename].html`
> Rules: Match existing page structure exactly. Ask for page content before generating.
---
### /new-blog [topic]
Create a new blog post page for teedotnailbar:
1. Follow the same structure as existing blog posts (blog-wedding-nails.html etc.)
2. Apply all design rules — fonts, CSS vars, nav, responsive breakpoints
3. Add the new post as a card entry in `blog.html` index
4. Output both the new blog post `.html` and updated `blog.html` as downloadable files
> Rules: No emoji. Match existing blog post tone — polished, editorial, nail-focused.
---
### /edit-service [service name]
Edit a specific service entry in `services.html`:
1. Confirm which tab: Manicure / Pedicure / Nail Art / Removals / Omakase
2. Show the current content for that service
3. Apply the requested edit
4. Output updated `services.html` as downloadable file
> Rules: Preserve `.service-card-img { aspect-ratio: 4/3 }` and local PNG image references.
---
### /check-nav
Audit navigation consistency across all pages:
1. Check all pages have the correct nav: Home · Services · The Design Vault · Studio · About · Blog · Notices · T&Cs · [Book Now]
2. Confirm The Design Vault links to `index.html#design-vault`
3. Flag any page where nav is missing or incorrect
4. Output a fix summary with corrected nav HTML snippet ready to paste
> Rules: Check all files listed in ## Files section.
---
### /check-css
Audit `style.css` for consistency:
1. Confirm all CSS vars are defined: `--cream` `--gold` `--text` `--text-mid` `--cream-mid` `--white` `--gold-dark` `--text-light`
2. Check 900px and 640px breakpoints exist
3. Flag any hardcoded colors that should use CSS vars
4. Flag any unused or duplicate rules
5. Output a clean summary of issues found
> Rules: Output issues as a numbered list with file + line reference where possible.
---
### /push
Prepare files for GitHub Pages deployment:
1. Confirm all edited files are listed
2. Check all internal links use relative paths (no absolute URLs)
3. Check all image references match local PNG filenames
4. Output a pre-push checklist
5. Remind: push to `main` branch, all files in root
> Rules: Do not push automatically. Output checklist only for owner to review.
---
### /seo [pagename]
Run a basic SEO check on a specific page:
1. Check `<title>` tag exists and is descriptive
2. Check `<meta name="description">` exists
3. Check heading hierarchy (H1 → H2 → H3)
4. Check image `alt` attributes
5. Suggest improvements
> Rules: Output as a table with Pass / Fail / Suggest columns.
---
<!-- ============================================ -->
<!-- END Shortcuts block                          -->
<!-- ============================================ -->
---
## Files
| File | Purpose |
|---|---|
| index.html | Home |
| services.html | Services & Pricing (tabs: Manicure, Pedicure, Nail Art, Removals, Omakase) |
| studio.html | Studio (press-ons, shop, masterclasses) |
| about.html | About, FAQ, socials |
| notice.html | Notices |
| terms.html | T&Cs |
| blog.html | Blog index |
| blog-wedding-nails.html · blog-color-psychology.html · blog-nail-makeover.html · blog-nail-shapes.html · blog-about-us.html | Blog posts |
| style.css | Shared stylesheet |
---
## Design
- Fonts: Playfair Display (headings) + Inter (body) — Google Fonts
- Colors: `#faf8f5` cream · `#c9a96e` gold · `#1a1a1a` dark
- CSS vars: `--cream` `--gold` `--text` `--text-mid` `--cream-mid` `--white` `--gold-dark` `--text-light`
- Responsive: 900px + 640px breakpoints. No CSS frameworks. No emoji.
- `.service-card-img { aspect-ratio: 4/3 }` · `.page-hero { background: var(--cream-mid) }`
- Service card images: local PNGs — `manicure-image.png` `extensions-image.png` `pedicure-dry-image.png` `pedicure-full-image.png`
- Omakase bullet: `content: "·"`
---
## Nav (all pages)
Home · Services · The Design Vault (→ index.html#design-vault) · Studio · About · Blog · Notices · T&Cs · [Book Now]
---
## Hosting
GitHub Pages — `main` branch, all files in root.
