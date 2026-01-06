---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
layout: default
title: Home
---
<section class="blog-list">
	<h2 style="text-align:center; margin-bottom:2rem;">Latest Blog Posts</h2>
	<ul style="list-style:none; padding:0; max-width:700px; margin:0 auto;">
		{% for post in site.posts %}
			<li style="margin-bottom:2rem; border-bottom:1px solid #eee; padding-bottom:1rem;">
				<a href="{{ post.url }}" style="font-size:1.5rem; color:#007acc; text-decoration:none;">{{ post.title }}</a>
				<div style="color:#888; font-size:0.95rem; margin:0.5rem 0;">{{ post.date | date: "%B %d, %Y" }}</div>
				<p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
			</li>
		{% endfor %}
	</ul>
</section>
