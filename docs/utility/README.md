---
icon: feather
description: >-
  Die Utility-Befehle sind Befehle, die sich in die anderen Befehlsgruppen nicht
  einsortieren lassen. Sie können alles mögliche machen.
---

# Utility-Befehle

## `Avatar`-Befehl

Mit dem `/verschiedenes avatar [nutzer]`-Befehl kannst du dir den Avatar eines Benutzers anzeigen lassen. Sollte der Nutzer einen Server-Avatar haben, wird dieser groß angezeigt und oben in der Ecke des Embeds der standardmäßige, server-übergreifende Avatar des Nutzers.

## `Banner`-Befehl

Mit dem `/verschiedenes banner [nutzer]`-Befehl kannst du dir den Banner eines Nutzers anzeigen lassen.

{% hint style="info" %}
Tanjun kann den Banner des Servers nicht anzeigen, da Bots/Apps aufgrund von Discord-Einschränkungen darauf nicht zugreifen können
{% endhint %}

## `Avatardekoration`-Befehl

Mit dem `/verschiedenes avatardekoration [nutzer]`-Befehl kannst du dir die Avatardekoration von einem Nutzer anzeigen lassen.

{% hint style="info" %}
Tanjun kann die server-spezifische Avatardekoration und die Profileffekte eines Nutzers aufgrund von Discord-Einschränkungen nicht anzeigen.

Wenn du möchtest, dass Discord diese Einschränkungen überarbeitet, kannst du der Feature Request [HIER](https://github.com/discord/discord-api-docs/discussions/7315) einen Upvote geben.
{% endhint %}

## `Feedback`-Befehl

Mit dem `/verschiedenes feedback`-Befehl kannst du uns Feedback zu Tanjun geben. Ganz egal, ob du eine Idee für einen neuen Befehl hast oder dir etwas nicht gefällt, wir freuen uns über jedes Feedback!

## `AFK`-Befehl

Mit dem `/verschiedenes afk <grund>`-Befehl kannst du dich selbst AFK[^1] stellen. Wenn andere Nutzer dich zu pingen, werden sie darüber informiert, dass du AFK bist und gleichzeitig erfahren, wieso du AFK bist. Wenn du wieder etwas schreibst, wird dir Tanjun eine Nachricht senden, in der aufgelistet steht, wo du überall gepingt wurdest, während du abwesend warst.

{% hint style="info" %}
Das AFK-System ist server-spezifisch. Du kannst dich also auf einem Server AFK stellen und auf einem anderen Server weiter schreiben, ohne dass sich dein AFK-Status ändert.
{% endhint %}

## `Report`-Befehl

Wenn das Report-System auf dem Server aktiviert ist, kannst du mit `/verschiedenes report <nutzer> <grund>`-Befehl einen anderen Nutzer an das Serverteam melden. Im Idealfall wird sich die Server Administration dann um deinen Report kümmern.

Weitere Informationen zum Report-System:

{% content-ref url="../admin/moderation.md" %}
[moderation.md](../admin/moderation.md)
{% endcontent-ref %}

## Weitere Utility-Befehle

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><strong>Booster-Rollen</strong></td><td>Wenn ein Nutzer deinen Server boostet, kann sich dieser mithilfe dieser Funktion eine eigene Booster-Rolle abholen.</td><td><a href="booster-roles.md">booster-roles.md</a></td></tr><tr><td><strong>Booster-Kanäle</strong></td><td>Wenn ein Nutzer deinen Server boostet, kann sich dieser mithilfe dieser Funktion einen eigenen Booster-Sprachkanal erstellen lassen.</td><td><a href="booster-channels.md">booster-channels.md</a></td></tr><tr><td><strong>Autopublish-Befehle</strong></td><td>Mit der Autopublish-Funktion werden Nachrichten, die in bestimmte Ankündigungskanäle gesendet werden, automatisch veröffentlich.</td><td><a href="autopublish.md">autopublish.md</a></td></tr><tr><td><strong>Brawlstars-Befehle</strong></td><td>Mit den Brawlstars-Befehlen kannst du einige Statistiken über verknüpfte Brawlstars-Accounts erhalten.</td><td><a href="brawlstars.md">brawlstars.md</a></td></tr><tr><td><strong>Twitch-Befehle</strong></td><td>Mit dem Twitch-Befehlen kannst du deinen Discord-Server benachrichtigen, wenn ein Twitch-Kanal live geht!</td><td><a href="twitch.md">twitch.md</a></td></tr><tr><td><strong>Geplante-Nachrichten-Befehle</strong></td><td>Mit dieser Funktion lassen sich Nachrichten planen, die zu einem späteren Zeitpunkt automatisch versendet werden sollen.</td><td><a href="scheduledmessages.md">scheduledmessages.md</a></td></tr></tbody></table>

[^1]: Sich selbst als "away from keyboard" bzw. als abwesend markieren
