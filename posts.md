---
layout: page
title: posts | tomsterbg
---

<section>
    {% assign posts = site.posts | where_exp:"item", "item.hidden != true" | sort: "date" }}
    {% if posts.size > 0 %}

    {% capture currentyear %}{{ 'now' | date: "%Y" }}{% endcapture %}
    {% capture postyear %}{{ posts[0].date | date: '%Y' }}{% endcapture %}
    {% if currentyear == postyear %}
        <h3>This year's posts</h3>
    {% else %}
        <h3>{{ postyear }}</h3>
    {% endif %}

    {% for post in posts %}
        {% unless post.next %}
            <ul>
        {% else %}
            {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
            {% capture nyear %}{{ post.next.date | date: '%Y' }}{% endcapture %}
            {% if year != nyear %}
                </ul>
                <h3>{{ post.date | date: '%Y' }}</h3>
                <ul>
            {% endif %}
        {% endunless %}
        <li><time>{{ post.date | date:"%d %b" }} - </time>
            <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
                {{ post.title }}
            </a>
        </li>
    {% endfor %}
    </ul>

    {% endif %}
</section>
