---

description: On this page you'll learn about the counting minigames.
icon: list-ol

---

# Counting

## Counting (Default variant)

### Explanation

The goal of the counting game is to count in increments of 1 to infinity. The users must take turns counting. If incorrect characters or numbers are sent to the channel, or if someone sends two messages in a row, the message will be deleted.

### Setup

* Use the `/minigame counting set_channel <channel>` command to designate a channel on the server as the counting channel. You can also run counting games in multiple channels at the same time.
* Use the `/minigame counting remove_channel <channel>` command to end the counting game in a channel.
* Use the `/minigame counting set_progress <channel> <progress>` command to set the progress to a specific number. If you set the progress to `100`, for example, the next correct number would be `101`.

## Counting Modes variant

### Explanation

In the _Counting Modes_ variant, you have to count according to a different principle in each round. Each round has a target number that you must count up to. When the target is reached, a new round begins.

Also, you can’t make any mistakes when in _Counting Modes_, because as soon as someone sends an incorrect number or two numbers in a row, a new round begins.

{% hint style="success" %}
To enable the _Counting Modes_ minigame, the server needs the **Tanjun Pro** subscription. When the subscription expires, the minigame will remain active and fully functional. It can also be disabled without any issues and you can set the progress without a Tanjun Pro subscription.
{% endhint %}

### Game Modes Overview

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><strong>Positive numbers</strong></td><td><a href="1.md">1.md</a></td></tr><tr><td><strong>Negative numbers</strong></td><td><a href="2.md">2.md</a></td></tr><tr><td><strong>Even numbers</strong></td><td><a href="3.md">3.md</a></td></tr><tr><td><strong>Odd numbers</strong></td><td><a href="4.md">4.md</a></td></tr><tr><td><strong>From 100 to 0</strong></td><td><a href="5.md">5.md</a></td></tr><tr><td><strong>Increments of 100</strong></td><td><a href="6.md">6.md</a></td></tr><tr><td><strong>Square numbers</strong></td><td><a href="7.md">7.md</a></td></tr><tr><td><strong>Cubic numbers</strong></td><td><a href="8.md">8.md</a></td></tr><tr><td><strong>Prime numbers</strong></td><td><a href="9.md">9.md</a></td></tr><tr><td><strong>Fibonacci sequence</strong></td><td><a href="10.md">10.md</a></td></tr><tr><td><strong>Binary numbers</strong></td><td><a href="11.md">11.md</a></td></tr><tr><td><strong>Roman numerals</strong></td><td><a href="12.md">12.md</a></td></tr></tbody></table>

### Setup

* Use the `/minigame countingmodes set_channel <channel>` command to designate a channel on the server as the channel for the _Counting Modes_ game. You can also run counting games in multiple channels at the same time.
* Use the `/minigame countingmodes remove_channel <channel>` command to end the _Counting Modes_ game in a channel.
* Verwende den `/minispiel countingmodes fortschritt_setzen <kanal> <fortschritt>`-Befehl, um den Fortschritt zu ändern.

## Counting Challenge-Variante

### Explanation

Im Countingchallenge-Modus kann man in 1er-Schritten unendlich weit zählen, aber der Fortschritt wird bei Fehlern oder wenn eine Person zwei Nachrichten nacheinander sendet, zurückgesetzt.

### Setup

* Use the `/minigame countingchallenge set_channel <channel>` command to designate a channel on the server as the channel for the *Counting Challenge* game. You can also run counting games in multiple channels at the same time.
* Use the `/minigame countingchallenge remove_channel <channel>` command to end the *Counting Challenge* game in a channel.
* Use the `/minigame countingchallenge set_progress <channel> <progress>` command to set the progress to a specific value.
