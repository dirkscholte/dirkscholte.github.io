# PhD candidate in Astrophysics

I am a PhD candidate in Extragalactic Astrophysics at UCL. I am studying galaxy evolution through some of the largest optical spectroscopic surveys.

I am deriving gas mass estimates from spectroscopy using photoionization modelling and machine learning. Using weak lensing to derive dark matter halo masses.

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
