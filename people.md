---
layout: post
title: People
permalink: /people/
---

## People

A list of people who work on free / open source software, either as designers or programmers and are a part of our community.

<ul>
  {% for person in site.people %}
    {% if person.status == "core" or person.status == "active" %}
      <li>
        <a href="#{{person.slug}}">
            {{ person.name }}
            {% if person.status == "core" %}
            <i class="fa fa-star" aria-hidden="true"></i>
            {% endif %}
        </a>
    </li>
    {% endif %}
  {% endfor %}
</ul>

## Add Yourself

Want to add yourself to this list? 

<a href="/people-form/" class="btn btn-primary">Add Yourself</a>

Or if you prefer technical approach, do the following:

* Sign in / up to Github
* Fork this repository
* Copy `person-template.md` into the `people` folder, so you have `people/your-name.md`
* Send a pull request
* Voila!
