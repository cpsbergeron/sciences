# Eclipse 3

## @showdialog

Programme le micro:bit pour qu'il affiche luminosité pendant l'éclipse solaire.

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

Remplace la valeur ``||basic:0||`` du bloc ``||basic:montrer nombre||`` par le bloc ``||math:0   /   0||``.

Regarde l'indice au besoin.


```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(0 / 0)
})


```

## Étape 4

Remplace la valeur ``||math:0||`` de gauche du bloc  ``||math:0   /   0||`` par le bloc ``||math:0   x   0||``.

Regarde l'indice au besoin.


```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(0 * 0 / 0)
})

```

## Étape 5

Remplace les valeurs ``||math:0||``.

Remplace la valeur ``||math:0||`` de gauche par le bloc ``||input:niveau d'intensité lumineuse||``.

Remplace la valeur ``||math:0||`` du centre par la valeur ``||math:100||``.

Remplace la valeur ``||math:0||`` de droite par la valeur ``||math:255||``.

Regarde l'indice au besoin.

```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.lightLevel() * 100 / 255)
})

```

## Étape 6

Ajoute le bloc ``||basic:pause (ms)||`` sous le bloc ``||basic:montrer nombre||``.

Remplace la valeur ``||basic:100||`` par ``||basic:1000||``.

Regarde l'indice au besoin.

```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.lightLevel() * 100 / 255)
    basic.pause(1000)
})

```

## Étape 7

Ajoute le bloc ``||basic:montrer LEDs||`` sous le bloc ``||basic:pause (ms)||``.

Dessine les lettres Lu.

Regarde l'indice au besoin.

```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.lightLevel() * 100 / 255)
    basic.pause(1000)
    basic.showLeds(`
        # . . . .
        # . # . #
        # . # . #
        # . # # #
        # # . . .
        `)
})

```

## Étape 8

Ajoute le bloc ``||basic:pause (ms)||`` sous le bloc ``||basic:montrer LEDs||``.

Remplace la valeur ``||basic:100||`` par ``||basic:1000||``.

Regarde l'indice au besoin.

```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.lightLevel() * 100 / 255)
    basic.pause(1000)
    basic.showLeds(`
        # . . . .
        # . # . #
        # . # . #
        # . # # #
        # # . . .
        `)
    basic.pause(2000)
})

```

## Étape 9

Ajoute le bloc ``||basic:effacer l'écran||`` sous le bloc ``||basic:pause (ms)||``.

Regarde l'indice au besoin.


```blocks

input.onButtonPressed(Button.A, function () {
    basic.showNumber(input.lightLevel() * 100 / 255)
    basic.pause(1000)
    basic.showLeds(`
        # . . . .
        # . # . #
        # . # . #
        # . # # #
        # # . . .
        `)
    basic.pause(2000)
    basic.clearScreen()
})

```

## @showdialog

Télécharge la programmation dans le micro:bit et teste la programmation.