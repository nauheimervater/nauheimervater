# Thomas Nauheimer — Independent Research Portfolio

**AI Systems Architecture · Applied Algebraic Topology · Unified-Memory Scientific Computing (AMD ROCm)**  
📧 Contact: `nauheimer.t@gmail.com`

---

## Featured Research & Open-Source Releases (`v1.0.0`)

### 1. [SuperCon Zero-Copy Discovery](https://github.com/nauheimervater/supercon-zero-copy-discovery) — *AI-for-Science on Unified-Memory APUs*
[![Release v1.0.0](https://img.shields.io/badge/Release-v1.0.0-orange.svg)](https://github.com/nauheimervater/supercon-zero-copy-discovery/releases/tag/v1.0.0)
[![Paper PDF](https://img.shields.io/badge/Paper-PDF-red.svg)](https://github.com/nauheimervater/supercon-zero-copy-discovery/releases/download/v1.0.0/SuperCon_Zero_Copy_Discovery.pdf)

> **AI-Driven Superconductor Discovery on Unified-Memory APUs: Equivariant Crystal Diffusion, Zero-Copy MACE Relaxation, and First-Principles DFT Verification**
* **Hardware Target:** AMD Ryzen AI Max+ 395 (*Strix Halo* `gfx1151`, Radeon 8060S, 128 GB Unified Memory, ROCm 7.2).
* **Zero-Copy C++/HIP Kernel (`hipHostMallocMapped`):** Eliminates PCIe host–device copy overhead (**0 bytes transferred**) between GPU equivariant message-passing (MACE via `libtorch_hip`) and CPU pre-screening, accelerating 54-atom supercell relaxation from **16.70 s (16-core CPU)** to **144.7 ms (115.4× speedup)**.
* **End-to-End Physics Validation:** Screens 21,263 superconductors ($R^2 = 0.9288$, $\text{MAE} = 5.36\text{ K}$), trains an equivariant crystal diffusion generator (`DiffCSP-SC`, $99.01\%$ loss reduction), and validates the top 5 candidates in **Quantum ESPRESSO v7.3 PBE-GGA DFT** ($100\%$ SCF convergence and metallic character, led by $\text{BaBiTe}$ with $E_F = 2.98\text{ eV}$).

---

### 2. [Spectral Inconsistency Entropy](https://github.com/nauheimervater/spectral-inconsistency-entropy) — *Discrete Hodge Theory & Consensus Networks*
[![Release v1.0.0](https://img.shields.io/badge/Release-v1.0.0-orange.svg)](https://github.com/nauheimervater/spectral-inconsistency-entropy/releases/tag/v1.0.0)
[![Paper PDF](https://img.shields.io/badge/Paper-PDF-red.svg)](https://github.com/nauheimervater/spectral-inconsistency-entropy/releases/download/v1.0.0/Spectral_Inconsistency_Entropy.pdf)

> **Spectral Inconsistency Entropy: A Gauge-Invariant Hodge-Theoretic Complexity Measure for Non-Transitive Consensus Networks**
* Introduces a gauge-invariant Shannon entropy $H(G, w)$ over the eigenspaces of the cycle-space Hodge Laplacian $L_{\mathcal{Z}} = Z^T B_0^T B_0 Z$ to quantify the structural dimensionality of harmonic frustration $w_{\text{harm}}$.
* **Theorem 1 (Complete-Graph Symmetry Absorption):** Proves via the simplicial Eckmann identity $B_0^T B_0 + B_1 B_1^T = n I_{|E|}$ that $L_{\mathcal{Z}} = n I_{\beta_1(K_n)}$ on every complete graph $K_n$ ($n \ge 3$), yielding $H(K_n, w) \equiv 0\text{ bits}$ for all non-transitive flow fields.
* **Theorem 3 (Exact Dirichlet–Digamma Asymptote):** Derives the closed-form isotropic expectation $H_{\text{iso}}(G) = \frac{1}{\ln 2}\sum_{\lambda} \frac{d_\lambda}{\beta_1}[\psi(\beta_1/2+1)-\psi(d_\lambda/2+1)]$, matching 1,000-trial Monte Carlo simulations on $G(15, 0.4)$ to within $0.01\text{ bits}$ ($4.1175\text{ bits}$ vs. $4.1274 \pm 0.0124\text{ bits}$).

---

### 3. [Cymatic $\Phi$-NeRF](https://github.com/nauheimervater/cymatic-phi-nerf) — *3D Nyquist Anti-Aliasing & Golden-Ratio Positional Encoding*
[![Release v1.0.0](https://img.shields.io/badge/Release-v1.0.0-orange.svg)](https://github.com/nauheimervater/cymatic-phi-nerf/releases/tag/v1.0.0)
[![Paper PDF](https://img.shields.io/badge/Paper-PDF-red.svg)](https://github.com/nauheimervater/cymatic-phi-nerf/releases/download/v1.0.0/Cymatic_Phi_NeRF.pdf)

> **Cymatic $\Phi$-NeRF: Quasi-Periodic Golden-Ratio Positional Encoding and 3D Nyquist Anti-Aliasing in Neural Radiance Fields**
* **Volumetric 3D Nyquist Analysis (Proposition 1):** Demonstrates that standard dyadic NeRF encoding ($2^k \pi$, $L=8$) places half of its frequency bands above the 3D Shannon–Nyquist cutoff $\omega_{\text{Nyq}} = \frac{\pi}{2}N^{1/3} \approx 10.08\pi\text{ rad/unit}$ (at $N=8,192$), causing inter-ray aliasing.
* **Diophantine Incommensurability (Proposition 2):** Replacing $2^k$ with powers of the Golden Ratio $\Phi = \frac{1+\sqrt{5}}{2} \approx 1.618$ reduces integer harmonic phase collisions by **$45\times$** and improves held-out 3D test PSNR by **$+1.84\text{ to }+2.03\text{ dB}$** on spherical shells ($+5.30\text{ dB}$ single-seed fast convergence) and **$+1.00\text{ to }+1.04\text{ dB}$** on a neutral 3D Schoen Gyroid minimal surface.

---

### 4. [Topological Barriers in GCT](https://github.com/nauheimervater/gct-milnor-topology) — *Algebraic Geometry & Complexity Theory*
[![Release v1.0.0](https://img.shields.io/badge/Release-v1.0.0-orange.svg)](https://github.com/nauheimervater/gct-milnor-topology/releases/tag/v1.0.0)
[![Paper PDF](https://img.shields.io/badge/Paper-PDF-red.svg)](https://github.com/nauheimervater/gct-milnor-topology/releases/download/v1.0.0/Topological_Barriers_in_GCT_Permanent_vs_Determinant.pdf)

> **Topological Barriers in Geometric Complexity Theory: Milnor Fiber Betti Numbers of the Determinant vs. Permanent**
* Establishes via Milnor's Fibration Theorem ($\mu(f) = (n-1)^{n^2}$) why naive Betti-number comparisons on homogeneous hypersurface fibers cannot bypass the orbit-closure degenerations required for $\mathsf{VP} \neq \mathsf{VNP}$.

---

### 5. [Plastic Transformer](https://github.com/nauheimervater/plastic-transformer) — *Test-Time Hebbian Synaptic Plasticity*
[![Repository](https://img.shields.io/badge/GitHub-Repository-blue.svg)](https://github.com/nauheimervater/plastic-transformer)

> **Hebbian Fast-Weight Synaptic Plasticity in Self-Attention Networks**
* Augments standard frozen-weight Transformer blocks with dynamic Hebbian fast-weight state updates during inference for rapid in-context sequence adaptation.

---

## Summary Table of Publications & Reproducible Benchmarks

| Repository | Domain | Key Result / Metric | Paper PDF |
| :--- | :--- | :--- | :---: |
| [`supercon-zero-copy-discovery`](https://github.com/nauheimervater/supercon-zero-copy-discovery) | AI-for-Science / AMD ROCm | **115.4× speedup** (`144.7 ms` zero-copy MACE), **5/5 QE DFT** metals | [PDF](https://github.com/nauheimervater/supercon-zero-copy-discovery/releases/download/v1.0.0/SuperCon_Zero_Copy_Discovery.pdf) |
| [`spectral-inconsistency-entropy`](https://github.com/nauheimervater/spectral-inconsistency-entropy) | Algebraic Topology / Graph Theory | **$H(K_n, w) \equiv 0$** $\forall n \ge 3$; exact Digamma asymptote ($4.12\text{ bits}$) | [PDF](https://github.com/nauheimervater/spectral-inconsistency-entropy/releases/download/v1.0.0/Spectral_Inconsistency_Entropy.pdf) |
| [`cymatic-phi-nerf`](https://github.com/nauheimervater/cymatic-phi-nerf) | 3D Vision / Neural Fields | **$+1.84\text{ to }+4.08\text{ dB}$** held-out Test PSNR via 3D Nyquist packing | [PDF](https://github.com/nauheimervater/cymatic-phi-nerf/releases/download/v1.0.0/Cymatic_Phi_NeRF.pdf) |
| [`gct-milnor-topology`](https://github.com/nauheimervater/gct-milnor-topology) | Geometric Complexity Theory | Exact Milnor number obstruction $\mu(f) = (n-1)^{n^2}$ for $\det_n$ vs. $\operatorname{perm}_n$ | [PDF](https://github.com/nauheimervater/gct-milnor-topology/releases/download/v1.0.0/Topological_Barriers_in_GCT_Permanent_vs_Determinant.pdf) |
| [`plastic-transformer`](https://github.com/nauheimervater/plastic-transformer) | Neuro-Inspired Deep Learning | Online Hebbian fast-weight plasticity in attention layers | [Repo](https://github.com/nauheimervater/plastic-transformer) |
