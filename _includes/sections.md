

{% assign sorted_pages = site.sections | sort:"order_no" %}

{% for section in sorted_pages | sort:order_no %}	
    <section id="{{ section.about }}"class="main-content text-center">
      <h2>{{ section.title }}</h2> 
      <p>{{ section.output  }}</p>
    </section>
{% endfor %}

