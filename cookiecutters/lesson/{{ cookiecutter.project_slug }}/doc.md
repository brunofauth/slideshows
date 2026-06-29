---
{% raw -%}
# vim: foldmethod=marker foldlevel=1


# PANDOC STANDARD VARIABLES {{{
{%- endraw %}

lang: pt-BR

title: "{{ cookiecutter.lesson_title }}"
{% if cookiecutter.lesson_subtitle | length != 0 -%}
subtitle: "{{ cookiecutter.lesson_subtitle }}"
{%- endif %}

{% if cookiecutter.full_name | length != 0 -%}
author: "{{ cookiecutter.full_name  }}"
{%- endif %}

{% if cookiecutter.lesson_presentation_date | length != 0 -%}
date: "{{ cookiecutter.lesson_presentation_date }}"
{%- endif %}

incremental: true
slide-level: 2

{% raw -%}
# }}} PANDOC STANDARD VARIABLES


# REVEALJS-SPECIFIC VARIABLES {{{

# revealjs-url: "https://unpkg.com/reveal.js@5.2.1"
revealjs-url: ../../reveal.js

# All [reveal.js](https://revealjs.com/config/) configuration options can be
# set through variables. For example, themes can be used by setting the theme
# variable: 'theme: moon'

# Changes the behavior of our navigation directions.
#
# "default"
# Left/right arrow keys step between horizontal slides, up/down
# arrow keys step between vertical slides. Space key steps through
# all slides (both horizontal and vertical).
#
# "linear"
# Removes the up/down arrows. Left/right arrows step through all
# slides (both horizontal and vertical).
#
# "grid"
# When this is enabled, stepping left/right from a vertical stack
# to an adjacent vertical stack will land you at the same vertical
# index.
#
# Consider a deck with six slides ordered in two vertical stacks:
# 1.1    2.1
# 1.2    2.2
# 1.3    2.3
#
# If you're on slide 1.3 and navigate right, you will normally move
# from 1.3 -> 2.1. If "grid" is used, the same navigation takes you
# from 1.3 -> 2.3.
navigationMode: 'linear'

width: 1280
height: 1024
{%- endraw %}

theme: '{{ cookiecutter.theme }}'

{% raw -%}
# }}} REVEALJS VARIABLES
{%- endraw %}
...


{% raw -%}
# Introdução
{%- endraw %}
