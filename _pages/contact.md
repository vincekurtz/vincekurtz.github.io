---
layout: page
title: Contact
permalink: /contact/
nav: true
nav_order: 4
horizontal: false
social: true
---

Email is the most reliable way to get in touch: `vjkurtz at gmail dot com`.

<!-- Social -->
{%- if page.social %}
  <div class="social">
    <div class="contact-icons">
      {% include social.html %}
    </div>

    <div class="contact-note">
      {{ site.contact_note }}
    </div>

  </div>
{%- endif %}

