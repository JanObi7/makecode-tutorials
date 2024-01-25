# compass

## Einleitung

Dieser elektronische Kompass zeigt dir genau wo Norden ist.

## Programm

Hier das vollständige Programm

```blocks
basic.forever(function () {
    if (input.compassHeading() > 22.5 && input.compassHeading() <= 67.5) {
        basic.showArrow(ArrowNames.NorthWest)
    } else if (input.compassHeading() > 67.5 && input.compassHeading() <= 112.5) {
        basic.showArrow(ArrowNames.West)
    } else if (input.compassHeading() > 112.5 && input.compassHeading() <= 157.5) {
        basic.showArrow(ArrowNames.SouthWest)
    } else if (input.compassHeading() > 157.5 && input.compassHeading() <= 202.5) {
        basic.showArrow(ArrowNames.South)
    } else if (input.compassHeading() > 202.5 && input.compassHeading() <= 247.5) {
        basic.showArrow(ArrowNames.SouthEast)
    } else if (input.compassHeading() > 247.5 && input.compassHeading() <= 292.5) {
        basic.showArrow(ArrowNames.East)
    } else if (input.compassHeading() > 292.5 && input.compassHeading() <= 337.5) {
        basic.showArrow(ArrowNames.NorthEast)
    } else {
        basic.showArrow(ArrowNames.North)
    }
})
```

## Geschafft!

Herzlichen Glückwunsch!

<script src="https://makecode.com/gh-pages-embed.js"></script>
<script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
