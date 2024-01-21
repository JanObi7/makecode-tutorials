# Lichtschalter

## Einleitung

Die LEDs deines micro:bit sollen mit dem Knopf **A** eingeschaltet und mit dem Knopf **B** ausgeschaltet werden.

## Knopf A abfragen

Schaue auf der linken Seite in deine Wergzeuge unter **Eingabe**.
Ziehe jetzt den Block **wenn Knopf A geklickt** in dein Programm.

```blocks
input.onButtonPressed(Button.A, function () {
})
```

## Licht einschalten

Alles was wir in **wenn Knopf A geklickt** einfügen, wird dann einmal ausgeführt.
Ziehe aus Grundlagen den Block **zeige LEDs** in dein Programm und füge ihn in **wenn Knopf A geklickt** ein.
Aktiviere in dem Block alle LEDs mit der Maus.

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showLeds(`
        # # # # #
        # # # # #
        # # # # #
        # # # # #
        # # # # #
        `)
})
```

## Licht ausschalten

Ziehe jetzt den Block **wenn Knopf A geklickt** ein zweites Mal in dein Programm.
Wähle jetzt in dem Block statt **A** den Knopf **B** aus.
Füge jetzt hier aus Grundlagen den Block **Bilschirminhalt löschen** ein.

```blocks
input.onButtonPressed(Button.B, function () {
    basic.clearScreen()
})
```

## Geschafft!

Herzlichen Glückwunsch! Dein Schalter ist fertig.

Probiere ihn gleich in deinem virtuellen micro:bit ganz links aus,
indem Du abwechselnd die Knöpfe **A** oder **B** mit der Maus anklickst.

<script src="https://makecode.com/gh-pages-embed.js"></script>
<script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
