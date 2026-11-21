# Adam Ruiz Herrero

**B.Sc. in Aerospace Systems Engineering, EETAC – Universitat Politècnica de Catalunya (UPC), Spain**
Navigational Systems specialisation · final-year courses · expected graduation 2027–28
I write simulation, estimation and optimisation software for aerospace problems, and I
validate it against theory and published benchmarks.

🎯 **Seeking an internship in GNC, radar, UAV or defense systems engineering.**
Full-time from **23 June 2027**, or part-time from **January 2027** · open to an industry Bachelor's thesis

📧 [adruizherrero@gmail.com](mailto:adruizherrero@gmail.com) · 🗣️ Spanish (native) · Catalan (C1) · English (B2, C1 in progress)

## Projects

| Project | What it does | Evidence |
|---|---|---|
| 📡 [**pulsed-radar**](https://github.com/Adh3r/pulsed-radar) · MATLAB | Radar processing chain from echoes to detections: Barker-13 pulse compression, MTI, CA-CFAR, ROC | Detects a 0.1 m² target at 12.3 km that is invisible before compression; 49 tests against closed-form theory and Monte Carlo |
| 🛰️ [**gnss-matlab**](https://github.com/Adh3r/gnss-matlab) · MATLAB | GNSS from scratch: orbits from YUMA almanacs and TLEs, ECEF/WGS-84/NED, DOP, least-squares positioning | Fix converges in 5 iterations from ~13,000 km away; sky plot and DOP match gnssmissionplanning.com |
| 🌀 [**lid-driven-cavity**](https://github.com/Adh3r/lid-driven-cavity) · Python | Navier–Stokes CFD solver: direct Newton solver for steady flow, Runge–Kutta for transients | Matches the spectral benchmark to 2 × 10⁻⁶; second-order accuracy measured on grids up to 513² |
| ✈️ [**atfm-gdp-lebl**](https://github.com/Adh3r/atfm-gdp-lebl) · Python | Air traffic flow management at Barcelona–El Prat: ground delay programs, optimal ground holding, rail substitution | Exact slot optimisation cuts the cost of delay by 23 % on a real traffic day; parameters traced to EUROCONTROL and ICAO sources; 90 tests |

Every repository runs its tests in CI on each commit and documents how its results were checked.
The projects started as team coursework; partners are credited in each one.

## Toolbox

| Area | Topics |
|---|---|
| Radar and detection | pulse compression, matched filtering, CFAR, MTI, Swerling models, Neyman–Pearson, ROC |
| Navigation | GNSS orbits and time systems, coordinate frames, DOP, least squares |
| Numerical methods | finite differences, Newton's method with sparse Jacobians, Runge–Kutta, verification and validation, grid convergence |
| Optimisation and ATM | assignment problems, integer programming, queueing (Newell curves), ATFM regulations, cost of delay |
| Software | Python (NumPy, SciPy, pandas, pytest, ruff), MATLAB (`matlab.unittest`), Git, GitHub Actions |

## How I work

- **Verified, not just plotted.** Each model is checked against a closed form, a Monte Carlo
  run, a published benchmark or an independent tool, and those checks run automatically.
- **Honest about errors.** When I revise a project I document what was wrong and how much it
  changed the results (see the revision notes in `lid-driven-cavity` and `atfm-gdp-lebl`).
- **Reproducible.** Modular code, fixed seeds, and scripts that regenerate every figure.
