# Eclipse 1

## @showdialog

Programme le micro:bit pour qu'il affiche l'animation de l'éclipse solaire.

## Étape 1

Supprime les blocs ``||basic:au démarrage||`` et ``||basic: toujours||``.

## Étape 2

Glisse le bloc ``||input:lorsque secouer||`` dans la zone de programmation.

Ajoute le bloc ``||basic:montrer LEDs||`` dans le bloc ``||input:lorsque secouer||``.

À l'aide de l'indice, dessine le soleil.


```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
})

```

## Étape 3

Ajoute le bloc ``||basic:pause (ms)||`` sous le bloc ``||basic: montrer LEDs||``.

Remplace la valeur ``||basic:100||`` par ``||basic:500||``.

```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
})

```

## Étape 4

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:pause (ms) 500||``.

À l'aide de l'indice, dessine une partie de l'éclipse solaire.


```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
})

```

## Étape 5

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:montrer LEDs||``.

À l'aide de l'indice, dessine une partie de l'éclipse solaire.


```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
    basic.showLeds(`
        . . # # .
        . . . # #
        . . . # #
        . . . # #
        . . # # .
        `)
})

```

## Étape 6

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:montrer LEDs||``.

À l'aide de l'indice, dessine une partie de l'éclipse solaire.

```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
    basic.showLeds(`
        . . # # .
        . . . # #
        . . . # #
        . . . # #
        . . # # .
        `)
    basic.showLeds(`
        . . . # .
        . . . . #
        . . . . #
        . . . . #
        . . . # .
        `)
})


```

## Étape 7

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:montrer LEDs||``.

À l'aide de l'indice, dessine une partie de l'éclipse solaire.

```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
    basic.showLeds(`
        . . # # .
        . . . # #
        . . . # #
        . . . # #
        . . # # .
        `)
    basic.showLeds(`
        . . . # .
        . . . . #
        . . . . #
        . . . . #
        . . . # .
        `)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
})

```

## Étape 8

Ajoute le bloc ``||basic:pause (ms)||`` sous le bloc ``||basic: montrer LEDs||``.

Remplace la valeur ``||basic:100||`` par ``||basic:1000||``.

```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
    basic.showLeds(`
        . . # # .
        . . . # #
        . . . # #
        . . . # #
        . . # # .
        `)
    basic.showLeds(`
        . . . # .
        . . . . #
        . . . . #
        . . . . #
        . . . # .
        `)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
    basic.pause(1000)
})

```

## Étape 9

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:pause (ms) 1000||``.

À l'aide de l'indice, dessine une partie de l'éclipse solaire.


```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
    basic.showLeds(`
        . . # # .
        . . . # #
        . . . # #
        . . . # #
        . . # # .
        `)
    basic.showLeds(`
        . . . # .
        . . . . #
        . . . . #
        . . . . #
        . . . # .
        `)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
    basic.pause(1000)
    basic.showLeds(`
        . # . . .
        # . . . .
        # . . . .
        # . . . .
        . # . . .
        `)
})

```

## Étape 10

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:montrer LEDs||``.

À l'aide de l'indice, dessine une partie de l'éclipse solaire.

```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
    basic.showLeds(`
        . . # # .
        . . . # #
        . . . # #
        . . . # #
        . . # # .
        `)
    basic.showLeds(`
        . . . # .
        . . . . #
        . . . . #
        . . . . #
        . . . # .
        `)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
    basic.pause(1000)
    basic.showLeds(`
        . # . . .
        # . . . .
        # . . . .
        # . . . .
        . # . . .
        `)
    basic.showLeds(`
        . # # . .
        # # . . .
        # # . . .
        # # . . .
        . # # . .
        `)
})

```

## Étape 11

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:montrer LEDs||``.

À l'aide de l'indice, dessine une partie de l'éclipse solaire.

```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
    basic.showLeds(`
        . . # # .
        . . . # #
        . . . # #
        . . . # #
        . . # # .
        `)
    basic.showLeds(`
        . . . # .
        . . . . #
        . . . . #
        . . . . #
        . . . # .
        `)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
    basic.pause(1000)
    basic.showLeds(`
        . # . . .
        # . . . .
        # . . . .
        # . . . .
        . # . . .
        `)
    basic.showLeds(`
        . # # . .
        # # . . .
        # # . . .
        # # . . .
        . # # . .
        `)
    basic.showLeds(`
        . # # # .
        # # # . .
        # # # . .
        # # # . .
        . # # # .
        `)
})

```

## Étape 12

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:montrer LEDs||``.

À l'aide de l'indice, dessine une partie de l'éclipse solaire.

```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
    basic.showLeds(`
        . . # # .
        . . . # #
        . . . # #
        . . . # #
        . . # # .
        `)
    basic.showLeds(`
        . . . # .
        . . . . #
        . . . . #
        . . . . #
        . . . # .
        `)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
    basic.pause(1000)
    basic.showLeds(`
        . # . . .
        # . . . .
        # . . . .
        # . . . .
        . # . . .
        `)
    basic.showLeds(`
        . # # . .
        # # . . .
        # # . . .
        # # . . .
        . # # . .
        `)
    basic.showLeds(`
        . # # # .
        # # # . .
        # # # . .
        # # # . .
        . # # # .
        `)
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
})

```

## Étape 13

Ajoute le bloc ``||basic:pause (ms)||`` sous le bloc ``||basic: montrer LEDs||``.

Remplace la valeur ``||basic:100||`` par ``||basic:500||``.

```blocks

input.onGesture(Gesture.Shake, function () {
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
    basic.showLeds(`
        . # # # .
        . . # # #
        . . # # #
        . . # # #
        . # # # .
        `)
    basic.showLeds(`
        . . # # .
        . . . # #
        . . . # #
        . . . # #
        . . # # .
        `)
    basic.showLeds(`
        . . . # .
        . . . . #
        . . . . #
        . . . . #
        . . . # .
        `)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
    basic.pause(1000)
    basic.showLeds(`
        . # . . .
        # . . . .
        # . . . .
        # . . . .
        . # . . .
        `)
    basic.showLeds(`
        . # # . .
        # # . . .
        # # . . .
        # # . . .
        . # # . .
        `)
    basic.showLeds(`
        . # # # .
        # # # . .
        # # # . .
        # # # . .
        . # # # .
        `)
    basic.showLeds(`
        . # # # .
        # # # # #
        # # # # #
        # # # # #
        . # # # .
        `)
    basic.pause(500)
})

```

## @showdialog

Télécharge la programmation dans le micro:bit et teste la programmation.
