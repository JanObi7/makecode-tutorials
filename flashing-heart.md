# Blinkendes Herz

## Einleitung

Unser micro:bit soll ein blinkendes Herz anzeigen.

## Herz anzeigen

Schaue auf der linken Seite in deine Wergzeuge unter **Grundlagen**.
Ziehe jetzt den Block **zeige Symbol** mit dem Herz in dein Programm und füge ihn in **dauerhaft** ein.

```blocks
basic.forever(function () {
    basic.showIcon(IconNames.Heart)
})
```

## Herz ausblenden

Damit unser Herz blinkt, müssen wir es wieder ausschalten.

Ziehe dazu den Block **Bilschirminhalt löschen** in dein Programm und füge ihn nach **zeige Symbol** ein.

```blocks
basic.forever(function () {
    basic.showIcon(IconNames.Heart)
    basic.clearScreen()
})
```

## Pausen einfügen

Für ein schönes, regelmäßiges Blinken brauchen wir noch ein paar Wartezeiten.

Ziehe dazu zweimal den Block **pausiere (ms)** in dein Programm
und füge diese jeweils hinter **zeige Symbol** und **Bildschirminhalt löschen** ein.
Stelle als Zeit **500 ms** ein.

```blocks
basic.forever(function () {
    basic.showIcon(IconNames.Heart)
    basic.pause(500)
    basic.clearScreen()
    basic.pause(500)
})
```

## Geschafft!

Herzlichen Glückwunsch! Dein Herz blinkt.

Du kannst Dein Programm noch etwas anpassen, indem Du ein anderes Symbol oder andere Pausenzeiten wählst.


<script src="https://makecode.com/gh-pages-embed.js"></script>
<script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
