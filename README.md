<div align="center">
  <a href="https://dhuvie.github.io/Dhuvie/terminal.html">
    <img src="./banner.svg" alt="readelf -h memory.bin: Dhruv Narayan Bajaj" width="100%" />
  </a>
</div>

<details>
<summary><b>readelf -a memory.bin</b> (click to expand the full header, not just the summary shown above)</summary>

```
ELF Header:
  Magic:   7f 45 4c 46 02 01 01 00 00 00 00 00 00 00 00 00
  Class:                             ELF64
  Data:                              2's complement, little-endian
  Type:                              EXEC (Full-Stack Engineer and Systems Programmer)
  Machine:                           Next.js/TS, Rust, C++, OpenGL, PyTorch
  Entry point address:               0x00000000dhruv

Section Headers:
  [Nr] Name              Type        Size      Notes
  [ 0] .text             ABOUT       n/a       who I am, in more than one paragraph
  [ 1] .dynsym           SYMTAB      5 of 18   featured repositories, expandable below
  [ 2] .rodata           CONST       2         active research areas
  [ 3] .symtab           SYMTAB      17        languages, frameworks, infra
  [ 4] .init             LIVE        instant   real-time status, refreshed per request
  [ 5] /proc             LIVE        daily     real GitHub data, refreshed by CI
  [ 6] .dynamic          LINK        daily     dependency graph, built from real repo data
  [ 7] .comment          META        n/a       the one section that isn't serious

Program Headers:
  Type    Offset     VirtAddr    FileSiz  MemSiz  Flg  Align
  LOAD    0x000000   0x00000000  n/a      n/a     R E  hire me if it compiles
```
</details>

<p align="center">
  <a href="https://dhruvnarayanbajaj.dev/"><img src="https://img.shields.io/badge/dhruvnarayanbajaj.dev-0A0E14?style=flat-square&logo=vercel&logoColor=4FD6FF" /></a>
  <a href="mailto:dhruvnarayanbajaj@gmail.com"><img src="https://img.shields.io/badge/email-0A0E14?style=flat-square&logo=gmail&logoColor=FFB454" /></a>
  <a href="https://dhuvie.github.io/Dhuvie/terminal.html"><img src="https://img.shields.io/badge/terminal-0A0E14?style=flat-square&logo=gnometerminal&logoColor=7EE787" /></a>
</p>

---

<div align="center">

### this readme is a static file. the terminal below is alive.

<a href="https://dhuvie.github.io/Dhuvie/terminal.html">
  <img src="./terminal-launch.svg" alt="launch the interactive terminal" width="100%" />
</a>

A real terminal running on a static page. Boot sequence, CRT scanlines, a
virtual filesystem you can `cd` and `cat` through, tab completion, command
history, easter eggs, and a guestbook. No build step, no framework, one HTML
file. Click the card above to open it.

</div>

---

<br/>
<p><code>.text</code></p>

## About

I am a full-stack engineer, systems programmer, and occasional AI enthusiast. My work sits in an unusual middle ground: I design and ship complete products end to end, then go a layer deeper and build the infrastructure those products actually run on, rather than treating that infrastructure as someone else's problem. Most engineers pick a lane, product surfaces or platform internals, and stay in it. I have spent the last few years deliberately refusing to choose, because the most interesting failures I have seen in production happened exactly at the seam between the two: a feature that shipped cleanly, then collapsed the moment it met a real database, a real network, or a real adversarial user.

On the product side, that means modern full-stack applications built on Next.js 15, TypeScript, and scalable backends, often solving problems with machine learning and generative AI. I reach for the right tool rather than the fashionable one: XGBoost for structured prediction, PyTorch where a custom model earns its keep, and Google Gemini where a large language model is genuinely the correct primitive rather than the default people reach for when they have run out of ideas. On the systems side, it means writing a distributed version-control system in Rust, building a WebAssembly sandbox to run untrusted plugins safely, and writing real-time OpenGL engines with classical AI behavior underneath them. A\* and Dijkstra do the actual pathfinding instead of a black box I cannot reason about.

The projects below are not toy demos. **AgriVision AI** predicts crop yield and detects pest and disease pressure for Indian farmers, in a setting where a wrong answer costs someone a season. The **UPI fraud detector** runs real-time predictions against Indian digital payment transactions at an 87 percent F1-score, against data that is noisy, imbalanced, and adversarial by construction. I care about the difference between a project that compiles and a project that would survive contact with a real user, and I try to build the second kind. If a system cannot survive the user, the model, and the network all misbehaving at once, it is not done yet.

<div align="center">
  <a href="https://dhruvnarayanbajaj.dev">
    <img src="./hero.svg" alt="dhruv.ts compiling" width="100%" />
  </a>
</div>

<div align="center">
  <img src="./snake.svg" alt="animated contribution snake over the heap" width="100%" />
</div>

<br/>
<p><code>.dynsym</code></p>

## Featured work

<div align="center">
  <img src="./projects.svg" alt="symbol table of featured repos" width="100%" />
</div>

<details>
<summary><b>agrivision-ai</b> (an AI-powered agricultural intelligence platform)</summary><br/>

Crop yield prediction, pest and disease detection, soil analysis, and market intelligence for Indian farmers. Built to run where bandwidth is unreliable and a wrong answer is expensive, so the inference path is defensive about latency and the model choices are defensive about edge deployment. Gemini handles the unstructured agricultural queries; structured yield and risk prediction stays on classical and gradient-boosted models where the decision boundary is auditable.

`Next.js 15 · Google Gemini · TypeScript`

&middot; [Open repository](https://github.com/Dhuvie/agrivision-ai)
</details>

<details>
<summary><b>Pac-man</b> (a modern C++ Pac-Man with real ghost AI)</summary><br/>

A\*/Dijkstra pathfinding driving four distinct ghost personalities, OpenGL rendering, and particle effects. This is the project in this list that exists purely because I wanted to write the algorithm myself instead of importing it, and the difference shows: each ghost has a genuinely different pursuit strategy, and the pathing degrades gracefully when the maze state changes mid-frame.

`C++17 · OpenGL · CMake`

&middot; [Open repository](https://github.com/Dhuvie/Pac-man)
</details>

<details>
<summary><b>DashCode</b> (a competitive programming analytics dashboard)</summary><br/>

Tracks LeetCode, Codeforces, CodeChef, and HackerRank in one place, with live streaks and global leaderboards. Four inconsistent APIs normalized into one coherent model, with a Postgres layer that handles the awkward fact that "a contest" means something different on every platform.

`Next.js · TypeScript · PostgreSQL`

&middot; [Open repository](https://github.com/Dhuvie/DashCode)
</details>

<details>
<summary><b>UPI-ML-Fraud-Detection</b> (real-time transaction fraud detection)</summary><br/>

Tuned to an 87 percent F1-score over Indian UPI transactions, served through notebooks and a Flask API. The interesting part is not the score. It is the class imbalance, the adversarial drift of fraud patterns, and the cost asymmetry between a false positive (a blocked payment) and a false negative (a stolen one). The pipeline is built around that asymmetry rather than around raw accuracy.

`Python · XGBoost · Scikit-learn · Flask`

&middot; [Open repository](https://github.com/Dhuvie/UPI-ML-Fraud-Detection)
</details>

<details>
<summary><b>UniSlot</b> (real-time slot booking and chat for university students)</summary><br/>

Live booking and messaging with AI-driven content moderation built into the chat layer. The moderation is not an afterthought bolted on at the end; it runs inline on the message stream so toxic content never round-trips to the other client, which is the only design that actually protects a user.

`Node.js · Firebase · JavaScript`

&middot; [Open repository](https://github.com/Dhuvie/UniSlot)
</details>

<br/>
<p><code>.rodata</code></p>

## Research

<table>
<tr>
<td width="50%" valign="top">

### Adaptive quantization in TinyML

Dynamic, per-layer, runtime-aware quantization to push state-of-the-art accuracy on microcontrollers with under 512 KB of RAM, while cutting energy consumption three to five times over static eight-bit methods. The core idea is that not all layers deserve the same precision at the same moment. A convolution near the input and a classifier near the output fail in very different ways, and a static bit-width throws away budget on layers that could tolerate less.

</td>
<td width="50%" valign="top">

### Memory forensics

Lightweight tooling and algorithms for post-mortem and live data recovery, anomaly detection, and reverse engineering in constrained embedded environments. The constraint is the point: full desktop forensic stacks do not fit, so the work is about which signals you can recover from a partial, possibly-corrupted image when you cannot assume the kernel is telling you the truth.

</td>
</tr>
</table>

<br/>
<p><code>.symtab</code></p>

## Stack

<div align="center">

**Languages**

<img src="https://skillicons.dev/icons?i=ts,rust,cpp,python,c,js" />

**Frameworks and libraries**

<img src="https://skillicons.dev/icons?i=nextjs,react,pytorch,flask,opengl,nodejs" />

**Infrastructure and tools**

<img src="https://skillicons.dev/icons?i=git,docker,wasm,linux,vercel,vscode" />

</div>

<br/>
<p><code>.init</code></p>

## Live status

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://dhuvie.vercel.app/api/status">
  <source media="(prefers-color-scheme: light)" srcset="https://dhuvie.vercel.app/api/status?theme=light">
  <img src="https://dhuvie.vercel.app/api/status" alt="real-time status: current time in IST and latest public GitHub activity" width="100%" />
</picture>

<br/>
<p><code>/proc</code></p>

## Live memory

<div align="center">
  <img src="./dump.svg" alt="live language and commit activity" width="100%" />
</div>

<br/>
<p><code>.dynamic</code></p>

## Dependency graph

<div align="center">
  <img src="./linker.svg" alt="linker map: shared languages resolved into repositories" width="100%" />
</div>

<br/>
<p><code>.comment</code></p>

<div align="center">
  <img src="./pacman.svg" alt="a small looping Pac-Man scene: the author's own C++ project chases him along a dotted line of his tech stack" width="100%" />
</div>

<br/>

<div align="center">
  <a href="https://dhuvie.github.io/Dhuvie/terminal.html"><img src="https://img.shields.io/badge/launch%20interactive%20terminal-0A0E14?style=for-the-badge&logo=gnometerminal&logoColor=4FD6FF" /></a>
</div>

<br/>
<div align="center">
  <sub>Always glad to talk systems, machine learning, or why I keep rewriting tools that already exist. Reach out anytime.</sub>
</div>
