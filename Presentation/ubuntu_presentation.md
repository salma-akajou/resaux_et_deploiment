---
marp: true
theme: default
_class: lead
_paginate: false
paginate: true
backgroundColor: #ffffff
style: |
  section {
    font-size: 22px;
    color: #1a1a1a;
    line-height: 1.6;
    padding: 60px 80px;
  }

  footer { 
    width: 100%; 
    text-align: right; 
    font-size: 14px; 
    color: #0B3C5D; 
  }

  .logo-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: absolute;
    top: 20px;   
    left: 40px;
    right: 40px;
  }

  .logo-header img { 
    height: 90px; 
  }

  h1 { 
    color: #0B3C5D; 
    font-size: 2.6em; 
    margin-top: 100px; 
    text-align: left; 
  }

  h2 { 
    color: #0B3C5D; 
    font-size: 2em; 
    border-bottom: 3px solid #0B3C5D; 
    margin-bottom: 30px;
  }

  h3 { 
    color: #123; 
    margin-top: 10px; 
  }

  .sommaire-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin-top: 30px;
  }

  .sommaire-item {
    display: flex;
    align-items: center;
    background: #eaf2f8;
    border-radius: 12px;
    padding: 15px 20px;
    border-left: 6px solid #0B3C5D;
  }

  .sommaire-num {
    background: #0B3C5D; 
    color: white; 
    width: 35px; 
    height: 35px;
    display: flex; 
    justify-content: center; 
    align-items: center;
    border-radius: 50%; 
    font-weight: bold; 
    margin-right: 15px;
  }

  .dt-card {
    background: #f4f9fc;
    padding: 25px;
    border-radius: 12px;
    border-top: 6px solid #0B3C5D;
    margin-top: 20px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
  }

  .tech-container {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 20px;
  }

  .badge-simple {
    padding: 8px 18px;
    border-radius: 6px;
    font-weight: 600;
    background-color: #0B3C5D;
    color: white;
    font-size: 0.85em;
  }

  code {
    background: #1e1e1e;
    color: #f8f8f8;
    padding: 3px 8px;
    border-radius: 6px;
    font-size: 0.9em;
  }
---

<div class="logo-header">
  <img src="images/ofppt-logo.png" alt="Logo Left">
  <img src="images/logo-solicode.png" alt="Logo Right">
</div>

# **Présentation Ubuntu & Linux**
### **Installation d'Ubuntu sur une Machine Virtuelle**

**Réalisée par :** Salma Akagou, Youssra Akagou, Fadna Lakhouchen, Ayoub Jlaita, Yasmine Haddad, Adnane  
**Encadré par :** M. ESSARRAJ Fouad  
**Filière :** Développement Mobile

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

# Sommaire

<div class="sommaire-grid">
<div class="sommaire-item"><div class="sommaire-num">1</div> C’est quoi Linux ?</div>
<div class="sommaire-item"><div class="sommaire-num">2</div> C’est quoi Ubuntu ?</div>
<div class="sommaire-item"><div class="sommaire-num">3</div> La Machine Virtuelle</div>
<div class="sommaire-item"><div class="sommaire-num">4</div> Pourquoi utiliser une VM ?</div>
<div class="sommaire-item"><div class="sommaire-num">5</div> Les prérequis nécessaires</div>
<div class="sommaire-item"><div class="sommaire-num">6</div> Le fichier ISO Ubuntu</div>
<div class="sommaire-item"><div class="sommaire-num">7</div> Passage à la pratique</div>
<div class="sommaire-item"><div class="sommaire-num">8</div> Commandes Linux de base</div>
</div>

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

## 1. C'est quoi Linux ?

<div class="dt-card">

**Linux** est un système d'exploitation libre et open-source.

Contrairement à Windows, Linux n’appartient pas à une seule entreprise et son code source est accessible à tous.

### Pourquoi Linux est important ?

- Gratuit et sans licence payante
- Très sécurisé et stable
- Léger et performant
- Utilisé dans les serveurs, smartphones, cloud et cybersécurité
- Excellent pour apprendre le fonctionnement réel d’un système

</div>

<div class="tech-container">
<span class="badge-simple">Open Source</span>
<span class="badge-simple">Gratuit</span>
<span class="badge-simple">Sécurisé</span>
<span class="badge-simple">Stable</span>
</div>

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

## 2. C'est quoi Ubuntu ?

<div class="dt-card">

**Ubuntu** est l’une des distributions Linux les plus populaires.

Une distribution Linux = Linux + interface graphique + logiciels + gestionnaire de paquets.

Ubuntu est développé par Canonical et il est conçu pour être :

- Simple à utiliser
- Moderne
- Stable
- Idéal pour débutants et développeurs

Ubuntu est aujourd’hui largement utilisé dans les écoles, entreprises et serveurs cloud.

</div>

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

## 3. C'est quoi une Machine Virtuelle ?

<div class="dt-card">

Une **Machine Virtuelle (VM)** est un environnement logiciel qui simule un ordinateur complet à l’intérieur de notre vrai ordinateur.

Elle possède virtuellement :

- processeur
- mémoire RAM
- disque dur
- carte réseau

Le logiciel qui permet cela s'appelle un **Hyperviseur**.

### Exemples d’hyperviseurs :

- VMware → professionnel
- VirtualBox → gratuit et pédagogique

</div>

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

## 4. Pourquoi utiliser une Machine Virtuelle ?

<div class="dt-card">

L’utilisation d’une VM présente plusieurs avantages pédagogiques :

### ✔ Tester sans risque
On peut faire des erreurs sans toucher au vrai PC.

### ✔ Isolation totale
La VM fonctionne dans une boîte fermée.

### ✔ Utiliser plusieurs OS
Windows + Ubuntu sur la même machine.

### ✔ Snapshot
Possibilité de revenir en arrière rapidement.

### ✔ Très utilisé en entreprise
Les administrateurs systèmes travaillent énormément avec des VM.

</div>

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

## 5. Les prérequis nécessaires

<div class="dt-card">

Avant d’installer Ubuntu sur VirtualBox, il faut vérifier :

### 🧠 Mémoire RAM
Au moins 8 Go recommandés.

### 💾 Espace disque
30 Go minimum libre.

### ⚙️ Virtualisation BIOS
Intel VT-x ou AMD-V doit être activé.

### 🖥 Logiciels nécessaires
- VirtualBox installé
- Fichier ISO Ubuntu téléchargé

</div>

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

## 6. C'est quoi un fichier ISO ?

<div class="dt-card">

Un fichier **.iso** est une image disque.

C’est la copie numérique exacte d’un DVD d’installation.

Au lieu de graver Ubuntu sur un CD :

nous donnons simplement ce fichier ISO à VirtualBox qui va le lire comme un lecteur virtuel.

### Exemple utilisé :
`ubuntu-22.04-desktop-amd64.iso`

Taille approximative : 4.7 Go

</div>

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

## 7. Passage à la pratique dans le Lab

<div class="dt-card">

Maintenant que la partie théorique est claire, nous allons passer à la démonstration pratique.

### Étapes du Lab :

1. Télécharger VirtualBox
2. Télécharger Ubuntu ISO
3. Créer la machine virtuelle
4. Configurer RAM et disque
5. Lancer l’installation Ubuntu
6. Créer l’utilisateur
7. Premier démarrage

</div>

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

## 8. Les premières commandes Linux

<div class="dt-card">

Après installation, nous allons utiliser le Terminal Ubuntu.

### Mise à jour du système

`sudo apt update && sudo apt upgrade -y`

### Vérifier l'adresse IP

`ip a`

### Aller dans un dossier

`cd /etc`

### Afficher le contenu

`ls -la`

### Vérifier l'utilisateur courant

`whoami`

</div>

---

<div class="logo-header">
  <img src="images/ofppt-logo.png">
  <img src="images/logo-solicode.png">
</div>

# Conclusion

<div class="dt-card">

À travers cette présentation, nous avons compris :

- ce qu’est Linux,
- pourquoi Ubuntu est utilisé,
- l’intérêt des machines virtuelles,
- les ressources nécessaires,
- et les premières commandes pour commencer.

La prochaine étape est de pratiquer directement sur Ubuntu afin de se familiariser avec l’environnement Linux.

</div>

# Merci pour votre attention