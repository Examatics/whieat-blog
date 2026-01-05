
---
layout: default
title: Home
---


<div class="homepage-intro">
	<h1>Welcome to WHIEAT Blog</h1>
	<p>Your source for insightful articles on technology, productivity, and inspiration. We share tutorials, tips, and stories to help you stay informed and motivated.</p>
</div>

<div class="homepage-content">
	<h2>Latest Blog Posts</h2>
	<ul class="post-list">
		{% for post in site.posts %}
			<li>
				<a href="{{ post.url }}">{{ post.title }}</a>
				<span class="post-date">{{ post.date | date: "%b %d, %Y" }}</span>
			</li>
		{% endfor %}
	</ul>
</div>
