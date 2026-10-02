---
title: "Accepted Papers"
description: "Papers accepted at SuRE 2026"
math: true
---

We received **27 submissions** and accepted **9 papers**, for an acceptance rate of **33%**.

A heartfelt thank you to everyone who submitted their work.
The quality and breadth of the submissions made for a difficult but rewarding selection process, and we are grateful for the community's enthusiasm around sustainable and resource-efficient AI.
We also thank our [Program Committee](/program-committee/) once more for their careful, constructive reviews.
This workshop would not be possible without their time and expertise.

The following papers have been accepted for presentation at **SuRE @ IJCAI 2026**.
See the [Schedule](/schedule/) for the presentation order.

<div style="text-align: center; margin: 1.5rem 0;">
  <a href="https://ceur-ws.org/Vol-4275/" target="_blank" class="contact-button">📚 Proceedings (CEUR-WS Vol-4275)</a>
</div>

## Full Papers

<div class="paper-cards">

<div class="paper-card" id="safety-constrained-bandit">
<h3>Safety-Constrained Contextual Bandit for Dynamic Power Management</h3>
<div class="paper-authors">Yasin Esfandiari, Karan Rajshekar, Cicy Kuriakose Agnes, Hannah Stein, Sabine Janzen, Wolfgang Maass</div>
<a class="paper-pdf" href="https://ceur-ws.org/Vol-4275/paper18.pdf" target="_blank">📄 PDF</a> <button type="button" class="paper-pdf paper-cite" data-key="esfandiari2026safety">❝ Cite</button>
<pre class="bibtex" hidden>@inproceedings{esfandiari2026safety,
  author    = {Yasin Esfandiari and Karan Rajshekar and Cicy Agnes and Hannah Stein and Sabine Janzen and Wolfgang Maass},
  title     = {Safety-Constrained Contextual Bandit for Dynamic Power Management},
  booktitle = {Proceedings of the 1st Workshop on Sustainability and Resource-Efficiency of Artificial Intelligence (SuRE 2026) co-located with IJCAI-ECAI 2026},
  editor    = {Vitor Fortes Rey and Ren{\'{e}} Schuster and Niklas Baumgarten and Sungho Suh and Tobias Christian Nauen},
  series    = {CEUR Workshop Proceedings},
  volume    = {4275},
  publisher = {CEUR-WS.org},
  address   = {Bremen, Germany},
  year      = {2026},
  url       = {https://ceur-ws.org/Vol-4275/paper18.pdf}
}</pre>
<div class="paper-abstract">

Real time AI model serving workloads are characterized by bursty and variable request patterns, yet production GPUs commonly operate at their maximum frequency, wasting substantial energy whenever latency headroom exists. Reducing energy consumption without violating tail-latency SLOs is challenging because frequency scaling affects latency in highly nonlinear, workload-dependent ways. This paper presents _HALO_ (Hierarchical Adaptive Latency-Oriented DVFS), a fully black-box power-management controller that uses probe p95 latency to classify the system into coarse safety zones, gates the set of admissible frequency actions per zone, and runs a contextual bandit within those constraints to adapt online, requiring no offline profiling, model instrumentation, or serving-framework modifications. For LLM inference on the Azure LLM Inference Trace (Coding workload), HALO reduces total GPU energy by 39.4% on the primary model and up to 50.0% across model scales, while maintaining tail latency under the SLO. Applied to LLM pretraining, the same controller reduces energy with convergence unaffected, demonstrating that the approach generalizes across both inference and training workloads.

</div>
</div>

<div class="paper-card" id="wattgpu">
<h3>WattGPU: Predicting Inference Power and Latency on Unseen GPUs and LLMs</h3>
<div class="paper-authors">Mauricio Fadel Argerich, Jonathan Fürst, Marta Patiño-Martínez</div>
<a class="paper-pdf" href="https://ceur-ws.org/Vol-4275/paper7.pdf" target="_blank">📄 PDF</a> <button type="button" class="paper-pdf paper-cite" data-key="fadelargerich2026wattgpu">❝ Cite</button>
<pre class="bibtex" hidden>@inproceedings{fadelargerich2026wattgpu,
  author    = {Mauricio {Fadel Argerich} and Jonathan F{\"{u}}rst and Marta Pati{\~{n}}o-Mart{\'{\i}}nez},
  title     = {WattGPU: Predicting Inference Power and Latency on Unseen GPUs and LLMs},
  booktitle = {Proceedings of the 1st Workshop on Sustainability and Resource-Efficiency of Artificial Intelligence (SuRE 2026) co-located with IJCAI-ECAI 2026},
  editor    = {Vitor Fortes Rey and Ren{\'{e}} Schuster and Niklas Baumgarten and Sungho Suh and Tobias Christian Nauen},
  series    = {CEUR Workshop Proceedings},
  volume    = {4275},
  publisher = {CEUR-WS.org},
  address   = {Bremen, Germany},
  year      = {2026},
  url       = {https://ceur-ws.org/Vol-4275/paper7.pdf}
}</pre>
<div class="paper-abstract">

Large Language Model (LLM) inference workloads are a rapidly growing contributor to data center energy consumption. Optimizing these deployments requires matching specific LLMs to the most efficient GPUs, but operators currently lack the tools to do so without exhaustively profiling each combination. While some predictive models exist, they still require profiling data and struggle to generalize to hardware unseen during training. To address this, we introduce WattGPU, featuring two predictive models for mean GPU power draw and Inter-Token Latency (ITL). Our approach leverages only publicly available LLM metadata and GPU specifications, eliminating the need for hardware access or profiling while enabling generalization to unseen NVIDIA server-grade GPUs and LLMs. We evaluate our models using rigorous leave-one-GPU-out and leave-one-LLM-out cross-validation on a dataset of 42 open-source LLMs (0.1B--27B parameters) and 8 GPUs under both offline and server scenarios. The mean power draw model achieves a median absolute percentage error of $\leq3.4$ % for offline and $\leq13.5$ % for server scenarios on unseen GPUs, while the latency model achieves $\leq8.5$ % in server mode, both maintaining strong GPU ranking correlations for server scenarios (Kendall $\tau\geq0.76$). Compared to standard physically grounded baselines ---Load-Scaled Thermal Design Power (TDP) for power draw and roofline for latency--- our models reduce median absolute percentage error by approximately 4$\times$ on unseen LLM-GPU combinations for server scenarios or approximately 2$\times$ for completely unseen GPUs. WattGPU's data and code are publicly available at <https://github.com/maufadel/wattgpu>.

</div>
</div>

<div class="paper-card" id="wattlayer">
<h3>WattLayer: Get Layers Right to Estimate Inference Energy of Neural Networks</h3>
<div class="paper-authors">Adrien Sardi, Marie-Line Alberi Morel, Sara Alouf, Frédéric Giroire, Joanna Moulierac</div>
<a class="paper-pdf" href="https://ceur-ws.org/Vol-4275/paper9.pdf" target="_blank">📄 PDF</a> <button type="button" class="paper-pdf paper-cite" data-key="sardi2026wattlayer">❝ Cite</button>
<pre class="bibtex" hidden>@inproceedings{sardi2026wattlayer,
  author    = {Adrien Sardi and Marie Line Alberi-Morel and Sara Alouf and Fr{\'{e}}d{\'{e}}ric Giroire and Joanna Moulierac},
  title     = {WattLayer: Get Layers Right to Estimate Inference Energy of Neural Networks},
  booktitle = {Proceedings of the 1st Workshop on Sustainability and Resource-Efficiency of Artificial Intelligence (SuRE 2026) co-located with IJCAI-ECAI 2026},
  editor    = {Vitor Fortes Rey and Ren{\'{e}} Schuster and Niklas Baumgarten and Sungho Suh and Tobias Christian Nauen},
  series    = {CEUR Workshop Proceedings},
  volume    = {4275},
  publisher = {CEUR-WS.org},
  address   = {Bremen, Germany},
  year      = {2026},
  url       = {https://ceur-ws.org/Vol-4275/paper9.pdf}
}</pre>
<div class="paper-abstract">

The widespread adoption of Artificial Intelligence (AI) has led to increasing concerns about energy consumption, yet there is a lack of standardized methodologies to accurately estimate AI inference energy consumption, particularly across various tasks and architectures.
In this study, we propose a task independent, layer-wise energy estimation model
for AI architectures.
Our model is evaluated on a large dataset of more than 100,000 layers for 295 neural network architectures across 3 widely-used tasks and 3 distinct hardware platforms.
Our approach achieves a median error of 19.6%, outperforming state-of-the-art methods.
We further show that layer-wise decomposition generalize to new tasks without complete retraining, by leveraging shared layers across architectures.
It offer tools, insights and a precise methodology to empower stakeholders in designing energy-efficient AI systems.

</div>
</div>

<div class="paper-card" id="compresskv">
<h3>CompressKV: Semantic-Retrieval-Guided KV-Cache Compression for Resource-Efficient Long-Context LLM Inference</h3>
<div class="paper-authors">Xiaolin Lin, Jingcun Wang, Olga Kondrateva, Yiyu Shi, Bing Li, Grace Li Zhang</div>
<a class="paper-pdf" href="https://ceur-ws.org/Vol-4275/paper13.pdf" target="_blank">📄 PDF</a> <button type="button" class="paper-pdf paper-cite" data-key="lin2026compresskv">❝ Cite</button>
<span class="award-badge">🏆 SuRE 2026: Best Paper</span>
<pre class="bibtex" hidden>@inproceedings{lin2026compresskv,
  author    = {Xiaolin Lin and Jingcun Wang and Olga Kondrateva and Yiyu Shi and Bing Li and Grace Li Zhang},
  title     = {CompressKV: Semantic-Retrieval-Guided KV-Cache Compression for Resource-Efficient Long-Context LLM Inference},
  booktitle = {Proceedings of the 1st Workshop on Sustainability and Resource-Efficiency of Artificial Intelligence (SuRE 2026) co-located with IJCAI-ECAI 2026},
  editor    = {Vitor Fortes Rey and Ren{\'{e}} Schuster and Niklas Baumgarten and Sungho Suh and Tobias Christian Nauen},
  series    = {CEUR Workshop Proceedings},
  volume    = {4275},
  publisher = {CEUR-WS.org},
  address   = {Bremen, Germany},
  year      = {2026},
  url       = {https://ceur-ws.org/Vol-4275/paper13.pdf}
}</pre>
<div class="paper-abstract">

Long-context large language model (LLM) inference is increasingly constrained by the memory footprint and decoding cost of key-value (KV) caches, limiting sustainable deployment on resource-constrained hardware. Existing KV cache eviction methods typically apply heuristic token scoring over all heads in GQA-based LLMs. These methods ignore the different functionalities of attention heads, leading to the eviction of critical tokens and thus degrading the performance of LLMs.
To address this issue, we propose CompressKV, a resource-efficient KV-cache compression framework for GQA-based LLMs. Instead of aggregating attention scores from all heads, CompressKV identifies Semantic Retrieval Heads (SRHs) that capture both the initial and final tokens of a prompt and semantically important mid-context evidence, and uses them to select tokens whose KV pairs should be retained.
Furthermore, CompressKV allocates cache budgets across layers according to offline estimates of layer-wise eviction error. Experiments on LongBench and Needle-in-a-Haystack show that CompressKV consistently outperforms existing KV-cache eviction methods across memory budgets. Notably, it preserves over 97\% of full-cache performance using only 3\% of the KV cache on LongBench question-answering tasks and achieves 90\% accuracy with just 0.7\% KV storage on Needle-in-a-Haystack. These results demonstrate an improved resource--performance trade-off for long-context LLM inference. Our code is publicly available at:
<https://github.com/TUDa-HWAI/CompressKV>.

</div>
</div>

<div class="paper-card" id="tinyhybrid">
<h3>TinyHybrid: Ultra-Efficient CNN-Transformer Architecture for Edge-Deployable Brain Tumor Classification</h3>
<div class="paper-authors">Krystian Krukowski, Paweł Powroźnik, Maria Skublewska-Paszkowska</div>
<a class="paper-pdf" href="https://ceur-ws.org/Vol-4275/paper10.pdf" target="_blank">📄 PDF</a> <button type="button" class="paper-pdf paper-cite" data-key="krukowski2026tinyhybrid">❝ Cite</button>
<pre class="bibtex" hidden>@inproceedings{krukowski2026tinyhybrid,
  author    = {Krystian Krukowski and Pawe{\l} Powro{\'{z}}nik and Maria Skublewska-Paszkowska},
  title     = {TinyHybrid: Ultra-Efficient CNN-Transformer Architecture for Edge-Deployable Brain Tumor Classification},
  booktitle = {Proceedings of the 1st Workshop on Sustainability and Resource-Efficiency of Artificial Intelligence (SuRE 2026) co-located with IJCAI-ECAI 2026},
  editor    = {Vitor Fortes Rey and Ren{\'{e}} Schuster and Niklas Baumgarten and Sungho Suh and Tobias Christian Nauen},
  series    = {CEUR Workshop Proceedings},
  volume    = {4275},
  publisher = {CEUR-WS.org},
  address   = {Bremen, Germany},
  year      = {2026},
  url       = {https://ceur-ws.org/Vol-4275/paper10.pdf}
}</pre>
<div class="paper-abstract">

Brain tumor classification from magnetic resonance imaging (MRI) is critical for clinical diagnosis, yet state-of-the-art deep learning models require substantial computational resources. We present TinyHybrid, an ultra-efficient CNN-Transformer hybrid architecture that achieves a mean 3-fold CV accuracy of 95.66\% with only 89K parameters and 0.047 GFLOPs - a 976$\times$ reduction in parameters compared to Swin Transformer. Our design combines depthwise separable convolutions for local feature extraction with a lightweight transformer encoder for global context modeling.\\\\ Critically, TinyHybrid achieves 2.5ms CPU inference (24$\times$ faster than Swin Transformer's 59.4ms) and requires only 0.37MB storage, enabling real-time processing on edge devices without GPU acceleration. We also present a full-scale Hybrid model achieving a mean 3-fold CV accuracy of 96.73\% with 2.25M parameters and 13.3ms CPU inference. Comprehensive ablation studies validate each architectural component, revealing that the transformer encoder is critical ($\sim$11\% accuracy impact), while attention mechanisms can be removed without accuracy loss. Aligned with the principles of Green AI, our models enable deployment in resource-constrained clinical settings, significantly reducing the carbon footprint of medical AI inference.

</div>
</div>

<div class="paper-card" id="enas">
<h3>ENAS: An Efficient Hardware-Aware Neural Architecture Search Framework for TinyML on Resource-Constrained Microcontrollers</h3>
<div class="paper-authors">Mohd Moin Khan, Naman Srivastava, Pandarasamy Arjunan</div>
<a class="paper-pdf" href="https://ceur-ws.org/Vol-4275/paper22.pdf" target="_blank">📄 PDF</a> <button type="button" class="paper-pdf paper-cite" data-key="khan2026enas">❝ Cite</button>
<pre class="bibtex" hidden>@inproceedings{khan2026enas,
  author    = {Mohd Moin Khan and Naman Srivastava and Pandarasamy Arjunan},
  title     = {ENAS: An Efficient Hardware-Aware Neural Architecture Search Framework for TinyML on Resource-Constrained Microcontrollers},
  booktitle = {Proceedings of the 1st Workshop on Sustainability and Resource-Efficiency of Artificial Intelligence (SuRE 2026) co-located with IJCAI-ECAI 2026},
  editor    = {Vitor Fortes Rey and Ren{\'{e}} Schuster and Niklas Baumgarten and Sungho Suh and Tobias Christian Nauen},
  series    = {CEUR Workshop Proceedings},
  volume    = {4275},
  publisher = {CEUR-WS.org},
  address   = {Bremen, Germany},
  year      = {2026},
  url       = {https://ceur-ws.org/Vol-4275/paper22.pdf}
}</pre>
<div class="paper-abstract">

We present ENAS, a hardware-aware Neural Architecture Search (NAS)
framework that combines a static feasibility check, a cell-based search space
supporting standard, depthwise-separable, and bottleneck blocks with optional
skip connections, and a three-stage hybrid search strategy
(random $\rightarrow$ top-$K$ $\rightarrow$ mutation) with persistent
cross-run caching. Unlike many existing NAS frameworks that rely on GPU
acceleration, ENAS is designed to operate efficiently without requiring GPUs,
making it suitable for resource-constrained development environments. We
evaluate ENAS on two TinyML benchmarks, Visual Wake Words and Melanoma Cancer,
across eight microcontrollers with memory footprints ranging from 20\,KB to
1\,MB SRAM and nine input image resolutions. Our experimental results show that
ENAS achieves mean search-time speedups of $2.41{\times}$ and $1.70{\times}$ on
the Visual Wake Words and Melanoma Cancer datasets, respectively, while
maintaining competitive test accuracy compared with the recent NanoNAS
framework. A measured resource analysis further shows that ENAS-selected models
use substantially lower peak activation RAM, the binding constraint for
microcontroller deployment at matched accuracy. Additionally, ENAS achieves
$79.4\%$ test accuracy on an STM32H743-based microcontroller, outperforming the
greedy CPU-only baseline by $2.6$ percentage points. We release the ENAS
framework as open-source at: <https://github.com/EdgeIntelligenceLab/ENAS>

</div>
</div>

</div>

## Short Papers

<div class="paper-cards">

<div class="paper-card" id="jetson-vision">
<h3>Efficient Vision Models for Jetson: Steel Classification via Knowledge Distillation</h3>
<div class="paper-authors">Yasin Esfandiari, Karan Rajshekar, Sabine Janzen, Wolfgang Maass</div>
<a class="paper-pdf" href="https://ceur-ws.org/Vol-4275/short27.pdf" target="_blank">📄 PDF</a> <button type="button" class="paper-pdf paper-cite" data-key="esfandiari2026jetson">❝ Cite</button>
<pre class="bibtex" hidden>@inproceedings{esfandiari2026jetson,
  author    = {Yasin Esfandiari and Karan Rajshekar and Sabine Janzen and Wolfgang Maass},
  title     = {Efficient Vision Models for Jetson: Steel Classification via Knowledge Distillation},
  booktitle = {Proceedings of the 1st Workshop on Sustainability and Resource-Efficiency of Artificial Intelligence (SuRE 2026) co-located with IJCAI-ECAI 2026},
  editor    = {Vitor Fortes Rey and Ren{\'{e}} Schuster and Niklas Baumgarten and Sungho Suh and Tobias Christian Nauen},
  series    = {CEUR Workshop Proceedings},
  volume    = {4275},
  publisher = {CEUR-WS.org},
  address   = {Bremen, Germany},
  year      = {2026},
  url       = {https://ceur-ws.org/Vol-4275/short27.pdf}
}</pre>
<div class="paper-abstract">

Deploying vision models at the industrial edge requires balancing accuracy against energy and latency constraints that server-oriented models cannot meet, yet prior distilled-ViT work measures efficiency through proxy metrics (FLOPs and server-GPU throughput) rather than actual on-device energy. We close this gap on the DOES non-alloyed steel-scrap benchmark (8,131 test tiles, eight EU steel grades), distilling ViT-Large and Vision-LSTM (ViL-Base, an xLSTM-based backbone) teachers into 5.5M-parameter DeiT-Tiny students and benchmarking every model on an NVIDIA Jetson Xavier NX with onboard power monitoring and latency measurement. Our distilled students achieve 88.81% and 87.07% top-1 with 2.93–3.56% accuracy gaps to their teachers, reducing inference energy by 15.9–34× and latency by 18.1–44×. To the best of our knowledge, this is also the first cross-inductive-bias comparison in knowledge distillation for vision involving a recurrent xLSTM-based teacher: same-family distillation (ViT→DeiT, 88.81%) achieves 1.74 pp higher accuracy than cross-family (ViL→DeiT, 87.07%), yet both deliver equivalent on-device efficiency.

</div>
</div>

<div class="paper-card" id="bias-eval">
<h3>Accounting for Bias Enables Sustainable LLM Evaluation</h3>
<div class="paper-authors">Harshita Katoch, David Antony Selby, Gerrit Großmann, Sebastian Josef Vollmer</div>
<a class="paper-pdf" href="https://ceur-ws.org/Vol-4275/short14.pdf" target="_blank">📄 PDF</a> <button type="button" class="paper-pdf paper-cite" data-key="katoch2026bias">❝ Cite</button>
<pre class="bibtex" hidden>@inproceedings{katoch2026bias,
  author    = {Harshita Katoch and David Antony Selby and Gerrit Gro{\ss}mann and Sebastian Vollmer},
  title     = {Accounting for Bias Enables Sustainable LLM Evaluation},
  booktitle = {Proceedings of the 1st Workshop on Sustainability and Resource-Efficiency of Artificial Intelligence (SuRE 2026) co-located with IJCAI-ECAI 2026},
  editor    = {Vitor Fortes Rey and Ren{\'{e}} Schuster and Niklas Baumgarten and Sungho Suh and Tobias Christian Nauen},
  series    = {CEUR Workshop Proceedings},
  volume    = {4275},
  publisher = {CEUR-WS.org},
  address   = {Bremen, Germany},
  year      = {2026},
  url       = {https://ceur-ws.org/Vol-4275/short14.pdf}
}</pre>
<div class="paper-abstract">

LLM-as-a-judge has become the de facto standard for scalable, subjective evaluation, yet current leaderboards compensate for systematic measurement bias by running ever more comparisons, an approach that is both statistically unsound and computationally wasteful. The root cause is an incomplete measurement model, treating LLM judges as neutral, interchangeable instruments ignores documented biases like position bias, verbosity bias, judge severity, and self-enhancement, that no volume of additional data can eliminate. We propose a unified latent variable framework that jointly models pairwise and ordinal data while explicitly correcting for these confounders, recovering reliable rankings from substantially fewer comparisons. Because fitting this model costs negligible compute relative to a single round of LLM inference, bias correction is not only more statistically rigorous but also a more sustainable approach to trustworthy evaluation.

</div>
</div>

</div>

## Position Papers

<div class="paper-cards">

<div class="paper-card" id="slag">
<h3>Generative AI has a Slag Problem</h3>
<div class="paper-authors">Vanessa Utz</div>
<div class="paper-abstract">

AI-generated content (AIGC) consumes infrastructure energy for as long as it remains stored, yet environmental research on generative AI has not addressed this. Iterative generation produces large volumes of intermediate output, most of it discarded but retained by default. This position paper, condensing a longer treatment, names that residue AI slag and distinguishes it from the low-value terminal outputs existing work calls AI slop. Both belong to a four-dimensional taxonomy that classifies AIGC by storage burden. Two proposed metrics make slag measurable: Slag Rate captures how much of a workflow becomes slag, while Waste Stream Intensity converts retained slag into annual carbon equivalents. A case application finds a Slag Rate of 0.88, meaning 88% of generated outputs were never used. Storage is a distinct phase of generative AI's environmental footprint, and the interventions that would address it are absent from current platforms.

</div>
</div>

</div>

<dialog id="cite-modal">
<pre></pre>
<div class="cite-actions">
<button type="button" data-act="copy">Copy</button>
<button type="button" data-act="download">Download</button>
<button type="button" data-act="close">Close</button>
</div>
</dialog>

<script>
(() => {
  const dlg = document.getElementById("cite-modal"), pre = dlg.querySelector("pre");
  let key;
  document.querySelectorAll(".paper-cite").forEach(b => b.addEventListener("click", () => {
    key = b.dataset.key;
    pre.textContent = b.closest(".paper-card").querySelector(".bibtex").textContent;
    dlg.showModal();
  }));
  dlg.addEventListener("click", e => {
    const act = e.target.dataset.act;
    if (e.target === dlg || act === "close") dlg.close();
    if (act === "copy") navigator.clipboard.writeText(pre.textContent).then(() => {
      e.target.textContent = "Copied!";
      setTimeout(() => e.target.textContent = "Copy", 1500);
    });
    if (act === "download") {
      const a = document.createElement("a");
      a.href = URL.createObjectURL(new Blob([pre.textContent + "\n"], {type: "application/x-bibtex"}));
      a.download = key + ".bib";
      a.click();
      URL.revokeObjectURL(a.href);
    }
  });
})();
</script>
