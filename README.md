# Low Noise Amplifier Design Summary UNDER CONSTRUCTION

<p align="justify">

</p>

| Layout                                                        | Schematic                                                           |
| ------------------------------------------------------------- | ------------------------------------------------------------------- |
| ![Quadrature Hybrid Layout](repo/QuadratureHybrid_Layout.png) | ![Quadrature Hybrid Schematic](repo/QuadratureHybrid_Schematic.png) |

| ADS Simulation                                                          |
| ----------------------------------------------------------------------- |
| ![Quadrature Hybrid Simulation Overview](repo/QuadratureHybrid_Sim.png) |

---

## Design Criteria

- **Input match:** S(1,1) < -25 dB
- **Gain at output port 2:** 18 dB < S(2,1) < 19 dB
- **Noise figure at port 2:** nf(2) < 1.1
- **Stability:** Unconditional stability from 100 MHz to 6 GHz

---

## Substrate Properties

- **Substrate thickness (h):** 62 mil
- **Relative permittivity (εᵣ):** 4.4
- **Relative permeability (μᵣ):** 1
- **Conductor conductivity (σ):** 5.85 × 10⁷ S/m
- **Clearance to upper reference (hᵤ):** 3.93701 × 10³⁴ mil (effectively open)
- **Copper thickness (t):** 1.5 mil
- **Dielectric loss tangent (tan δ):** 0.02
- **Surface roughness:** 0 mil

---

## Repository Layout

-

---

## Running the Code

1. Open MATLAB and change into the repository folder.
2. Run the project entry point:

   ```matlab
   >> main
   ```

<p align="justify">
The script will read measurement and simulation files from the configured directories, map the local two-port VNA data to the appropriate global S-parameter labels, and write comparison plots into the <code>output/</code> directory for inspection and documentation.
</p>

---

## Measurement vs. Simulation

| S11                                                     | S12                                                     |
| ------------------------------------------------------- | ------------------------------------------------------- |
| <figure><img src="output/S11.png" alt="S11" /></figure> | <figure><img src="output/S12.png" alt="S12" /></figure> |

| S13                                                     | S14                                                     |
| ------------------------------------------------------- | ------------------------------------------------------- |
| <figure><img src="output/S13.png" alt="S13" /></figure> | <figure><img src="output/S14.png" alt="S14" /></figure> |

| S21                                                     | S22                                                     |
| ------------------------------------------------------- | ------------------------------------------------------- |
| <figure><img src="output/S21.png" alt="S21" /></figure> | <figure><img src="output/S22.png" alt="S22" /></figure> |

| S23                                                     | S31                                                     |
| ------------------------------------------------------- | ------------------------------------------------------- |
| <figure><img src="output/S23.png" alt="S23" /></figure> | <figure><img src="output/S31.png" alt="S31" /></figure> |

| S32                                                     | S33                                                     |
| ------------------------------------------------------- | ------------------------------------------------------- |
| <figure><img src="output/S32.png" alt="S32" /></figure> | <figure><img src="output/S33.png" alt="S33" /></figure> |

| S41                                                     | S44                                                     |
| ------------------------------------------------------- | ------------------------------------------------------- |
| <figure><img src="output/S41.png" alt="S41" /></figure> | <figure><img src="output/S44.png" alt="S44" /></figure> |
