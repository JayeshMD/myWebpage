---
layout: page
permalink: /publications/
title: publications
description: creative work
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography --query @*[my_publication=true]%}

</div>
