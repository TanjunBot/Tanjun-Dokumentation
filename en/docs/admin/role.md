---
description: Hier geht es um die Commands /admin addrole, /admin removerole, /admin createrole und /admin deleterole.
icon: id-badge
---

# Rollen-Befehle

{% hint style="info" %}
Man könnte sich ja fragen: Warum gibt es diese Commands in Tanjun? Das kann man doch auch alles normal in den Servereinstellungen in Discord machen.\
Ja, das ist soweit richtig, allerdings ist dies besonders an Mobilgeräten häufig sehr umständlich und nervig. Diese Commands sind vorallem dafür gedacht, die Verwaltung des Servers in der mobilen App angenehmer und einfacher zu gestalten.
{% endhint %}

## `Rolle_hinzufügen`-Befehl

Mit `/admin rolle rolle_hinzufügen <benutzer> <rolle>` kann man einem Nutzer eine Rolle geben.

## `Rolle_entfernen`-Befehl

Mit `/admin rolle rolle_entfernen <benutzer> <rolle>` kann man einem Nutzer eine Rolle entziehen.

## Rolle\_erstellen-Befehl

Mit

```
/admin rolle rolle_erstellen <name> [farbe] [anzeige_icon] [getrennt_anzeigen] [erwähnbar] [grund] [anzeige_emoji]
```

&#x20;kann man eine neue Rolle erstellen.

<details>

<summary>Bedeutungen der einzelnen Parameter</summary>

- Mit `name` gibt man den Namen der Rolle an.
- Mit `farbe` kann man die Farbe der Rolle als [HEX-Code](https://htmlcolorcodes.com) angeben. (Beispiel: `#ECC3EF`)\
  Wenn man keine Farbe angibt, hat die Rolle die Standardfarbe.
- Mit `anzeige_icon` kann man ein Bild hochladen, das als Rollenicon z.B. [neben dem Namen von Mitgliedern mit dieser Rolle](#user-content-fn-1)[^1] angezeigt wird.\
  **Achtung:** Der Server muss Boost-Level 2 sein, um ein Rollenicon zu verwenden. Das Bild muss kleiner als 256 kB und mindestens 64x64 Pixel groß sein.
- Mit `anzeige_emoji` kann man ein Emoji auswählen, das als Rollenicon z.B. [nebem dem Namen von Mitgliedern mit dieser Rolle](#user-content-fn-2)[^2] angezeigt wird.\
  **Achtung:** Dieser Parameter kann [**nicht in Kombination**](#user-content-fn-3)[^3] mit `display_icon` angegeben werden.
- Mit `getrennt_anzeigen` kann man festlegen, ob Mitglieder mit dieser Rolle auf der rechten Seite gruppiert werden sollen.
- Mit `erwähnbar` kann man festlegen, ob Mitglieder diese Rolle erwähnen dürfen oder nicht.
- Mit `grund` kann man einen Text festlegen, der als [Begründung für das Erstellen der Rolle im Audit-Log](#user-content-fn-4)[^4] angezeigt wird.

</details>

## `Rolle_löschen`-Befehl

Mit `/admin rolle rolle_löschen <rolle> [grund]` kann man eine Rolle löschen.

<details>

<summary>Bedeutungen der einzelnen Parameter</summary>

- Mit `role` gibt man die Rolle an, die gelöscht werden soll.
- Mit `reason` kann man einen Text festlegen, der als [Begründung für das Erstellen der Rolle im Audit-Log](#user-content-fn-5)[^5] angezeigt wird.

</details>

[^1]: Wenn Mitglieder mehrere Rollen besitzen, wird immer das Icon der höchsten Rolle angezeigt, die ein Icon besitzt.

[^2]: Wenn Mitglieder mehrere Rollen besitzen, wird immer das Icon der höchsten Rolle angezeigt, die ein Icon besitzt.

[^3]: Das display\_icon wird bevorzugt.

[^4]: Begründungen, die im Audit-Log angezeigt werden, sind für viele Sachen in Discord implementiert, können aber in den meisten Fällen nur über Bots verwendet werden.

[^5]: Begründungen, die im Audit-Log angezeigt werden, sind für viele Sachen in Discord implementiert, können aber in den meisten Fällen nur über Bots verwendet werden.
