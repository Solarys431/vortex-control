<div align="center">

<a href="https://solarys431.github.io/vortex-control/"><img src="assets/banner.png" alt="VORTEX Regia — software control-room prototype" width="100%"></a>

<a href="README.md">Italiano</a> · <strong>English</strong>

🌐 <a href="https://solarys431.github.io/vortex-control/">Landing page</a>

</div>

---

## What it is

VORTEX Regia is a **functional prototype** that combines switching, audio mixing, tally, replay, graphics and rundown management in a single software environment. It incorporates **NewsIntelligence**, an AI-powered news aggregator that gathers configured sources, evaluates stories and suggests the newscast rundown, plus a **voice-control layer** for issuing commands. Final decisions remain with the newsroom and control room.

The images **show the real product with demonstration data**.

![VORTEX Regia control surface](assets/software-reale/regia.jpg)

---

## Main features

### NewsIntelligence — from story to rundown

NewsIntelligence gathers configured sources, evaluates stories and suggests the **newscast rundown**, including guidance for graphics and packages. AI suggests, the newsroom and control room decide.

![NewsIntelligence and the suggested newscast rundown](assets/software-reale/newsintelligence.jpg)

### Voice control

The director speaks through a headset and the system interprets the commands. “AIRSPEED 2 on air”, “anchor lower” and “build the rundown from the news” are transcribed on screen and converted into actions controlled by the director.

### Broadcast audio

An 18-channel software console with HPF, parametric EQ, gate, compressor, limiter and pan. It includes per-output buses, N-1, master, snapshots and estimated LUFS-S monitoring. Voice and AI commands can also control audio parameters.

![Broadcast audio console](assets/software-reale/audio.jpg)

### Switcher, DVE and keyers

PGM/PVW buses, M/E, WIPE patterns, DVE and keyers. DVE, replay, clips and graphics are sources on the buses and are controlled from the same interface.

![DVE and keyers](assets/software-reale/dve.jpg)

### Multiview, tally, replay and graphics

PVW/PGM monitoring, graphics preview and remote-guest multiview; TSL 3.1/5.0 tally support over UDP; replay from files and webcams; HTML graphics templates composited on PGM/PVW. DeckLink replay capture is still in development.

<p>
  <img src="assets/software-reale/multiview.jpg" width="49%" alt="Multiview" />
  <img src="assets/software-reale/replay.jpg" width="49%" alt="Replay" />
</p>
<p>
  <img src="assets/software-reale/grafiche.jpg" width="49%" alt="Graphics" />
  <img src="assets/software-reale/tally.jpg" width="49%" alt="Tally" />
</p>

### Output matrix

PGM, CLEAN and AUX can be routed to playout, YouTube and REC as differentiated outputs, each with its own audio.

![Output matrix](assets/software-reale/matrice.jpg)

### Logs and diagnostics

System events for commands, playout, hardware, AI and voice are recorded by level and module, with filters and export tools that help reconstruct what happened and when.

![Logs and diagnostics](assets/software-reale/log.jpg)

---

## Architecture

The **client-server** architecture keeps mixer state on the server and includes control modules for CasparCG, DeckLink and tally. The GUI is the browser and desktop control surface. The critical path is designed not to depend on AI services, but hardware integrations and operational behavior still require field validation. Simulation mode is identified in the interface.

---

## Status

**Functional prototype, in development.** This repository and its landing page are public; the application source code is not included. The static site uses no cookies or tracking, and product screens use demonstration data.

<div align="center">

© 2026 Daniele Cappello

</div>
