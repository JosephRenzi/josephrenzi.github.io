---
layout: default
---

## Welcome to my Website!

Hello! I'm Joseph. This is my personal corner of the internet where I write about mathematics and code.

---

### Recent Articles

<!-- This "for loop" goes through every post in the _posts folder -->
<ul>
  {% for post in site.posts %}
    <li>
      <!-- This creates a clickable link to the post, and prints the date -->
      <span>{{ post.date | date: "%B %d, %Y" }}</span> &raquo; 
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
