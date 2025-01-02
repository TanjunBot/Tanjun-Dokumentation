---
icon: screwdriver-wrench
description: On this page you'll learn about the commands /admin kick, /admin ban, /admin unban, /admin timeout, /admin timeout_override and the warning system.
---

# Moderation commands

## Basic features

Tanjun can execute the basic moderation commands. These include:

- `/admin kick <user> [reason]`
- `/admin ban <user> [reason]`
- `/admin unban <user> [reason]`
- `/admin timeout <user> <duration (in minutes)> [reason]`
- `/admin remove_timeout <user> [reason]`

## Warning system <a href="#warn" id="warn"></a>

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

[^1]: If the warned user has blocked the bot, for example, or generally does not accept direct messages, Tanjun cannot write a message to this user.

[^2]: Direct Message
