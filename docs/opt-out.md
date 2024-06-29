---
description: >-
  So kannst du dafür sorgen, dass Tanjun deine Nachrichten nicht verarbeitet
  oder nachverfolgt.
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 🔕 Nachrichtenverfolgung deaktivieren

Tanjun liest oder verarbeitet **keine** deiner normalen Chatnachrichten. Lediglich Text in Befehlen, Formularen oder Minispielen wird von Tanjun verarbeitet, da dies für die Funktionsweise des Bots notwendig ist.

Für weitere Informationen über den Datenschutz in Tanjun, klicke [hier](http://tanjun.bot/privacy-policy).

## Befehl zum Deaktivieren der Nachrichtenverfolgung

Um die Nachrichtenverfolgung von Tanjun zu deaktivieren, kannst du den folgenden Befehl verwenden:

{% tabs %}
{% tab title="English" %}
```
/utilitycmd utility_messagetracking_name utility_messageoptout_name 
```
{% endtab %}

{% tab title="Deutsch" %}
```
/verschiedenes nachrichtenverfolgung deaktivieren 
```
{% endtab %}
{% endtabs %}

### Vorteile

Du kannst mit diesem Befehl die Privatsphäre von dir und deinen Nachrichten weiter erhöhen, da Tanjun alle deine Nachrichten [(außer Befehle und Einträge in z.B. Formulare von Tanjun)](#user-content-fn-1)[^1] nicht liest und ignoriert.

### Nachteile

Wenn du die Nachrichtenverfolgung deaktivierst, kannst du z.B. nicht mehr an Minispielen von Tanjun teilnehmen und der Bot wird auf deine normale Chatnachrichten nicht mit Reaktionen reagieren.

Außerdem kannst du durch das Deaktivieren der Nachrichtenverfolgung im Levelsystem keine XP mehr sammeln und du kannst [an manchen Gewinnspielen](#user-content-fn-2)[^2] nicht mehr teilnehmen.

## Befehl zum Reaktivieren der Nachrichtenverfolgung

Falls du die Nachrichtenverfolgung in der Vergangenheit deaktiviert hast und dich dazu entschieden hast, sie wieder zu aktivieren, kannst du dies mit dem folgenden Befehl tun:

{% tabs %}
{% tab title="English" %}
```
/utilitycmd utility_messagetracking_name utility_messageoptin_name
```
{% endtab %}

{% tab title="Deutsch" %}
```
/verschiedenes nachrichtenverfolgung aktivieren
```
{% endtab %}
{% endtabs %}

Nachdem du den Befehl ausgeführt hast, kannst du wieder an Minispielen teilnehmen und der Bot wird wieder mit Reaktionen auf deine Chatnachrichten reagieren.

[^1]: Dies sind Interaktionen mit dem Bot, sind lediglich diese, die du aktiv und bewusst tätigst.

[^2]: Du kannst an den Gewinnspielen, bei denen eine Voraussetzung das Schreiben einer bestimmten Anzahl an Nachrichten ist, nicht mehr teilnehmen.
