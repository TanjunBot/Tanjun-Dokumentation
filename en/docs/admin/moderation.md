---
icon: screwdriver-wrench
description: >-
  On this page you'll learn about the commands /admin kick, /admin ban, /admin unban, /admin timeout, /admin timeout_override and the warning system.
---

# Moderation Commands

## Basic Features

Tanjun can execute the basic moderation commands. These include:

- `/admin kick <user> [reason]`
- `/admin ban <user> [reason]`
- `/admin unban <user> [reason]`
- `/admin timeout <user> <duration (in minutes)> [reason]`
- `/admin remove_timeout <user> [reason]`

## Warning System <a href="#warn" id="warn"></a>

The warning system in Tanjun can be used to warn other members if they have broken the rules.

### `Config` command

The `/admin warn configure` command can be used to configure the warning system. This will open a popup in which the warning system can be configured.

{% hint style="warning" %}
Changing the expiry dates has no effect on past warnings and will only be applied to future warnings.
{% endhint %}

<details>

<summary>Meaning of the individual values</summary>

- The **expiry days** determine after how many days a warning should automatically expire.
- The **Threshold for timeout** determines after how many warnings a user is automatically sent to timeout. The user is sent to timeout again for each additional warning above the threshold value.
- The **duration of the timeout** determines how long the user should be sent to timeout.
- The **Threshold for kick** specifies after how many timeouts the user should be kicked. After a kick, the user can be invited back to the server at any time. If the **threshold value for timeout** is ≥ the **threshold value for kick**, the user is also sent to timeout, which continues to run even after re-entering the server. The user will be kicked again for each additional warning.
- The **Threshold for kick** specifies after how many timeouts the user should be kicked.

</details>

<figure><img src="../../.gitbook/assets/warn_config_modal.png" alt="" width="331"><figcaption><p>Example of the pop-up for configuring the warning system</p></figcaption></figure>

### Warn someone

A user can be warned with the `/admin warn add <user> [reason]` command. Authorized users can only warn users with a lower highest role than themselves. If a user is warned, they will receive a DM[^2] [if possible](#user-content-fn-1)[^1].

### Retrieve warnings

The `/admin warn anzeigen <user>` command can be used to retrieve warnings from individual users.

Warnings can also be easily deleted here. When a warning is removed, the warned user is **not** notified (both when it expires and when it is removed manually).

If a user is sent to timeout, kicked or banned via the warning system, this is displayed as the reason in the audit logs in the server settings.

## Reporting System

With the reporting system, users on the server can use the `/miscellaneous report <nutzer> <grund>` command to report other users to the server team in the event of a rule violation.

Tanjun sends the incoming report to a channel that must be defined in advance for the report system to work.

### Set channel for reports

The `/admin report set_channel <kanal>` command can be used to specify the channel which new reports are sent in.

Below the messages for incoming reports there are buttons for **accepting or** **rejecting the report** and for [**blocking** **the user**](moderation.md#blockieren-funktion).

The functions for accepting and rejecting reports are solely for the organization of your server team. They make it easier to see which reports have already been processed, whether action was taken, or if they were invalid.

{% hint style="info" %}
This should be a private channel that only the server team (e.g. moderators) can access, as users share potentially sensitive information here when reporting others.
{% endhint %}

### Remove channel for reports

The current report channel can be removed with the `/admin report remove_channel` command. New reports are then no longer sent to the previously defined channel, but the `/miscellaneous report` command still works, the moderators are just no longer informed directly about incoming reports.

### Display all reports

Admins or moderators can use the `/admin report show_reports [user]` command to display all current reports for a user.

#### Block function

The block function is there to prevent users who submit false reports or spam from being able to send further reports.

#### Unblocking a user

The `/admin report unblock_user <nutzer>` command can be used to unblock a previously blocked user, allowing them to submit reports again. Unblocked users can be blocked again at any time using one of the buttons under the report embeds.

### Extra notes

We recommend pointing out in a channel that is easily accessible to all users (e.g. in the rules channel) that the report command exists so that members know that it exists and how to use it.

[^1]: If the warned user has blocked the bot or does not accept direct messages in general, Tanjun cannot send a message to this user.

[^2]: Direct Message
