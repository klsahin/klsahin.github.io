# klsahin.github.io

Personal portfolio — Karla Sahin. Hand-built static HTML/CSS/JS, no build step.

## Deploy on GitHub Pages

1. Create a **public** repo named exactly `klsahin.github.io`
2. Push these files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/klsahin/klsahin.github.io.git
   git push -u origin main
   ```
3. Repo → Settings → Pages → Source: "Deploy from a branch" → `main` / root
4. Site goes live at `https://klsahin.github.io` within a couple of minutes

## Structure

```
index.html          # the entire site (styles + RRT animation inline)
assets/
  img/              # project images / video posters go here
  Karla_Sahin_Resume.pdf   # TODO: add your resume PDF
README.md
```

## TODO checklist

Search `TODO` in `index.html` for every fill-in spot:

- [ ] Add resume PDF to `assets/` (hero "Resume" button points there)
- [ ] **Locus featured slot** — write-up, stack, focus line, and media at end of
      summer. Confirm with your manager what's shareable before publishing.
- [ ] Add project cards for `Lizarx`, `frox`, `DHCS` if you want them public-facing
- [ ] Add images to project cards (optional — cards work text-only)
- [ ] Link the RTL/FPGA project repo if it can be made public
      (careful with course academic-integrity policies on published solutions)

## Editing

- All theme colors/fonts are CSS variables at the top of `index.html` under
  `/* TOKENS */` — change once, applies everywhere.
- To add a project: copy any `<div class="card">…</div>` block and edit.
- The hero animation is a real RRT (goal-biased, obstacle-checked). It renders
  a static solved tree for users with reduced-motion enabled.
