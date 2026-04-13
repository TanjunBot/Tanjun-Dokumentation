---
description: >-
  Hier geht es um die Commands /admin say, /admin embed, /admin createemoji und /admin copyemoji.
icon: ellipsis
---

# Miscellaneous

## `Say` command

With the `/admin say <message> [channel]` command, you can have Tanjun send a normal text message to a specific channel on the server.

## `Embed` command

With the `/admin embed <message> [channel]` command, you can create an embed that the bot sends to a specific channel.

When you execute the command, the bot responds with a message that is only visible to you, in which you can make all possible settings for the embed.

With `Preview` you can see what the created embed would look like and with `Send` the bot sends the finished embed either to the current or the previously selected channel.

## `Create_emoji` command

This command is intended to make it easier to manage a Discord server, especially in the mobile app.

With the `/admin create_emoji <name> <image_url>` command, you can add an emoji to the server via the bot.

With `name` you enter the name that the emoji should have and with `image_url` you insert a direct link to an image that should be uploaded to the server as an emoji.

{% hint style="info" %}
The file type for the emoji must be either [`JPEG`](#user-content-fn-1)[^1], [`PNG`](#user-content-fn-2)[^2] or [`GIF`](#user-content-fn-3)[^3].

Discord empfiehlt eine Dateigröße von maximal 256 kB und eine Auflösung von 128x128.
{% endhint %}

## `Emoji_kopieren`-Befehl

Mit dem `/admin emoji_kopieren <emoji>`-Befehl können Emojis von anderen Servern kopiert werden. Dieses Emoji wird dann genau so heißen wie das originale Emoji.&#x20;

{% hint style="info" %}
Wenn der Server [Tanjun Pro](../../subscriptions.md#tanjun-pro) besitzt, können mehrere Emojis auf einmal kopiert werden. Server ohne Tanjun Pro können immer nur ein Emoji auf einmal kopieren.
{% endhint %}

[^1]: JPEG and JPG are the same.

[^2]: Use this file type for static, transparent emojis that should not have a background.

[^3]: Use this file type for animated emojis.
