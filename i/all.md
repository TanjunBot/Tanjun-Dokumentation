---
description: Auf dieser Seite findest du nützliche Hinweise zur Bedienung von Tanjun.
---

# ℹ Allgemeine Tipps

{% hint style="warning" %}
**Wichtig:** Diese Seite ist noch nicht fertig und wird noch bearbeitet!
{% endhint %}

## Hilfe-Command <a href="#a1" id="a1"></a>

Wie die meisten Discord Bots hat auch Tanjun einen Hilfe Command. Mit diesem kannst du dir alle aktuell verfügbaren Commands und deren Beschreibung anzeigen lassen.

Du kannst die Hilfe wie folgt aufrufen:&#x20;

```
/help
```

Es wird dir eine Nachricht angezeigt, unter der du in einem Menü aus verschiedenen Kategorien auswählen kannst.

<figure><img src="https://img.arion2000.xyz/r/RoZoVaFyQH.png" alt="Screenshot der Nachricht, die angezeigt wird, wenn man den Hilfe-Command verwendet."><figcaption></figcaption></figure>

Wenn du eine Kategorie auswählst, werden dir alle Commands dieser Kategorie plus einer Beschreibung angezeigt.

<div data-full-width="false">

<figure><img src="https://img.arion2000.xyz/r/fa0Ika996S.png" alt="Screenshot der Nachricht, die angezeigt wird, wenn man beim Hilfe-Command eine Kategorie auswählt (in diesem Beispiel wurde die Kategorie &#x22;utility&#x22; verwendet)."><figcaption></figcaption></figure>

</div>

***

## Commandgruppen <a href="#a2" id="a2"></a>

Tanjun arbeitet in der neuesten Version fast vollständig mit Commandgruppen. Das kann in Kombination mit Discords Slash-Command-Menü dabei helfen, bestimmte Commands schneller zu finden, indem man nach dem / eine bestimmte Kategorie eingibt.&#x20;

{% hint style="info" %}
Die Kategorien in den Slash Commands und im [#a1](all.md#a1 "mention") sind die gleichen. Wenn man z.B. einen Utility-Command senden will, gibt man einfach `/utility` ein und es werden die Commands aus der Hilfe-Nachricht direkt vorgeschlagen.
{% endhint %}

Die Commands sind meistens wie folgt aufgebaut:

```
/<Command-Kategorie> <Subcommand> [Argument]
```

{% hint style="info" %}
Die korrekte Command-Kategorie ist die, die oben als Titel in der Hilfe-Nachricht steht.
{% endhint %}

***

## Hinweise zur Angabe von Commands <a href="#a3" id="a3"></a>

Wenn wir Commands angeben, dann sind oft Elemente enthalten, die du durch etwas ersetzen musst. Wir geben diese Fälle wie folgt an:

<pre><code><strong>/commandname &#x3C;Erforderliches Argument> [Optionales Argument]
</strong></code></pre>

Die `<`, `>`, `[` und `]` Zeichen weisen wie im Beispiel auf erforderliche und optionale Argumente hin, die du an dieser Stelle selbst einsetzen musst.&#x20;
