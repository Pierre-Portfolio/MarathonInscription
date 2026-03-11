# 🏃 MarathonInscription

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-scraping-43B02A?logo=selenium&logoColor=white)
![Status](https://img.shields.io/badge/Statut-Opérationnel-success)
![Year](https://img.shields.io/badge/Année-2026-lightgrey)

> **Surveillance automatique des inscriptions au Marathon de Paris.**  
> Le script scrape le site officiel à intervalle régulier et envoie une notification dès que les inscriptions s'ouvrent — plus besoin de rafraîchir manuellement.

---

## 🎯 Contexte

Les inscriptions au Marathon de Paris ouvrent à une date non communiquée à l'avance et se ferment en quelques heures. Rater la fenêtre d'inscription, c'est rater la course.

Ce projet automatise la veille : un script Python surveille la page d'inscription en continu et alerte immédiatement dès que le bouton d'inscription devient accessible.

---

## ⚙️ Fonctionnement

```
Marathon.py / Marathon.ipynb
        │
        ▼
  Scraping de la page d'inscription
  (Selenium / Requests + BeautifulSoup)
        │
        ▼
  Détection du changement d'état
  (bouton actif / statut ouvert)
        │
        ▼
  Envoi d'une notification
  (email / alerte système)
```

1. **Scraping** — chargement de la page cible à intervalle défini
2. **Détection** — comparaison de l'état du formulaire ou du bouton d'inscription
3. **Notification** — alerte envoyée dès que le statut passe à "ouvert"

---

## 🛠️ Stack technique

| Outil | Usage |
|---|---|
| `Python 3.10` | Langage principal |
| `Selenium` / `Requests` | Scraping de la page web |
| `BeautifulSoup` | Parsing HTML |
| `smtplib` | Envoi de notification par email |
| `time` / `schedule` | Boucle de surveillance |
| `Jupyter Notebook` | Exploration et prototypage |

---

## 🚀 Lancer le script

```bash
# Cloner le repo
git clone https://github.com/Pierre-Portfolio/MarathonInscription.git
cd MarathonInscription

# Installer les dépendances
pip install -r requirements.txt

# Lancer la surveillance
python Marathon.py
```

> 💡 Configurer les paramètres de notification (email, intervalle) directement dans le script avant de le lancer.

---

## 📁 Structure

```
MarathonInscription/
├── Marathon.py          # Script de surveillance autonome
├── Marathon.ipynb       # Notebook d'exploration et de debug
└── README.md
```

---

## 💡 Ce que ce projet démontre

- Automatisation d'une tâche répétitive avec Python
- Scraping web robuste avec gestion des états dynamiques
- Mise en place d'un système d'alerte léger et autonome
- Approche pratique orientée résultat (use case réel)

---

*Pierre Petillion — 2026*
