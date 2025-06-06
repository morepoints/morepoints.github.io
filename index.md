---
layout: default
title: Home
---

# 🧠 My Hacking Blog

Welcome to my blog on cybersecurity, red teaming, and ethical hacking. Here you'll find writeups, tool reviews, and insights from real-world assessments and CTFs.

<h2>🔍 Search Posts</h2>
<input type="text" id="search-input" placeholder="Search posts...">
<ul id="results-container"></ul>

<script src="https://cdn.jsdelivr.net/npm/simple-jekyll-search@1.10.0/dest/simple-jekyll-search.min.js"></script>
<script>
  SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    json: '/search.json',
    searchResultTemplate: '<li><a href="{url}">{title}</a></li>',
    noResultsText: 'No results found',
    limit: 10,
    fuzzy: false,
  });
</script>

## 📌 Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

---

## ⚠️ Disclaimer

This blog is for **educational purposes only**. I do not condone unauthorized access or illegal hacking activities.
