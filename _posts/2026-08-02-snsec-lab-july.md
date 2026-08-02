---
layout: post
title: "SNSec Lab in July: Two Weeks on Binaries, and a Summer Dinner"
date: 2026-08-02 21:00:00+09:00
description: A July of special sessions on binary analysis, lunches and desserts in between, and a lab dinner with all six of us.
tags: seminar
images:
  - /assets/img/2026-08-02-snsec-lab-july/lab-dinner-table.jpg
  - /assets/img/2026-08-02-snsec-lab-july/dinner-appetizer.jpg
  - /assets/img/2026-08-02-snsec-lab-july/dinner-main.jpg
  - /assets/img/2026-08-02-snsec-lab-july/dinner-dessert.jpg
---

July at SNSec Lab was two things: a long stretch of special sessions on binary analysis, and a dinner where all six of us finally sat at the same table.

<!--more-->

### Special sessions on binary analysis

From July 8 to July 17 we ran special sessions in the lab, every day from 10:30 to 16:00. The idea was to spend an uninterrupted block of the summer on something our group had only touched in passing — how compiled programs actually look from the outside, and what it takes to read one.

<div class="text-center mt-3 mb-3">
  <img src="/assets/img/2026-08-02-snsec-lab-july/session-ida-disassembly.jpg" alt="Walking through a disassembly listing during a special session" data-zoomable style="max-width:100%; border-radius:8px; box-shadow:0 1px 5px rgba(0,0,0,.25);">
  <div class="mt-1" style="font-size:0.9em; opacity:0.75;">Reading a disassembly listing together in IDA/x64dbg (July 15).</div>
</div>

We started from static analysis and basic reverse engineering, then worked through the things you cannot skip once you open a real executable: calling conventions, the PE file format, and the layout of headers, sections, and the import and export tables. From there we moved to dynamic linking — how a DLL is built, how it is linked, how imports get resolved at load time, and what DLL injection looks like when someone abuses that machinery. We closed with memory protection and call hijacking.

Rather than only reading about the PE format, we wrote a small PE parser in C++ from scratch and checked its output against PEview, so the structure fields stopped being a diagram on a slide and became bytes at an offset. We also spent time on classic crackme binaries, which are a fast way to build the habit of following control flow you did not write.

<div class="text-center mt-3 mb-3">
  <img src="/assets/img/2026-08-02-snsec-lab-july/session-pe-parser-code.jpg" alt="Going through the PE parser source code on the projector" data-zoomable style="max-width:100%; border-radius:8px; box-shadow:0 1px 5px rgba(0,0,0,.25);">
  <div class="mt-1" style="font-size:0.9em; opacity:0.75;">Going through the PE parser source line by line (July 13).</div>
</div>

What the sessions really set up is what we have been doing since they ended. Our group works on data-driven security, so the question waiting on the other side of two weeks of manual disassembly was what happens when a neural network is pointed at a binary. We are working through how the field has approached that so far — Asm2Vec (IEEE S&P 2019), jTrans (ISSTA 2022), Trex, and CodeArt (FSE 2024) — alongside HermesSim (USENIX Security 2024), whose "code is not natural language" framing is a useful provocation, and two papers from the learning side, Neural Networks and the Chomsky Hierarchy (ICLR 2023) and Stack Attention (ICLR 2024). Coming to these papers straight from the disassembler changes how they land. Once you have spent a morning tracing arguments through registers and the stack across a function boundary, a model that treats the same instructions as a flat sequence of tokens starts to feel like it is leaving something on the table. That is roughly where our reading is pointed now.

<div class="text-center mt-3 mb-3">
  <img src="/assets/img/2026-08-02-snsec-lab-july/session-paper-reading.jpg" alt="Reading a binary code analysis paper at a lab desk" data-zoomable style="max-width:100%; border-radius:8px; box-shadow:0 1px 5px rgba(0,0,0,.25);">
  <div class="mt-1" style="font-size:0.9em; opacity:0.75;">Paper reading after the day's session (July 14).</div>
</div>

Five and a half hours a day for two weeks is a lot of assembly, and the breaks mattered as much as the sessions. We walked out for lunch together every day, came back with coffee, and there was almost always dessert involved.

<div class="row mt-3 mb-3">
  <div class="col-sm-6 mt-2">
    <img src="/assets/img/2026-08-02-snsec-lab-july/lunch-stairs.jpg" alt="Heading out of the building for lunch" data-zoomable style="width:100%; border-radius:8px;">
  </div>
  <div class="col-sm-6 mt-2">
    <img src="/assets/img/2026-08-02-snsec-lab-july/lunch-campus-walk.jpg" alt="Walking back across campus after lunch" data-zoomable style="width:100%; border-radius:8px;">
  </div>
</div>

<div class="text-center mt-3 mb-3">
  <img src="/assets/img/2026-08-02-snsec-lab-july/session-dessert.jpg" alt="Dessert cups on the table during a break" data-zoomable style="max-width:100%; border-radius:8px; box-shadow:0 1px 5px rgba(0,0,0,.25);">
  <div class="mt-1" style="font-size:0.9em; opacity:0.75;">The afternoon break, reliably (July 15).</div>
</div>

Somewhere in the middle of all this, Chaeri and Hyekyo got their new monitors.

<div class="text-center mt-3 mb-3">
  <img src="/assets/img/2026-08-02-snsec-lab-july/new-monitors.jpg" alt="New monitors installed at lab desks" data-zoomable style="max-width:100%; border-radius:8px; box-shadow:0 1px 5px rgba(0,0,0,.25);">
  <div class="mt-1" style="font-size:0.9em; opacity:0.75;">New monitors at Chaeri's and Hyekyo's desks (July 17).</div>
</div>

### A dinner with all six of us

On July 30 we closed out the month with a lab dinner. This was the first time the whole lab was in one place since Hyekyo joined us in July, so all six of us — Chaeri, Chaeyoung, Jisoo, Hyekyo, Semin, and me — were finally at the same table, with the city and Namsan behind the window.

<div class="text-center mt-3 mb-3">
  <img src="/assets/img/2026-08-02-snsec-lab-july/lab-dinner-group.jpg" alt="SNSec Lab members at the July dinner" data-zoomable style="max-width:100%; border-radius:8px; box-shadow:0 1px 5px rgba(0,0,0,.25);">
  <div class="mt-1" style="font-size:0.9em; opacity:0.75;">The whole lab, July 30.</div>
</div>

Over dinner Chaeyoung shared her own news: she is graduating this August. Congratulations, Chaeyoung.

It has been a full first half of the year — a conference trip to Charlotte, a first journal submission, papers accepted, a new member, and two weeks of assembly. Everyone earned the break. Stay cool this summer, and see you all back in the lab rested.

<div class="card-columns">
    {% for img in page.images %}
    <div class="card">
        <img class="card-img-top" src="{{ img }}" data-zoomable />
    </div>
    {% endfor %}
</div>
