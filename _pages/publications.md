---
layout: page
permalink: /publications/
title: Publications
description: selected publications organized by year
nav: false
nav_order: 2
_styles: |
  /* Venue badge: compact pill sized to its text, not the whole column.
     The theme ships .w-100 as an !important utility, and bib.liquid puts
     that class on the <abbr>, so this override has to be !important too. */
  .publications ol.bibliography li .abbr abbr {
    width: auto !important;
    padding: 0.2rem 0.6rem;
    font-size: 0.75rem;
    font-weight: 600;
    letter-spacing: 0.02em;
  }

  /* Keep the badge column narrow so the entry text gets the room. */
  .publications ol.bibliography li .col-sm-2 {
    flex: 0 0 auto;
    width: 8rem;
    max-width: 8rem;
  }

  .publications ol.bibliography li .col-sm-8 {
    flex: 1 1 auto;
    width: auto;
    max-width: none;
  }

  /* Clickable titles. */
  .publications ol.bibliography li .title a {
    color: var(--global-theme-color);
    text-decoration: none;
  }

  .publications ol.bibliography li .title a:hover {
    text-decoration: underline;
  }

  .publications ol.bibliography li .links a.btn {
    margin-right: 0.3rem;
    margin-top: 0.3rem;
  }

  .publications ol.bibliography li .links a.btn i {
    margin-right: 0.15rem;
  }

  @media (max-width: 576px) {
    .publications ol.bibliography li .col-sm-2 {
      width: 100%;
      max-width: 100%;
    }
  }
---

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>
