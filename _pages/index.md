---
layout: page
title: Home
id: home
permalink: /
---

# Welcome yoooooooo! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Your first note]]</span> to get started on your exploration.
</p>

You've managed to find your way into my working notes, which I've accumulated over the course of several years. This database is part of my endeavor to arrange my own notions and ideas in a more public place where I can link notes on various topics together. These are in a constant state of flux. I also post/experiment with visual stuff [on my YouTube channel](https://www.youtube.com/c/RobertBlanc), ideas and theories that interest me. I use it to alleviate boredom and occasionally heighten my thought processes.

Content curation (craftdocs://open?blockId=7EFFB30B-9FBC-4F30-A8FB-0FDD56B39891&spaceId=ff2ca708-4452-8a9a-189d-1d1237b86794) is crucial in a society where knowledge is abundant. A form of artistic expression. Curating is all about spotting the hidden gems and putting your skills and enthusiasm to work highlighting the bits that matter to you.


If you want to hear about what I'm building, writing, and thinking about each week, then my Newsletter ➜ [here](https://linkincubator.substack.com/) 🫀


<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
