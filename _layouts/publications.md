---
# Mr. Green Jekyll Theme (https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme)
# Copyright (c) 2022 Mr. Green's Workshop https://www.MrGreensWorkshop.com
# Licensed under MIT

layout: default
# Generic static content page
---
{%- include multi_lng/get-lng-by-url.liquid -%}
{%- assign lng = get_lng -%}
<div class="multipurpose-container">
  <h1>{{ page.title | default: site.data.lang[lng][page.layout].title }}</h1>
  <div class="markdown-style">
    {{ content }}
  </div>
</div>
