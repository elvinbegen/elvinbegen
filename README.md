## Photonics researcher · FMCW LiDAR · Quantum-dot photodetectors

I work on **FMCW LiDAR with colloidal quantum-dot photodetectors**, covering the whole chain from the material to the system: first-principles material modeling (DFT), optical and electrical device simulation (FDTD / CHARGE), optical experiments, and system-level signal simulation in Python.

---

### Research

| Project | What it answers | Methods |
|---|---|---|
| [**Ag₂Te QD bandgap from first principles**](https://github.com/elvinbegen/Ag2Te-DFT-Simulations) | What QD size absorbs at 1550 nm? → **3.81 nm**, within 2% of experiment | VASP HSE06+SOC, Kane effective masses, hyperbolic Brus model |
| [**QD photodetector simulations**](https://github.com/elvinbegen/QD-Photodetector-Simulations) | How much light does the QD layer absorb, and how much photocurrent does it give? | Lumerical FDTD + CHARGE |
| **FMCW LiDAR system model** *(in progress)* | How do detector responsivity, bandwidth and noise set range accuracy? | Python: chirp → beat signal → FFT → range, with a detector model |

```text
DFT (material) ──► FDTD/CHARGE (device) ──► FMCW system model (range, SNR)
                                   ▲
                    Michelson experiment (validation)
```

### Toolbox

**Simulation:** VASP · VASPKIT · Lumerical FDTD / CHARGE · VESTA
**Programming:** Python (NumPy, SciPy, Matplotlib) · Bash · HPC/Slurm (TRUBA)
**Lab:** free-space optics, Michelson interferometry, photodiode measurements
