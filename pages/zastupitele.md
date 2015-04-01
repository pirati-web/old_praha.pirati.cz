---
layout:    portal
unit:      praha
menu:      people
permalink: lide/zastupitele/
title:     Klub zastupitelů
sub:       za Piráty v zastupitelstvu hl. m. Prahy
image:     /media/lide/klub.jpg
---

Zastupitelstvo hl. m. Prahy je orgán volený všemi Pražany, který

* volí a odvolává primátora a další členy Rady hl. m. Prahy,
* schvaluje obecně závazné vyhlášky platné na území Prahy,
* projednává rozpočet a zásadní koncepce rozvoje města.

Zastupitelé
-----------------------------------

{% assign pages = site.people | where: "category", "zastupitel" | sort_by: "number" %}
{% include list.html %}

Tým
-----------------------------------
{% assign pages = site.people | where: "category", "tym" | sort_by: "number" %}
{% include list.html %}
