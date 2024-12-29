---
icon: joystick
description: >-
  Hier geht es um die Spiele Tic-Tac-Toe, Vier gewinnt, Akinator, Worlde,
  Galgenmännchen, Flaggenquiz und Schere-Stein-Papier.
---

# Arcade & klassische Spiele

## Tic-Tac-Toe

Mit dem `/spiele tic_tac_toe [user]`-Befehl kannst du gegen einen beliebigen Nutzer Tic-Tac-Toe spielen. Du kannst auch gegen Tanjun spielen, wenn du das Argument `user` auslässt.&#x20;

## Vier gewinnt

Mit dem `/spiele 4_gewinnt [user] [size]`-Befehl kannst du 4-Gewinnt gegen einen beliebigen anderen Nutzer spielen. Mit dem Argument `size` kannst du auswählen, wie groß das Spielfeld sein soll, wodurch du einzigartige 4-Gewinnt-Spielweisen kennen lernen kannst. Wenn du keinen Nutzer angibst, spielst du auch hier gegen Tanjun.

{% hint style="info" %}
Du benötigst ein Tanjun Pro Abo, um ein Spiel mit einer anderen Spielfeldgröße zu starten. Du kannst aber auch ohne Tanjun Pro Spiele mit anderer Spielfeldgröße von anderen annehmen.
{% endhint %}

## Akinator

Führe den `/spiele akinator [theme]`-Befehl aus und denke an eine Figur deiner Wahl. Akinator wird anschließend Fragen stellen und versuchen, deine Figur zu erraten.

Mit dem `theme`-Argument kannst du eine Kategorie für deine Figur festlegen, um den Akinator nicht komplett im Dunkeln tappen zu lassen. :wink: Wenn du `theme` nicht angibst, wird standardmäßig "Charaktere" verwendet.

## Wordle

Mit dem `/spiele wordle [sprache]`-Befehl kannst du in einem Wordle-Spiel deine Sprachkenntnisse auf die Probe stellen! Tanjun wird ein [zufälliges Wort](#user-content-fn-1)[^1] aussuchen und du musst versuchen, es in 5 Versuchen zu erraten.&#x20;

* Ein **grauer Buchstabe** ist nicht im gesuchten Wort enthalten
* Ein **gelber Buchstabe** ist enthalten, aber aktuell noch an der falschen Position
* Ein **grüner Buchstabe** ist enthalten und an der korrekten Position.

Du kannst Wordle in jeder von Discord unterstützten Sprache spielen.

{% hint style="info" %}
Wenn ein Buchstabe in einem geratenen Versuch mehrfach vorkommt, aber im Zielwort z.B. nur ein Mal enthalten ist, wird er an allen Stellen, an denen er vorkommt, entsprechend markiert.\
\
Rätst du z.B. <mark style="color:purple;">WI</mark><mark style="color:purple;background-color:orange;">E</mark><mark style="color:purple;">S</mark><mark style="color:purple;background-color:orange;">E</mark> und das gesuchte Wort ist <mark style="color:purple;">SAG</mark><mark style="color:purple;background-color:green;">E</mark><mark style="color:purple;">N</mark>, werden beide <mark style="color:purple;">E</mark> gelb markiert, obwohl das <mark style="color:purple;">E</mark> nur ein Mal vorkommt.
{% endhint %}

## Galgenmännchen

Mit dem `/spiele galgenmännchen [sprache]`-Befehl kannst du den Klassiker Galgenmännchen (auch genannt Galgenraten) spielen. Tanjun wird an ein Wort denken und du musst versuchen, es zu erraten.

Dafür kannst du einzelne Buchstaben tippen oder versuchen, das ganze Wort aufzulösen. Dafür hast du **12 Versuche**.

{% hint style="warning" %}
Um das Wort zu lösen, musst du das gesamte Wort noch einmal eintippen, sonst wird die Runde nicht als gewonnen gezählt.
{% endhint %}

## Flaggenquiz

Mit dem `/spiele flaggen_quiz [sprache]`-Befehl kannst du deine Kenntnisse über Flaggen auf die Probe stellen! Tanjun wird dir eine zufällige Flagge eines Landes zeigen und du musst versuchen, dieses zu erraten. Doch pass auf, Tanjun zeigt dir nicht nur bekannte Länderflaggen, sondern z.B. auch Überseegebiete. :map::thinking:

## Schere-Stein-Papier

Mit dem `/spiele schere_stein_papier [nutzer]`-Befehl kannst du gegen einen anderen Nutzer Schere-Stein-Papier spielen. Wenn du `nutzer` nicht angibst, kannst du gegen Tanjun spielen.

[^1]: Das zufällige Wort ist eines der 200 häufigsten Wörter mit 5 Buchstaben. Es kann ein Verb, ein Substantiv, ein Adjektiv oder ein konjugiertes Wort sein.
