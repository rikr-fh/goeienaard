---
title: Contact
permalink: /contact/
label: Contact
kop: Benieuwd wat ik voor jouw tuin kan betekenen?
intro: Of je al precies weet wat je wilt, of alleen het gevoel hebt dat het anders kan, een kennismaking is de beste start. Laagdrempelig, gratis en je zit nergens aan vast.
kennismaken: false
---

<div id="kennismaking" class="gn-kennismaking" markdown="1">

## Kennismaking aanvragen

1. **{% if site.formspree and site.formspree != "" %}Je vult het formulier hieronder in.{% else %}Je stuurt me een berichtje of belt.{% endif %}** Een paar zinnen over je tuin is genoeg.
2. **Ik neem binnen een paar werkdagen contact met je op.**
3. **We maken kennis.** Aan de telefoon, of met een kort bezoek aan je tuin als je in de buurt woont. Dit eerste gesprek is gratis.
{: .gn-kennismaking__stappen}

{% if site.formspree and site.formspree != "" %}
{% include kennismaking-form.html %}
<p class="gn-form__alt">Liever direct contact? Mail naar <a href="mailto:{{ site.email }}">{{ site.email }}</a> of bel <a href="tel:{{ site.telefoon | remove: ' ' }}">{{ site.telefoon }}</a>.</p>
{% else %}
<div class="gn-acties">
  <a class="gn-knop" href="mailto:{{ site.email }}?subject=Kennismaking%20Studio%20Goeienaard&amp;body=Hoi%20Beau%2C%0A%0AIk%20wil%20graag%20kennismaken.%0A%0AWaar%20ligt%20mijn%20tuin%20%28plaats%29%3A%20%0AHoe%20groot%20is%20de%20tuin%20ongeveer%3A%20%0AWat%20ik%20zou%20willen%3A%20%0AWanneer%20ik%20graag%20wil%20beginnen%3A%20%0AJe%20kunt%20me%20bellen%20op%3A%20%0A%0AGroet%2C%0A">Mail {{ site.email }}</a>
  <a class="gn-knop gn-knop--licht" href="tel:{{ site.telefoon | remove: ' ' }}">Bel {{ site.telefoon }}</a>
</div>
{% endif %}

</div>

## Wat handig is om te vertellen

Je hoeft nog niet alles te weten, maar hiermee kan ik je sneller en beter helpen:

- **Waar je tuin ligt:** de plaats is genoeg.
- **Hoe groot je tuin ongeveer is:** een schatting is prima.
- **Wat je wensen zijn:** bijvoorbeeld meer bloemen en vogels, minder tegels, een plek in de zon of minder onderhoud.
- **Een paar foto's van je tuin zoals hij nu is:** gewoon met je telefoon.
- **Je planning:** wanneer zou je graag willen beginnen?

## Na de kennismaking

Klikt het, dan ontvang je een offerte op maat. Je beslist in alle rust of je verder wilt.

## Gegevens

**Studio Goeienaard**<br>
Tilburg<br>
<a href="mailto:{{ site.email }}">{{ site.email }}</a><br>
<a href="tel:{{ site.telefoon | remove: ' ' }}">{{ site.telefoon }}</a><br>
<a href="{{ site.instagram }}">Instagram: @studiogoeienaard</a>
