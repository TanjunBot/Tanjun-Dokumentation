---
icon: id-badge
description: >-
  On this page you'll learn about the commands /admin addrole, /admin removerole, /admin createrole and /admin deleterole.
---

# Role Commands

{% hint style="info" %}
You might ask yourself: Why do these commands exist in Tanjun? I can also do all of this normally in the settings of my server.\
Yes, that's true so far, but especially on mobile devices, this is often very cumbersome and annoying. These commands are primarily intended to make managing your server in the mobile app more convenient and easier.
{% endhint %}

## `Add_role` command

With `/admin role add_role <user> <role>` you can give a user a role.

## `Remove_role` command

With `/admin role role_remove <user> <role>` you can remove a role from a user.

## `Create_role` command

With

```
/admin role role_create <name> [color] [display_icon] [display_seperately] [mentionable] [reason] [display_emoji]
```

&#x20;you can create a new role.

<details>

<summary>Meaning of the individual parameters</summary>

- Use `name` to specify the name of the role.
- With `color` you can specify the color of the role as [HEX code](https://htmlcolorcodes.com). (Example: `#ECC3EF`)\
  If you don't specify a color, the role has the default color.
- With `display_icon` you can upload an image that is displayed as a role icon e.g. [next to the name of members with this role](#user-content-fn-1)[^1].\
  **Important:** The server must have boost level 2 to use a role icon. The image must be smaller than 256 kB and at least 64x64 pixels in size.
- With `display_emoji` you can select an emoji that is displayed as a role icon, e.g. [next to the name of members with this role](#user-content-fn-2)[^2].\
  **Important:** This parameter [**can't be specified in combination**](#user-content-fn-3)[^3] with `display_icon`.
- With `display_seperately` you can specify whether members with this role should be grouped on the right-hand side.
- With `mentionable` you can specify whether members are allowed to mention this role or not.
- With `reason` you can define a text that is displayed as [reason for creating the role in the audit log](#user-content-fn-4)[^4].

</details>

## `Delete_role` command

You can delete a role with `/admin role role_delete <role> [reason]`.

<details>

<summary>Meaning of the individual parameters</summary>

- Use `role` to specify the role that is to be deleted.
- With `reason` you can define a text that is displayed as [reason for creating the role in the audit log](#user-content-fn-5)[^5].

</details>

[^1]: If members have multiple roles, the icon of the highest role that has an icon is always displayed.

[^2]: If members have multiple roles, the icon of the highest role that has an icon is always displayed.

[^3]: The display\_icon is preferred.

[^4]: Reasons that are displayed in the audit log are available for many things in Discord, but in most cases can only be used via bots.

[^5]: Reasons that are displayed in the audit log are available for many things in Discord, but in most cases can only be used via bots.
