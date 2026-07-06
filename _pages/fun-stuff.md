---
layout: page
permalink: /fun-stuff/
title: Fun Stuff
description: A collection of side quests, jokes, and things that do not fit neatly into a formal CV.
nav: true
nav_order: 5
---

<style>
  .fun-tabs {
    margin-top: 1.5rem;
  }

  .fun-tabs input[type="radio"] {
    position: absolute;
    opacity: 0;
    pointer-events: none;
  }

  .fun-tab-labels {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem;
    border-bottom: 1px solid var(--global-divider-color);
    margin-bottom: 1.35rem;
  }

  .fun-tab-labels label {
    border: 1px solid var(--global-divider-color);
    border-bottom: 0;
    border-radius: 8px 8px 0 0;
    color: var(--global-text-color-light);
    cursor: pointer;
    font-size: 0.95rem;
    font-weight: 600;
    margin-bottom: -1px;
    padding: 0.55rem 0.9rem;
  }

  #fun-tab-paper:checked ~ .fun-tab-labels label[for="fun-tab-paper"],
  #fun-tab-honors:checked ~ .fun-tab-labels label[for="fun-tab-honors"] {
    background: var(--global-bg-color);
    border-color: var(--global-theme-color);
    color: var(--global-theme-color);
  }

  .fun-tab-panel {
    display: none;
  }

  #fun-tab-paper:checked ~ .fun-tab-panels #fun-panel-paper,
  #fun-tab-honors:checked ~ .fun-tab-panels #fun-panel-honors {
    display: block;
  }

  .fun-tab-note {
    color: var(--global-text-color-light);
    font-size: 0.98rem;
    margin-bottom: 1.2rem;
  }

  .fun-honor-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
    gap: 1rem;
    margin-top: 1.2rem;
  }

  .fun-honor-item {
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    background: var(--global-card-bg-color);
    padding: 0.8rem;
  }

  .fun-honor-item img {
    display: block;
    width: 100%;
    height: 230px;
    object-fit: contain;
  }

  .fun-honor-item figcaption {
    color: var(--global-text-color-light);
    font-size: 0.88rem;
    margin-top: 0.65rem;
    text-align: center;
  }

  @media (min-width: 768px) {
    .fun-honor-item img {
      height: 260px;
    }
  }
</style>

<div class="fun-tabs">
  <input type="radio" id="fun-tab-paper" name="fun-tabs" checked>
  <input type="radio" id="fun-tab-honors" name="fun-tabs">

  <div class="fun-tab-labels" role="tablist" aria-label="Fun Stuff sections">
    <label for="fun-tab-paper" role="tab">SHIT paper</label>
    <label for="fun-tab-honors" role="tab">Special Honors</label>
  </div>

  <div class="fun-tab-panels">
    <section class="fun-tab-panel" id="fun-panel-paper">
      <p class="fun-tab-note">A small corner for playful and unconventional academic artifacts.</p>

      <div class="publications">
        <h2 class="bibliography">SHIT paper</h2>
        <ol class="bibliography">
          <li>
            <div class="row">
              <div class="col col-sm-2 abbr">
                <abbr class="badge rounded w-100" style="background-color:#6c757d">
                  NOI
                </abbr>
              </div>
              <div id="won2026freewill" class="col-sm-8">
                <div class="title">
                  因果链条下的人生：并不存在的自由意志
                </div>
                <div class="author">
                  闻人若彼
                </div>
                <div class="periodical">
                  <em>Web of Nothing</em>, 2026
                </div>
                <div class="periodical">
                  10.N0/rp.202606.A.0303.0001
                </div>
                <div class="links">
                  <a
                    href="https://webofnothing.org/noi/10.N0/rp.202606.A.0303.0001"
                    class="btn btn-sm z-depth-0"
                    role="button"
                    rel="external nofollow noopener"
                    target="_blank"
                  >
                    URL
                  </a>
                </div>
              </div>
            </div>
          </li>
        </ol>
      </div>
    </section>

    <section class="fun-tab-panel" id="fun-panel-honors">
      <p class="fun-tab-note">
        There is a lot you have that I do not; there is also a little I have that you may not.
      </p>

      <div class="fun-honor-grid">
        <figure class="fun-honor-item">
          <img src="{{ '/assets/img/fun-stuff/security-guard-certificate.jpg' | relative_url }}" alt="Security guard certificate">
          <figcaption>Security Guard Certificate</figcaption>
        </figure>
        <figure class="fun-honor-item">
          <img src="{{ '/assets/img/fun-stuff/career-planner.jpg' | relative_url }}" alt="Career planner certificate">
          <figcaption>Career Planner Certificate</figcaption>
        </figure>
        <figure class="fun-honor-item">
          <img src="{{ '/assets/img/fun-stuff/psychological-counselor.jpg' | relative_url }}" alt="Psychological counselor certificate">
          <figcaption>Psychological Counselor</figcaption>
        </figure>
        <figure class="fun-honor-item">
          <img src="{{ '/assets/img/fun-stuff/social-etiquette-certificate.jpg' | relative_url }}" alt="Social etiquette certificate">
          <figcaption>Social Etiquette Certificate</figcaption>
        </figure>
        <figure class="fun-honor-item">
          <img src="{{ '/assets/img/fun-stuff/general-management.jpg' | relative_url }}" alt="General management certificate">
          <figcaption>General Management</figcaption>
        </figure>
        <figure class="fun-honor-item">
          <img src="{{ '/assets/img/fun-stuff/best-debater.jpg' | relative_url }}" alt="Best debater award">
          <figcaption>Best Debater</figcaption>
        </figure>
        <figure class="fun-honor-item">
          <img src="{{ '/assets/img/fun-stuff/english-club-persistence-award.jpg' | relative_url }}" alt="English club persistence award">
          <figcaption>English Club Persistence Award</figcaption>
        </figure>
      </div>
    </section>
  </div>
</div>
