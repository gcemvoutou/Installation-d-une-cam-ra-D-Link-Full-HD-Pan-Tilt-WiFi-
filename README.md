# Compte Rendu : Installation et Configuration d'une Caméra IP

**Auteur :** Clara EMVOUTOU  
**Date :** 27 Février 2026  
**Contexte :** Mission de configuration d'une solution de vidéosurveillance pour un client.

---

## 📋 Sommaire

1. [Présentation du Matériel](#1-présentation-du-matériel)
2. [Procédure d'Installation](#2-procédure-dinstallation)
3. [Analyse des Modes de Connexion](#3-analyse-des-modes-de-connexion)
4. [Exploration de l'Interface et Fonctionnalités](#4-exploration-de-linterface-et-fonctionnalités)
5. [Bilan et Critique Professionnelle](#5-bilan-et-critique-professionnelle)
6. [Configuration Réseau : Le protocole DHCP](#6-configuration-réseau--le-protocole-dhcp)

---

## 1. Présentation du Matériel
Le matériel utilisé pour cette intervention est une caméra **D-Link DCS-8525LH**.
Voici à quoi elle ressemble :
<img src="camera_modèle.png" width="300" alt="Ma caméra D-Link">

### Caractéristiques principales :
* **Résolution :** Full HD (1080p).
* **Mobilité :** Motorisée avec fonctions Pan & Tilt (panoramique et inclinaison).
* **Connectivité :** Wi-Fi/Ethernet.

### Contenu du pack :
* Caméra et bloc d'alimentation.
* Câble réseau (RJ45).
* Support de fixation, vis et chevilles.
* Guide d'installation rapide avec QR Code.

---

## 2. Procédure d'Installation

### Prérequis techniques
* Un réseau Wi-Fi fonctionnel.
* Un smartphone avec l'application **mydlink** installée.
* Un compte utilisateur mydlink créé et configuré.
  <br>
  <img src="interface_mydlink.png" width="300" alt="Interface D-Link">
  > [!NOTE]
> **Interface de connexion :** Une fois le compte mydlink configuré


### Étapes de mise en service
1. **Installation physique :** Choix de l'emplacement et branchement de l'alimentation électrique.
2. **Réinitialisation :** Utilisation d'un trombone dans l'orifice "Reset" situé à l'arrière de la caméra pendant 10 secondes pour détacher l'appareil d'un ancien compte.
3. **Appairage logiciel :** * Ouverture de l'application et sélection de "Ajouter un appareil".
    * Scan du QR Code présent sur l'étiquette ou la carte d'installation.
    * Configuration de la liaison réseau (choix du Wi-Fi pour ce TP).

---

## 3. Analyse des Modes de Connexion
L'analyse comparative des deux modes de configuration disponibles :

| Mode | Avantages | Inconvénients |
| :--- | :--- | :--- |
| **Ethernet** | Connexion ultra-stable, latence minimale, meilleure sécurité (accès physique requis). | Nécessite de tirer un câble, moins flexible pour le placement. |
| **Wi-Fi** | Installation rapide sans câble, grande flexibilité de placement. | Sensible aux interférences, à la distance et aux obstacles (murs). |

---

## 4. Exploration de l'Interface et Fonctionnalités
L'application **mydlink** centralise la gestion de la caméra via une interface intuitive :

* **Flux en direct :** Visualisation immédiate et accès aux contrôles **Pan & Tilt** (joystick virtuel pour orienter l'objectif).
* **Gestion des Scènes :** Configuration de modes (Maison, Absent, Sommeil) pour activer ou désactiver les alertes en un clic.
* **Automatisation :** Programmation de détections de mouvements ou de sons avec envoi de notifications push.
* **Calendrier :** Consultation des séquences enregistrées sur le Cloud sécurisé ou sur la carte MicroSD locale.


> **Interface de connexion :** Une fois le compte mydlink configuré, l'accès à la caméra est centralisé et sécurisé, permettant une consultation à distance via 4G/5G.

---

## 5. Bilan et Critique Professionnelle

### Points positifs
L'installation est particulièrement simple grâce au guidage pas à pas de l'application. L'interface est fluide, rendant la surveillance accessible même pour un utilisateur non-technicien.

### Limites techniques identifiées
1. **Stabilité réseau :** En mode Wi-Fi, la qualité dépend de la portée du signal. Un répéteur peut être nécessaire pour les grandes distances.
2. **Sécurité :** L'Ethernet est recommandé pour une installation fixe afin d'éviter le risque de brouillage du signal Wi-Fi.
3. **Usage :** Ce modèle DCS-8525LH est strictement réservé à un usage intérieur .

---

## 6. Configuration Réseau Avancée

### 6.1 Le protocole DHCP
La caméra a été configurée par défaut en **DHCP** (*Dynamic Host Configuration Protocol*).
* **Fonctionnement :** Le routeur attribue automatiquement une adresse IP libre à la caméra dès sa connexion.
* **Identification :** L'adresse IP a été retrouvée en faisant correspondre l'adresse MAC (physique) de l'appareil via la table ARP du réseau.
