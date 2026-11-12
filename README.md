# CartoFisc
CartoFisc France est une application web cartographique destinée à visualiser des périmètres liés à trois dispositifs d’exonérations fiscales et sociales :
- ZFU-TE : Zones franches urbaines – Territoires entrepreneurs (dispositif historique) ;
- BER : Bassins d’emploi à redynamiser ;
- ZRD : Zones de restructuration de la défense.
Elle permet de rechercher une adresse ou de sélectionner un point sur la carte afin de vérifier si celui-ci se trouve dans l’un des périmètres géographiques chargés.
Fonctionnalités principales
- Recherche d’adresse : recherche par adresse ou commune, avec propositions de résultats.
- Géolocalisation : utilisation de la position de l’utilisateur si le navigateur autorise l’accès à la localisation.
- Vérification sur la carte : clic direct sur la carte ou recherche d’un lieu pour obtenir un diagnostic géographique.
- Affichage des zones : visualisation indépendante des couches ZFU-TE, BER et ZRD, avec possibilité de les afficher ou de les masquer.
- Périmètres proches : signalement des zones répertoriées situées à moins de 10 km du point sélectionné.
- Fiches dispositifs : consultation d’un résumé des règles fiscales et sociales, des conditions présentées dans l’application, de la période de validité et des références juridiques.
- Import GeoJSON : chargement manuel des données d’une couche à partir d’un fichier .geojson ou .json.
- Diagnostic des données : affichage du nombre de périmètres chargés, de leur source et du statut de chargement.
- Fonds de carte : choix entre le Plan IGN, un fond clair et une photographie aérienne IGN.
- Navigation géographique : accès rapide à la métropole, à la Guadeloupe, à la Martinique, à la Guyane et à La Réunion.
- Réglage de l’opacité : adaptation de la transparence des zones affichées.
- Thème clair/sombre : changement manuel du thème de l’interface.
Utilisation rapide
1. Ouvrir le fichier HTML dans un navigateur récent.
2. Attendre le chargement des couches géographiques et vérifier leur statut dans le panneau latéral.
3. Saisir une adresse ou une commune, puis sélectionner une proposition. Il est également possible de cliquer directement sur la carte.
4. Lire le diagnostic : périmètre détecté, dispositifs correspondants et éventuelles zones proches.
5. Ouvrir la fiche complète d’un dispositif pour consulter les informations fiscales, sociales et les références indiquées.
6. Utiliser les filtres pour afficher ou masquer les couches, ou importer un GeoJSON si les données distantes ne sont pas disponibles.
Données et fonctionnement
L’application tente de charger les données géographiques depuis des sources distantes. Elle utilise également un cache enregistré dans le stockage local du navigateur. Si les flux distants ne répondent pas, des données de secours intégrées au code sont prévues.

Les données GeoJSON doivent contenir des géométries de type Polygon ou MultiPolygon. Pour importer un fichier, utiliser le bouton « MAJ GeoJSON » correspondant à la couche concernée.

Les fonds de carte, la recherche d’adresse et certaines données nécessitent une connexion Internet. L’application s’appuie notamment sur Leaflet, les services IGN/Géoportail, l’API Adresse et des référentiels géographiques publics.
Limites et précautions
- Le diagnostic est géographique et informatif : la présence d’un établissement dans un périmètre ne suffit pas, à elle seule, à confirmer son éligibilité à une exonération.
- Les conditions propres à l’entreprise, à l’activité, à la date d’implantation, aux salariés et aux plafonds doivent être vérifiées au regard des textes applicables.
- Les données de secours intégrées au fichier sont limitées : les polygones ZFU-TE embarqués sont explicitement des exemples et les codes ZRD de secours sont présentés comme des exemples. Ils ne constituent donc pas une couverture exhaustive.
- En cas d’échec de chargement, de couverture partielle ou de doute sur un périmètre, importer un GeoJSON officiel à jour et contrôler la source et la date affichées.
- Les résumés réglementaires intégrés à l’application doivent être vérifiés auprès des textes officiels avant toute décision fiscale ou sociale.
CartoFisc France est un outil d’aide au repérage et non un avis juridique, fiscal ou social.
