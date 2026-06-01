---
layout: page
permalink: /dashboard/
title: dashboard
description: Schedule and activity overview
nav: true
nav_order: 8
---

<div class="text-center mt-3 mb-4">
  <a href="https://auth.snsec.net" target="_blank" rel="noopener" role="button"
     style="display:inline-block; padding:0.55rem 1.5rem; border-radius:0.3rem; font-weight:600; color:#fff; background-color:var(--global-theme-color); text-decoration:none;">
    🔐&nbsp; Lab members &mdash; sign in at auth.snsec.net &nbsp;&rarr;
  </a>
  <div style="font-size:0.8rem; margin-top:0.4rem; opacity:0.75;">
    Single sign-on to the lab's self-hosted services &amp; Google&nbsp;Workspace
  </div>
</div>

## Lab infrastructure

Lab members sign in once with their **snsec.net Google account** at **[auth.snsec.net](https://auth.snsec.net)** to reach every service below through single sign-on.

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

## PythonJudgeSystem
The source code for the custom python judge system is available on [GitHub](https://github.com/seonghoony/2026-PythonJudgeSystem-ICP).

**[프로그래밍입문-001]({{ '/dashboard/icp-spring26/001' | relative_url }})**
<iframe src="{{ '/dashboard/icp-spring26/001' | relative_url }}" style="border:solid 1px #777; width: 100%; max-width: 800px;" height="425" frameborder="0"></iframe>
<br>

**[프로그래밍입문-003]({{ '/dashboard/icp-spring26/003' | relative_url }})**
<iframe src="{{ '/dashboard/icp-spring26/003' | relative_url }}" style="border:solid 1px #777; width: 100%; max-width: 800px;" height="425" frameborder="0"></iframe>
<br>

## GPU Infrastructure

Hosts `*.infra.snsec.net` are accessible within the SNSec Lab intranet.
<iframe src="https://grafana.snsec.net/public-dashboards/ebbfe189bc7b44f78f052f7a309cbb44" width="800" height="600" frameborder="0"></iframe>
<br>

## Schedule
<iframe src="https://calendar.google.com/calendar/embed?height=600&wkst=1&ctz=Asia%2FSeoul&bgcolor=%23ffffff&title=Schedule&showTitle=0&showPrint=0&mode=WEEK&showCalendars=0&hl=en&src=c2Vvbmdob29uQHNoamVvbmcubmV0&src=a28uc291dGhfa29yZWEjaG9saWRheUBncm91cC52LmNhbGVuZGFyLmdvb2dsZS5jb20&color=%230e61b9&color=%237CB342" style="border:solid 1px #777; width: 100%; max-width: 800px;" height="600" frameborder="0" scrolling="no"></iframe>
<br>

## GitHub Activity

<img id="gh-chart-seonghoony" alt="GitHub Contributions" style="width: 100%; max-width: 800px;" />
<script>document.getElementById('gh-chart-seonghoony').src = 'https://ghchart.rshah.org/003087/seonghoony?' + Date.now();</script>
