---
description: Wenn ein Nutzer deinen Server boostet, kann sich dieser mithilfe dieser Funktionen eine eigene Booster-Rolle abholen.
icon: rocket-launch
---

# Booster-Rollen

## `Informationen`-Befehl

Mit dem `/verschiedenes boosterrole informationen` Befehl erfährst du weitere Einzelheiten über die Booster-Rollen.

## `Einfordern`-Befehl

Mit dem `/verschiedenes boosterrolle einfordern <name> [farbe] [icon]`-Befehl kann man sich, sofern man den Server aktiv boostet, eine eigene Booster-Rolle erstellen lassen, welche einem dann auch automatisch vom Bot zugeordnet wird.

{% hint style="warning" %}
Die Rolle von Tanjun muss höher sein, als die Boosterrollen, damit diese den Mitgliedern zugeordnet werden können.
{% endhint %}

## `Einrichten`-Befehl

Mit dem `/verschiedenes boosterrolle einrichten <rolle>`-Befehl kann die Boosterrollen-Funktion aktiviert werden, wodurch Nutzer Booster-Rollen einfordern können.

Der `Rolle`-Parameter legt eine Rolle fest, die in Bezug auf die Berechtigungen der Booster-Rollen als Vorlage genutzt wird.

{% hint style="info" %}
Nur Nutzer mit Administrator-Rechten können diesen Befehl ausführen.
{% endhint %}

## `Entfernen`-Befehl

Mit dem `/verschiedenes boosterrolle entfernen`-Befehl kann die Boosterrollen-Funktion deaktiviert werden. Es können dann keine weiteren Booster-Rollen mehr eingefordert werden. Bereits abgeholte Rollen bleiben bestehen und werden weiterhin automatisch entfernt, wenn der Nutzer aufhört, den Server zu boosten.
