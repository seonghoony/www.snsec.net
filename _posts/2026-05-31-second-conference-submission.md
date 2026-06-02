---
layout: post
title: Second submission with Chaeri and Chaeyoung

images:
  - /assets/img/2026-05-31-second-conference-submission/1.jpeg
  - /assets/img/2026-05-31-second-conference-submission/2.jpeg
  - /assets/img/2026-05-31-second-conference-submission/3.jpeg
  - /assets/img/2026-05-31-second-conference-submission/4.jpeg
  - /assets/img/2026-05-31-second-conference-submission/5.jpeg
  - /assets/img/2026-05-31-second-conference-submission/6.jpeg
  - /assets/img/2026-05-31-second-conference-submission/7.jpeg

---
Chaeri, Chaeyoung, and I submitted our second paper, this time on cleansing data contamination in a cybersecurity dataset. Hope it went through well — again.

<!--more-->

<div id="carouselExampleControls" class="carousel slide mb-4" data-ride="carousel">
    <div class="carousel-inner">
        {% for img in page.images %}
            <div class="carousel-item {% if forloop.first %}active{% endif %}">
                <img src="{{ img }}" class="d-block w-100" alt="">
            </div>
        {% endfor %}
    </div>
    <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
    </a>
</div>
