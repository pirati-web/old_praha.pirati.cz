---
layout:    portal
unit:      praha
permalink: /sdruzeni/
title:     Místní sdružení
image:     /media/lide/klub.jpg
---

Krajské sdružení Pirátů v Praze sestává z místních sdružení a skupin, které
se věnují místním kauzám.

Přehled místních sdružení
-----------------------------------

{% assign pages = site.pages | where: "superior", "praha" %}
{% include list.html %}
