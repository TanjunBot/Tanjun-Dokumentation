---
icon: align-left
description: On this page you'll learn about the commands /admin purge, /admin nuke, /admin slowmode, /admin lock and /admin unlock.
---

# Channel commands

## `Purge` command

With the `/admin purge <limit> [channel] [setting]` command, you can delete a certain number of messages at once from a channel.

You can use the `setting` argument to filter more precisely which messages are to be deleted.

{% hint style="info" %}
Messages that are older than 2 weeks can usually no longer be deleted with this command.
{% endhint %}

## `Nuke` command

If the amount of messages that can be deleted with the `/admin purge` command is not sufficient, you can use this command to delete **all messages** from a channel.

This works by the bot making an exact copy of the channel and deleting the original channel.

{% hint style="success" %}
To prevent this command from being executed by mistake, you must write NUKE[^1] in the channel after sending the command before this action is executed.
{% endhint %}

## `Slowmode` command

With the command `/admin slowmode <seconds> [channel]` you can set the slow mode in a channel to any number of seconds.

This command is particularly useful if you want to set the slow mode to a number that cannot be selected by default in the channel settings.

With `/admin slowmode 0 [channel]` you can deactivate the slow mode in a channel.

## 'Lock' and 'Unlock' commands

With these two commands, you can either prevent members from writing messages in a channel or allow them to write messages again.

When the `/admin lock` command is executed, @everyone and all additional roles and members will have their `send messages` permission set to ❌. This means that nobody (except administrators) can write in the channel. The `/admin unlock` command restores the status before the lock (anyone who was not allowed to write before the lock is not allowed to write afterwards either).

[^1]: Must be written exactly like this, completely in capital letters!
