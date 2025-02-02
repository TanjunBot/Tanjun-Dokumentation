---
description: >-
  Wenn ein Nutzer deinen Server boostet, kann sich dieser mithilfe dieser
  Funktion einen eigenen Booster-Sprachkanal erstellen lassen.
icon: rocket-launch
---

# Booster-Kanäle

## `Informationen`-Befehl

Mit dem `/verschiedenes boosterkanal informationen`-Befehl erfährst du weitere Einzelheiten über die Booster-Kanäle.

## `Einfordern`-Befehl

Mit dem `/verschiedenes boosterkanal einfordern <name>`-Befehl kann man sich, sofern man den Server aktiv boostet, einen eigenen Booster-Kanal erstellen lassen, in welchem man durch den Bot dann auch automatisch Berechtigungen zur Verwaltung des Kanals bekommt.

## `Einrichten`-Befehl

Mit dem `/verschiedenes boosterkanal einrichten <kategorie>`-Befehl kann die Boosterkanal-Funktion aktiviert werden, wodurch Nutzer Booster-Kanäle einfordern können.

Der `Kategorie`-Parameter legt eine Kategorie fest, in der die Booster-Sprachkanäle erstellt werden.

{% hint style="warning" %}
Aufgrund von Discord-Einschränkungen können nur maximal 50 Kanäle in einer Kategorie erstellt werden, was sich auf Servern mit _sehr vielen_ (50+) Boostern auch auf die Funktionalität dieses Features auswirken wird.
{% endhint %}

## `Entfernen`-Befehl

Mit dem `/verschiedenes boosterkanal entfernen`-Befehl kann die Boosterkanal-Funktion deaktiviert werden. Es können dann keine weiteren Booster-Kanäle mehr eingefordert werden. Bereits erstellte Kanäle bleiben bestehen und werden weiterhin automatisch entfernt, wenn der Nutzer aufhört, den Server zu boosten.
