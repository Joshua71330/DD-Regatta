# ⛵ DD-Regatta

[![School](https://img.shields.io/badge/ENSTA%20campus%20Brest-Cours%20Drones-002E5D)]()
[![Status](https://img.shields.io/badge/status-en%20cours-yellow)]()

> 🇫🇷 Programmation d'un DD-Boat (véhicule de surface autonome) pour le défi en bassin du cours *Les drones — de la théorie à la navigation* (ENSTA, campus de Brest).
> 🇬🇧 Programming a DD-Boat (autonomous surface vehicle) for the pool challenge of the *Drones — from theory to navigation* course (ENSTA, Brest campus).

**[🇫🇷 Version française](#-français)** · **[🇬🇧 English version](#-english)**

---

## 🇫🇷 Français

### Contexte

Ce dépôt s'inscrit dans le cours **"Les drones — De la théorie à la navigation"** de l'**ENSTA (campus de Brest)**, dispensé par **Luc Jaulin** (31h, 1ère année, à partir de février 2026). Le support utilisé est le **DD-Boat** : un bateau autonome de 80 cm employé depuis plus de 10 ans par la spécialité Robotique sur le lac de Guerlédan.

L'objectif du cours est de concevoir, programmer et rendre autonome ce robot mobile, jusqu'à le faire participer à la **DD-Regatta** : un challenge en bassin, par équipes de 5, où chaque DD-Boat doit naviguer de façon autonome.

### 🎯 Objectif du projet

Développer le logiciel de navigation autonome du DD-Boat, en couvrant :

- **Capteurs** : lecture et **calibration** du GNSS, du magnétomètre et de l'accéléromètre (correction d'ellipsoïde pour le magnétomètre, estimation du cap).
- **Actionneurs** : commande des propulseurs (deux moteurs différentiels).
- **Modélisation** : mise en équations d'état du véhicule.
- **Commande / régulation** : lois de suivi de ligne et d'atteinte de point de passage (*waypoint*).
- **Simulation** : simulateur du système dynamique en Python, utilisable avant les essais réels (y compris via la **Virtual Regatta**, un simulateur Unity développé pour s'entraîner en amont du bassin).
- **Communication temps réel** avec le bateau (wifi / ssh), via la librairie `ddboatlib.py` fournie par le cours.

### 🏁 Jalons du cours (grille d'évaluation)

| Jalon | Contenu | Points |
|---|---|---|
| 1. Simulateur | Simulateur du DD-Boat, téléopération au clavier, génération des données GPS/magnétiques | /2 |
| 2. Trace GPS | Trajet autour de l'école, tracé sur Google Earth | /2 |
| 3. Calibration magnétomètre | Correction d'ellipsoïde, estimation du cap en temps réel | /2 |
| 4. Commande | Loi de commande pour rejoindre un point ou suivre une ligne | /2 |
| DD-Regatta (bassin) | Performance en course, par équipe | /6 |
| Examen sur table (QCM) | Évaluation individuelle des connaissances | /6 |

La **DD-Regatta** elle-même se déroule au grand bassin de l'ENSTA (sessions des 18 et 21 mai), une heure par équipe.


---

## 🇬🇧 English

### Context

This repository is part of the **"Drones — From Theory to Navigation"** course at **ENSTA (Brest campus)**, taught by **Luc Jaulin** (31h, 1st-year students, starting February 2026). The course uses the **DD-Boat**: an 80 cm autonomous surface vehicle used for over 10 years by the Robotics track on Lake Guerlédan.

The course's goal is to design, program, and make this mobile robot autonomous, up to competing in the **DD-Regatta**: a pool challenge, in teams of 5, where each DD-Boat must navigate autonomously.

### 🎯 Project goal

Develop the DD-Boat's autonomous navigation software, covering:

- **Sensors**: reading and **calibrating** the GNSS, magnetometer, and accelerometer (ellipsoid correction for the magnetometer, heading estimation).
- **Actuators**: control of the two differential thrusters.
- **Modeling**: state-space equations of the vehicle.
- **Control**: line-following and waypoint-reaching control laws.
- **Simulation**: a Python simulator of the dynamic system, usable ahead of real trials (including via the **Virtual Regatta**, a Unity-based simulator built for pool-free practice).
- **Real-time communication** with the boat (wifi / ssh), via the course-provided `ddboatlib.py` library.

### 🏁 Course milestones (grading)

| Milestone | Content | Points |
|---|---|---|
| 1. Simulator | DD-Boat simulator, keyboard teleoperation, GPS/magnetic data generation | /2 |
| 2. GPS trace | Route around campus, plotted on Google Earth | /2 |
| 3. Magnetometer calibration | Ellipsoid correction, real-time heading estimate | /2 |
| 4. Control | Control law to reach a point or follow a line | /2 |
| DD-Regatta (pool) | Team race performance | /6 |
| Written exam (multiple choice) | Individual knowledge assessment | /6 |

The **DD-Regatta** itself takes place in ENSTA's main pool (sessions on May 18 and 21), one hour per team.

