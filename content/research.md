---
title: "Research"
heading: "Research Experience"
boxes:
  - title: "Themes"
    items:
      - "Quantum machine learning"
      - "QKD security"
      - "Quantum error correction"
      - "Quantum networks"
      - "Quantum metrology"
---

<p style="color:#777;font-size:13px">Research programmes I lead, each with an accompanying simulation
codebase. All quantum results are simulation-based; no claim is made about performance on real hardware
unless stated. For the resulting manuscripts, see <a href="publications.html">Publications</a>.</p>

<div class="proj">
<h4>NEMA-Q &mdash; Hyperbolic Quantum-Classical Graph Neural Network
  <span class="badge badge-success">Accepted</span>
  <span class="badge badge-primary">M.Sc. Thesis</span>
  <span class="pull-right" style="font-weight:400;color:#777">2026 &ndash; Present</span></h4>
<div class="proj-stack">Python, PennyLane, PyTorch, SHAP &nbsp;&middot;&nbsp;
  <a href="https://github.com/Mahadi5577/Nema-Q" target="_blank"><i class="fa fa-github"></i> Code</a></div>
<ul>
  <li>Hybrid quantum-classical GNN operating in hyperbolic (Poincar&eacute;) space for node classification,
    paired with a five-principle explainability suite.</li>
  <li>Introduced Quantum Observable Attribution (QOA): per-node gradients of class logits with respect to
    measured quantum observables, cross-checked against input integrated gradients and SHAP over the fused
    representation.</li>
  <li>Component-isolating ablations over five seeds; negative results reported honestly, including seed
    variance, a minority-class F1 collapse, and evidence that noise stability comes from the classical bypass
    rather than intrinsic quantum robustness.</li>
  <li>Accepted as a regular research paper at ICEQT'26; Springer Nature proceedings.</li>
</ul>
</div>

<div class="proj">
<h4>ML Detection of Quantum-Hacking Attacks on Decoy-State BB84
  <span class="badge badge-info">Under Review</span>
  <span class="pull-right" style="font-weight:400;color:#777">2026 &ndash; Present</span></h4>
<div class="proj-stack">Python, PyTorch, scikit-learn, NumPy</div>
<ul>
  <li>Decoy-state BB84 simulator with physics-level intercept-resend, photon-number-splitting, and
    detector-blinding attack models, validated by ten simulator consistency checks.</li>
  <li>Benchmarked 1-D CNN, BiLSTM, and MLP detectors against two incumbent baselines &mdash; a QBER threshold
    and decoy Y<sub>1</sub>/e<sub>1</sub> bounds with a gain-ratio consistency check &mdash; at a matched
    false-alarm rate over five seeds.</li>
  <li>Per-attack detection gains of +6.1 (intercept-resend), +14.8 (PNS), and +66.6 (blinding) points against
    the stronger incumbent for each attack; AUC 0.918 vs 0.763.</li>
  <li>Online sliding-window latency measured at a 1% session false-alarm rate; evaluated under
    distribution-shift and leave-one-attack-out protocols.</li>
</ul>
</div>

<div class="proj">
<h4>QKD-IDS &mdash; Deep SVDD Pipeline for Zero-Day QKD Intrusion Detection
  <span class="pull-right" style="font-weight:400;color:#777">2026 &ndash; Present</span></h4>
<div class="proj-stack">Python, PyTorch, scikit-learn &nbsp;&middot;&nbsp;
  <a href="https://github.com/Mahadi5577/Deep-SVDD-" target="_blank"><i class="fa fa-github"></i> Code</a></div>
<ul>
  <li>52,000-window physics-grounded benchmark for unsupervised intrusion detection on a 25 km decoy-state
    BB84 link, with two of six attack families held out entirely from training.</li>
  <li>Deep SVDD one-class detectors plus a fusion ensemble, evaluated leave-one-attack-out to measure genuine
    zero-day generalization rather than in-distribution recall.</li>
  <li>Deterministic release with checksum manifest, Croissant metadata, and a public leaderboard scaffold.</li>
</ul>
</div>

<div class="proj">
<h4>Cross-Code Logical Teleportation Simulator
  <span class="pull-right" style="font-weight:400;color:#777">2026 &ndash; Present</span></h4>
<div class="proj-stack">Python, Stim, NumPy, SciPy</div>
<ul>
  <li>Constructed and verified a heterogeneous CSS adapter merging a distance-3 surface code with the
    bivariate-bicycle [[72,12,6]] code &mdash; commutation, logical count, and distance confirmed across five
    independent search seeds; a distance-5 case matched its predicted bound exactly.</li>
  <li>Circuit-level Stim syndrome-extraction cycle for the BB code, with a valid six-layer CNOT schedule
    derived from bipartite edge-colouring of the provably 6-regular check graph.</li>
  <li>Diagnosed and fixed a determinism bug caused by mixing X- and Z-check CNOTs within a round; root cause
    isolated through Heisenberg-picture analysis and confirmed empirically.</li>
</ul>
</div>

<div class="proj">
<h4>EA-CQC &mdash; Entanglement-Assisted Covert Quantum Communication Simulator
  <span class="pull-right" style="font-weight:400;color:#777">2025 &ndash; Present</span></h4>
<div class="proj-stack">Python, NumPy, SciPy, Matplotlib</div>
<ul>
  <li>Closed-form capacity analysis comparing unassisted Gaussian and entanglement-assisted (TMSV) schemes
    over thermal-loss bosonic channels.</li>
  <li>Computed quantum relative entropy, quantum Chernoff bound, finite-blocklength penalties, and Square Root
    Law scaling without approximation.</li>
  <li>Validated 21 analytical invariants, including EA dominance, dispersion ordering, and monotone
    transmissivity-sweep behaviour.</li>
</ul>
</div>

<div class="proj">
<h4>Congestion-Triggered Distillation &mdash; Quantum-Repeater Buffer Management
  <span class="badge badge-primary">B.Sc. Thesis</span>
  <span class="pull-right" style="font-weight:400;color:#777">2025 &ndash; Present</span></h4>
<div class="proj-stack">Python, NumPy, Matplotlib &nbsp;&middot;&nbsp;
  <a href="https://github.com/Mahadi5577/Congestion-Triggered-Entanglement-Distillation-for-Quantum-Repeaters" target="_blank"><i class="fa fa-github"></i> Thesis code</a>
  &nbsp;&middot;&nbsp;
  <a href="https://github.com/Mahadi5577/Congestion-Triggered-Distillation-Turning-Buffer-Saturation-into-Entanglement-Quality" target="_blank"><i class="fa fa-github"></i> Manuscript code</a></div>
<ul>
  <li>My undergraduate thesis, now extended into a manuscript targeting IEEE Transactions on Quantum
    Engineering.</li>
  <li>Dual-threshold Congestion-Triggered Distillation policy for quantum-repeater entanglement memories under
    Poisson traffic.</li>
  <li>Three-way policy benchmark (Always-Distill, Never-Distill, CTD) across hardware-sensitivity and
    jitter-robustness scenarios.</li>
  <li>Demonstrated yield improvements and reduced memory-cutoff waste across parameter sweeps.</li>
</ul>
</div>

<div class="proj">
<h4>GME Certification Tool &mdash; SDP Witness for a 2&times;3&times;3 Qudit System
  <span class="pull-right" style="font-weight:400;color:#777">2025 &ndash; Present</span></h4>
<div class="proj-stack">Python, CVXPY, NumPy</div>
<ul>
  <li>Exact fidelity-based thresholds for genuine multipartite entanglement in composite-dimension qudit
    systems via semidefinite programming.</li>
  <li>Derived and verified a PPT-criterion-based SDP witness with a numerical certificate confirming GME above
    the computed thresholds.</li>
  <li>Decoherence model and hardware-noise robustness analysis for realistic near-term devices.</li>
</ul>
</div>

<div class="proj">
<h4>Distributed Quantum Sensing &mdash; Adaptive Entanglement Allocation
  <span class="pull-right" style="font-weight:400;color:#777">2026 &ndash; Present</span></h4>
<div class="proj-stack">Python, NumPy, SciPy</div>
<ul>
  <li>Partitioning of an N-sensor array into parallel GHZ blocks under heterogeneous, time-varying local
    dephasing, using quantum Fisher information as the figure of merit.</li>
  <li>Quantified how much of the optimal allocation's advantage survives non-oracle noise knowledge.</li>
</ul>
</div>

<div class="proj">
<h4>Variational-Circuit Trainability &mdash; Magic Anchors &amp; DLA Criteria
  <span class="pull-right" style="font-weight:400;color:#777">2026 &ndash; Present</span></h4>
<div class="proj-stack">Python, PennyLane, NumPy</div>
<ul>
  <li>Magic-anchored initialization: Clifford / Clifford+T native parameter points with trainability
    certificates, plus a parity obstruction result that ruled out a naive hardness-by-echo construction.</li>
  <li>Numerical verification that gradient variance is governed by the dynamical Lie algebra dimension rather
    than the Hilbert-space dimension, with multi-seed error bars and off-model replication on an XXZ-HVA
    ansatz.</li>
</ul>
</div>

<div class="proj">
<h4>QRC-ECG &mdash; Quantum Reservoir Computing with a Surrogate Advantage Audit
  <span class="pull-right" style="font-weight:400;color:#777">2026 &ndash; Present</span></h4>
<div class="proj-stack">Python, Qiskit, scikit-learn</div>
<ul>
  <li>Fixed, untrained &le;10-qubit gate-model reservoir with a trained classical linear readout &mdash;
    barren-plateau-free by construction.</li>
  <li>Every quantum result audited against a matched classical echo-state network surrogate and a noise sweep,
    so any claimed advantage is testable rather than asserted.</li>
</ul>
</div>

<div class="proj">
<h4>Seam-Aware Real-Time Decoding for Multi-QPU Surface Codes
  <span class="badge badge-default">Early stage</span>
  <span class="pull-right" style="font-weight:400;color:#777">2026 &ndash; Present</span></h4>
<div class="proj-stack">Python, Stim, queueing analysis</div>
<ul>
  <li>Models a distance-d surface-code patch split across two QPUs, where seam stabilizers consume heralded
    Bell pairs each syndrome round.</li>
  <li>Compares stall (synchronous) and skip (asynchronous) failure regimes when a Bell pair is unavailable at
    a round boundary, treating skipped checks as time-like erasures at known locations in the matching graph.</li>
</ul>
</div>