# AYA BERDAY — Portfolio cybersécurité

Version de revue, non publiée. Site statique sans dépendance externe, sans traceur et sans formulaire transmettant des données. HTML / CSS / JavaScript. Introduction en perspective CSS 3D sur fond SOC fourni : il ne s’agit pas d’un modèle 3D WebGL navigable.

## Consulter
Ouvrir index.html dans un navigateur, ou lancer `python -m http.server 8000` depuis ce dossier. Les pages projet fonctionnent directement et les liens sont relatifs. L’introduction est jouée une fois par onglet ; le bouton de la page permet de la rejouer. Escape et « Passer » ferment l’introduction. Les préférences reduced-motion sont respectées.

## Contenu
15 fiches dédiées sous projets/. projects.json contient les données structurées sources. Les pages HTML sont pré-générées pour une lecture sans JavaScript et un hébergement simple. En cas de modification manuelle, mettre à jour les données ET la page concernée. Les fichiers HTML sont directement modifiables. Le comportement immersif est dans cyber.js ; les filtres et l’introduction dans app.js.

## Déploiement — après validation
### GitHub Pages
Créer un dépôt, ajouter le contenu de ce dossier à sa racine. Dans Settings → Pages, choisir Deploy from a branch, main, / (root). Aucun build requis. `.nojekyll` est fourni. Aucun secret n’est nécessaire.
### Vercel
Importer le dépôt, choisir Other, ne pas définir de commande de build et choisir `.` comme répertoire de sortie. vercel.json configure les chemins statiques. Le domaine final dépend du projet créé.

## Périmètre et points à compléter
Le prototype V2 en HTML/ZIP n’était pas joint : reconstruction à partir du dossier texte, de l’image SOC, du CV et des rapports disponibles. Le stage bancaire est un laboratoire, jamais une mise en production. Le SOAR complet est un lot collaboratif distinct. Zero Trust est un plan de projet non déployé. Aucun indicateur ni lien de dépôt projet n’a été fabriqué.

À compléter : preuves de certifications et liens de vérification ; architecture VPN et DMZ / contribution personnelle ; sujets forensic et IA ; données et résultats ML ; rapport RSA ; détails cabinet dentaire ; année et filière du baccalauréat ; captures pipeline et scans. Les rapports complets ne sont pas exposés en téléchargement, le CV l’est. Vérifier les informations personnelles avant toute publication publique.

Le dossier fourni et les rapports ont servi au contenu ; les catégories de compétences ne sont pas des scores de maîtrise. Formations CS50 et React indiquées en cours. L’image de référence contient du texte décoratif ; seules les mentions HTML sont les informations du portfolio.

## Version immersive V3
Globe de particules Canvas animé, trajectoires synthétiques, alertes mobiles à durée limitée et nombre borné, séquence SOC de 10,5 secondes et apparition de l’identité. Bouton de pause des alertes, contrôle des animations et respect de prefers-reduced-motion. Les vidéos fournies sont des inspirations, non intégrées comme des réalisations personnelles. L’environnement reste un décor en perspective CSS, sans modèle WebGL. Aucun stroboscope.

## V4 — bureau vidéo et interface de commandement
L’ordinateur de l’intro est désormais celui de la vidéo MOV fournie par Aya. Une version MP4 muette de 8,7 secondes est incluse localement ; aucun lecteur externe. La vidéo est une référence visuelle, pas un travail 3D réalisé par Aya. Confirmer les droits de diffusion de cette référence avant publication publique. L’introduction est rejouable, accessible via un dialogue, et désactivée en réduction des animations. Les fenêtres sont simulées par le site ; les textes inclus dans le métrage appartiennent à la référence.
La séquence conserve le cadrage vertical de la vidéo pour afficher tout le bureau. Sur écran large, deux consoles et un fond sombre occupent les côtés. Aucun faux ordinateur CSS ne subsiste. Le décor réaliste provient du métrage : ce n’est pas un modèle 3D interactif.
Après l’introduction : rail de navigation avec suivi de section, navigation basse mobile, progression de lecture, léger mouvement du décor au pointeur, cartes à relief réactif, panneaux flottants, ruban animé et transitions au défilement. Le contenu des quinze projets reste conservé. Les comportements pointeur sont réservés à la souris et désactivés en mode de réduction des animations.
Vérifications effectuées : syntaxe des scripts, liens de fichiers locaux, présence des quinze pages projet, lecture de la vidéo par FFmpeg. Aucun test visuel dans un navigateur n’a pu être effectué dans cet environnement. Aucune publication.

## V4.1 — corrections après captures
Le fond de maquette a été supprimé de l’accueil : il est remplacé par un décor CSS original (grille, halos et anneaux), sans texte ni boutons dessinés. La hauteur de l’accueil suit désormais son contenu pour éviter de couper le panneau d’événements. Typographie du nom unifiée en sans-serif. Alertes d’accueil déplacées vers le haut à droite sur ordinateur. Cadrage vidéo ajusté selon le format de l’écran, consoles plus discrètes et surimpression fixe qui masquait l’écran retirée. La source reste verticale : le cadrage varie selon la largeur pour conserver un ordinateur visible. Aucun nouveau décor horizontal original n’est revendiqué. Vérifications statiques uniquement, sans contrôle navigateur.

## V4.2 — études de cas documentées
Les trois fiches SOC Wazuh, DevSecOps et supervision comprennent désormais des architectures fonctionnelles en HTML, des tableaux de scénarios/contrôles/mesures et des bilans avec limites. Sources : rapports fournis, références de chapitres dans chaque fiche. Les diagrammes sont des synthèses, pas des captures de déploiement. Aucun dépôt GitHub ajouté et aucune capture fabriquée. Les captures techniques originales restent à sélectionner et intégrer après vérification de leur lisibilité et de leur périmètre.

## V4.3 — certificat Oracle
Certificat fourni intégré en PDF : intitulé exact Oracle Cloud Infrastructure Certified Architect Associate, obtenu le 3 septembre 2026, valable jusqu’au 3 septembre 2028. Justificatif consultable dans la section Certifications. Aucun lien de vérification externe inventé. Les autres certifications restent déclarées dans le dossier, sans justificatif joint. Données Oracle disponibles dans certifications.json.

## V4.4 — cinq justificatifs supplémentaires
Captures originales ajoutées pour les deux formations CrossKnowledge (19 mai 2026), Interactivity with JavaScript (18 novembre 2024), Introduction à la programmation orientée objet en C++ et The Unix Workbench (14 décembre 2024). Titres et dates repris des captures. Les identifiants Coursera correspondent aux captures. Les cinq pages externes n’ont pas pu être consultées par l’outil : aucun contrôle en ligne réussi n’est revendiqué. Les deux liens CrossKnowledge sont regroupés sans attribution individuelle non vérifiée. Les images s’ouvrent dans un nouvel onglet ; seuls les visuels de certificats fournis sont exposés.
