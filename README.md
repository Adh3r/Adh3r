# Hi, I'm Adam Ruiz Herrero 👋

**Engineering student at EETAC – Universitat Politècnica de Catalunya (UPC), Spain**
Radar signal processing · Satellite navigation (GNSS) · Detection and estimation for GNC

🎯 **Seeking internships in GNC, radar, UAV and defense systems engineering.**

I build sensor-processing chains from first principles and verify every model against theory,
with automated tests on each commit.

---

## Featured work

### 📡 [radar-pulsado](https://github.com/Adh3r/radar-pulsado): pulsed-radar processing chain (MATLAB)
Simulated S-band surveillance scene, from echoes to detections: radar equation → Barker-13 pulse
compression → MTI clutter cancellation → non-coherent integration → CA-CFAR → ROC.
- Detects a **0.1 m² target at 12.3 km** that is invisible before compression (+11.1 dB of
  compression gain), and quantifies how a **slow 0.01 m² drone** survives a single canceller but
  is lost in a double canceller's notch.
- Detection theory from scratch: exact Marcum-Q, Swerling I/III fluctuation loss (**8 dB** for
  Swerling I at Pd = 0.9), CFAR loss and failure modes (clutter edges, target masking).
- **49 unit tests** in CI. Every result is checked against closed-form theory or Monte Carlo.

### 🛰️ [gnss-matlab](https://github.com/Adh3r/gnss-matlab): GNSS from scratch (MATLAB)
Keplerian orbit propagation from YUMA almanacs and TLEs → ECEF / WGS-84 / NED → satellite
visibility → DOP → iterative least-squares positioning from pseudoranges.
- The position fix converges in **5 iterations** from ~13 000 km away and recovers the
  receiver height of 4 m to about **0.1 mm**.
- Sky plot and DOP validated against **gnssmissionplanning.com**; regression tests in CI.

---

## Technical toolbox

| Area | Tools and topics |
|---|---|
| Radar | pulse compression, matched filtering, ambiguity function, CFAR, MTI, RCS, Swerling models |
| Navigation | GNSS orbits and time systems, coordinate frames (ECEF, WGS-84, NED), DOP, least squares |
| Estimation and detection | Neyman–Pearson detection, ROC, Monte Carlo validation |
| Software | MATLAB (`matlab.unittest`), Python, Git, GitHub Actions CI |

## How I work
- **Verified, not just plotted:** each model is checked against its closed form, a Monte Carlo
  run or an independent tool, and those checks run automatically.
- **Readable and reproducible:** modular code, fixed random seeds, one script regenerates every
  figure.
- **Team player:** both projects were developed with lab partners, credited in each repository.
