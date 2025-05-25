# MontOrganise_Microgrid


# MontOrganise_Microgrid

Ce dépôt contient les fichiers de simulation associés à une étude de faisabilité d’un micro-réseau hybride photovoltaïque pour la commune de Mont-Organisé, Haïti. Le projet s’inscrit dans le cadre d’un travail de recherche doctorale réalisé entre l’Université de Liège et l’Université d’État d’Haïti.

## 📁 Contenu

- **Demand_simulation_RAMP.ipynb** : Script Jupyter de génération des profils de charge à l’aide de l’outil RAMP (Residential Appliance Modeling Platform).
- **PV_Simulation_TMY_MontOrganise.py** : Script Python basé sur PVlib pour simuler la production photovoltaïque horaire à partir d’un fichier météo TMY.
- **TMY3_Haiti_NSRDB.csv** : Données climatiques horaires sur un an (fichier TMY) issues de la base de données NSRDB.
- **Demand.csv** : Données agrégées de demande énergétique simulée sur 8760 heures.
- **RES_Time_Series.csv** : Série temporelle de la production photovoltaïque simulée sur 8760 heures.
- **Slide_Projet_NRJ_Trans.pdf** : Présentation synthétique du projet pour diffusion académique.

## ⚙️ Méthodologie

1. **Demande** : Simulation à l’aide de RAMP pour générer les profils de charge représentatifs de différentes catégories de consommateurs (ménages, institutions, services…).
2. **Production PV** : Utilisation du modèle PVWatts avec température cellule estimée par le modèle NOCT, et irradiance sur plan inclinée via le modèle isotropique.
3. **Couplage** : Les courbes issues de la demande et de la production sont ensuite utilisées pour dimensionner un système hybride optimisé (à l’aide de MicroGridsPy ou autre outil).

## 🔧 Outils utilisés

- `Python` (version ≥ 3.9)
- `PVlib` (modélisation photovoltaïque)
- `RAMP` (modélisation de la demande électrique)
- `pandas`, `numpy`, `matplotlib`…

## 👤 Auteur

Jean-Claude Lysias Orelus  
Doctorant en physique de l’énergie solaire photovoltaïque  
Université de Liège & Université d’État d’Haïti

## 📝 Licence

Ce projet est partagé à titre académique et ne comporte pas encore de licence. Veuillez contacter l’auteur pour toute réutilisation.
