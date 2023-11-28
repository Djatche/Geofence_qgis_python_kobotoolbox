## Améliorer la qualité des données géospatiales avec le « geofencing ». Un exemple avec la collecte d’échantillons pour la surveillance environnementale.

Le geofencing est un outil basé sur la localisation lors de la collecte des données. Il vous aide à savoir si vous êtes dans la bonne zone pour collecter les données. 

Pour ce tutoriel nous avons utilisé les outils suivants :
-	QGIS
-	Kobotoolbox
-	Python et ses libraires pandas et numpy.                                                                     

Une équipe chargée de la surveillance épidémiologique environnementale doit collecter des échantillons dans des eaux usées. Elle doit se rassurer que les prélèvements se feront dans le site (polygone) préalablement définit.  La conception de l'outil de geofencing a suivi les étapes suivantes décrites dans ce tutoriel :
###	Création d’un projet QGIS sous le nom "geofence_kobo.qgs".
-	Un shapefile de type polygone a été creé sous le nom "site_prelevement.shp" avec deux champs "id" et "nom" de type texte. Quatre (4) entités ont été digitalisées  Ces 4 entités sont en fait des sites (polygones) de prélèvement prédéfinis. Ce sont les lacs municipal et Obili de Yaoundé et deux sites sur le fleuve mbam de part et d’autre du bac de Bioko 1 à Ngambe tikar.
-	Exportation de cette couche sous forme de fichiers csv ("site_prelevement_polygons.csv")
###	Création d'un fichier jupyter notebook "geofence_polygons.ipynb"    
- Le nettoyage et la manipulation des données de ce fichier à l’aide de pandas et numpy ainsi que sa sauvegarde sous le nom ("preload_polygons.csv"). Tout le script se trouve dans le fichier jupyter notebook.     
###	Création d’un projet kobotoolbox.
-	Importation du fichier csv ("preload_polygons.csv") comme fichier attaché dans le projet kobotoolbox.
-	Création du fichier XLSForm au nom de ("XLSForm_site_prelevement")  pour la conception du formulaire de collecte et son importation dans le projet kobotoolbox.Les fonction PULL DATA, BEGIN REPEAT, END REPEAT, repeat_count ont été particulièrement utiles.                                  

Ce tutoriel nous a été fortement inspiré de celui de "Humanitarian Data Solutions". Le nettoyage et la manipulation des données ont été faites par les librairies pandas et numpy de python dans jupyter notebook en lieu et place de Power Bi.             
il est disponiple ici https://www.youtube.com/watch?v=yg26PLctcEQ
