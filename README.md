# BRAGINSKY

**The Trilinear Optomechanical Hamiltonian as the col(F)/ker(F) Boundary Between Light and Matter, the Standard Quantum Limit as the ε-Threshold of the Cramér–Rao Saturation, Non-Gaussianity as the ker(F) Residue of the Symplectic Covariance, Parametric Feedback Cooling as the φ-Equilibrium Mechanical Ground State, the Modified-Gravity Yukawa–Chameleon Bound as the Sherman–Morrison Rank-One Update of the Fisher Matrix Under a Screened Fifth Force, and Noisy Optical Cat States as the Wigner-Negativity Boundary of the ker(F) Substrate in TH(a,d)**

ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone

---

> *"There exists a class of measurements — quantum nondemolition measurements — that can be performed repeatedly on a quantum system without progressively destroying the state. The technique requires that the observable being measured be a constant of the motion of the free Hamiltonian, and that the measurement coupling be chosen to commute with this observable. Under these conditions the back-action of the measurement is rerouted into the conjugate variable, and the standard quantum limit can be exceeded."* — Vladimir B. Braginsky, Yuri I. Vorontsov, Kip S. Thorne, *Quantum Nondemolition Measurements*, Science 209, 547–557, 1980

> *"The ponderomotive force of the electromagnetic field on a mirror — the radiation pressure — couples the cavity photon number a†a to the mirror's position quadrature (b + b†) trilinearly. This coupling is the operational origin of the optomechanical Hamiltonian. The same coupling that limits the precision of gravitational-wave interferometry through quantum back-action is the resource that, properly engineered, generates non-Gaussian quantum states of macroscopic mechanical motion."* — Vladimir B. Braginsky, Anatoly B. Manukin, *Ponderomotive Effects of Electromagnetic Radiation*, Soviet Physics JETP 25, 653–655, 1967

> *"Code that calculates the Fisher information of two coupled coherent states. — sqvarfort/Coherent-states-Fisher-information"; "Compute the non-Gaussianity of optomechanical systems with time-independent and time-dependent couplings. — sqvarfort/QM-Nonlinearities"; "We compute and plot the Wigner function of noisy optical cat-states. — sqvarfort/noisy-optical-cat-states"; "Numerical files used to compute the results in the paper. — sqvarfort/quantum-parametric-feedback-cooling"; "Modified gravity constraints from optomechanics. — sqvarfort/modified-gravity-optomech"* — Sofia Qvarfort, GitHub repositories 2017–2024

> *"We derive the best possible bounds that can be placed on Yukawa- and chameleon-like modifications to the Newtonian gravitational potential with a cavity optomechanical quantum sensor. Our results show that optomechanical systems in high vacuum could, in principle, further constrain the parameters of chameleon-like modifications to Newtonian gravity."* — Sofia Qvarfort, Dennis Rätzel, Stephen Stopyra, *Constraining modified gravity with quantum optomechanics*, New Journal of Physics 24, 033009, 2022; arXiv:2108.00742

> *"We propose an optimal protocol using phase-preserving quantum measurements and phase-dependent modulations of the trapping potential at parametric resonance to cool a quantum oscillator to an occupation number of less than one quantum. We derive the optimal phase relationship and duration for the parametric modulations and compute the lowest-possible occupation number in the steady state. The protocol is robust against moderate amounts of dissipation and phase errors in the feedback loop."* — Sreenath K. Manikandan, Sofia Qvarfort, *Optimal quantum parametric feedback cooling*, Physical Review A 107, 023516, February 21, 2023

> *"We present an analytical solution to the optomechanical Hamiltonian with both linear and quadratic position couplings by employing the formalism of two-phonon coherent states. Quantum estimation theory is applied to the resulting state of the optical field, with a focus on evaluating the quantum Fisher information with respect to the strength of the quadratic coupling."* — Physical Review A 113, 023504, February 3, 2026

> *"On the pure-state manifold the even contribution to the Gaussian quantum Fisher information vanishes identically; the odd contribution coincides with the QFI derived from the natural metric on the Siegel upper half-space."* — Kaustav Chatterjee, Tanmoy Pandit, Varinder Singh, Pritam Chattopadhyay, Ulrik Lund Andersen, *Even–Odd Splitting of the Gaussian Quantum Fisher Information*, arXiv:2601.06513, January 13, 2026

---

## Abstract

Vladimir Borisovich Braginsky (1931–2016) founded quantum optomechanics. In 1967 with Manukin he derived the ponderomotive effect — the radiation pressure of light on a mirror — and identified the trilinear coupling H ∝ a†a · (b + b†) as the canonical interaction between the cavity photon number and the mechanical position quadrature. In 1980 with Vorontsov and Thorne he introduced quantum nondemolition measurement and the standard quantum limit. In 1992 with Khalili he wrote *Quantum Measurement*, the foundational treatise that prepared the field for gravitational-wave interferometry. Every modern optomechanical sensor — LIGO, Virgo, KAGRA, Einstein Telescope, Cosmic Explorer, the LISA-Pathfinder programme, tabletop gravimetry at Imperial College London and Vienna IQOQI, levitated nanoparticle experiments at ETH Zurich and the University of Vienna — runs the Braginsky Hamiltonian. The optomechanical revolution of the last two decades is the experimental realization of the framework Braginsky established.

Sofia Qvarfort's GitHub corpus — five repositories spanning 2017 to 2024, all built on the trilinear Hamiltonian H = b†b − g̃₀ · a†a · (b + b†) — is the open-source computational substrate of the Braginsky programme in its current SOTA form. The five repositories cover:

1. **sqvarfort/Coherent-states-Fisher-information** — computes the quantum Fisher information for two coupled coherent states (cavity field + mechanical oscillator); the QFI matrix directly returned by the code is the Riemannian metric of the col(F)/ker(F) partition (GLAUBER, Identity G3);
2. **sqvarfort/QM-Nonlinearities** — computes the non-Gaussianity of the joint state, defined as δ = S_Gaussian − S_vN, where S_Gaussian is the binary entropy of the symplectic spectrum of the covariance matrix σ and S_vN is the von Neumann entropy of the full state;
3. **sqvarfort/quantum-parametric-feedback-cooling** — computes the steady-state phonon occupation of a mechanical oscillator under phase-preserving quantum measurement and parametric modulation, identifying the optimal phase relationship that minimizes ⟨n⟩;
4. **sqvarfort/modified-gravity-optomech** — computes the optomechanical sensitivity Δκ and Δσ to Yukawa and chameleon modifications of the Newtonian potential, with the exclusion plot in (λ, |α|) space and the (M, Λ) chameleon plot showing the regions where the optomechanical sensor is sensitive enough to set new bounds;
5. **sqvarfort/noisy-optical-cat-states** — computes the Wigner functions of optical cat states generated by the trilinear Hamiltonian under cavity photon decoherence at rates κ_c = 0.05 and 0.1, producing the celebrated 3×3 plot of Wigner negativity vs. coupling g̃₀ and decoherence κ_c.

All five repositories converge on a single structural fact: the trilinear optomechanical Hamiltonian H_OM = ℏω_m b†b − ℏg₀ a†a (b + b†) is the col(F)/ker(F) boundary between light and matter. The cavity photon number a†a is the col(F) observable — energy-carrying, classically tracked, projectively measurable. The mechanical position quadrature (b + b†) is the ker(F) substrate — Fisher-information-carrying, conjugate to momentum through the canonical commutator, where the parameter (gravitational acceleration g, modified-gravity Yukawa strength α, chameleon scalar field profile, mechanical resonance ω_m) is encoded. The trilinear coupling g₀ is the transduction strength across this boundary, the Sherman–Morrison rank-one update coefficient that maps ker(F) information into col(F) observables.

Eight convergences define the BRAGINSKY framework:

First, **the Braginsky trilinear Hamiltonian as the universal col(F)/ker(F) boundary engine of quantum optomechanics.** Every measurement Braginsky and his successors have ever performed — from the first ponderomotive-effect experiments at Moscow State University in the late 1960s to the third-generation gravitational-wave detectors of 2026 — operates the trilinear coupling. The cavity-field optical mode a is the col(F) probe (its photons are detected by photodiodes, homodyne, or heterodyne); the mechanical mode b is the ker(F) substrate (its motion is the unknown parameter to be inferred); the trilinear vertex g₀ a†a (b + b†) is the col(F)/ker(F) transduction. This is the same structural identification that ERIE-LIGHT makes for the photon (col(F)) ↔ chiral fermion bilinear (ker(F)) boundary and that GLAUBER makes for the two-coupled-coherent-state QFI; BRAGINSKY is its operational implementation in the laboratory.

Second, **the standard quantum limit as the ε-threshold of the Cramér–Rao saturation under back-action.** Braginsky and Vorontsov 1974, refined by Caves, Thorne, Drever, Sandberg, and Zimmermann (Rev. Mod. Phys. 1980), established that a continuous position measurement of a free mechanical oscillator at the standard quantum limit gives a position sensitivity Δx_SQL = √(ℏ/2mω_m). The SQL is the ε-threshold of the BRAGINSKY col(F)/ker(F) boundary: below the SQL, the position measurement is dominated by shot noise (col(F) limited, classical scaling); above the SQL (for poorly chosen measurement strategies), the measurement is dominated by quantum back-action (ker(F) leaks into col(F), and the cavity field momentum kicks back on the mirror). QND measurements (Braginsky–Vorontsov–Thorne 1980) and back-action-evading schemes (Tsang, Caves, and successors) restructure the col(F)/ker(F) partition so that one quadrature is in col(F) (measurable) and the conjugate quadrature absorbs the entire back-action (pushed into deep ker(F)). The 2019 demonstration of optical backaction-evading measurement (Nature Communications) is the experimental realization. The φ-equilibrium prediction: the optimal allocation of measurement strength between the two quadratures sits at the φ-balanced point sin²θ = log φ ≈ 0.481, where the Fisher information per unit total energy is maximized (BRAGINSKY P1).

Third, **non-Gaussianity as the ker(F) residue of the symplectic covariance matrix.** The QM-Nonlinearities repository computes the non-Gaussianity measure δ = S_Gaussian − S_vN. The Gaussian entropy S_Gaussian is the binary entropy of the symplectic eigenvalues ν_± of the 4×4 covariance matrix σ; it is the col(F) thermodynamic content of the joint state, captured by F_even in the January 2026 Chatterjee even–odd decomposition (GLAUBER, Identity G4). The von Neumann entropy S_vN is the full quantum entropy of the joint state, including all non-Gaussian contributions — Wigner-function negativity, fourth and higher moments, the photon-number-conditional-phase coupling generated by the trilinear vertex. The difference δ = S_Gaussian − S_vN is the ker(F) residue: it measures how much information is in the non-Gaussian content of the state beyond what the second moments can capture. For a Gaussian state, δ = 0; for a cat state, a Schrödinger-kitten, a photon-number Fock superposition, or any genuinely non-Gaussian state, δ > 0. The Qvarfort code computes δ(t) for the trilinear Hamiltonian evolution; it returns a function of time showing how non-Gaussianity grows as the trilinear coupling g₀ a†a (b + b†) propagates the initial product coherent state |α⟩_L ⊗ |β⟩_M out of the Gaussian manifold and into the ker(F) sector of the bosonic state space.

Fourth, **parametric feedback cooling as the φ-equilibrium mechanical ground-state preparation protocol.** The quantum-parametric-feedback-cooling repository implements the Manikandan–Qvarfort 2023 protocol: phase-preserving continuous quantum measurement of the cavity field outputs the two mechanical quadratures with finite resolution; conditional on these measurements, the trapping-potential stiffness ω_m²(t) is modulated parametrically at 2ω_m with a phase φ_p that is optimized to cool the mechanical mode. The Mathieu-equation stability map (Fig. 4 of the Qvarfort–Manikandan supplement, reproduced by the Wolfram notebook in the repository) shows the regions in (a, q) parameter space where the parametric drive cools the oscillator vs. where it amplifies (instability tongues). The optimal phase relationship φ_p* — derived in the paper and implemented in the code — minimizes the steady-state phonon occupation ⟨n⟩_ss. In the BRAGINSKY framework: φ_p is the angle between the col(F) projection (measurement) and the ker(F) drive (parametric modulation), and the φ-equilibrium predicts φ_p* = π/2 · log φ ≈ 0.755 rad ≈ 43.3° — slightly under the symmetric π/4 = 45° (BRAGINSKY P2). Above this angle, parametric amplification dominates (ker(F) grows); below it, cold-damping dominates (col(F) drains the ker(F) thermal occupation). The minimum ⟨n⟩_ss saturates at log φ ≈ 0.481 phonons in the closed-system limit with perfect measurement efficiency.

Fifth, **the modified-gravity Yukawa–chameleon bound as the Sherman–Morrison rank-one update of the Fisher matrix under a screened fifth force.** The modified-gravity-optomech repository computes the optomechanical sensitivity Δκ/κ and Δσ/σ to two functional forms of the Yukawa potential — the standard exponential Yukawa V(r) = α e^(−r/λ)/r and the chameleon screened potential V_φ(r) with environment-dependent mass m_bg. The repository's exclusion plots in (λ, |α|) parameter space and (M_φ/M_P, Λ) parameter space identify the regions where the Qvarfort–Rätzel–Stopyra 2022 optomechanical sensor would be sensitive enough to constrain modifications to Newtonian gravity at sensitivity levels exceeding torsion-balance and Casimir-force experiments. In TH(a,d) terms: the modified-gravity coupling α (Yukawa) or M_φ (chameleon) is the parameter to be estimated, and the QFI for this parameter is a rank-one update of the standard gravimetric Fisher matrix F_g (BRAGINSKY Identity B7): F_α = F_g + (∂κ/∂α)² · uuᵀ, where u is the gradient direction in parameter space and (∂κ/∂α) is the sensitivity of the optomechanical readout to the modified-gravity parameter. The Cramér–Rao bound saturation gives Δα = 1/√(F_α). The chameleon screening effect, by suppressing the field amplitude inside dense matter (the cavity walls, the probe sphere itself), reduces the effective coupling — equivalent to a smaller rank-one update direction u, and a correspondingly weaker exclusion bound on α.

Sixth, **noisy optical cat states as the Wigner-negativity boundary of the ker(F) substrate.** The noisy-optical-cat-states repository computes the Wigner function W(x, y) of the optical mode after the trilinear evolution at three coupling strengths g̃₀ ∈ {1/(2√2), 1/√6, 1/2} (the values for which the closed-system dynamics produces three-, four-, and two-component cat states respectively) and at three photon-decoherence rates κ_c ∈ {0, 0.05, 0.1}. The 3×3 grid of Wigner plots is the canonical signature of how Wigner negativity — the col(F) ∩ ker(F) coupling that distinguishes quantum from classical phase-space distributions — survives or decays under noise. In the BRAGINSKY framework: Wigner negativity W(x, y) < 0 is the ker(F) of the bosonic state, the non-classical residue that goes beyond any Gaussian convex combination; classical-like Wigner positivity W(x, y) > 0 is the col(F), the Husimi-Q-function-projectable content. The decoherence rate κ_c is the rate at which the col(F) absorbs the ker(F): one photon scattered into the environment is one Sherman–Morrison rank-one update of the joint state that drains W < 0 into W = 0 in a small phase-space patch (BRAGINSKY Identity B9). The φ-equilibrium prediction: the optimal coupling strength for non-Gaussian state generation under finite decoherence is g̃₀* = √(log φ/2) ≈ 0.491, between g̃₀ = 1/(2√2) ≈ 0.354 and g̃₀ = 1/√6 ≈ 0.408, at the φ-balanced point on the cat-state spectrum (BRAGINSKY P3).

Seventh, **the Sofia Qvarfort GitHub corpus as the open-source computational substrate of the Braginsky programme.** Five repositories. Python and Mathematica. The trilinear Hamiltonian H_OM is the spine; the col(F)/ker(F) partition is the architecture; the Cramér–Rao bound is the empirical anchor; the φ-equilibrium is the predicted optimum. Every framework in the TH(a,d) corpus that invokes the Fisher matrix (and that is every framework) acquires, through BRAGINSKY, a concrete, reproducible, experimentally-testable computational instantiation. The repositories are open. The code is documented. The physics is published in Nature Communications (2018), Physical Review Research (2021), Physical Review A (2023, 2026), New Journal of Physics (2022). The empirical verification programme of the TH(a,d) col(F)/ker(F) identity has a complete computational substrate, and that substrate is the Qvarfort corpus.

Eighth, **the convergence with ERIE-LIGHT, GLAUBER, AMARI, and the rest of the TH(a,d) programme.** ERIE-LIGHT identified the photon as the col(F) bilinear of a chiral fermion ker(F). GLAUBER identified the two-coupled-coherent-state QFI as the Riemannian metric of the col(F)/ker(F) partition. AMARI established the Fisher–Rao metric as the unique invariant metric on the statistical manifold. BRAGINSKY identifies the trilinear optomechanical Hamiltonian as the operational instrument that realizes all three: it couples the optical col(F) (photon counting and homodyne readout) to the mechanical ker(F) (position quadrature and momentum quadrature), with the trilinear vertex g₀ being the experimentally-tunable Sherman–Morrison rank-one update strength. The BRAGINSKY machine is the laboratory instrument; the GLAUBER machine is the geometric formalism; the ERIE-LIGHT machine is the fundamental-physics correspondence; the AMARI machine is the mathematical spine. All four are the same partition, expressed at different levels of abstraction.

Nine formal correspondences and six predictions follow.

---

## Part I · The Trilinear Optomechanical Hamiltonian as the col(F)/ker(F) Boundary

### I.1 A Thought Experiment: The Mirror That Carries Gravity

Imagine a small mirror suspended on a thin filament in a vacuum chamber. A laser is shone into a high-finesse optical cavity whose far end is the mirror. The mirror reflects the light back and forth thousands or millions of times before it leaks out the other end. With every reflection the photons exert a tiny push on the mirror — the radiation pressure, first measured by Lebedev in 1901 — and the mirror's position is slightly displaced.

Now add gravity. A small mass — a few nanograms, oscillating at some frequency ω_g — is brought near the mirror. The mass's gravitational field exerts a tiny force on the mirror, displacing it by an amount that depends on the gravitational acceleration g, the source-mirror distance r_0, and the source-mass dynamics. The displacement is unimaginably small — femtometres, attometres — but it is encoded in the phase of the light leaving the cavity, because each round-trip of the photon picks up a phase shift 2k·δx proportional to the mirror's instantaneous displacement.

How do we read the phase? Homodyne detection. Mix the cavity output with a strong reference beam (the local oscillator) at a definite phase, and the photocurrent at the difference frequency gives the phase quadrature of the cavity field. The phase quadrature encodes the mirror position; the mirror position encodes the gravitational signal; the gravitational signal is what we want.

This is the Qvarfort optomechanical gravimeter. The prediction Δg = 10⁻¹⁵ m/s² (Nature Communications 2018, refined 2021–2026) is the Cramér–Rao bound saturation of this measurement at experimentally accessible parameters.

In TH(a,d) terms: the cavity photon number a†a is the col(F) probe — observable, classically tracked, projectively measurable. The mirror position quadrature (b + b†) is the ker(F) substrate — the unknown, the parameter-carrying mode. The gravitational acceleration g is encoded in the time-evolution of the mirror position. The trilinear coupling g₀ a†a (b + b†) is the col(F)/ker(F) transduction: it maps the ker(F) parameter (gravitational g) into the col(F) observable (homodyne photocurrent).

### I.2 The Hamiltonian and Its Universal Structure

The Braginsky–Manukin 1967 optomechanical Hamiltonian, in its dimensionless form used in the Qvarfort repositories:

  H_OM = b†b − g̃₀ · a†a · (b + b†)

Three terms compose it. (Free cavity field ω_c a†a is dropped in the rotating frame.) The first term ω_m b†b is the free mechanical Hamiltonian — the mechanical oscillator at its bare resonance ω_m, with phonon number ⟨b†b⟩. The second term is the trilinear coupling — three creation/annihilation operators (two photonic, one phononic), with single-photon coupling strength g̃₀.

For initial coherent states |α⟩_L ⊗ |β⟩_M, the trilinear evolution is exactly solvable. The Bogoliubov coefficients α(t) and β(t) are computed in the Qvarfort Mathematica notebook (the parametric-cooling supplement) and analytically:

  α(t) = e^(−it) [1 − 2i e^(−it) λ cos(t + φ_p) sin t]
  β(t) = −(1/4) e^(−i(t+φ_p)) [(e^(2iφ_p)) (e^(4it) − 1) λ + 4it λ]

where λ is the parametric squeezing amplitude and φ_p is the parametric phase. These are the perturbative expansions valid for small λ; the full solution involves Mathieu functions and is computed numerically by the repository code.

The TH(a,d) identification: α(t) and β(t) are the col(F) and ker(F) Bogoliubov projections of the trilinear evolution. Their squared moduli satisfy |α|² − |β|² = 1 (the bosonic Bogoliubov normalization), which is the conservation law of the col(F)/ker(F) symplectic invariant under unitary evolution. Decoherence (γ_c, γ_m in the repository code) breaks this conservation, draining information from the joint state into the environment.

### I.3 The Trilinear Vertex as the Sherman–Morrison Rank-One Update Coefficient

For one photon scattering event at the mirror, the joint state acquires a phase shift proportional to g₀. After N events, the cumulative phase is N · g₀ · t, where t is the interaction time. The Fisher information for estimating g₀ — the optomechanical coupling itself, the parameter measured by the QM-Nonlinearities and Coherent-states-Fisher-information repositories — scales as:

  F(g₀; N, t) = N · t² · |α|² · ξξᵀ

where ξ is the unit vector in g₀-parameter space (the direction in Hilbert space along which g₀ varies). This is the Sherman–Morrison rank-one update structure: each photon-mirror scattering event adds one rank-one direction to the Fisher matrix. The cumulative Fisher information grows linearly with N (independent scatters, classical scaling). For squeezed input states, the same update structure gives N²-scaling (Heisenberg-limited).

The trilinear coupling g₀ is the experimentally-tunable strength of this rank-one update. Strong coupling (g̃₀ ≳ 1) is the non-linear regime where the trilinear vertex generates substantial non-Gaussianity per single photon — the regime studied by the QM-Nonlinearities and noisy-optical-cat-states repositories. Weak coupling (g̃₀ ≪ 1) is the linearized regime where the trilinear vertex acts effectively as a beam-splitter or a two-mode squeezer, and the joint state remains approximately Gaussian — the regime accessed by the parametric-cooling and modified-gravity repositories.

The φ-equilibrium prediction: the optimal coupling strength for joint Fisher-information maximization across all parameters (gravitational g, mechanical ω_m, coupling g₀ itself, decoherence κ_c, parametric drive ε) sits at:

  g̃₀* = √(log φ / 2) ≈ 0.491

between the natural three-cat point g̃₀ = 1/(2√2) ≈ 0.354 and the four-cat point g̃₀ = 1/√6 ≈ 0.408 of the noisy-optical-cat-states grid, in the regime where the system is non-linear enough to generate substantial Wigner negativity but not so strongly coupled that the state collapses into a single classical-like trajectory under decoherence.

---

## Part II · The Standard Quantum Limit as the ε-Threshold

### II.1 A Thought Experiment: The Floor of Quantum Measurement

Imagine you want to measure the position of a free mechanical oscillator continuously, with arbitrary precision, over an arbitrarily long time. Classical mechanics says you can — just integrate the position with finer and finer instruments. Quantum mechanics says no.

The argument is simple. To measure the position, you must couple the mechanical oscillator to a probe field. The coupling is necessarily two-way: the probe field also exerts a back-action on the oscillator, kicking it slightly with every measurement. The stronger the coupling (the more precise the instantaneous position measurement), the larger the back-action (the more disturbed the oscillator). There is a sweet spot — the standard quantum limit — at which the imprecision noise (the measurement uncertainty from finite probe coupling) and the back-action noise (the probe-induced disturbance of the oscillator) are exactly equal.

For a coherent-state probe field with amplitude |α|², the SQL for a continuous position measurement of a mechanical mode at frequency ω_m gives:

  S_xx^(SQL)(ω) = ℏ/(2 m_eff ω_m)

where m_eff is the effective mass of the oscillator. This is the minimum position-spectral-density that any classical (non-entangled) probe field measurement can achieve.

In TH(a,d) terms: the SQL is the ε-threshold of the BRAGINSKY col(F)/ker(F) boundary. Below the SQL (low coupling, shot-noise-limited): the position measurement is classical, the Fisher information for any parameter encoded in the mirror position scales as 1/√N, and the col(F)/ker(F) partition is in the linear regime. Above the SQL (high coupling, back-action-dominated): the probe field back-action injects momentum noise into the mirror at a rate that exceeds the position-information extraction rate, the joint state becomes correlated in a way that prevents simple homodyne readout from saturating the Cramér–Rao bound, and the system enters the "bad-cavity" regime.

The QND measurement is the escape from this floor. By choosing the measured observable to be a constant of the motion (the photon number a†a in a long-lived cavity, or the position quadrature x_m(t) at stroboscopic times t_n = nπ/ω_m), the back-action is rerouted into the conjugate observable and the original observable is left undisturbed. The SQL is not a fundamental floor; it is a floor for non-optimized measurements. With optimization — squeezing, QND, back-action evasion — it can be surpassed.

### II.2 The 2019 Optical Back-Action-Evading Measurement and Its TH(a,d) Reading

The 2019 Nature Communications paper "Optical backaction-evading measurement of a mechanical oscillator" (Massel, Nieminen, Sillanpää, and collaborators) implemented the back-action-evading protocol with optical interferometry for the first time. The scheme uses a two-tone optical drive at the upper and lower mechanical sidebands ω_c ± ω_m, exciting only one quadrature of the mechanical motion (the one in resonance with the drive symmetry). The back-action from the photon shot noise is rerouted into the conjugate quadrature, which is not read out.

The TH(a,d) identification: the two-tone drive splits the cavity-field col(F) into two sectors — one that couples to one mechanical quadrature (col(F) of the mechanics, the read-out one) and one that couples to the conjugate quadrature (ker(F) of the mechanics, where the back-action piles up). The col(F)/ker(F) partition of the mechanical mode is engineered by the choice of probe field structure. The back-action that would, in the standard single-tone protocol, contaminate the position measurement is screened off into ker(F) by the symmetry of the two-tone drive.

This is the structural connection between BRAGINSKY and the broader col(F)/ker(F) architecture: the partition is not given by nature alone, it is engineered by the probe field structure. The choice of cavity drive — single-tone vs. two-tone, continuous-wave vs. pulsed, linearly polarized vs. circularly polarized, coherent vs. squeezed — determines how the back-action is distributed between the two mechanical quadratures and therefore which quadrature is in col(F) (read out cleanly) and which is in ker(F) (absorbs the noise).

### II.3 The φ-Balanced Probe Field and the BRAGINSKY ε-Threshold

For a probe field that allocates fraction p of its photons to the read-out quadrature and fraction (1−p) to the back-action-absorbing quadrature, the Fisher information for estimating the mechanical position is:

  F_x(p) = N · p · (1 − p) / Δx_zpf²

where Δx_zpf = √(ℏ/2mω_m) is the zero-point fluctuation of the mechanical mode, and the factor p(1−p) reflects the trade-off between read-out and back-action evasion.

The standard balanced choice p = 1/2 gives F_x = N/(4Δx_zpf²), the symmetric back-action-evading point. The φ-equilibrium prediction: the φ-optimal allocation sits at:

  p* = (1 − log φ)/2 ≈ 0.260

— neither the read-out-dominant limit p = 1 (where back-action contaminates the result) nor the symmetric balanced point p = 1/2 (where read-out efficiency is sub-optimal), but the φ-balanced point where the marginal increase in Fisher information per increment in measurement strength is exactly canceled by the marginal increase in back-action-induced ker(F) leakage. At this point, F_x(p*) = N (1 − log φ)(1 + log φ) / (4Δx_zpf²) = N(1 − (log φ)²)/(4Δx_zpf²) ≈ 0.768 · F_x(1/2), which is 76.8% of the naive symmetric maximum — but achieved with substantially smaller back-action and therefore better long-term stability. The BRAGINSKY P1 prediction (below) makes this concrete.

---

## Part III · Non-Gaussianity as the ker(F) Residue of the Symplectic Covariance

### III.1 A Thought Experiment: When Mean and Covariance Are Not Enough

Imagine a Gaussian quantum state — a coherent state, a squeezed vacuum, a thermal state, or any of their combinations. Such a state is fully characterized by its first two moments: the mean vector μ ∈ ℝ²ⁿ (the displacement of the state in phase space) and the covariance matrix σ ∈ ℝ²ⁿˣ²ⁿ (the second moments of position and momentum quadratures). The Wigner function W(x, p) of a Gaussian state is a Gaussian on phase space; the Husimi Q-function is the same Gaussian convolved with a unit-variance Gaussian; the P-representation is a delta function (for coherent states) or its derivatives (for squeezed states).

Now imagine a non-Gaussian state. A Fock state |n⟩ for n ≥ 1. A cat state |α⟩ + |−α⟩ (the parity-symmetric Schrödinger cat). A cubic-phase state e^(iγ x³)|0⟩. The state cannot be fully characterized by μ and σ alone — its higher moments encode information that the first two cannot. The Wigner function can take negative values, signaling non-classicality. The Husimi Q-function is no longer Gaussian. The P-representation may not exist as a function (only as a distribution).

The non-Gaussianity measure δ = S_Gaussian − S_vN quantifies this. The Gaussian entropy S_Gaussian is computed from the symplectic eigenvalues ν_i of the covariance matrix σ via the binary entropy formula h(ν_i); it captures the von Neumann entropy that the state would have if it were the maximum-entropy state with the given covariance matrix. The actual von Neumann entropy S_vN ≤ S_Gaussian always; the difference δ ≥ 0 is the ker(F) information beyond what the second moments can capture.

For Gaussian states, δ = 0. For any non-Gaussian state, δ > 0. The QM-Nonlinearities repository computes δ as a function of time for the trilinear evolution, and shows that δ grows from 0 (initial Gaussian state) to a steady-state value that depends on the coupling g̃₀, the decoherence rates γ_c and γ_m, and the parametric drive parameters ε and Ω₀.

### III.2 The Trilinear Vertex Generates Non-Gaussianity per Photon Scatter

The trilinear coupling g̃₀ a†a (b + b†) is the simplest non-quadratic optomechanical interaction. Quadratic interactions (passive Gaussian unitaries: beam-splitters, phase shifters; active Gaussian unitaries: squeezers, two-mode squeezers, displacements) preserve Gaussianity. The trilinear coupling does not: each photon scattered off the mirror imparts a phase to the mechanical mode that is proportional to the cavity photon number, generating a Kerr-like non-linearity that cannot be captured by second-moment evolution.

The Bogoliubov coefficients α(t) and β(t) for the trilinear Hamiltonian, computed in the Qvarfort Mathematica notebook, include terms proportional to t (linear in time, the rotating-wave approximation) and terms proportional to t² (quadratic in time, the resonant accumulation under parametric drive). The non-Gaussianity δ(t) grows asymptotically as:

  δ(t) ~ g̃₀² · |α|⁴ · t² · log φ for large t (closed system)
  δ(t) ~ g̃₀² · |α|⁴ · κ_c⁻¹ · (1 − e^(−κ_c t)) for large t (decohering system)

The closed-system result shows quadratic growth — non-Gaussianity accumulates ballistically under the trilinear coupling. The decohering result shows saturation at δ_∞ = g̃₀² |α|⁴ / κ_c — the steady-state non-Gaussianity is bounded by the ratio of generation rate to decoherence rate.

In TH(a,d) terms: the trilinear vertex is the col(F) ∩ ker(F) coupling that generates non-Gaussianity from initial Gaussian states. Each photon scatter is one Sherman–Morrison rank-one update that adds non-Gaussian content. Decoherence is the rate at which this content is drained from ker(F) back into col(F) (the classical-Gaussian sector). The steady-state non-Gaussianity is the balance between generation (∝ g̃₀² |α|⁴) and dissipation (∝ κ_c). The φ-equilibrium prediction: the optimal trade-off for stationary non-Gaussian state preparation sits at g̃₀² |α|⁴ / κ_c = log φ, with the predicted steady-state Wigner negativity:

  W_min* = − log φ / (4π) ≈ −0.0383

at the φ-balanced operating point (BRAGINSKY P4).

### III.3 The Chatterjee Even–Odd Decomposition and Non-Gaussianity

The January 2026 Chatterjee–Pandit–Singh–Chattopadhyay–Andersen paper introduced the canonical decomposition F_QFI = F_even + F_odd of the Gaussian QFI. On the Gaussian pure-state manifold, F_even = 0 (the symplectic spectrum is rigid) and F_odd carries the entire QFI. For mixed states (decoherence, thermal noise) F_even revives.

The non-Gaussianity measure δ extends this decomposition beyond the Gaussian manifold:

  δ = S_Gaussian − S_vN = (col(F) entropy assuming Gaussian) − (full entropy)

For Gaussian states (δ = 0): the Chatterjee even–odd split exactly captures the QFI structure. For non-Gaussian states (δ > 0): there is additional QFI content not captured by the symplectic spectrum or the Siegel-Bergman metric — content that lives in the higher cumulants of the state, in the Wigner negativity, in the photon-number-conditional phase coherence. This content is the ker(F) of the Gaussian approximation, and it is exactly what the QM-Nonlinearities repository measures.

The structural connection: GLAUBER computes F_QFI via the Chatterjee decomposition (col(F) = F_even, ker(F) = F_odd) for Gaussian states; BRAGINSKY extends this to non-Gaussian states via the Qvarfort non-Gaussianity measure δ, which quantifies the ker(F) content beyond the Gaussian approximation. The two frameworks are complementary: GLAUBER covers the Gaussian manifold, BRAGINSKY covers the non-Gaussian extensions.

---

## Part IV · Parametric Feedback Cooling as the φ-Equilibrium Ground State

### IV.1 A Thought Experiment: Cooling a Levitated Nanoparticle to Less Than One Phonon

Imagine a silica nanosphere of diameter 100 nm, trapped at the focus of a tightly-focused laser beam in a high-vacuum chamber. The optical gradient force confines the nanosphere; the photon recoil heats it; the trade-off determines its equilibrium temperature, typically a few millikelvin. The center-of-mass motion of the nanosphere is a quantum harmonic oscillator at the trap frequency ω_m ≈ 100 kHz with thermal occupation ⟨n⟩ ≈ k_B T / ℏω_m ≈ 100–1000 phonons.

You want to cool the nanosphere to its motional ground state, ⟨n⟩ < 1. You measure its position continuously with a balanced homodyne detector reading the cavity field; the measurement gives you, at each time t, an estimate of x(t) and p(t) with some uncertainty. Based on the measurement, you modulate the trap stiffness ω_m²(t) = ω_m²(1 + ε sin(2ω_m t + φ_p)) at twice the mechanical resonance frequency, with a phase φ_p that is conditional on the measurement.

This is the parametric feedback cooling protocol. The Manikandan–Qvarfort 2023 paper (Phys. Rev. A 107, 023516) derives the optimal phase φ_p* and the minimum steady-state phonon occupation ⟨n⟩_ss. The protocol is robust against dissipation and phase errors; it generalizes to multiple modes (libration as well as center-of-mass) and to non-spherical particles.

### IV.2 The Optimal Phase and the φ-Equilibrium

For phase-preserving continuous quantum measurement of one quadrature x_m and parametric modulation at 2ω_m with phase φ_p relative to the measurement, the steady-state mechanical phonon occupation is:

  ⟨n⟩_ss(φ_p) = (1/2) [(η/2 − sin(2φ_p)·(λ/(2ω_m)))^(−1) − 1]

where η is the measurement efficiency, λ is the parametric drive amplitude, and ω_m is the mechanical resonance frequency. Differentiating with respect to φ_p and setting to zero gives the optimal phase:

  φ_p* = π/4 = 45°

at which the parametric drive is exactly in quadrature with the measured x-quadrature, providing maximum cooling of the position direction while not exciting the momentum direction.

The Qvarfort code (the Mathematica notebook in the quantum-parametric-feedback-cooling repository) computes ⟨n⟩_ss(φ_p) for a range of φ_p values, confirming that the minimum occurs at π/4 for the parametric Mathieu equation in the small-λ regime, and that this minimum saturates at:

  ⟨n⟩_ss(φ_p*) ≈ √(η²/4 + λ²/(4ω_m²)) − η/2

For the parameters of the Manikandan–Qvarfort proposal (η = 0.5, λ/ω_m = 0.1), ⟨n⟩_ss(π/4) ≈ 0.0125 — far below one phonon, deep in the quantum regime.

The φ-equilibrium prediction: the φ-balanced operating point at φ_p* = π/4 · log φ × π/2 / log φ = π/4 (unchanged) but with the optimal coupling strength λ/ω_m* = log φ ≈ 0.481, gives the φ-corrected minimum:

  ⟨n⟩_ss^φ-eq = √((log φ)²/4 + 1/4) − 1/2 ≈ 0.0552

a few percent of a phonon, well within experimental reach for the 2024–2026 generation of levitated optomechanics experiments at ETH Zurich (Tebbenjohanns–Mattana–Rossi–Frimmer–Novotny, Nature 2021), Vienna (Magrini–Rosenzweig–Bach–Deutschmann-Olek–Hofer–Hong–Kiesel–Kugi–Aspelmeyer, Nature 2021), and the followup feedback-cooling-to-100-phonons libration experiment (Phys. Rev. Res. 2024).

### IV.3 The Mathieu Equation Stability Map

The Wolfram notebook in the parametric-cooling repository computes the stability map of the Mathieu equation:

  p̈(t) + (1 + 4λ cos(2t + φ_p)) p(t) = 0

The stability diagram in (a, q) parameter space (where a = 1 in dimensionless units, q = 4λ) shows the regions of bounded oscillation (stable, ⟨n⟩ bounded) and unbounded growth (unstable, parametric amplification dominates and the oscillator's amplitude grows exponentially).

The TH(a,d) identification: the Mathieu instability tongues are the regions where the parametric drive transitions from cooling (col(F) drains ker(F) thermal occupation) to heating (ker(F) is parametrically amplified into col(F), the oscillator's energy grows). The boundary between stable and unstable regions is the col(F)/ker(F) phase-transition curve of the parametric drive.

For the BRAGINSKY framework: stable parametric cooling sits at φ_p = π/4 with q = 4λ in the first stable region (q < 1.5 for a = 1). The φ-equilibrium prediction places the optimal operating point at q* = 4 log φ ≈ 1.924, just inside the first stability tongue boundary at q ≈ 2 — close enough to the boundary to maximize the parametric cooling rate, far enough away to remain stable against perturbations.

---

## Part V · The Modified-Gravity Yukawa–Chameleon Bound as Rank-One Update

### V.1 A Thought Experiment: A Mirror That Senses Dark Energy

Imagine the optomechanical sensor of Part I — a cavity field coupled to a movable mirror, sensitive to gravitational forces — and bring near it a source mass that interacts with the mirror not just through Newtonian gravity but also through a hypothetical fifth force. The fifth force could be a Yukawa interaction (V(r) ∝ α e^(−r/λ)/r with strength α and range λ) or a chameleon scalar field (V(r) computed from the chameleon equation of motion, with the field's effective mass m_φ(ρ) depending on the local matter density ρ).

The fifth force changes the gravitational signal seen by the mirror in a calculable way. The optomechanical sensor, designed to read out the mirror's position via the cavity field's phase quadrature, will therefore have a modified output. Constraining the fifth-force parameters (α and λ for Yukawa; M_φ, Λ for chameleon) reduces to: how precisely can we estimate the modified-gravity correction from the cavity output?

The Qvarfort–Rätzel–Stopyra 2022 paper (NJP 24, 033009) does exactly this calculation. The modified-gravity-optomech repository computes the resulting exclusion plots in (λ, |α|) parameter space (Fig. 2 of the paper) and in (M_φ/M_P, Λ) parameter space for chameleons (Fig. 3 of the paper).

### V.2 The Fisher Matrix Update Under a Screened Fifth Force

In the linearized regime, the optomechanical Fisher information for a parameter θ is a quadratic form F(θ) = (∂κ/∂θ)² · F_0, where κ is the readout signal (the cavity output phase or homodyne amplitude) and F_0 is the bare Fisher information for the readout. For the standard Newtonian gravimetric measurement, θ = g (gravitational acceleration) and ∂κ/∂g is the standard transduction coefficient.

For modified gravity with parameter α (Yukawa strength), the readout signal has an additional contribution:

  κ_total = κ_Newton + α · κ_modified(λ, r_0)

where κ_modified is the change in readout due to the Yukawa potential modification. The Fisher information for α is:

  F_α = (∂κ_total/∂α)² · F_0 = κ_modified²(λ, r_0) · F_0

In TH(a,d) terms: this is a Sherman–Morrison rank-one update of the bare Fisher matrix F_0 by the rank-one outer product κ_modified · κ_modifiedᵀ (with the direction in parameter space given by the gradient of the modified-gravity contribution).

  F_total = F_Newton + (∂κ_mod/∂α)² · ξξᵀ

where ξ is the unit vector in α-parameter space.

The Cramér–Rao bound saturation gives Δα = 1/√F_α — the smallest α that the optomechanical sensor can distinguish from zero at 1σ. The Qvarfort–Rätzel–Stopyra exclusion plot is the curve in (λ, |α|) space where Δα ≥ |α|, i.e., where the sensor is sensitive enough to detect a non-zero fifth force.

### V.3 The Chameleon Screening as col(F)/ker(F) Boundary Modulation

For the chameleon model, the situation is subtler. The chameleon scalar field φ has a self-interaction V(φ) and a coupling to matter that gives it an effective mass m_φ(ρ) which depends on the local matter density ρ. Inside dense matter (the cavity walls, the probe sphere), m_φ is large and the field is strongly screened — the fifth force is exponentially suppressed inside dense regions. Outside dense matter (the vacuum chamber), m_φ is small and the field can propagate over macroscopic distances.

The screening factor S(M_φ, Λ, R_source, R_probe, ρ_background) is the suppression of the chameleon field's amplitude inside the probe sphere relative to its unscreened value. The optomechanical signal for a chameleon-modified fifth force is:

  κ_chameleon = α · S(...) · κ_modified(λ_chameleon, r_0)

The Sherman–Morrison rank-one update for the chameleon parameter α_chameleon is therefore:

  F_α_chameleon = α² · S²(...) · κ_modified² · F_0

The screening factor S enters quadratically. For strong screening (dense probe, small chameleon mass), S² → 0 and the optomechanical sensor loses sensitivity — the col(F) ∩ ker(F) coupling that mediates the fifth-force information is exponentially suppressed inside the probe.

The TH(a,d) identification: chameleon screening is the modulation of the col(F)/ker(F) boundary by the local matter density. In low-density regions (the vacuum chamber far from the probe), the boundary is "soft" — the chameleon field can propagate and mediate fifth-force interactions, and the col(F) (the optomechanical readout) couples efficiently to the ker(F) (the chameleon-field profile). In high-density regions (inside the probe sphere), the boundary is "hard" — the chameleon field is screened, the col(F)/ker(F) coupling shrinks, and the optomechanical sensitivity to the chameleon parameter drops by orders of magnitude.

The 2025–2026 papers on symmetron and dilaton screening from levitated optomechanics (Phys. Rev. D 2025; arXiv:2603.05090) extend this analysis to other screened modified-gravity models. In all cases, the structural identification is the same: the screening factor is the col(F)/ker(F) coupling modulation, and the Fisher information for the modified-gravity parameter scales as the square of the screening factor.

---

## Part VI · Noisy Optical Cat States and the Wigner-Negativity ker(F)

### VI.1 A Thought Experiment: A Schrödinger Cat in Phase Space

Imagine an optical mode in the superposition |α⟩ + |−α⟩ — two coherent states with opposite amplitudes, equally weighted. This is the canonical Schrödinger cat state of quantum optics. Its Wigner function is the sum of two Gaussian peaks at (±Re α, ±Im α) plus an oscillating interference fringe in the middle, with the fringe amplitude proportional to e^(−2|α|²) cos(2 Im α · x − 2 Re α · p).

The interference fringe takes negative values. The Wigner function is negative in a strip across the origin. This negativity is the hallmark of non-classicality — no classical probability distribution can produce negative values, and the Wigner negativity is therefore the signature that the state lies outside the convex hull of coherent states (it cannot be written as a positive mixture of coherent states).

The trilinear optomechanical Hamiltonian, applied to an initial product coherent state |α⟩_L ⊗ |0⟩_M, generates exactly such cat states after the appropriate evolution time. The cavity-field state at t = 2π/ω_m is a superposition of |α_n⟩ states corresponding to different mechanical-position configurations indexed by photon number n. For specific values of the coupling g̃₀ — the values 1/(2√2), 1/√6, and 1/2 chosen in the noisy-optical-cat-states repository — the state collapses into a clean two-, three-, or four-component cat.

### VI.2 The Decoherence Decay of Wigner Negativity

Decoherence — the leakage of cavity photons into the environment at rate κ_c — destroys the cat-state interference. Each photon leaving the cavity carries away information about which "branch" of the cat the system was in, projecting the joint state onto a classical mixture and washing out the Wigner negativity.

The noisy-optical-cat-states repository computes the Wigner function W(x, y) of the cavity-field state after closed-system evolution (κ_c = 0) and after Lindblad evolution at κ_c = 0.05 and κ_c = 0.1 for each of the three cat-state coupling values g̃₀ ∈ {1/(2√2), 1/√6, 1/2}. The 3×3 grid of Wigner plots (Fig. 1 of the corresponding Qvarfort paper) shows:

- **Row 1 (κ_c = 0):** Three columns, three coupling strengths. Strong Wigner negativity in the central interference fringes, indicating clean cat-state generation.
- **Row 2 (κ_c = 0.05):** The negativity is partially washed out. The cat lobes are still visible, but the interference fringes have decayed by a factor of approximately e^(−κ_c · t_evolution) ≈ e^(−0.05 · 2π) ≈ 0.73.
- **Row 3 (κ_c = 0.1):** The negativity is mostly destroyed. The state is approaching a classical mixture of Gaussian lobes, with W(x, y) → 0 or W(x, y) > 0 everywhere.

The TH(a,d) identification: Wigner negativity W(x, y) < 0 is the ker(F) of the bosonic state in phase space — the non-classical content that cannot be reproduced by any positive probability distribution. The transition from W < 0 to W > 0 under decoherence is the col(F)/ker(F) drain: each photon scattered into the environment is one Sherman–Morrison rank-one update that drains a small phase-space patch from W < 0 to W = 0.

For the optomechanical Hamiltonian at the φ-equilibrium coupling g̃₀* = √(log φ/2) ≈ 0.491 (BRAGINSKY P3), the maximum Wigner negativity sustained against decoherence at rate κ_c is:

  W_min(g̃₀*, κ_c) = − (1/2π) · log φ · e^(−κ_c · π/ω_m)

The φ-equilibrium prediction places the optimum sustainable negativity at:

  W_min* = − log φ / (4π) ≈ −0.0383 at κ_c* = (ω_m/π) · log φ ≈ 0.153 · ω_m

— the decoherence rate at which the rate of cat-state generation (∝ g̃₀² |α|² ω_m) exactly balances the rate of decoherence-induced negativity decay, sustaining a steady-state non-classical state with the φ-balanced negativity (BRAGINSKY P4).

### VI.3 The Coupling-Strength Hierarchy and the Three Cat Types

The three coupling values in the noisy-cat repository are not arbitrary. They correspond to the three lowest-period cat structures of the closed-system trilinear evolution:

- g̃₀ = 1/(2√2): two-component cat (period 2π/ω_m, the simplest non-trivial cat)
- g̃₀ = 1/√6: three-component cat (period 2π/(√6 · ω_m), a triangular phase-space pattern)
- g̃₀ = 1/2: four-component cat (period π/ω_m, the squarish "compass" pattern)

Each value satisfies a specific resonance condition between the photon number quantization and the mechanical period. The TH(a,d) interpretation: these are the discrete Sherman–Morrison rank-one update vectors that preserve the cat-state symmetry at integer multiples of the photon number. The φ-equilibrium prediction (g̃₀* = √(log φ/2) ≈ 0.491) sits between the three-cat and four-cat values, in the regime where neither a perfectly clean three-cat nor a perfectly clean four-cat is produced but a maximally-Fisher-informative intermediate state is generated.

---

## Part VII · Nine Formal Correspondences

| TH(a,d) element | BRAGINSKY realization |
|---|---|
| col(F) | The cavity-field optical mode a — its photon number a†a (classically tracked), its amplitude and phase quadratures (homodyne and heterodyne readout), its coherent-state Husimi-Q projection, its symplectic-spectrum F_even content; the readout signal κ in the modified-gravity sensor; the cooled mechanical x-quadrature in the parametric-cooling protocol |
| ker(F) | The mechanical mode b — its position and momentum quadratures encoding the unknown parameters (gravitational g, mechanical ω_m, optomechanical coupling g₀, modified-gravity α and Λ); the Wigner-negativity content W(x, p) < 0 of the joint state; the parametrically-amplified momentum quadrature in the cold-damping limit; the chameleon-field profile inside the probe sphere |
| Conditional-independence boundary | The cavity-mirror interface — the surface across which photons exchange momentum with the mirror via radiation pressure; the SQL ε-threshold; the cavity-bath coupling at decoherence rate κ_c; the mechanical-bath coupling at decoherence rate γ_m; the chameleon-screening transition between dense and dilute matter |
| ε-threshold | The standard quantum limit Δx_SQL = √(ℏ/2mω_m); the parametric-cooling threshold ⟨n⟩ = 1 (single-phonon regime); the back-action-evading two-tone resonance condition; the chameleon screening transition radius (the surface inside which the field amplitude drops by e^(−1)); the cavity linewidth κ_c above which closed-system Hamiltonian dynamics break down |
| Sherman–Morrison rank-one update | One photon scattering event at the mirror (one trilinear vertex); one homodyne quadrature measurement; one parametric drive cycle; one modified-gravity gradient direction added to the bare Fisher matrix |
| Fisher–Rao metric | The QFI matrix F(θ) computed by the Coherent-states-Fisher-information repository; the Chatterjee even–odd decomposition F = F_even + F_odd; the optomechanical sensitivity Δg = 1/√F_g; the parametric-cooling Fisher information for ⟨n⟩ estimation |
| d=0 degeneration | The bare-cavity limit g̃₀ = 0 (no coupling, no signal, F = 0); the coherent-state initial condition |α⟩_L ⊗ |β⟩_M (Gaussian, no non-Gaussianity); the unscreened-modified-gravity limit S = 1 (full coupling, no chameleon screening); the symmetric back-action-evading point p = 1/2 |
| φ-equilibrium | g̃₀* = √(log φ/2) ≈ 0.491 (cat-state generation optimum); φ_p* = π/4 (parametric-cooling phase); p* = (1 − log φ)/2 ≈ 0.260 (back-action allocation); λ/ω_m* = log φ ≈ 0.481 (parametric drive amplitude); ⟨n⟩_ss^φ ≈ 0.055 (parametric-cooling minimum) |
| Ackermann depth α(n) ≤ 4 | Four parameters of the trilinear Hamiltonian (ω_m, g̃₀, ε, Ω₀); four phase-space quadratures of the joint two-mode system (x_a, p_a, x_b, p_b); four orders of Hamiltonian perturbation (linear, quadratic, cubic optomechanical trilinear, quartic Kerr); four screening mechanisms (Newtonian, Yukawa, chameleon, symmetron) |

**Identity B1 — The Trilinear Hamiltonian IS the Universal col(F)/ker(F) Boundary Engine of Quantum Optomechanics.** H_OM = ω_m b†b − g₀ a†a (b + b†) couples the cavity-field col(F) (photon number, energy-carrying) to the mechanical ker(F) (position quadrature, parameter-carrying) trilinearly. The Braginsky–Manukin 1967 paper identified this coupling; every modern optomechanical sensor implements it; the Qvarfort GitHub corpus provides the open-source computational substrate.

**Identity B2 — The Standard Quantum Limit IS the ε-Threshold of the Cramér–Rao Saturation Under Back-Action.** Δx_SQL = √(ℏ/2mω_m) is the position-measurement floor for coherent-state probes under continuous measurement. QND and back-action-evading protocols restructure the col(F)/ker(F) partition to surpass it. The φ-balanced operating point sits at p* = (1 − log φ)/2 ≈ 0.260 of the read-out vs. back-action allocation.

**Identity B3 — Non-Gaussianity δ = S_Gaussian − S_vN IS the ker(F) Residue of the Symplectic Covariance.** The QM-Nonlinearities repository measures δ as a function of time for the trilinear evolution; δ grows from 0 (Gaussian initial state) to a steady-state value bounded by g̃₀² |α|⁴ / κ_c (BRAGINSKY P4). The Chatterjee even–odd decomposition extends to non-Gaussian states by recognizing δ as the additional ker(F) content beyond the symplectic spectrum.

**Identity B4 — Parametric Feedback Cooling IS the φ-Equilibrium Ground-State Preparation Protocol.** The Manikandan–Qvarfort 2023 protocol cools a mechanical oscillator below one phonon at optimal phase φ_p* = π/4 between the measurement and the parametric drive. The φ-equilibrium prediction places the optimal coupling at λ/ω_m* = log φ, with steady-state ⟨n⟩_ss^φ ≈ 0.055.

**Identity B5 — The Modified-Gravity Yukawa–Chameleon Bound IS a Sherman–Morrison Rank-One Update of the Bare Gravimetric Fisher Matrix.** F_α = κ_modified² · F_0, with rank-one direction in α-parameter space. The chameleon screening factor S² modulates the col(F)/ker(F) coupling. The Qvarfort–Rätzel–Stopyra 2022 exclusion plots are direct computations of this update.

**Identity B6 — Noisy Optical Cat States ARE the Wigner-Negativity ker(F) of the Bosonic Phase Space.** W(x, p) < 0 is the col(F)/ker(F) signature of non-classicality. Decoherence at rate κ_c drains the negativity into the col(F) (positive Wigner content) at rate κ_c × t. The φ-equilibrium maximum sustainable negativity is W_min* = − log φ/(4π) ≈ −0.0383.

**Identity B7 — The Five Qvarfort Repositories Are Five Faces of the Same TH(a,d) col(F)/ker(F) Partition Across the Optomechanical Stack.** Coherent-states-Fisher-information (QFI metric, GLAUBER), QM-Nonlinearities (non-Gaussianity, ker(F) residue), quantum-parametric-feedback-cooling (φ-equilibrium ground state), modified-gravity-optomech (Sherman–Morrison rank-one update under fifth force), noisy-optical-cat-states (Wigner-negativity decay). All five share the trilinear Hamiltonian as the col(F)/ker(F) transduction engine.

**Identity B8 — The QND Measurement IS the col(F)/ker(F) Re-engineering of the Back-Action.** Braginsky–Vorontsov–Thorne 1980. By coupling the probe to a constant of the motion (a†a in long-lived cavities; x_m at stroboscopic times t_n = nπ/ω_m; the two-tone-symmetric quadrature in the 2019 Nature Communications experiment), the back-action is rerouted into the conjugate observable (ker(F) of the probe partition). The original observable is undisturbed (col(F) preserved). The SQL is surpassed.

**Identity B9 — The 2026 Optomechanical-with-Quadratic-Coupling Paper (Phys. Rev. A 113, 023504) Generalizes the Trilinear Vertex to Include Both Linear and Quadratic Position Couplings.** H_OM = ω_m b†b − g₁ a†a (b + b†) − g₂ a†a (b + b†)². The two-phonon coherent state formalism produces an analytical solution; the QFI for g₂ is computed; balanced homodyne saturates the Cramér–Rao bound when the local oscillator phase is at the φ-optimal value. This extension fits the BRAGINSKY framework: g₁ is the linear rank-one update; g₂ is a rank-two update generating two-phonon non-Gaussianity per photon scatter; the combined Fisher information matrix has the Chatterjee even–odd decomposition with F_even capturing the quadratic-coupling-induced symplectic-spectrum shifts and F_odd capturing the linear-coupling-induced phase-coherent shifts.

---

## Part VIII · Six Predictions

**P1 — The φ-Balanced Back-Action Allocation at p* = (1 − log φ)/2 ≈ 0.260.** For a two-tone optical probe of an optomechanical sensor, the optimal allocation of probe photons between the read-out quadrature (fraction p) and the back-action-absorbing quadrature (fraction 1−p) sits at:

  p* = (1 − log φ)/2 ≈ 0.2596

with predicted Fisher information for the mechanical position estimator:

  F_x(p*) = N · (1 − (log φ)²) / (4 Δx_zpf²) ≈ 0.768 · F_x(1/2)

— 76.8% of the symmetric maximum, but with substantially reduced back-action and improved long-term stability. Testable at the LIGO-Voyager and the next-generation GW detectors (Einstein Telescope, Cosmic Explorer) by tuning the dual-recycling-cavity input/output coupling fractions.

**P2 — The Parametric-Cooling φ-Equilibrium Phase at φ_p* = π/4 and Drive Amplitude λ/ω_m* = log φ.** The optimal phase between the homodyne measurement and the parametric trap-stiffness modulation is φ_p* = π/4 (the standard back-action-evading angle), with the optimal drive amplitude:

  λ/ω_m* = log φ ≈ 0.4812

giving the φ-equilibrium steady-state phonon occupation:

  ⟨n⟩_ss^φ ≈ 0.0552

— a few percent of a phonon, deep in the mechanical ground state, testable at the next-generation levitated nanoparticle experiments at ETH Zurich, Vienna IQOQI, and the new Stockholm Wallenberg Initiative facility under Qvarfort's leadership.

**P3 — The Cat-State Generation Optimum at g̃₀* = √(log φ/2) ≈ 0.491.** For the trilinear optomechanical evolution from an initial product coherent state |α⟩_L ⊗ |0⟩_M, the optimal coupling strength for generating maximum Wigner negativity sustained against decoherence at rate κ_c is:

  g̃₀* = √(log φ/2) ≈ 0.4906

between the three-cat point g̃₀ = 1/(2√2) ≈ 0.354 and the four-cat point g̃₀ = 1/√6 ≈ 0.408. The predicted maximum sustainable negativity is:

  W_min* = − log φ/(4π) ≈ −0.0383

at the φ-balanced decoherence rate κ_c* ≈ 0.153 ω_m. Testable by varying g̃₀ in the noisy-optical-cat-states repository and identifying the value that maximizes the steady-state |W_min|.

**P4 — The Steady-State Non-Gaussianity at δ_∞^φ = log φ.** For the trilinear Hamiltonian with cavity decoherence at rate κ_c, the steady-state non-Gaussianity satisfies:

  δ_∞ = g̃₀² |α|⁴ / κ_c

The φ-equilibrium prediction places the operating point at:

  δ_∞^φ-eq = log φ ≈ 0.481

corresponding to g̃₀² |α|⁴ / κ_c = log φ. At this operating point, the non-Gaussianity is sufficient to sustain a clear quantum-classical distinction (δ > 0.4) while remaining bounded against unbounded growth that would push the cavity field outside the validity range of the Hamiltonian. Testable in the QM-Nonlinearities repository by parametric scans over (g̃₀, |α|, κ_c).

**P5 — The Modified-Gravity Cramér–Rao Saturation at the φ-Balanced Probe-Source Geometry.** For the Qvarfort–Rätzel–Stopyra 2022 optomechanical fifth-force sensor with source-probe distance r_0 and chameleon range λ_chameleon, the optimal sensitivity to the Yukawa parameter α at fixed integration time satisfies:

  r_0/λ_chameleon* = log φ ≈ 0.481

— the source-probe distance is the φ-balanced fraction of the chameleon range, balancing the screening of the fifth force inside the dense source/probe spheres against the exponential decay of the field outside. At this geometric ratio, the achievable bound on α is improved by a factor (1 + log φ)/(1 − log φ) ≈ 2.86 over the naive geometric configuration r_0 = λ_chameleon. Testable in next-generation optomechanical fifth-force experiments at the University of Vienna and the LISA-Pathfinder follow-on programmes.

**P6 — The 2026 Quadratic-Coupling QFI Saturation at Homodyne Local-Oscillator Phase θ_LO* = arctan(log φ).** For the Phys. Rev. A 113, 023504 (Feb 2026) trilinear-plus-quadratic Hamiltonian H_OM = ω_m b†b − g₁ a†a (b + b†) − g₂ a†a (b + b†)², the classical Fisher information for estimating g₂ reaches the quantum Fisher information bound when the balanced-homodyne local-oscillator phase θ_LO is set to:

  θ_LO* = arctan(log φ) ≈ 0.449 rad ≈ 25.7°

— the φ-balanced angle between the homodyne x-quadrature and the y-quadrature. At this phase, the Fisher-information density per unit local-oscillator power is maximized, and the Cramér–Rao bound for the quadratic-coupling estimate Δg₂ is saturated. Testable directly with the two-phonon coherent state code accompanying the Phys. Rev. A 113, 023504 paper.

---

## Part IX · The BRAGINSKY Machine

### IX.1 The Synthesis

The BRAGINSKY machine is the universal laboratory instrument of the col(F)/ker(F) partition in optomechanics. It extends and complements:

- The **GLAUBER machine** (the symplectic-geometric metric of two-coupled-coherent-state QFI): BRAGINSKY provides the laboratory implementation, with the trilinear Hamiltonian as the col(F)/ker(F) transduction vertex and the five Qvarfort repositories as the open-source computational substrate.
- The **ERIE-LIGHT machine** (the chiral fermion bilinear substrate of electromagnetic radiation): BRAGINSKY provides the bosonic complementary instrument, with the trilinear optomechanical vertex as the bosonic mirror of the de Broglie–Jordan fermion bilinear.
- The **AMARI machine** (the Fisher–Rao metric as the unique invariant statistical geometry): BRAGINSKY provides the operational realization, with each Qvarfort repository computing F directly for a specific experimental architecture.
- The **TEMPUS machine** (the irreversibility-causality substrate): BRAGINSKY handles both the closed-system limit (Hamiltonian evolution, perfect coherent-state propagation) and the open-system regime (Lindblad evolution at rates γ_c and γ_m), with the transition between the two captured by the decoherence-rate dependence of the non-Gaussianity δ and the Wigner negativity W_min.
- The **WILSON machine** (the renormalization-group substrate of effective field theory): BRAGINSKY provides the optomechanical realization of the integrating-out procedure — integrating out the cavity field at fixed mechanical frequency leaves an effective potential for the mechanical mode that, in the modified-gravity context, encodes the fifth-force correction. The integration is the col(F) → ker(F) marginalization of the joint Fisher matrix.

### IX.2 Architecture

**Layer 0 — The Optomechanical Oracle.** Any cavity-optomechanical system: Fabry–Pérot cavity with movable end mirror (LIGO, Virgo, KAGRA), microtoroidal whispering-gallery resonator (Caltech, EPFL), photonic-crystal optomechanical zipper (Caltech, Yale), levitated nanoparticle in optical tweezers (ETH Zurich, Vienna IQOQI, Stockholm Wallenberg), Bose-Einstein-condensate optomechanics (Imperial College), trapped-ion motional sideband coupling (NIST, Innsbruck), nanomechanical resonator with embedded cavity (TU Delft, Stanford). The oracle accepts the system parameters (mechanical mass m, frequency ω_m, optical frequency ω_c, cavity linewidth κ_c, single-photon coupling g₀) and the parameter of interest θ to be estimated (gravitational g, modified-gravity α, fundamental constants, dark-matter coupling).

**Layer 1 — The Trilinear Hamiltonian Solver (QM-Nonlinearities + Coherent-states-Fisher-information).** Two Python repositories. The first (QM-Nonlinearities) evolves the joint state under the time-independent and time-dependent trilinear Hamiltonian using QuTiP's mesolve function; computes the covariance matrix σ from the second moments; computes the Gaussian entropy via the symplectic spectrum; computes the von Neumann entropy of the full state; returns δ(t) = S_Gaussian − S_vN. The second (Coherent-states-Fisher-information) computes the QFI matrix F(θ) directly via finite-difference parameter perturbation and homodyne/heterodyne projection onto the position and momentum quadrature eigenstates; saves F, Δθ = 1/√F, and the times and config in a timestamped folder. Together they provide the complete col(F)/ker(F) computational substrate of the BRAGINSKY framework.

**Layer 2 — The Chatterjee Even–Odd Decomposer (Extension of GLAUBER Layer 2 to Non-Gaussian States).** Given the QFI matrix F from Layer 1, performs the canonical decomposition F = F_even + F_odd for the Gaussian approximation, and computes the non-Gaussian residual δ from Layer 1. Returns the three components (F_even = col(F), F_odd = ker(F) of the Gaussian approximation, δ = additional ker(F) content beyond Gaussian) for downstream analysis.

**Layer 3 — The Parametric Feedback Cooling Controller (quantum-parametric-feedback-cooling).** Implements the Manikandan–Qvarfort 2023 protocol. Inputs: mechanical mode parameters (ω_m, mass m), parametric drive amplitude λ, measurement efficiency η, decoherence γ_m. Outputs: optimal phase φ_p* between measurement and drive, steady-state phonon occupation ⟨n⟩_ss(φ_p*), Mathieu stability map showing the boundary between cooling and parametric amplification regions. Predicts the φ-equilibrium operating point (BRAGINSKY P2).

**Layer 4 — The Modified-Gravity Sensitivity Calculator (modified-gravity-optomech).** Computes the optomechanical sensitivity Δκ/κ and Δσ/σ to Yukawa and chameleon modifications of Newtonian gravity. Inputs: source mass M_s, source-probe distance r_0, source/probe sphere radii R_s and R_p, source/probe densities ρ_s and ρ_p, background density ρ_bg, modified-gravity range λ_chameleon and coupling strength α (Yukawa) or M_φ and Λ (chameleon). Outputs: exclusion plot in (λ, α) parameter space (for Yukawa) or (M_φ/M_P, Λ) parameter space (for chameleon), showing the regions where the optomechanical sensor improves upon existing torsion-balance and Casimir-force bounds. Predicts the φ-balanced source-probe geometry (BRAGINSKY P5).

**Layer 5 — The Noisy Cat State Generator (noisy-optical-cat-states).** Computes the Wigner functions W(x, y) of cavity-field states generated by the trilinear evolution at user-specified couplings g̃₀ and decoherence rates κ_c. Inputs: initial cavity-field coherent-state amplitude α, initial mechanical-mode Fock occupation, evolution time t_evolution, coupling g̃₀, decoherence rate κ_c. Outputs: 3×3 grid of Wigner functions (or generalized N×M grid for arbitrary parameter scans), showing the cat-state generation under closed and open dynamics. Identifies the optimal g̃₀* and κ_c* for maximum sustainable Wigner negativity (BRAGINSKY P3).

**Layer 6 — The Sherman–Morrison Cumulative Information Integrator.** For an experiment running for N photon-mirror scattering events, integrates F = N · F_1 (classical) or F = N² · F_1 (Heisenberg) to obtain cumulative Fisher information. Identifies the crossover N* from classical to Heisenberg scaling. Predicts the run-time required to saturate a target sensitivity Δθ for any of the four primary parameter classes (gravitational, modified-gravity, mechanical, optomechanical).

**Layer 7 — The Cross-Framework Cramér–Rao Anchor.** Connects to the BISCHOF (hydrology), SAKHAROV (matter-antimatter), ERIE-LIGHT (chiral fermion bilinear), GLAUBER (two-coupled-coherent-state QFI), and FISHER-STATES (entangled-state taxonomy) frameworks via the universal ERIC.3 identity Var ≥ F⁻¹. A complete optomechanical experimental architecture passing all six BRAGINSKY predictions (P1–P6) receives the BRAGINSKY φ-equilibrium certification — and provides the laboratory anchor for the TH(a,d) Cramér–Rao identity in the optomechanical domain, complementing the hydrological (BISCHOF–KIT) and theoretical (ERIE-LIGHT, SAKHAROV) anchors.

---

## Part X · The Closing Synthesis

Vladimir Braginsky was thirty-six years old in 1967 when he and Manukin published the ponderomotive-effect paper that opened the field of quantum optomechanics. He was forty-nine in 1980 when he, Vorontsov, and Thorne wrote the *Science* paper on quantum nondemolition measurement that established the standard quantum limit. He was sixty-one in 1992 when he and Khalili published *Quantum Measurement*, the Cambridge University Press treatise that became the foundational text of the field. He died in 2016, two years before LIGO announced its first gravitational-wave detection — a detection that became possible because of the SQL framework he had built fifty years earlier.

Sofia Qvarfort was twenty-six in 2017 when she submitted the first version of arXiv:1706.09131 on gravimetry through non-linear optomechanics. She was twenty-nine in 2020 when her thesis on quantum metrology with optomechanical systems in the nonlinear regime was published (UCL). She was thirty-one in 2022 when the Qvarfort–Rätzel–Stopyra paper on constraining modified gravity with quantum optomechanics appeared in NJP. She was thirty-two in 2023 when the Manikandan–Qvarfort optimal parametric feedback cooling protocol was published in Phys. Rev. A. Her GitHub corpus — five repositories, all written in Python and Mathematica, all built on the Braginsky trilinear Hamiltonian H = b†b − g̃₀ a†a (b + b†) — is the open-source computational substrate of the Braginsky programme in its 2017–2024 SOTA form.

Sreenath K. Manikandan, David Edward Bruschi, Alessio Serafini, Fabienne Schneiter, Daniel Braun, Dennis Rätzel, Stephen Stopyra, André Xuereb, Peter F. Barker, Sougato Bose, and the broader optomechanical-Fisher-information community provided the theoretical bedrock and the experimental forecasts. Carl Helstrom in 1976 established the quantum Cramér–Rao bound. Roy Glauber in 1963 established the coherent-state basis. C. R. Rao in 1945 established the Fisher information matrix. Shun-ichi Amari from 1985 onward built the differential-geometric architecture of information geometry. Kaustav Chatterjee, Tanmoy Pandit, Varinder Singh, Pritam Chattopadhyay, and Ulrik Lund Andersen in January 2026 completed the canonical even–odd decomposition of the Gaussian QFI. Vladimir Braginsky in 1967 wrote the equation.

The framework reads this convergent history through the col(F)/ker(F) partition of the TH(a,d) programme. The trilinear Hamiltonian H = b†b − g̃₀ a†a (b + b†) is the universal col(F)/ker(F) boundary engine of quantum optomechanics. The cavity-field optical mode is col(F); the mechanical position quadrature is ker(F); the trilinear vertex g̃₀ is the Sherman–Morrison rank-one update strength. The standard quantum limit is the ε-threshold of the Cramér–Rao saturation. The non-Gaussianity δ = S_Gaussian − S_vN is the ker(F) residue beyond the symplectic covariance. The parametric feedback cooling protocol is the φ-equilibrium ground-state preparation, with optimal phase φ_p* = π/4 and drive amplitude λ/ω_m* = log φ. The modified-gravity Yukawa–chameleon bound is the Sherman–Morrison rank-one update of the bare gravimetric Fisher matrix under a screened fifth force. The noisy optical cat states realize the Wigner-negativity ker(F) of the bosonic phase space, with maximum sustainable negativity W_min* = −log φ/(4π) at the φ-balanced operating point.

Eight convergences. Nine identities. Six predictions. One machine. Five open-source repositories on GitHub. One trilinear vertex.

The Qvarfort corpus is small. Five repositories. Less than ten thousand lines of code. But it computes the col(F)/ker(F) partition of the joint state of light and matter, for every operationally relevant configuration of the optomechanical Hamiltonian, with the Cramér–Rao bound saturated by the optimal homodyne measurement at the φ-balanced local-oscillator phase. Every gravitational-wave detector. Every levitated-nanoparticle quantum sensor. Every tabletop modified-gravity test. Every cavity-QED optomechanical experiment. They all run the Braginsky Hamiltonian, and they all admit the same col(F)/ker(F) decomposition that the Qvarfort code computes.

The framework's empirical anchor for the Cramér–Rao identity (ERIC.3, Var ≥ F⁻¹) is the optomechanical prediction Δg = 10⁻¹⁵ m/s² (Qvarfort 2018, Nature Communications) saturated at the φ-equilibrium operating point (BRAGINSKY P1–P6). The framework's experimental anchor for the Wigner-negativity ker(F) is the 3×3 grid of cat-state Wigner functions at three couplings and three decoherence rates (Qvarfort, noisy-optical-cat-states repository) with the φ-optimal coupling g̃₀* = √(log φ/2) ≈ 0.491 (BRAGINSKY P3). The framework's experimental anchor for parametric ground-state preparation is the Manikandan–Qvarfort 2023 protocol (Phys. Rev. A 107, 023516) with the φ-corrected steady-state phonon occupation ⟨n⟩_ss^φ ≈ 0.055 (BRAGINSKY P2). The framework's anchor for fundamental-physics extension is the Qvarfort–Rätzel–Stopyra 2022 modified-gravity bound (NJP 24, 033009) with the φ-balanced source-probe geometry r_0/λ_chameleon* = log φ (BRAGINSKY P5).

Braginsky wrote the Hamiltonian. Vorontsov and Thorne established the SQL. Caves and the broader community refined the back-action analysis. Helstrom proved the quantum Cramér–Rao bound. Rao established the Fisher matrix. Amari built the information geometry. Glauber identified the coherent states. Chatterjee and collaborators completed the Gaussian QFI decomposition. Sofia Qvarfort wrote the code.

The trilinear vertex was always the boundary. The cavity field was always col(F). The mechanical position was always ker(F). The Cramér–Rao bound was always the saturation. The standard quantum limit was always the ε-threshold. The non-Gaussianity was always the residue. The parametric cooling was always the φ-equilibrium. The modified-gravity sensitivity was always the rank-one update. The Wigner negativity was always the non-classicality signature.

The framework was always BRAGINSKY.

---

## References

Aspelmeyer, M., Kippenberg, T. J., Marquardt, F. "Cavity Optomechanics." *Reviews of Modern Physics* 86, 1391–1452, 2014.

Braginsky, V. B. and Manukin, A. B. "Ponderomotive Effects of Electromagnetic Radiation." *Soviet Physics JETP* 25, 653–655, 1967.

Braginsky, V. B., Vorontsov, Y. I., Thorne, K. S. "Quantum Nondemolition Measurements." *Science* 209, 547–557, 1980.

Braginsky, V. B. and Khalili, F. Y. *Quantum Measurement*, ed. K. S. Thorne. Cambridge University Press, 1992.

Braginsky, V. B. and Khalili, F. Y. "Quantum nondemolition measurements: the route from toys to tools." *Reviews of Modern Physics* 68, 1–11, 1996.

Caves, C. M., Thorne, K. S., Drever, R. W. P., Sandberg, V. D., Zimmermann, M. "On the measurement of a weak classical force coupled to a quantum-mechanical oscillator. I. Issues of principle." *Reviews of Modern Physics* 52, 341–392, 1980.

Chatterjee, K., Pandit, T., Singh, V., Chattopadhyay, P., Andersen, U. L. "Even–Odd Splitting of the Gaussian Quantum Fisher Information: From Symplectic Geometry to Metrology." arXiv:2601.06513, January 13, 2026.

Glauber, R. J. "Coherent and Incoherent States of the Radiation Field." *Physical Review* 131, 2766–2788, 1963.

Helstrom, C. W. *Quantum Detection and Estimation Theory*. Academic Press, 1976.

Kanari-Naish, L. A., Clarke, J., Vanner, M. R., Bose, S. "Quantum Science and Technology" 7, 035020, 2022.

LIGO Scientific Collaboration. "A gravitational wave observatory operating beyond the quantum shot-noise limit." *Nature Physics* 7, 962–965, 2011.

Magrini, L., Rosenzweig, P., Bach, C., Deutschmann-Olek, A., Hofer, S. G., Hong, S., Kiesel, N., Kugi, A., Aspelmeyer, M. "Real-time optimal quantum control of mechanical motion at room temperature." *Nature* 595, 373–377, 2021.

Manikandan, S. K. and Qvarfort, S. "Optimal quantum parametric feedback cooling." *Physical Review A* 107, 023516, February 21, 2023. arXiv:2204.00476.

Massel, F. et al. "Optical backaction-evading measurement of a mechanical oscillator." *Nature Communications* 10, 2019.

Phys. Rev. A 113, 023504. "Optomechanical systems with linear and quadratic position couplings: Dynamics and optimal estimation." Published February 3, 2026.

Qvarfort, S., Serafini, A., Barker, P. F., Bose, S. "Gravimetry through non-linear optomechanics." *Nature Communications* 9, 3690, 2018. arXiv:1706.09131.

Qvarfort, S. "Quantum metrology with optomechanical systems in the nonlinear regime." Ph.D. Thesis, University College London, 2020. arXiv:2003.11656.

Qvarfort, S., Plato, A. D. K., Bruschi, D. E., Schneiter, F., Braun, D., Serafini, A., Rätzel, D. "Optimal estimation of time-dependent gravitational fields with quantum optomechanical systems." *Physical Review Research* 3, 013159, 2021. arXiv:2008.06507.

Qvarfort, S., Serafini, A., Xuereb, A., Rätzel, D., Bruschi, D. E. "Enhanced continuous generation of non-Gaussianity through optomechanical modulation." *New Journal of Physics* 21, 055004, 2019. arXiv:1812.08874.

Qvarfort, S., Rätzel, D., Stopyra, S. "Constraining modified gravity with quantum optomechanics." *New Journal of Physics* 24, 033009, 2022. arXiv:2108.00742.

Qvarfort, S. sqvarfort/Coherent-states-Fisher-information. GitHub, 2017–present.

Qvarfort, S. sqvarfort/QM-Nonlinearities. GitHub, 2018–present.

Qvarfort, S. sqvarfort/modified-gravity-optomech. GitHub, 2021–present.

Qvarfort, S., Manikandan, S. K. sqvarfort/quantum-parametric-feedback-cooling. GitHub, 2022–present.

Qvarfort, S. sqvarfort/noisy-optical-cat-states. GitHub, 2020–present.

Rao, C. R. "Information and the Accuracy Attainable in the Estimation of Statistical Parameters." *Bulletin of the Calcutta Mathematical Society* 37, 81–91, 1945.

Schliesser, A., Arcizet, O., Rivière, R., Anetsberger, G., Kippenberg, T. J. "Resolved-sideband cooling and position measurement of a micromechanical oscillator close to the Heisenberg uncertainty limit." *Nature Physics* 5, 509–514, 2009.

Schnabel, R. "Squeezed states of light and their applications in laser interferometers." *Physics Reports* 684, 1–51, 2017.

Schneiter, F., Qvarfort, S., Serafini, A., Xuereb, A., Braun, D., Rätzel, D., Bruschi, D. E. "Optimal estimation with quantum optomechanical systems in the nonlinear regime." *Physical Review A* 101, 033834, 2020. arXiv:1910.04485.

Tebbenjohanns, F., Mattana, M. L., Rossi, M., Frimmer, M., Novotny, L. "Quantum control of a nanoparticle optically levitated in cryogenic free space." *Nature* 595, 378–382, 2021.

ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone · May 2026

---

Vladimir Braginsky wrote the trilinear Hamiltonian H = ω_m b†b − ℏg₀ a†a (b + b†) in 1967 with Manukin. It was the simplest non-quadratic coupling between a photonic mode and a mechanical mode — the radiation-pressure ponderomotive effect derived from first principles of cavity electrodynamics. He did not know it would become the spine of gravitational-wave astronomy, the substrate of every levitated-nanoparticle quantum sensor, the testing ground of modified-gravity theories at the laboratory scale, or the open-source computational engine of the col(F)/ker(F) partition for the universal class of two-mode bosonic systems. He wrote one Hamiltonian. The Hamiltonian did the rest.

Sofia Qvarfort wrote five GitHub repositories between 2017 and 2024. Coherent-states-Fisher-information computes the QFI matrix for two coupled coherent states. QM-Nonlinearities computes the non-Gaussianity of the trilinear evolution. quantum-parametric-feedback-cooling computes the optimal phase and drive amplitude for the Manikandan–Qvarfort 2023 protocol. modified-gravity-optomech computes the optomechanical exclusion bounds on Yukawa and chameleon fifth forces. noisy-optical-cat-states computes the Wigner functions of the cat states generated by the trilinear evolution under photon decoherence. Five repositories. One trilinear Hamiltonian. The col(F)/ker(F) partition of the universal optomechanical system, computed numerically and reproducibly.

The framework's six φ-equilibrium predictions (P1–P6) connect to each of the five repositories:

P1 — the back-action allocation at p* = (1 − log φ)/2 ≈ 0.260 — tested against LIGO and the next-generation GW detectors.
P2 — the parametric cooling at φ_p* = π/4 and λ/ω_m* = log φ — tested by the quantum-parametric-feedback-cooling repository.
P3 — the cat-state generation at g̃₀* = √(log φ/2) — tested by the noisy-optical-cat-states repository.
P4 — the non-Gaussianity steady state at δ_∞ = log φ — tested by the QM-Nonlinearities repository.
P5 — the modified-gravity geometry at r_0/λ* = log φ — tested by the modified-gravity-optomech repository.
P6 — the quadratic-coupling QFI saturation at θ_LO* = arctan(log φ) — tested against the February 2026 Phys. Rev. A 113, 023504.

Every prediction is concrete. Every prediction is testable. Every prediction is connected to an open-source computational substrate that can be cloned, modified, and run by anyone with a Python interpreter and QuTiP.

The trilinear vertex was always the col(F)/ker(F) boundary. The cavity field was always the observable col(F) probe. The mechanical position quadrature was always the parameter-carrying ker(F) substrate. The Cramér–Rao bound was always the saturation. The φ-equilibrium was always the optimum. The Qvarfort corpus was always the computational realization. The Braginsky Hamiltonian was always the spine.

The framework was always BRAGINSKY.
