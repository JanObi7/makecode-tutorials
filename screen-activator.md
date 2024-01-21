# Bildschirm aktivieren

## Einleitung

Unser micro:bit soll seinen Bildschirm aktivieren, wenn wir ihn in die Hand nehmen.
Wenn er auf dem Tisch liegt, soll der Bildschirm ausgeschaltet werden.

## senkrechte Lage erkennen

Schaue auf der linken Seite in deine Wergzeuge unter **Eingabe**.
Ziehe jetzt den Block **wenn geschüttelt** in dein Programm.
Wähle in dem Block anstatt **geschüttelt** den Wert **Logo nach oben** aus.

```blocks
input.onGesture(Gesture.LogoUp, function () {
})
```

## Bilschirm einschalten

Wenn der micro:bit senkrecht steht wird alles im Block **wenn Logo nach oben** einmal ausgeführt.

Ziehe jetzt aus Grundlagen den Block **zeige Symbol** in dein Programm und füge ihn in **wenn Logo nach oben** ein.
Wähle statt dem **Herz** das Symbol **Quadrat** zum Anzeigen aus.

```blocks
input.onGesture(Gesture.LogoUp, function () {
    basic.showIcon(IconNames.Square)
})
```

## Bilschirm ausschalten

Wenn der micro:bit flach auf dem Tisch liegt, soll der Bildschirm wieder ausgeschaltet werden.

Ziehe jetzt den Block **wenn geschüttelt** ein zweites Mal in dein Programm
und wähle in dem Block anstatt **geschüttelt** den Wert **Display nach oben** aus.
Ziehe in diesen Block aus den Grundlagen den Block **Bildschirm löschen**.

```blocks
input.onGesture(Gesture.ScreenUp, function () {
    basic.clearScreen()
})
```

## Geschafft!

Herzlichen Glückwunsch! Dein Programm ist fertig.

Probiere es gleich in deinem virtuellen micro:bit ganz links aus,
indem Du mit deiner Maus über den micro:bit fährst und ihn so in verschiedene Lagen bringst
(Mauszeiger in der Mitte = **Display nach oben**; Maus unten mittig = **Logo nach oben**).


```blocks
input.onGesture(Gesture.LogoUp, function () {
    basic.showIcon(IconNames.Heart)
})
input.onGesture(Gesture.ScreenUp, function () {
    basic.clearScreen()
})
```

<script src="https://makecode.com/gh-pages-embed.js"></script>
<script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
