---
description: >-
  Cuelist Sequencer est un composant (COMP) générique pour TouchDesigner, conçu
  pour organiser et déclencher une séquence de « cues » (états mémorisés) de
  manière ordonnée.
---

# Cuelist sequencer

{% file src="../.gitbook/assets/cuelist_sequencer.tox" %}

## Instructions

### Installation

Glisser la composante cuelist\_sequencer.tox dans votre projet touchdesigner. Aucune installation supplémentaire est nécéssaire.

### Configuration

#### 1. Création du Master Component

La première étape consiste à désigner un Master Operator. Ce composant (un `COMP base`) constitue la scène principaleet le moteur logique de votre projet.

Chaque Cue créée dans le séquenceur représente une modification d'état ou une variation spécifique de cette scène. Le système enregistre les paramètres du Master pour chaque étape afin de générer des transitions fluides entre elles.

Prérequis des sorties (Outputs) : Pour transmettre les données au reste de votre réseau TouchDesigner, votre Master Component doit impérativement inclure des opérateurs de sortie parmi les types suivants :

* TOP&#x20;
* CHOP
* SOP
* POP
* DAT&#x20;

Le Cuelist sequencer expose automatiquement ces mêmes types de sorties sur ses propres connecteurs, reflétant ainsi le contenu de votre scène en temps réel.

{% hint style="danger" %}
Définissez l'ensemble de vos sorties (TOP, CHOP, SOP, POP, DAT) avant l'assignation du Master Component à la Cuelist. Une fois le composant lié et en cours d'utilisation, la configuration des types et du nombre de sorties devient fixe pour garantir la stabilité du flux de données.
{% endhint %}

<figure><img src="../.gitbook/assets/ezgif-60b9c77a113b27ac.gif" alt=""><figcaption></figcaption></figure>



