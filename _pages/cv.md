---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 3
description:
---

{% comment %}
  The CV lives at a fixed filename so a new version can be uploaded
  straight over the old one without editing this page.
{% endcomment %}
{% assign cv_file = "/assets/pdf/rulis_cv.pdf" | relative_url %}

<style>
  .cv-actions {
    display: flex;
    align-items: center;
    gap: 1rem;
    flex-wrap: wrap;
    margin-bottom: 1.5rem;
  }
  .cv-download {
    display: inline-block;
    padding: 0.5rem 1.1rem;
    border: 1px solid var(--global-theme-color);
    border-radius: 6px;
    color: var(--global-theme-color);
    text-decoration: none;
    font-weight: 500;
    transition: background 0.2s ease, color 0.2s ease;
  }
  .cv-download:hover {
    background: var(--global-theme-color);
    color: var(--global-bg-color);
    text-decoration: none;
  }
  .cv-viewer {
    width: 100%;
    height: 85vh;
    min-height: 500px;
    border: 1px solid var(--global-divider-color);
    border-radius: 6px;
  }
  /* Inline PDF viewers are unreliable on phones and tablets, which
     usually ignore the embed and show nothing. Hide it there and let
     the download button do the work. */
  @media (max-width: 768px) {
    .cv-viewer {
      display: none;
    }
  }
</style>

<div class="cv-actions">
  <a class="cv-download" href="{{ cv_file }}" download="rulis_cv.pdf">Download CV (PDF)</a>
  <a href="{{ cv_file }}" target="_blank" rel="noopener">Open in a new tab</a>
</div>

<object class="cv-viewer" data="{{ cv_file }}" type="application/pdf">
  <p>
    Your browser cannot display PDFs inline.
    <a href="{{ cv_file }}">Download the CV instead</a>.
  </p>
</object>
