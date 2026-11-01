# Thomas Nauheimer — Independent Research

Independent researcher working on applied algebraic topology, neural fields, and scientific computing on unified-memory hardware (AMD ROCm).  
📧 `nauheimer.t@gmail.com`

All repositories include code and unit tests. Figures in the papers are only those reproducible from the published code; where something is still pending, the repository says so.

---

### [Spectral Inconsistency Entropy](https://github.com/nauheimervater/spectral-inconsistency-entropy) — discrete Hodge theory
[![Release v1.0.0](https://img.shields.io/badge/Release-v1.0.0-orange.svg)](https://github.com/nauheimervater/spectral-inconsistency-entropy/releases/tag/v1.0.0)
[![Paper PDF](https://img.shields.io/badge/Paper-PDF-red.svg)](https://github.com/nauheimervater/spectral-inconsistency-entropy/releases/download/v1.0.0/Spectral_Inconsistency_Entropy.pdf)

A gauge-invariant entropy over the eigenspaces of the cycle-space Hodge Laplacian that measures how "spread out" the non-transitive (cyclic) part of a pairwise-comparison network is. Includes a symmetry result for complete graphs and a closed-form Dirichlet–digamma expectation under isotropic noise, checked against Monte Carlo simulation.

### [Cymatic Φ-NeRF](https://github.com/nauheimervater/cymatic-phi-nerf) — positional-encoding bandwidth in coordinate MLPs
[![Release](https://img.shields.io/badge/Release-v1.0.1-orange.svg)](https://github.com/nauheimervater/cymatic-phi-nerf/releases)

Compares dyadic (2^k), golden-ratio (Φ^k) and Nyquist-matched frequency progressions for sinusoidal positional encodings on toy 3D fields with held-out test points (3 seeds). Main takeaway: matching the highest band to the sampling-density Nyquist limit matters most; Φ^k helps mainly because it is sub-dyadic.

### [Topological Barriers in GCT](https://github.com/nauheimervater/gct-milnor-topology) — algebraic geometry & complexity theory
[![Release v1.0.0](https://img.shields.io/badge/Release-v1.0.0-orange.svg)](https://github.com/nauheimervater/gct-milnor-topology/releases/tag/v1.0.0)
[![Paper PDF](https://img.shields.io/badge/Paper-PDF-red.svg)](https://github.com/nauheimervater/gct-milnor-topology/releases/download/v1.0.0/Topological_Barriers_in_GCT_Permanent_vs_Determinant.pdf)

Examines why Milnor-fiber / Betti-number comparisons of the determinant and permanent hypersurfaces do not by themselves give a separation in Geometric Complexity Theory, including the effect of padding-induced non-isolated singularities.

### [Plastic Transformer](https://github.com/nauheimervater/plastic-transformer) — test-time Hebbian plasticity
Self-attention blocks augmented with Hebbian fast-weight updates during inference for in-context adaptation.

### [SuperCon Zero-Copy Discovery](https://github.com/nauheimervater/supercon-zero-copy-discovery) — *work in progress*
Pipeline architecture for ML-guided superconductor screening on an AMD Strix Halo APU, with C++/HIP zero-copy (`hipHostMallocMapped` + `torch::from_blob`) sources and Quantum ESPRESSO v7.5 SCF inputs/outputs for five generated candidates. A measured zero-copy benchmark is pending (see the status section in the repository).
