# Brewers Anonymous · Water Lab

A brew-day water chemistry calculator for all-grain homebrewing. Enter your source
water and a target profile, tick the salts you have on hand, and it solves the
mineral additions — **separately for your mash tun and sparge vessel** — then predicts
mash pH and the acid needed to hit your target.

**Live app:** open `index.html`, or the GitHub Pages URL for this repo.

It's a single self-contained HTML file — no server, no build step, no dependencies,
no tracking. It runs entirely in your browser and works offline.

## What it does

- **Mineral solver** — weighted non-negative least-squares finds the salt additions
  that land your water closest to the target flavor profile (SO₄:Cl, calcium, etc.).
- **Two vessels, separately** — mash and sparge water are treated in their own
  containers, each with its own salt weights, acid, and resulting ppm.
- **Editable results** — every salt is an editable field; override the auto values
  and watch the resulting water profile and mash pH update live.
- **Mash pH prediction** — an estimated residual-alkalinity model from your grain
  bill, with a calibration slider to tune it to your own system.
- **Sparge acidification** — the acid needed to knock the sparge water's alkalinity
  down so hot runnings don't extract husk tannins.
- **CSV recipes** — save a recipe to a `.csv` file and load it back anytime.
- **Brew-day sheet** — a printable, tick-off checklist of exactly what goes in each
  vessel.

## Notes

- The salt→ion contributions are standard, published brewing-water chemistry.
- Mash pH is an **estimate** — always confirm with a meter and use the calibration
  slider to dial it in to your system, grain, and process.
- Saved recipes are plain `.csv` files on your own computer.

Built for the Brewers Anonymous homebrew club. *Strength Through Unity, Unity Through Zymurgy.*
