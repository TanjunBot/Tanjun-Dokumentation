---
icon: align-left
description: Hier geht es um die Commands /admin purge, /admin nuke, /admin slowmode, /admin lock und /admin unlock.
---

# Channel-Befehle

## `Löschen`-Befehl

Mit dem `/admin löschen <limit> [kanal] [einstellung]`-Befehl kann man eine bestimmte Anzahl an Nachrichten aus dem Kanal, in dem du den Command ausführst, auf einmal löschen.

Mit dem `einstellung`-Argument kannst du genauer filtern, welche Nachrichten gelöscht werden sollen.

{% hint style="info" %}
Nachrichten, die älter als 2 Wochen sind, können mit diesem Command in der Regel nicht mehr gelöscht werden.
{% endhint %}

## `Nuke`-Befehl

Falls die Menge an Nachrichten, die man mit dem `/admin löschen`-Befehl löschen kann, nicht ausreicht, kann man mit diesem Command **alle Nachrichten** aus einem Kanal löschen.

Dies funktioniert, indem der Bot eine exakte Kopie des Kanals anfertigt und den originalen Kanal löscht.

{% hint style="success" %}
Damit man diesen Befehl nicht versehentlich ausführt, muss man, nachdem man den Befehl gesendet hat, NUKE[^1] in den Kanal schreiben, bevor diese Aktion ausgeführt wird.
{% endhint %}

## `Slowmodus`-Befehl

Mit dem Befehl `/admin slowmodus <sekunden> [kanal]` kann man den Slow-Modus in einem Kanal auf eine beliebige Anzahl an Sekunden einstellen.

Dieser Command ist besonders praktisch, wenn du den Slow-Modus auf eine Zahl setzen möchtest, die man standardmäßig in den Kanaleinstellungen nicht auswählen kann.

Mit `/admin slowmodus 0 [kanal]` kannst du den Slow-Modus in einem Kanal wieder deaktivieren.

## `Sperren`- und Entsperren-Befehle

Mit diesen beiden Befehlen kann man Mitglieder entweder daran hindern, in einem Kanal Nachrichten zu schreiben oder das Schreiben von Nachrichten wieder erlauben.

Wenn der `/admin sperren`-Befehl ausgeführt wird, wird von @everyone und allen zusätzlichen Rollen und Mitgliedern die `Nachrichten senden`-Berechtigung auf ❌ gesetzt. So kann niemand (außer Administratoren) mehr in dem Kanal schreiben. Durch den `/admin entsperren`-Befehl wird der Zustand vor dem Sperren wiederhergestellt (wer vor dem Sperren nicht schreiben durfte, darf es danach auch nicht).

[^1]: Muss exakt so geschrieben werden, komplett in Großbuchstaben!
