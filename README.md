# 📊 Application de Pricing CRR – Étude et Interface Graphique

## 🎯 Objectif du projet
Ce projet vise à concevoir une **application interactive** de pricing d’options selon le modèle **Cox-Ross-Rubinstein (CRR)**, intégrant :
- le **calcul du prix théorique** de l’option,
- la **simulation de couverture (Δ-hedging)**,
- la **visualisation graphique** des arbres de prix et des résultats,
- et la **comparaison** entre différentes méthodes de pricing.

Le projet a également pour but de concevoir une **interface graphique complète**, intuitive et professionnelle, afin de rendre les résultats du modèle accessibles, visuels et pédagogiques.

---

## 🧩 Organisation du projet

```

📦 Projet_CRR_Interface/
├── notebooks/
│   └── Etude_comparative_des_solutions_d_interface_pour_application_de_pricing_CRR.ipynb
├── app/
│   ├── Home.py
│   ├── pages/
│   │   ├── 01_Pricing.py
│   │   ├── 02_Hedging.py
│   │   └── 03_Stress_Tests.py
│   └── utils/
│       └── crr_functions.py
├── data/
│   └── exemples_donnees.csv
├── requirements.txt
└── README.md

````

---

## ⚙️ Technologies utilisées

- **Python 3.x**
- **Streamlit** – interface interactive et multipage
- **Plotly / Altair** – visualisations interactives
- **NumPy / Pandas** – calculs et gestion des données
- **GitHub / Streamlit Cloud** – hébergement et diffusion du projet

---

## 🧱 Architecture du projet

| Composant | Description |
|------------|--------------|
| **`notebooks/`** | Contient les notebooks d’analyse et de recherche (dont le comparatif des interfaces). |
| **`app/`** | Code de l’application finale Streamlit, structurée en plusieurs pages. |
| **`app/pages/`** | Pages principales de l’application : Pricing, Δ-Hedging, Stress Tests. |
| **`app/utils/`** | Fonctions métiers : calcul CRR, Δ, Greeks, etc. |
| **`data/`** | Données d’exemple et fichiers de test. |
| **`requirements.txt`** | Liste des dépendances Python nécessaires à l’exécution. |
| **`README.md`** | Documentation principale du projet (ce fichier). |

---

## 🚀 Exécution de l'application

### 1️⃣ Cloner le dépôt
```bash
git clone https://github.com/<ton-nom-utilisateur>/Projet_Interface_CRR.git
cd Projet_Interface_CRR
````

### 2️⃣ Installer les dépendances

```bash
pip install -r requirements.txt
```

### 3️⃣ Lancer l'application Streamlit

```bash
streamlit run app/Home.py
```

---

## 🌐 Déploiement

L’application peut être déployée directement sur **Streamlit Cloud**.

### Étapes de déploiement :

1. Se connecter à [Streamlit Cloud](https://streamlit.io/cloud)
2. Connecter son compte GitHub
3. Sélectionner le dépôt `Projet_Interface_CRR`
4. Choisir le fichier principal : `app/Home.py`
5. Cliquer sur **Deploy**

> L’application sera accessible publiquement via une URL du type :
> 👉 [https://tonprojet.streamlit.app](https://tonprojet.streamlit.app)

---

## 🧠 Étude comparative des interfaces

Le notebook suivant présente une **analyse technique et comparative** des différentes solutions possibles pour l’interface graphique du projet :

[`notebooks/Etude_comparative_des_solutions_d_interface_pour_application_de_pricing_CRR.ipynb`](notebooks/Etude_comparative_des_solutions_d_interface_pour_application_de_pricing_CRR.ipynb)

### Synthèse :

* **Streamlit** : la solution retenue — la plus efficace, simple et professionnelle.
* **Dash** : alternative plus “industrielle”, adaptée à une version produit.
* **Panel / Voilà** : utiles pour des présentations scientifiques.
* **Gradio / Shiny** : bons pour des démos rapides.
* **FastAPI + Streamlit** : option ambitieuse pour une version modulaire (calculs backend séparés).

---

## 🧩 Choix technique retenu

| **Solution retenue**       | **Streamlit (multi-pages)**                                                                                                                                               |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Raisons du choix**       | - Rapidité de développement<br>- Interface moderne et intuitive<br>- Intégration native avec Plotly<br>- Hébergement simple et gratuit<br>- Excellente lisibilité du code |
| **Architecture envisagée** | Streamlit + module Python de calcul (CRR / Monte Carlo / Greeks).<br>Possibilité future d’un backend FastAPI pour les calculs lourds.                                     |
| **Résultat attendu**       | Application fluide, pédagogique et visuellement aboutie, prête à être présentée à un public technique.                                                                    |

---

## 👨‍💻 Équipe projet

**Projet CRR – Interface graphique et pricing d’options**

* **Vincent** — Responsable interface graphique et architecture Streamlit
* *(à compléter pour les autres membres du groupe)*

Encadré par : **[Nom du professeur / encadrant]**

---

## 🧭 Perspectives d’évolution

* Intégration d’un backend **FastAPI** pour déléguer les calculs lourds.
* Ajout d’un module **Black-Scholes** et d’une simulation Monte Carlo complète.
* Fonctionnalités avancées : gestion de portefeuille, calibration de volatilité, analyse de sensibilité.

---

## 📚 Licence et diffusion

Projet académique – École d’ingénieurs / Master Finance
Utilisation libre à des fins pédagogiques et de recherche.

---

## 🏁 Résumé

> Ce dépôt présente une approche complète, rigoureuse et structurée pour la conception d’une **application de pricing d’options (modèle CRR)**.
> L’étude comparative des frameworks a conduit au choix de **Streamlit**, offrant le meilleur compromis entre **simplicité, performance et rendu professionnel**.

```

