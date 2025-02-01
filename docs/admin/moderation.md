---
icon: screwdriver-wrench
description: >-
  Hier geht es um die Commands /admin kick, /admin ban, /admin unban, /admin
  timeout, /admin timeout_aufheben und das Warn-System.
---

# Moderator-Befehle

## Grundfunktionen

Tanjun kann die grundlegenden Moderationsbefehle ausführen. Dazu gehören:

* `/admin kick <nutzer> [grund]`
* `/admin ban <nutzer> [grund]`
* `/admin unban <nutzer> [grund]`
* `/admin timeout <mitglied> <länge (in Minuten)> [grund]`
* `/admin timeout_aufheben <mitglied> [grund]`

## Warn-System <a href="#warn" id="warn"></a>

Das Warn-System in Tanjun kann dazu verwendet werden, andere Mitglieder zu verwarnen, wenn sie gegen die Regeln verstoßen haben.

### `Config`-Befehl

Der `/admin warn konfigurieren`- Befehl kann verwendet werden, um das Warn-System zu konfigurieren. Hierbei wird sich ein Popup öffnen, in welchem das Warn-System konfiguriert werden kann.

{% hint style="warning" %}
Das Ändern der Verfallstage hat keinen Einfluss auf Verwarnungen in der Vergangenheit und wird nur auf zukünftige Verwarnungen angewendet werden.
{% endhint %}

<details>

<summary>Bedeutung der einzelnen Werte</summary>

* Die **Verfallstage** bestimmen, nach wie vielen Tagen eine Warnung automatisch verfallen soll.
* Der **Schwellwert für Timeout** bestimmt, nach wie vielen Warnungen ein Nutzer automatisch in Timeout geschickt wird. Der Nutzer wird für jede weitere Verwarnung über dem Schwellwert erneut in Timeout geschickt.
* Die **Dauer des Timeouts** bestimmt, wie lange der Nutzer in Timeout geschickt werden soll.
* Der **Schwellwert für Kick** gibt an, nach wie vielen Timeouts der Nutzer gekickt werden soll. Nach einem Kick kann der Nutzer jederzeit wieder auf den Server eingeladen werden. Wenn der **Schwellwert für Timeout** ≥ dem **Schwellwert für Kick** ist, wird der Nutzer auch in Timeout geschickt, welcher auch nach erneutem Betreten des Servers weiter abläuft. Für jede weitere Verwarnung wird der Nutzer erneut gekickt.
* Der **Schwellwert für Bann** gibt an, nach wie vielen Verwarnungen ein Nutzer gebannt werden soll.

</details>

<figure><img src="../../.gitbook/assets/warn_config_modal.png" alt="" width="331"><figcaption><p>Beispiel für das Popup zum Konfigurieren des Warn-Systems</p></figcaption></figure>

### Jemanden verwarnen

Mit dem `/admin warn hinzufügen <mitglied> [grund]`-Befehl kann ein Nutzer verwarnt werden. Berechtigte Nutzer können nur Nutzer mit einer niedrigeren höchsten Rolle verwarnen als sie selbst. Wenn ein Nutzer verwarnt wird, bekommt dieser, [wenn möglich](#user-content-fn-1)[^1], eine DM[^2].

### Verwarnungen abrufen

Mit dem `/admin warn anzeigen <mitglied>`-Befehl können Verwarnungen von einzelnen Nutzern abgerufen werden.

Warnungen, können hier auch ganz einfach gelöscht werden. Beim Entfernen einer Verwarnung wird der verwarnte Nutzer **nicht** benachrichtigt (sowohl wenn sie abläuft als auch wenn sie manuell entfernt wird).

Wenn ein Nutzer über das Warn-System in Timeout geschickt, gekickt oder gebannt wird, wird dies als Grund in den Audit Logs in den Servereinstellungen angezeigt.

## Report-System

Mit dem Report-System können Nutzer auf dem Server den `/verschiedenes report <nutzer> <grund>`-Befehl verwenden, um andere Nutzer bei einem Regelverstoß an das Serverteam zu melden.

Die eingehenden Meldungen sendet Tanjun in einen Kanal, der zuvor festgelegt werden muss, damit das Report-System funktioniert.

### Kanal für Reports festlegen

Mit dem `/admin report kanal_setzen <kanal>`-Befehl kann festgelegt werden, in welchen Kanal neue Reports gesendet werden sollen.

Unter den Nachrichten zu eingehenden Reports befinden sich Buttons zum **Akzeptieren oder** **Ablehnen des Reports** und zum [**Blockieren** **des Nutzers**](moderation.md#blockieren-funktion).

Die Funktionen zum Akzeptieren und Ablehnen des Reports dienen lediglich zur Organisation innerhalb des Serverteams, um leichter kenntlich zu machen, welche Reports bereits bearbeitet wurden und ob etwas unternommen wurde oder ob sie fehlerhaft sind.

{% hint style="info" %}
Dies sollte ein privater Kanal sein, auf den nur das Serverteam (z.B. Moderatoren) zugreifen können, da Nutzer hier potenziell sensible Informationen teilen, wenn sie andere melden.
{% endhint %}

### Kanal für Reports entfernen

Mit dem `/admin report kanal_entfernen`-Befehl kann der aktuelle Report-Kanal entfernt werden. Neue Reports werden dann nicht mehr in den zuvor festgelegten Kanal gesendet, der `/verschiedenes report`-Befehl funktioniert allerdings weiterhin, die Moderatoren werden nur nicht mehr direkt über eingehende Reports informiert.

### Alle Reports anzeigen lassen

Mit dem `/admin report reports_anzeigen [nutzer]`-Befehl können sich Admins oder Moderatoren alle aktuellen Reports anzeigen lassen.

#### Blockieren-Funktion

Die Blockieren-Funktion ist dafür da, um Nutzer, die Falschmeldungen oder Spam einreichen, daran zu hindern, weitere Reports absenden zu können.

#### Blockieren eines Nutzers rückgängig machen

Mit dem `/admin report nutzer_entblocken <nutzer>`-Befehl kann ein zuvor blockierter Nutzer entblockt werden, wodurch er wieder Reports einreichen kann. Entblockte Nutzer können jederzeit über einen der Buttons unter den Report-Embeds erneut blockiert werden.

### Weitere Hinweise

Wir empfehlen, in einem für alle Nutzer leicht zugänglichen Kanal (z.B. im Regelkanal) darauf hinzuweisen, dass es den Report-Befehl gibt, damit die Mitglieder wissen, dass er existiert und wie er zu verwenden ist.

[^1]: Falls der verwarnte Nutzer den Bot z.B. blockiert hat oder generell keine Direktnachrichten akzeptiert, kann Tanjun diesem Nutzer keine Nachricht schreiben.

[^2]: Direktnachricht
