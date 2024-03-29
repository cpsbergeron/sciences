# Eclipse 2

## @showdialog

Programme le micro:bit pour qu'il affiche la tempéraure pendant l'éclipse solaire.

## Étape 1

Supprime les blocs ``||basic:au démarrage||`` et ``||basic: toujours||``.

## Étape 2

Glisse le bloc ``||input:lorsque le bouton A est pressé||`` dans la zone de programmation.

Ajoute le bloc ``||basic:montrer nombre||`` dans le bloc ``||input:lorsque le bouton A est pressé||``.

Regarde l'indice au besoin.


```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(0)
})

```

## Étape 3

Remplace la valeur ``||basic:0||`` du bloc ``||basic:montrer nombre||`` par le bloc ``||input:température||``.

Regarde l'indice au besoin.


```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.temperature())
})

```

## Étape 4

Ajoute le bloc ``||basic:pause (ms)||`` sous le bloc ``||basic:montrer nombre||``.

Remplace la valeur ``||basic:100||`` par ``||basic:2000||``.

Regarde l'indice au besoin.


```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.temperature())
    basic.pause(2000)
})

```

## Étape 5

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:pause (ms)||``.

Dessine le symbole T°.

Regarde l'indice au besoin.


```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.temperature())
    basic.pause(2000)
    basic.showLeds(`
        . . . . .
        # # # . #
        . # . . .
        . # . . .
        . # . . .
        `)
})

```

## Étape 6

Ajoute le bloc ``||basic:pause (ms)||`` sous le bloc ``||basic:montrer LEDs||``.

Remplace la valeur ``||basic:100||`` par ``||basic:1000||``.

Regarde l'indice au besoin.


```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.temperature())
    basic.pause(2000)
    basic.showLeds(`
        . . . . .
        # # # . #
        . # . . .
        . # . . .
        . # . . .
        `)
    basic.pause(1000)
})

```

## Étape 7

Ajoute le bloc ``||basic:effacer l'écran||`` sous le bloc ``||basic:pause (ms)||``.

Regarde l'indice au besoin.


```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.temperature())
    basic.pause(2000)
    basic.showLeds(`
        . . . . .
        # # # . #
        . # . . .
        . # . . .
        . # . . .
        `)
    basic.pause(1000)
    basic.clearScreen()
})
```

## @showdialog

Télécharge la programmation dans le micro:bit et teste la programmation.