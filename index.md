---
layout: default
title: Home
nav_order: 1
has_children: true
---

# ADML Schema
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Schema Documentation

### Overview

  * [ADML overview](adml_schema/ADML Schema Overview.html)


### Objects

  * [Objects overview](adml_schema/Objects.html)

### Bridges


## JSON Files

```html
<ul class="post-list">
    <h2>Schema Documentation</h2>
    <h3>Overview</h3>
    {% for thing in site.adml_schema %}
        {% if thing.category == "overview" %}
            <li>
                <p><a href="{{ thing.url }}">{{ thing.title }}</a></p>
            </li>
        {% endif %}
    {% endfor %}
    <h3>Objects</h3>
    {% for thing in site.adml_schema %}
        {% if thing.category == "object" %}
            <li>
                <p><a href="{{ thing.url }}">{{ thing.title }}</a></p>
            </li>
        {% endif %}
    {% endfor %}
    <h3>Bridges</h3>
    {% for thing in site.adml_schema %}
        {% if thing.category == "bridge" %}
            <li>
                <p><a href="{{ thing.url }}">{{ thing.title }}</a></p>
            </li>
        {% endif %}
    {% endfor %}
    <h2>JSON Files</h2>
    <p><a href=" link _adml_schema/ADML.json ">ADML JSON Schema</a></p>
    <p><a href=" link _adml_schema/SampleADMLModel.json ">Sample ADML model</a></p>
</ul>
```
