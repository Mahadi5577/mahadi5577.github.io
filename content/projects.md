---
title: "Projects"
boxes:
  - title: "Build Stack"
    items:
      - "Kotlin / Android SDK"
      - "Node.js / WebSockets"
      - "Python / PyTorch"
      - "IoT &amp; LoRa"
      - "HTML / CSS / JavaScript"
---

<p style="color:#777;font-size:13px">Things I have built and shipped. For research programmes and their
simulation codebases, see <a href="research.html">Research</a>.</p>

<div class="proj">
<h4>Laptop IO &mdash; Android Phone as a Wireless Keyboard and Trackpad
  <span class="badge badge-success">Shipped</span>
  <span class="pull-right" style="font-weight:400;color:#777">2026</span></h4>
<div class="proj-stack">Kotlin, Android SDK, Node.js, WebSockets, nut.js</div>
<ul>
  <li>Two-part product: a Kotlin Android client (trackpad, mouse buttons, full keyboard, media keys) and a
    Node.js server that injects the events into Windows over the local network.</li>
  <li>Secured with TLS and a trust-on-first-use certificate pin, a fresh six-digit pairing code each launch,
    long-lived per-device tokens, schema validation on every inbound message, and a five-strike per-IP
    lockout.</li>
  <li>Power and open-URL capabilities are blocked by default and must be explicitly enabled; the wire protocol
    is versioned so a mismatched client is told to update rather than misbehave.</li>
  <li>Reads the laptop's Precision Touchpad cursor-speed setting and applies a matching acceleration curve, so
    the phone pad feels like the built-in touchpad.</li>
  <li>Packaged for real use: signed release keystore, QR-code pairing, and a one-click server launcher.</li>
</ul>
</div>

<div class="proj">
<h4>SmartFarmX &mdash; Off-Grid Farm Monitoring System
  <span class="badge badge-success">Deployed</span>
  <span class="pull-right" style="font-weight:400;color:#777">May 2025 &ndash; August 2025</span></h4>
<div class="proj-stack">IoT, LoRa, Web Development</div>
<ul>
  <li>Monitoring system for remote farm fields with no internet reliance, using LoRa radio links between field
    nodes and a gateway.</li>
  <li>Real-time sensor data visualization through a responsive web interface.</li>
</ul>
</div>

<div class="proj">
<h4>QKD-IDS-v5 &mdash; Public Benchmark Dataset Release
  <span class="badge badge-warning">Open Data</span>
  <span class="pull-right" style="font-weight:400;color:#777">2026</span></h4>
<div class="proj-stack">Python, PyTorch, Croissant metadata</div>
<ul>
  <li>Packaged a 52,000-window QKD intrusion-detection benchmark as a reusable public artifact: frozen CSV
    splits, per-feature data dictionary, Datasheets-for-Datasets record, SHA-256 manifest, and a leaderboard
    scaffold.</li>
  <li>One-command deterministic regeneration path, so any user can rebuild the release byte-for-byte from
    seed 42.</li>
  <li>Data released under CC-BY-4.0, code under MIT.</li>
</ul>
</div>

<div class="proj">
<h4>Academic Portfolio Website
  <span class="pull-right" style="font-weight:400;color:#777">2026</span></h4>
<div class="proj-stack">HTML, CSS, Bootstrap, GitHub Pages</div>
<ul>
  <li>This site &mdash; a static, dependency-light academic homepage covering publications, research
    programmes, projects, and awards.</li>
</ul>
</div>