---
layout: default
---

<!-- Si separas esto 
    <section>
	<header class="major">
		<h2>Erat lacinia</h2>
	</header>
	<div class="features">
		<article>
			<span class="icon fa-diamond"></span>
			<div class="content">
				<h3>Portitor ullamcorper</h3>
				<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			</div>
		</article>
		<article>
			<span class="icon fa-paper-plane"></span>
			<div class="content">
				<h3>Sapien veroeros</h3>
				<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			</div>
		</article>
		<article>
			<span class="icon fa-rocket"></span>
			<div class="content">
				<h3>Quam lorem ipsum</h3>
				<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			</div>
		</article>
		<article>
			<span class="icon fa-signal"></span>
			<div class="content">
				<h3>Sed magna finibus</h3>
				<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			</div>
		</article>
	</div>
</section>

de esto no se vera el material -->

<!-- Comentarios para borrar codigo -->
<section>
	<header class="major">
		<h2>Recientes</h2>
	</header>
	<div class="posts">
    {% for post in site.posts %}
		<article>
		    <a href="{{ post.url | prepend: site.baseurl }}" class="image"><img src="{{ site.baseurl }}/assets/images/{{ post.image }}" alt="" /></a>
	       <h3>{{ post.title }}</h3>
	       <p>{{ post.excerpt }}</p>
	        <ul class="actions">
				<li><a href="{{ post.url | prepend: site.baseurl }}" class="button">Más</a></li>
			</ul>
		</article>
    {% endfor %}
	</div>
</section>
