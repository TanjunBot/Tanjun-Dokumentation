---
description: Auf dieser Seite findest du Informationen über den /kanal logs Command.
---

# 📜 Logkanal festlegen

Mithilfe des **`/kanal logs` Commands** können **Servermitglieder mit "Rollen bearbeiten"-Rechten** den Kanal festlegen, in dem Tanjun die Lognachrichten sendet. Das Logsystem ist sehr umfangreich und genauere Informationen über das, was durch das Logsystem dokumentiert wird, findest du unter [#a1](logs.md#a1 "mention").

Nutze diesen Command wie folgt:

```
/kanal logs <Kanal>
```

{% hint style="info" %}
Alle Typen von Logeinträgen werden im selben Kanal gesendet. Es gibt aktuell keine Möglichkeit, verschiede Typen von Lognachrichten in unterschiedliche Kanäle zu senden.&#x20;
{% endhint %}

## Aktionen, die dokumentiert werden <a href="#a1" id="a1"></a>

* Automod Regel wird erstellt
* Automod Regel wird gelöscht
* Kanal wird erstellt
* Kanal wird gelöscht
* Kanal wird aktualisiert
* Emoji wird aktualisiert
* Sticker wird aktualisiert
* Einladung wird erstellt
* Einadung wird gelöscht
* Integration (auch Bot) wird hinzugefügt
* Integration (auch Bot) wird aktualisiert
* Mitglied tritt dem Server bei
* Mitglied verlässt den Server
* Mitglied wird aktualisiert (Name, Nickname, Avatar, Rollen)
* Mitglied wird gebannt
* Mitglied wird entbannt
* Nachricht wird bearbeitet
* Nachricht wird gelöscht
* Mehrere Nachrichten werden auf einmal gelöscht (durch einen Bot)
* Reaktion wird zu einer Nachricht hinzugefügt
* Reaktion wird von einer Nachricht entfernt
* Alle Reaktionen werden von einer Nachricht entfernt
* Alle Reaktionen eines Typs werden von einer Nachricht entfernt
* Rolle wird erstellt
* Rolle wird gelöscht
* Rolle wird aktualisiert
* Event wird erstellt
* Event wird gelöscht
* Event wird aktualisiert
* Mitglied meldet sich als interessiert an Event
* Mitglied meldet sich nicht mehr als interessiert an Event
* Stage-Event wird gestartet
* Stage-Event wird beendet
* Stage-Event wird aktualisiert (Thema, Berechtigungen um teilzunehmen, Sprecherlimit)
* Thread wird erstellt
* Thread wird aktualisiert (Name, Archiviert Ja/Nein, Geschlossen Ja/Nein, Kategorie)
* Thread wird gelöscht
* Mitglied tritt Thread bei
* Mitglied verlässt Thread
* Mitglied tritt Sprachkanal bei
* Mitglied verlässt Sprachkanal
* Mitglied wechselt Sprachkanal
