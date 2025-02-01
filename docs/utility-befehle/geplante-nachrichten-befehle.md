---
description: >-
  Mit dieser Funktion lassen sich Nachrichten planen, die zu einem späteren
  Zeitpunkt automatisch versendet werden sollen.
icon: calendar-circle-exclamation
---

# Geplante-Nachrichten-Befehle

## `Planen`-Befehl

Mit dem `/verschiedenes planen neu <inhalt> <send_in> [kanal] [wiederholungsintervall] [wiederholungs_anzahl]`-Befehl kannst du eine Nachricht planen.

Der `Wiederholungsintervall`-Parameter gibt an, in welchem Abstand die Nachricht [nach dem ersten ](#user-content-fn-1)[^1]Senden wiederholt werden soll.

Der `Wiederholungs_anzahl`-Parameter gibt an, wie oft die geplante Nachricht im durch `wiederholungsintervall` angegebenen Intervall gesendet werden soll.

{% hint style="success" %}
Verwende die Widerholungsanzahl **0** für unendlich oft und **1**, um einmalig eine Nachricht zu versenden. Verwende alle Zahlen, die größer als 1 sind, um die Nachricht x Mal zu senden.
{% endhint %}

{% hint style="info" %}
Damit die Nachricht wiederholt gesendet werden kann, müssen sowohl das `wiederholungsintervall` als auch die `wiederholungs_anzahl` definiert werden. Wenn nur eines von beiden definiert ist, wird die Nachricht nicht wiederholt sondern nur einmal gesendet.
{% endhint %}

## `Auflisten`-Befehl

Mit dem `/verschiedenes planen auflisten`-Befehl kannst du dir alle geplanten Nachrichten auflisten lassen. Hier erfährst du auch die Nachrichten-ID, welche zum Löschen benötigt wird.

## `Entfernen`-Befehl

Mit dem `/verschiedenes planen entfernen <nachricht_id>`-Befehl kannst du eine geplante Nachricht löschen. Die Nachrichten-ID, welche für den `nachricht_id`-Parametere benötigt wird, findest du im [Auflisten-Befehl](geplante-nachrichten-befehle.md#auflisten-befehl).

[^1]: Wie lange es vom Eingeben des Commands bis zum ersten Senden der Nachricht dauert, wird durch `send_in` angegeben.
