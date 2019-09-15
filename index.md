---
layout: default
title: Capstone Skynet
---

Welcome to the main website of UBC ECE Capstone 2019-2020 Team 109. Our project is **FPGA Object Recognition**.

## Index

<dl class="row dl-horizontal">
    {% for nav in site.data.navigation %}
    <dt class="col-md-2"><a href="{{ nav.url }}">{{ nav.text }}</a></dt>
    <dd class="col-md-10">{{ nav.desc }}</dd>
    {% endfor %}
</dl>