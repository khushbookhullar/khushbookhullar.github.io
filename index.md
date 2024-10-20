---
layout: default
title: Home
---

<div id="about" class="section">
  <h2>About Me</h2>
  <p>Hi, I'm [Dr. Khushboo Khullar], a [Venture Capitalist]. I am a Bitcoiner, VC and Part Time Founder/Builder.</p>
  <a href="#contact" class="btn">Get in Touch</a>
</div>

<div id="blog" class="section">
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
</div>

<div id="contact" class="section">
  <h2>Contact</h2>
  <p>Feel free to <a href="mailto:khushbookhullar@gmail.com">email me</a> or connect on <a href="https://linkedin.com/in/yourprofile">LinkedIn</a>.</p>
</div>

[My GitHub Profile](https://github.com/khushbookhullar)