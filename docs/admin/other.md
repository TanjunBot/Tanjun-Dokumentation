---
icon: ellipsis
description: Hier geht es um die Commands /admin say, /admin embed und /admin createemoji.
---

# Weiteres

## `Sagen`-Befehl

Mit dem `/admin sagen <nachricht> [kanal]`-Befehl kann man Tanjun eine normale Textnachricht in einen bestimmten Kanal auf dem Server senden lassen.

## `Embed`-Befehl

Mit dem `/admin embed <titel> [kanal]`-Befehl kannst du ein Embed erstellen, das der Bot in einen bestimmten Kanal sendet.

Wenn du den Befehl ausführst, antwortet der Bot mit einer nur für dich sichtbaren Nachricht, in der du alle möglichen Einstellungen am Embed vornehmen kannst.

Mit `Vorschau` kannst du dir anzeigen lassen, wie das erstellte Embed aussehen würde und mit `Senden` sendet der Bot das fertige Embed entweder in den aktuellen oder den vorher ausgewählten Kanal.

## `Emoji_erstellen`-Befehl

Dieser Befehl soll die Verwaltung eines Discord-Servers besonders in der mobilen App erleichtern.

Mit dem `/admin emoji_erstellen <name> <bild_url>`-Befehl kannst du über den Bot ein Emoji zum Server hinzufügen.

Mit `name` gibst du den Namen an, den das Emoji haben soll und bei `image_url` fügst du einen direkten Link zu einem Bild ein, das als Emoji auf dem Server hochgeladen werden soll.

{% hint style="info" %}
Der Dateityp für das Emoji muss entweder [`JPEG`](#user-content-fn-1)[^1], [`PNG`](#user-content-fn-2)[^2] oder [`GIF`](#user-content-fn-3)[^3] sein.

Discord empfiehlt eine Dateigröße von maximal 256 kB und eine Auflösung von 128x128.

Emoji-Namen müssen mindestens 2 Zeichen lang sein und dürfen nur [alphanumerische Zeichen](#user-content-fn-4)[^4] und Unterstriche enthalten.
{% endhint %}

[^1]: JPEG und JPG sind das gleiche.

[^2]: Verwende diesen Dateityp für statische, transparente Emojis, die keinen Hintergrund haben sollen.

[^3]: Verwende diesen Dateityp für animierte Emojis.

[^4]: Alphanumerische Zeichen umfassen alle Buchstaben (A-Z, a-z) und Ziffern (0-9).
