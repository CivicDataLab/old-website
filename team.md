---
layout: page
title: Team
---

<section class="content-section section-team" id="team">
  <div class="container text-center">
    <div class="content-section-heading">
      <h3 class="text-secondary mb-0">The people who make it happen!</h3>
      <h2 class="mb-5">The Team</h2>
    </div>
    <div class="row">
    {% for member in site.members %}
      <div class="col-md-4">
        <div class="card mb-4 box-shadow">
          <img class="card-img-top fluid-img" data-src="{{ member.photo }}" alt="{{ member.full_name }} Profile Pic" style="height: 225px; width: 100%; display: block;" src="{{ member.photo }}" data-holder-rendered="true">
          <div class="card-body">
            <p class="card-name">
              {{ member.full_name }}
            </p>
            <p class="card-text">{{ member.content | markdownify }}</p>
            <div class="social-icons text-center">
              <a href="{{ member.github }}" target="_blank" class="fa fa-github"></a>
              <a href="{{ member.twitter }}" target="_blank" class="fa fa-twitter"></a>
              <a href="{{ member.linkedin }}" target="_blank" class="fa fa-linkedin"></a>
            </div>
          </div>
        </div>
      </div>
    {% endfor %}
    </div>
  </div>
</section>