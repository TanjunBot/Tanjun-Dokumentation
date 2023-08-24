---
description: >-
  Auf dieser Seite findest du Informationen über den /channel jointocreate
  Command.
---

# 🔊 Jointocreate Kanal festlegen

Mithilfe des **`/channel jointocreate`** **Commands** können **Servermitglieder mit "Rollen bearbeiten"-Rechten** den Sprachkanal festlegen, der für das **"Join to create" System** genutzt wird. Genauere Informationen darüber, was das **"Join to create" System** ist und wie es funktioniert findest du unter [#wie-funktioniert-das-join-to-create-system](jointocreate.md#wie-funktioniert-das-join-to-create-system "mention").

Nutze diesen Command wie folgt:

```
/channel jointocreate <Sprachkanal>
```

## Wie funktioniert das "Join to create" System? <a href="#a1" id="a1"></a>

Für das "Join to create" System wird ein Sprachkanal benötigt, dem Severmitglieder beitreten können, um ihren eigenen erstellen zu lassen. Nachdem der Sprachkanal erstellt wurde, wird das Servermitglied seinen Kanal verschoben.

{% hint style="info" %}
Es ist egal, was für einen Namen oder Berechtigungen der **Join to create-Kanal** hat, dem Mitglieder beitreten können. Du kannst **jederzeit**, **ohne Probleme zu erzeugen**, den **Namen des Kanals** ändern oder **Berechtigungen ändern**.&#x20;
{% endhint %}

Wenn ein Servermitglied einen eigenen Sprachkanal erstellt hat, können diesem standardmäßig alle anderen Servermitglieder beitreten. Der Ersteller des Sprachkanals bekommt folgende Sonderrechte in diesem Kanal, um bestimmte Einstellungen vornehmen zu können:

* Kanal verwalten
* Rollen verwalten
* Verbinden
* Mitglieder stummschalten
* Ein- und Ausgabe von Mitgliedern deaktivieren
* Mitglieder verschieben

Sobald sich niemand mehr im eigenen Sprachkanal befindet, wird dieser gelöscht.

{% hint style="warning" %}
**Wichtig:** Die eigenen Sprachkanäle werden immer in der Kategorie erstellt, in der sich der **Join to create Kanal** befindet. Beachte, dass durch Einschränkungen von Discord so nur **max. 49 eigene Sprachkanäle** in dieser Kategorie erstellt werden können.\
\
**Je nachdem ob sich der Join to create Kanal in keiner Kategorie befindet**, trifft dies nicht zu.
{% endhint %}
