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

  .fun-carousel {
    min-width: 0;
  }

  .fun-carousel-viewport {
    position: relative;
    overflow: hidden;
    cursor: grab;
    touch-action: pan-y;
  }

  .fun-carousel-viewport:active {
    cursor: grabbing;
  }

  .fun-carousel-track {
    display: flex;
    transition: transform 0.35s ease;
  }

  .fun-carousel-slide {
    box-sizing: border-box;
    display: flex;
    flex: 0 0 100%;
    align-items: center;
    justify-content: center;
    min-width: 0;
    margin: 0;
    padding: 0;
  }

  .fun-carousel-control {
    position: absolute;
    top: 50%;
    z-index: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 2.25rem;
    height: 2.25rem;
    padding: 0;
    border: 0;
    border-radius: 50%;
    background: rgba(0, 0, 0, 0.48);
    color: #fff;
    cursor: pointer;
    font-size: 1.7rem;
    line-height: 1;
    transform: translateY(-50%);
  }

  .fun-carousel-control:hover,
  .fun-carousel-control:focus {
    background: rgba(0, 0, 0, 0.7);
  }

  .fun-carousel-prev {
    left: 0.65rem;
  }

  .fun-carousel-next {
    right: 0.65rem;
  }

  .fun-carousel-meta {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.8rem;
    margin-top: 0.85rem;
  }

  .fun-carousel-dots {
    display: flex;
    gap: 0.35rem;
  }

  .fun-carousel-dot {
    width: 0.55rem;
    height: 0.55rem;
    padding: 0;
    border: 0;
    border-radius: 50%;
    background: var(--global-divider-color);
    cursor: pointer;
  }

  .fun-carousel-dot[aria-current="true"] {
    background: var(--global-theme-color);
  }

  .fun-carousel-counter {
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 0.9rem;
  }

  @media (prefers-reduced-motion: reduce) {
    .fun-carousel-track {
      transition: none;
    }
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
        <figure class="fun-honor-item fun-carousel" data-fun-carousel>
          <div class="fun-carousel-viewport" tabindex="0" aria-label="Article published in Journey Ahead magazine">
            <div class="fun-carousel-track">
              {% assign travel_images = "1.jpg|2.jpg|3.jpg|4.jpg" | split: "|" %}
              {% for image in travel_images %}
              <div class="fun-carousel-slide">
                <img src="{{ '/assets/img/fun-stuff/travel-magazine/' | append: image | relative_url }}" alt="Journey Ahead magazine article, image {{ forloop.index }}" draggable="false">
              </div>
              {% endfor %}
            </div>
            <button class="fun-carousel-control fun-carousel-prev" type="button" data-carousel-prev aria-label="Previous travel magazine image">&#8249;</button>
            <button class="fun-carousel-control fun-carousel-next" type="button" data-carousel-next aria-label="Next travel magazine image">&#8250;</button>
          </div>

          <div class="fun-carousel-meta">
            <div class="fun-carousel-dots" role="group" aria-label="Journey Ahead magazine images">
              <button class="fun-carousel-dot" type="button" data-carousel-dot="0" aria-label="Show image 1" aria-current="true"></button>
              <button class="fun-carousel-dot" type="button" data-carousel-dot="1" aria-label="Show image 2" aria-current="false"></button>
              <button class="fun-carousel-dot" type="button" data-carousel-dot="2" aria-label="Show image 3" aria-current="false"></button>
              <button class="fun-carousel-dot" type="button" data-carousel-dot="3" aria-label="Show image 4" aria-current="false"></button>
            </div>
            <p class="fun-carousel-counter" aria-live="polite">Image 1 of 4</p>
          </div>
          <figcaption>Article Published in <em>Journey Ahead</em></figcaption>
        </figure>
        <figure class="fun-honor-item">
          <img src="{{ '/assets/img/fun-stuff/alipay-populus-euphratica.jpg' | relative_url }}" alt="Ant Forest 10th anniversary certificate for planting a Populus euphratica tree">
          <figcaption>Ant Forest Populus Euphratica Certificate</figcaption>
        </figure>
      </div>
    </section>
  </div>
</div>

<script>
  document.addEventListener('DOMContentLoaded', function () {
    document.querySelectorAll('[data-fun-carousel]').forEach(function (carousel) {
      var viewport = carousel.querySelector('.fun-carousel-viewport');
      var track = carousel.querySelector('.fun-carousel-track');
      var slides = carousel.querySelectorAll('.fun-carousel-slide');
      var dots = carousel.querySelectorAll('.fun-carousel-dot');
      var counter = carousel.querySelector('.fun-carousel-counter');
      var index = 0;
      var startX = null;

      function render(nextIndex) {
        index = (nextIndex + slides.length) % slides.length;
        track.style.transform = 'translateX(-' + (index * 100) + '%)';
        dots.forEach(function (dot, dotIndex) {
          dot.setAttribute('aria-current', dotIndex === index ? 'true' : 'false');
        });
        counter.textContent = 'Image ' + (index + 1) + ' of ' + slides.length;
      }

      carousel.querySelector('[data-carousel-prev]').addEventListener('click', function () {
        render(index - 1);
      });

      carousel.querySelector('[data-carousel-next]').addEventListener('click', function () {
        render(index + 1);
      });

      dots.forEach(function (dot) {
        dot.addEventListener('click', function () {
          render(Number(dot.getAttribute('data-carousel-dot')));
        });
      });

      viewport.addEventListener('pointerdown', function (event) {
        if (event.target.closest('button') || !event.isPrimary || event.button !== 0) {
          return;
        }
        startX = event.clientX;
        viewport.setPointerCapture(event.pointerId);
      });

      viewport.addEventListener('pointerup', function (event) {
        if (startX === null) {
          return;
        }
        var distance = event.clientX - startX;
        startX = null;
        if (Math.abs(distance) > 40) {
          render(index + (distance < 0 ? 1 : -1));
        }
      });

      viewport.addEventListener('pointercancel', function () {
        startX = null;
      });

      viewport.addEventListener('keydown', function (event) {
        if (event.key === 'ArrowLeft') {
          event.preventDefault();
          render(index - 1);
        } else if (event.key === 'ArrowRight') {
          event.preventDefault();
          render(index + 1);
        }
      });
    });
  });
</script>
