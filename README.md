# 🦌 Carrying Capacity Lab

An interactive island simulation for **Grade 10 Science, Second Term, Weeks 1–2**:
*ecosystem's carrying capacity and population growth.*

**Live demo:** https://YOUR-USERNAME.github.io/carrying-capacity-lab/

## What students discover

- **Food, water, shelter and mates** limit how many animals an ecosystem can support.
- The **scarcest resource** (the bottleneck) sets the carrying capacity, K.
- Population growth **slows as the herd approaches K**, producing an S-shaped curve.
- Upgrading a resource that is *not* the bottleneck changes nothing.

## Features

- Live island simulation with a herd of Visayan spotted deer (fictional island)
- Sliders for food, water, shelter, mate-finding difficulty and starting herd
- Events: typhoon, drought, bumper harvest, release, illegal hunting
- "Predict first" step, six missions, a six-question quiz, and CSV data download
- Charts of herd vs. K and growth-per-month vs. herd size, with the textbook logistic curve for comparison
- Keyboard accessible, screen-reader summaries, respects reduced-motion settings

## Run it locally

Download `index.html` and double-click it. No installation or build step is needed.
(Internet is only used for the Google Font; the app works without it.)

## The model (summary)

- K = min(K_food, K_water, K_shelter); K_food = meals/month, K_water = waterholes × 15, K_shelter = thickets × 8
- P(mate) = 1 − e^(−M/h)
- Each month an animal "gets enough" with probability 1 / (1 + (N/K)^4)
- Textbook comparison: dN/dt = rN(1 − N/K), r = 0.18 per month

The competition curve and species values are teaching assumptions, not field measurements.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole app (HTML, CSS and JavaScript in one file) |
| `README.md` | This page |
