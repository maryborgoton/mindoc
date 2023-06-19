---
layout: default
title: Introduction
number: 002
---
# Introduction

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce eget condimentum ligula. Vivamus ultricies massa ac arcu ornare, sit amet pellentesque dolor consequat. Aliquam pellentesque ante nunc, ut sollicitudin arcu dapibus mattis. Nullam fermentum condimentum mi, et maximus nisl elementum a. Aenean ac tellus justo. Vivamus iaculis facilisis nunc, ac bibendum enim. Nullam eu convallis lacus. Fusce nulla ex, bibendum nec convallis et, rutrum in ipsum. Phasellus in elementum dolor. Fusce id iaculis dui, a lacinia nunc. In rhoncus fringilla nisi.

{% assign intro_images = site.mindoc_images | sort:"order" | where_exp: "item", "item.page == 'introduction' and item.order == '01'" %}
{% include image.html pages=intro_images %}
