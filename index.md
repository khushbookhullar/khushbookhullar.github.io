---
layout: default
title: Home
---

<div id="main-content" class="main-section">
  <h2>About Me</h2>
  <p>Hi, I'm [Your Name], a [Your Profession] passionate about [Your Interests]. Welcome to my personal website, where I showcase my work and share my thoughts through my blog.</p>
  
  <div class="spacer"></div>

  <h2>Blog</h2>
  <div class="blog-posts">
    {% for post in site.posts limit: 3 %}
      <div class="post-preview">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt }}</p>
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
      </div>
    {% endfor %}
  </div>
  <a href="/blog" class="btn">View All Posts</a>

  <div class="spacer"></div>

  <h2>Contact</h2>
  <p>Feel free to <a href="mailto:khushbookhullar@gmail.com">email me</a> or connect on <a href="https://linkedin.com/in/yourprofile">LinkedIn</a>.</p>
</div>