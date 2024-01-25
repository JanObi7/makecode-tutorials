# compass

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