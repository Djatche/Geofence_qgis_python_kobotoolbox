# Améliorer la qualité des données géospatiales avec le « geofencing ». Un exemple avec la collecte d’échantillons pour la surveillance environnementale.

Le geofencing est un outil basé sur la localisation lors de la collecte des données. Il vous aide à savoir dans la bonne zone pour collecter les données. 

Pour ce tutoriel nous avons utilisé les outils suivants :
-	QGIS
-	Kobotoolbox
-	Python et ses libraires pandas et numpy.
Une équipe chargée de la surveillance épidémiologique environnementale doit collecter des échantillons dans des eaux usées. Les étapes du tutoriel ont été les suivantes :
-	Création d’un projet QGIS
-	Un shapefile de type polygone a été réalisé. 4 entités ont été digitalisées  Ces 4 entités sont en fait des sites (polygones) de prélèvement prédéfinis. Ce sont le lac municipal de Yaoundé, le lac d’Obili de Yaoundé et deux sites sur le fleuve mbam de part et d’autre du bac de Bioko 1 à Ngambe tikar.
-	Exportation de cette couche sous forme de fichiers csv (‘’site_prelevement_polygons.csv’’)
-	Nettoyage des données avec python.
-	Le nettoyage et la manipulation des données de ce fichier à l’aide de pandas et numpy et l’enregistrer sous le nom (‘’preload_polygons.csv’’).
-	Création d’un projet kobotoolbox.
-	Conception du fichier XLSForm ()  pour la conception du formulaire de collecte et importation dans le projet kobotoolbox.
-	Importation du fichier csv (‘’preload_polygons.csv’’) dans le projet kobotoolbox.
