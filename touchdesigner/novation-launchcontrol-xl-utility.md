---
description: >-
  Composant TouchDesigner simplifie le processus de mappage MIDI pour le
  Novation LaunchControl XL.
---

# Novation Launchcontrol XL Utility

{% file src="../.gitbook/assets/Novation_LaunchControlXL_Utility.tox" %}

## Équipements

Cette composante a été testé avec le _Novation LaunchControl MK2._ Le mappage des contrôles peut être adapté pour les autres versions du contrôleur.

{% embed url="https://novationmusic.com/products/launch-control-xl-mk" %}

## Configuration

#### 1. Installation

Glisser la composante Novation\_LaunchControlXL\_Utility.tox dans votre projet touchdesigner. Aucune installation supplémentaire est nécéssaire.

#### 2. Création et mappage

{% columns %}
{% column %}
Un seul mappage est actif par défaut. Utilisez les symboles + / - dans Controls pour modifier ce nombre.
{% endcolumn %}

{% column %}
<figure><img src="../.gitbook/assets/ezgif-43622c97ebee1cdc.gif" alt=""><figcaption></figcaption></figure>


{% endcolumn %}
{% endcolumns %}



{% columns %}
{% column %}
<figure><img src="../.gitbook/assets/Capture d’écran, le 2026-02-18 à 09.55.31.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
**RENAME:** Modifier le nom de l'assignation du canal pour cette piste.

**CHANNEL:** Choisissez la piste (colonne verticale) de votre contrôleur MIDI que vous souhaitez assigner.

**TYPE:** Choisissez le type de contrôle (potentiomètre ou fader) à assigner.

**RANGE**: Configurez l'amplitude (min/max) de la plage de données pour ce canal.

**BEHAVIOUR**: Définissez l'action du bouton ou du fader de votre contrôleur.&#x20;

* Default: Comportement standard (impulsion).&#x20;
* Toggle: Permet d'utiliser le bouton comme un interrupteur (On/Off).&#x20;
* Count: Incrémente une valeur à chaque pression du bouton (selon la plage définie).
{% endcolumn %}
{% endcolumns %}



