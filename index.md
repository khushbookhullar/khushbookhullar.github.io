---
layout: default
title: Home
---

<div id="main-content" class="main-section">
  <h2>About Me</h2>
  <p>Hi,Welcome to my personal website, 
  
  I am [Dr. Khushboo Khullar](https://www.linkedin.com/in/dr-khushboo-khullar-38251b43), a Venture Partner at Lightning Ventures, where I lead partnerships and investor allocations, focusing on Bitcoin-native startups. I have spearheaded fundraising efforts, managed syndicate funds, and possess a strong understanding of both Bitcoin and traditional finance models. My leadership in the Bitcoin ecosystem extends to speaking at major conferences such as Nicehash 2024 in Slovenia and Adopting Bitcoin 2024 in El Salvador. Frequently quoted by Bloomberg on Bitcoin trends, I also co-organize BitDevs meetups in Singapore and host AMAs with industry leaders. 
  
  As the Co-founder of Rebit Labs, I work to transition traditional banks to the Bitcoin standard, and was selected in the top 1% for the NUS-GRIP Accelerator program. Passionate about Bitcoin and venture capital, I am committed to supporting hyperbitcoinization and fostering innovation in the space. 
  
  I showcase my work and share my thoughts through [my blog]().</p>
  
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
  <p>Feel free to <a href="mailto:khushbookhullar@gmail.com">email me</a> or connect on <a href="https://www.linkedin.com/in/dr-khushboo-khullar-38251b43">LinkedIn</a>.</p>
</div>