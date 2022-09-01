# Les bons liens et les bons tuto
Les bons liens et les bons tutos toujours utile à avoir sous la main

## Carte utile ou cool :
- Une carte des fruits ramassable dans des vergers à l'abandon et des poubelles de super-marché qui sont visitable pour glaner de la bouffe afin de changer de façon de consommer. La carte est consultable [ici]( https://fallingfruit.org/)
- Parce que le site de téléchargement des données de l'IGn n'est pas des plus claire, la communauté de géotribu à mis en place cet outil de téléchargement. Par contre il repose toujours sur les serveurs FTP de l'IGN. La carte est [ici](https://geotribu.github.io/ign-fr-opendata-download-ui/index.html), et plus bas les informations de connexion des FTP de l'IGN
- La carte des lieux de naissances de personnes connues. Une carte divertissante disponible [ici](https://tjukanovt.github.io/notable-people)

## Blog et Site :
- Des tutos et des formations SIG, parfois gratuite [ici](https://spatialthoughts.com/)

## Arts de la mise en page et autre beauté cartographique
### Création de carte :
- Sortir de jolie carte rapidement pour de l'illustration avec [PrettyMap](https://chrieke-prettymapp-streamlit-prettymappapp-1k0qxh.streamlitapp.com/~/+/#prettymapp)
### Outils :
- Bien choisir ses couleurs, un guide pratique [ici](https://blog.datawrapper.de/beautifulcolors/index.html)
### Styles et templates :
- Bibliothèque de style QGIS créer par Klas Karlsson diponible [ici](https://style-hub.github.io/#)
- Dépôt d'icônes SVG pour QGIS [ici](https://www.svgrepo.com/)

## Tuto et documentation langages :
### Langage de programation
- PLPgSQL : Tout l'art de faire des fonctions pour PostGIS (Oui je sais PostGIS n'est qu'une extension, mais à quoi bon utiliser une BDD sans référence spatiale). De bon conseil se trouve [ici](https://public.dalibo.com/exports/formation/manuels/modules/p1/p1.handout.html)
- SQL Postgre : GitGood chez [CrunchyData](https://www.crunchydata.com/developers/tutorials)
- Batch (oui on parle du Shell de windows) : Une bonne documentation pour s'amuser a faire des script sur son PC est [ici](https://initscreen.developpez.com/tutoriels/batch/apprendre-la-programmation-de-script-batch/)
### Windows :
- Installation de GDAL sous Windows parce que l'installation fourni par QGIS est trop pourri pour servir à autre chose qu'à QGIS. Tout est expliquez chez [Geotribu](https://static.geotribu.fr/articles/2013/art_2013-09-26/)
- Un Cron sous Windows pour programmez des tâches répétitves, un [tuto](https://moreabout.tech/creating-cron-jobs-in-windows-10-and-windows-server-2016/)
- Générer des script pour le futur package manager de windows et ainsi faire des re-installations de windows plus vitement les détails [ici](https://winstall.app/)
### Autres :
- QGIS en ligne de commande chez [SpatialThoughts](https://spatialthoughts.com/2022/07/30/qgis_process_command_line/)

## Source :
### Donées
- Accès à des données Open Data de L'IGN : La connexion à un ftp étant crade, l’identifiant et le mot de passe sont écris en claire dans l’adresse envoyé au serveur selon le format : ftp://identifiant:mdp@hote
 - FTP OrthoHR libre (  Hote : ftp://ftp3.ign.fr - Identifiant : ORTHO_HR_ext - Mot de passe : Ithacah6ophai2vo)
 - FTP BD Carto libre (  Hote : ftp://ftp3.ign.fr - Identifiant : BD_CARTO_ext - Mot de passe : Oor4el8aeM3io0Ji)
 - FTP BD ALTI libre (  Hote : ftp://ftp3.ign.fr  - Identifiant : BD_ALTI_ext - Mot de passe : docoazeecoosh1Ai)
 - FTP RGE Alti libre (Hote : ftp://ftp3.ign.fr - Identifiant : RGE_ALTI_ext - Mot de passe : Thae5eerohsei8ve) 
- Données Soilgrids : La pédologie c'est [ici](https://files.isric.org/soilgrids)
- Données de Mars :
 - Altimétrique : ftp://pdsimage2.wr.usgs.gov/pub/pigpen/mars/mola/DEM_global_megt128ppd_merged64ppd/
 - Données général de Mars : ftp://pdsimage2.wr.usgs.gov/pub/pigpen/mars/
Logiciel est autre chose
### Logiciels
- GDAL en installeur msi (windows) en téléchagement [ici](https://www.gisinternals.com/index.html)