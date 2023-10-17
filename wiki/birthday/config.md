---
description: Auf dieser Seite findest du Informationen über den /birthday config Command.
---

# 🔧 Konfiguration des Geburtstagssystems

Mithilfe des **`/birthday config` Commands** können **Servermitglieder mit Administratorrechten** bestimmte **Einstellungen am Geburtstagssystem** vornehmen.

{% hint style="info" %}
Wir empfehlen, diese Konfigurationscommands auf jeden Fall mindestens einmal auszuführen, wenn du möchtest, dass zu Geburtstagen gratuliert wird. Wenn du das Geburtstagssystem schon einmal konfiguriert hast und plötzlich wieder deaktiviert erscheint, kann es helfen, diese Commands noch einmal auszuführen.
{% endhint %}

Zurzeit gibt es **3 Einstellungsmöglichkeiten**: Du kannst den **Kanal festlegen**, in dem Geburtstagsbenachrichtigungen gesendet werden sollen, du kannst die **Rolle festlegen**, die eine Person, die Geburtstag hat, **am Geburtstagstag bekommen soll** und du kannst eine **Pingrolle festlegen**, die in der Geburtstagsnachricht erwähnt wird.

Nutze diesen Command wie folgt:

```
/birthday config <Kanal> [Rolle] [Pingrolle]
```

{% hint style="info" %}
Man ändert immer alle Konfigurationsoptionen gleichzeitig. Also wenn du den Kanal ändern möchtest, solltest du trotzdem in diesem Command die Rolle und den Ping angeben.
{% endhint %}
