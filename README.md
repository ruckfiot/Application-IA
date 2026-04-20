#  Classifieur de Genres Musicaux (Track C - GTZAN)

Ce projet propose une interface intelligente permettant de classifier automatiquement le genre d'un extrait musical en utilisant plusieurs approches d'Intelligence Artificielle. Développé dans le cadre du module Track C, il compare l'efficacité du Machine Learning classique (Random Forest) face au Deep Learning (CNN & Transfer Learning).

##  Démo Live (Gradio)
L'application est accessible en ligne via le lien suivant :
 **[Accéder à l'interface Gradio](https://6de1a78107f32fa5d1.gradio.live)**
*(Note : Le lien est temporaire et hébergé via Google Colab Pro).*

---

## 📊 Comparaison des Modèles & Performance

Nous avons testé trois approches différentes pour identifier le genre musical parmi 10 classes (Rock, Jazz, Metal, Pop, etc.) :

| Modèle | Accuracy | Définition Technique du Score |
| :--- | :--- | :--- |
| **Random Forest (Champion)** | **87.00%** | Mesure de la corrélation statistique entre les signatures fréquentielles (MFCC) et les genres musicaux. |
| **CNN from scratch** | **55.22%** | Capacité d'extraction de motifs visuels sur spectrogrammes bruts sans pré-entraînement. |
| **Transfer Learning (HuBERT)** | **71.00%** | Efficacité de la réutilisation de connaissances acoustiques apprises sur la parole humaine vers la musique. |

**Gain total de performance : +31.78 points** (Indice de supériorité de l'ingénierie des caractéristiques sur l'apprentissage brut sur petit dataset).

---

## 🔍 Analyses de Cas Réels (Insights)

L'interface a été testée sur des morceaux iconiques pour évaluer sa robustesse :

* **In the End (Linkin Park) :** Le modèle détecte la nature hybride du morceau en hésitant intelligemment entre **Pop (23%)** et **Hiphop (21%)**, captant à la fois la mélodie et le flow.
* **Seven Nation Army (The White Stripes) :** Une "erreur intelligente" où le riff percutant est interprété comme du **Hiphop (42%)** à cause de la structure rythmique très marquée sur le spectrogramme.
* **Stayin' Alive (Bee Gees) :** Une hésitation historique entre **Pop** et **Disco**, illustrant la proximité spectrale de ces genres dans les années 70.

---

## 🛠️ Technologies Utilisées
* **Langage :** Python 🐍
* **Audio :** Librosa (Extraction MFCC, Chroma, Spectral Contrast)
* **Modèles :** Scikit-learn (Random Forest), PyTorch (CNN), Hugging Face (DistilHuBERT)
* **Interface :** Gradio
* **Hardware :** Entraîné sur Google Colab Pro avec GPU NVIDIA T4/G4.

---

## 👨‍💻 Auteur
Projet réalisé par **BERNA Valentin et BEN OLIEL Hugo** dans le cadre du module d'Application de l'IA.
