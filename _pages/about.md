---
layout: about
title: about
permalink: /
subtitle: Division of Artificial Intelligence Engineering, <a href='https://www.sookmyung.ac.kr'>Sookmyung Women's University</a>

profile:
  align: right
  image: SNSecLab_2026.JPG
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>SNSec Lab. members (Feb 27, 2026)</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

## Welcome to SNSec Lab
SNSec Lab. investigates and addresses cybersecurity challenges in Internet service applications through a data-driven approach that utilizes machine learning and deep learning methodologies. Our team analyzes massive live data streams to secure computer systems and networks from evolving threats, leveraging experience with diverse datasets including commercial server-side logs, root DNS servers, mobile payment transactions, and car hacking activities.

We specialize in identifying and explaining intrusions in connected vehicles, notably employing anomaly detection techniques trained solely on benign data.

<div class="text-center mt-3 mb-4">
  <a href="https://auth.snsec.net" target="_blank" rel="noopener" role="button"
     style="display:inline-block; padding:0.55rem 1.5rem; border-radius:0.3rem; font-weight:600; color:#fff; background-color:var(--global-theme-color); text-decoration:none;">
    🔐&nbsp; Lab members &mdash; sign in at auth.snsec.net &nbsp;&rarr;
  </a>
  <div style="font-size:0.8rem; margin-top:0.4rem; opacity:0.75;">
    Single sign-on to the lab's self-hosted services &amp; Google&nbsp;Workspace
  </div>
</div>

### Key Research Areas

*   **Trustworthy Network Intrusion Detection:** We aim to move beyond simple classification accuracy to build systems that are robust, adaptive, and explainable using Foundation Models.
    *   **Multi-modal Traffic Representation & Pre-training:** Integrating payload bytes, packet sequences, and protocol metadata to learn comprehensive traffic representations without information loss.
    *   **Drift Resilience & Efficient Adaptation:** Developing unsupervised metrics to detect concept drift in real-time and utilizing parameter-efficient fine-tuning (PEFT) to adapt models to new environments with minimal cost.
    *   **Generative & Causal Reasoning:** Applying generative AI to not only detect threats but also explain their causes (causal reasoning) and suggest response scenarios.

*   **Automotive Security:** We are developing an **Explainable Unsupervised IDS for Automotive Ethernet** and researching standardized intrusion prevention systems for connected vehicles to offer practical solutions for both industry and academia.

*   **Advanced Threat Detection:** We are developing **DRIFT (Drift-Resilient Invariant-Feature Transformer)**, an advanced DGA detector that uses a hybrid tokenization strategy and multi-task self-supervised pre-training to maintain robustness against evolving domain generation algorithms.

*   **AI-driven Proactive Resilience:** We engineer autonomous solutions that transform reactive defense into proactive resilience by bridging the gap between deep system telemetry (Linux, Windows, macOS) and multi-modal Foundation Models. Our goal is to automate the real-time situational assessment of live systems and identify potential cybersecurity issues before they escalate. [Read more about our research vision here.]({{ '/blog/2026/vision-cybersecurity-ai/' | relative_url }})

{% include figure.liquid path="assets/img/about_research.png" class="img-fluid z-depth-1 rounded" %}

## Research and collaborations in progress

*   Bi-modal *Enhanced* Explainable IDS for Controller Area Network (with Dr. Hyunjae Kang)
*   Explainable IDS for Automotive Ethernet (with Jisoo Kim)
*   Meta-learning based few-shot IDS for IoT devices (with the University of Queensland)
*   J1939 based IDS for connected vehicles (with Korea University)

## Lab infrastructure

Beyond research, the lab runs its own self-hosted infrastructure. Students who join the lab get an `@snsec.net` account and sign in once at **[auth.snsec.net](https://auth.snsec.net)** to reach every service below through single sign-on.

<div class="row">
  <div class="col-md-6 mt-3">
    <div class="card h-100 hoverable">
      <div class="card-body">
        <h5 class="card-title">Self-hosted services</h5>
        <ul class="card-text mb-0">
          <li><strong>Gitea</strong> &mdash; private Git hosting for code and experiments</li>
          <li><strong>Overleaf</strong> &mdash; collaborative LaTeX for papers</li>
          <li><strong>Grafana</strong> &mdash; live GPU-cluster dashboards and metrics</li>
          <li><strong>Tailscale</strong> &mdash; encrypted mesh VPN into the lab network</li>
          <li><strong>Gatus</strong> &mdash; service health and uptime monitoring</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="col-md-6 mt-3">
    <div class="card h-100 hoverable">
      <div class="card-body">
        <h5 class="card-title">Google Workspace <span style="font-weight:400; opacity:0.7;">(snsec.net)</span></h5>
        <ul class="card-text mb-0">
          <li><strong>Gmail</strong> &mdash; lab email on the snsec.net domain</li>
          <li><strong>Drive</strong> &mdash; shared storage and documents</li>
          <li><strong>Calendar</strong> &mdash; lab schedule and meetings</li>
          <li><strong>Sites</strong> &mdash; internal lab pages</li>
          <li><strong>Gemini</strong> &mdash; AI assistant</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="text-center mt-4">
  <a href="https://auth.snsec.net" target="_blank" rel="noopener" role="button"
     style="display:inline-block; padding:0.5rem 1.4rem; border-radius:0.3rem; font-weight:600; color:#fff; background-color:var(--global-theme-color); text-decoration:none;">
    Open the lab portal &nbsp;&rarr;
  </a>
</div>
