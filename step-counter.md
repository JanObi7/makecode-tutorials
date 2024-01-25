# step-counter

## Einleitung

Vollständiges Programm

```blocks
input.onButtonPressed(Button.AB, function () {
    steps = 0
})
input.onGesture(Gesture.ThreeG, function () {
    steps += 1
})
let steps = 0
steps = 0
basic.forever(function () {
    basic.showNumber(steps)
})
```

## Geschafft!

Herzlichen Glückwunsch!

<script src="https://makecode.com/gh-pages-embed.js"></script>
<script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
