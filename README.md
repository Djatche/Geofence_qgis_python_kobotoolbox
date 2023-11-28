## Améliorer la qualité des données géospatiales avec le « geofencing ». Un exemple avec la collecte d’échantillons pour la surveillance environnementale.

Le geofencing est un outil basé sur la localisation lors de la collecte des données. Il vous aide à savoir dans la bonne zone pour collecter les données. 

Pour ce tutoriel nous avons utilisé les outils suivants :
-	QGIS
-	Kobotoolbox
-	Python et ses libraires pandas et numpy.

Une équipe chargée de la surveillance épidémiologique environnementale doit collecter des échantillons dans des eaux usées. La conception de l'ouitil de geofencing ont suivi les étapes suivantes décrites dans ce tutoriel :
###	Création d’un projet QGIS sous le nom ''geofence_kobo.qgs''.
-	Un shapefile de type polygone a été creé sous le nom ''site_prelevement.shp''. 4 entités ont été digitalisées  Ces 4 entités sont en fait des sites (polygones) de prélèvement prédéfinis. Ce sont les lac municipal et Obili de Yaoundé et deux sites sur le fleuve mbam de part et d’autre du bac de Bioko 1 à Ngambe tikar.
-	Exportation de cette couche sous forme de fichiers csv (‘’site_prelevement_polygons.csv’’)
###	Nettoyage et la manipulation des données de ce fichier à l’aide de pandas et numpy et l’enregistrement sous le nom (‘’preload_polygons.csv’’).
###	Création d’un projet kobotoolbox.
-	Conception du fichier XLSForm ('' XLSForm_site_prelevement)  pour la conception du formulaire de collecte et importation dans le projet kobotoolbox.
-	Importation du fichier csv (‘’preload_polygons.csv’’) comme fichier attaché dans le projet kobotoolbox.
