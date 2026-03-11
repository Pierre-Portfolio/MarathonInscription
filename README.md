<h1 align="center">
  <img src="./assets/images/github/header.png" alt="SIMarathon Inscription" />
</h1>
<img src="./assets/images/github/star.gif" alt="star" />

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Selenium-scraping-43B02A?logo=selenium&logoColor=white" />
  <img src="https://img.shields.io/badge/Statut-Opérationnel-success" />
  <img src="https://img.shields.io/badge/Année-2026-lightgrey" />
</p>

---

# MarathonInscription – Surveillance automatique des inscriptions

## Aperçu
Script Python qui scrape le site officiel du Marathon de Paris et envoie une notification dès que les inscriptions s'ouvrent — plus besoin de surveiller manuellement une page qui ne change pas.

## Objectifs
- Automatiser la veille d'une page web à état variable.
- Détecter en temps réel l'ouverture des inscriptions.
- Envoyer une alerte immédiate par notification.
- Démontrer une automatisation Python concrète sur un cas réel.

## Technologies
- Python
- Selenium / Requests
- BeautifulSoup
- smtplib (notifications email)

## Fonctionnement

```
Scraping de la page  →  Détection du changement d'état  →  Envoi de la notification
```

1. Le script charge la page d'inscription à intervalle régulier
2. Il compare l'état du bouton / formulaire d'inscription
3. Dès que le statut passe à "ouvert", une alerte est envoyée

## Lancer le script
```bash
git clone https://github.com/Pierre-Portfolio/MarathonInscription.git
cd MarathonInscription
pip install -r requirements.txt
python Marathon.py
```

## Auteur
- [Pierre Petillion](https://github.com/Pierre-Portfolio/)

---

<p align="center">Projet réalisé en 2026.</p>
