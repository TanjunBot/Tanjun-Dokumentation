---
icon: ellipsis
description: Hier geht es um die Commands /admin say, /admin embed und /admin createemoji.
---

# More

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

Discord recommends a maximum file size of 256 kB and a resolution of 128x128.

Emoji names must be at least 2 characters long and may only contain [alphanumeric characters](#user-content-fn-4)[^4] and underscores.
{% endhint %}

[^1]: JPEG and JPG are the same.

[^2]: Use this file type for static, transparent emojis that should not have a background.

[^3]: Use this file type for animated emojis.

[^4]: Alphanumeric characters include all letters (A-Z, a-z) and digits (0-9).
