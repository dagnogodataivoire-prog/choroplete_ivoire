# Choroplèthe Côte d'Ivoire

Génération de cartes choroplèthes pour la Côte d'Ivoire à partir de fichiers CSV.

Description

Ce projet permet de créer des cartes choroplèthes pour la Côte d'Ivoire, avec plusieurs options de sortie :

* PNG haute résolution (600 DPI)

* SVG vectoriel

* HTML interactif avec Folium

*** Il est particulièrement utile pour visualiser des données statistiques par districts, régions, départements ou sous-préfectures ***


# Auteur

Dramane Dagnogo – dagnogo.data.ivoire@gmail.com

# Organisation : Data Ivoire

# Licence

Ce projet est libre et open-source.

# Dépendances

Python 3.x

pandas

geopandas

matplotlib

folium

requests

# Installation rapide via pip :

pip install pandas geopandas matplotlib folium requests
Installation

# Cloner le dépôt :

git clone https://github.com/ton-utilisateur/choropleth-cote-ivoire.git
cd choropleth-cote-ivoire

Placer votre fichier CSV dans le dossier du projet.

Le fichier doit contenir une colonne correspondant aux régions ou subdivisions et une colonne de valeurs à visualiser.

# Utilisation

Exemple simple pour générer une carte choroplèthe par région :

from choropleth import plot_choropleth1

plot_choropleth1(
    data_path="data.csv",
    element="region",        # options : CIV, district, region, departement, sous_prefecture
    data_column="Valeur",    # colonne du CSV à visualiser
    cmap="Purples",          # palette de couleurs matplotlib
    output_basename="ma_carte"
)

* NB: il ya d'autres arguments, fais "help(plot_choropleth1)" pour voir toutes les options.



# Contact

Pour toute question ou suggestion : dagnogo.data.ivoire@gmail.com
