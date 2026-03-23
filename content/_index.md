---
title: "SuRE @ IJCAI 2026"
layout: "home"
---

<div style="display: flex; align-items: center; gap: 0.5rem; flex-wrap: wrap;">
  <img src="/img/sure-logo.png" alt="" style="height: 3em; width: auto;">
  <h1 style="margin: 0;">1st Workshop on Sustainability and Resource-Efficiency of Artificial Intelligence @ IJCAI 2026</h1>
</div>

<span class="workshop-badge">SuRE Workshop @ IJCAI 2026 · Bremen, Germany</span>

Recent progress in AI has been driven by rapid scaling of data, models, and compute—most prominently
in large language and multimodal models. This trend, however, comes with growing energy, resource,
and environmental costs that are increasingly hard to ignore.

This workshop focuses on the **sustainability of AI systems** across their lifecycle, with a particular
emphasis on **data-, compute-, and energy-efficient methods** that scale to real-world deployments.
We emphasize moving from qualitative discussions of "Green AI" to **quantitative and reproducible
methodology**, including metrics, benchmarks, and standards.

<div style="text-align: center; margin: 1.5rem 0;">
  <div id="countdown"></div>
  <a href="/cfp" class="contact-button">Submit Your Paper</a>
</div>

<script>
const deadline = new Date("2026-05-15T23:59:59-12:00").getTime();
const el = document.getElementById("countdown");
function update() {
  const now = Date.now();
  const diff = deadline - now;
  if (diff <= 0) { el.innerHTML = "<span class=\"countdown-label\">Submission deadline has passed</span>"; return; }
  const d = Math.floor(diff / 86400000);
  const h = Math.floor((diff % 86400000) / 3600000);
  const m = Math.floor((diff % 3600000) / 60000);
  const s = Math.floor((diff % 60000) / 1000);
  el.innerHTML = "<span class=\"countdown-label\">Submission deadline:</span> " + d + "d " + h + "h " + m + "m " + s + "s";
}
update();
setInterval(update, 1000);
</script>

---

## Important Dates

<div class="deadline-alert">
All deadlines are <strong>Anywhere on Earth (AoE)</strong>.
</div>

| Milestone | Date |
|---|---|
| 📄 Submission deadline (all tracks) | **May 15, 2026** |
| 📬 Notification of acceptance | **June 1, 2026** |
| 📝 Camera-ready deadline | **June 15, 2026** |
| 🗓️ Workshop day | **August 2026 (TBD)** |

---

## Submission Tracks

| Track | Length | Purpose |
|:---|:---:|:---|
| **Full Papers** | 7 main + 2 ref | Original research |
| **Short Papers** | 4 main + 1 ref | Work-in-progress |
| **Position Papers** | 2 main + 1 ref | Visions & open challenges |

👉 [Full Call for Papers →](/cfp)

---

## Sponsored by

This workshop is sponsored by the [Carl Zeiss Foundation](https://www.carl-zeiss-stiftung.de/) via the [Sustainable Embedded AI](https://sembai.cs.uni-kl.de/) project.

<div class="funder-strip sponsor-strip">
  <a href="https://www.carl-zeiss-stiftung.de/" target="_blank"><img src="/img/czs.png" alt="Carl Zeiss Stiftung" title="Carl Zeiss Stiftung"></a>
  <a href="https://sembai.cs.uni-kl.de/" target="_blank"><img src="/img/sembedai.png" alt="Sustainable Embedded AI" title="Sustainable Embedded AI"></a>
</div>

---

## Organized by

<div class="funder-strip">
  <a href="https://www.dfki.de/" target="_blank"><img src="/img/dfki.png" alt="DFKI – German Research Center for AI" title="DFKI"></a>
  <a href="https://rptu.de/" target="_blank"><img src="/img/rptu.png" alt="RPTU Kaiserslautern-Landau" title="RPTU"></a>
  <a href="https://www.uni-heidelberg.de/" target="_blank"><img src="/img/heidelberg.jpg" alt="Heidelberg University" title="Heidelberg University"></a>
  <a href="https://www.korea.ac.kr/" target="_blank"><img src="/img/korea-uni.jpg" alt="Korea University" title="Korea University"></a>
</div>

