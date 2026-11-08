# Portfolio Aya BERDAY — V7

Version statique HTML, CSS et JavaScript, issue de la V6.2. Aucun npm install ni build requis. Cette livraison n'a pas été publiée automatiquement.

## Ouvrir le portfolio

Extraire le ZIP, ouvrir le dossier contenant index.html dans VS Code, puis lancer dans son terminal :

```sh
python -m http.server 8000
```

Ouvrir http://localhost:8000. Sous Windows, `py -m http.server 8000` fonctionne aussi si Python est installé via le lanceur py. Arrêter avec Ctrl+C.

## Changements V7

- 23 fiches : ajout des labs TryHackMe 04 Nmap et 05 Nmap Basic Port Scans, Cloud Security, CYBERNOVA et OSINT.
- Réécriture enrichie des fiches Forensic, IA et RSA à partir des comptes rendus disponibles.
- Statuts visibles, recherche textuelle et filtres catégorie/avancement combinables.
- Statut « À documenter » distinct : un manque de preuves ne signifie pas automatiquement « en cours ».
- Détails des démarches, résultats, sources et limites ; sommaire dans les nouvelles études de cas.
- Métadonnées canonical, Open Graph et Twitter sur les 24 pages.
- Conservation du portrait, des certifications, du CV, des contacts, des animations et du mode recruteur.
- Menu mobile ajouté aux fiches détaillées.

## Audit de la base

La base fournie est un site statique français (pas React/Vite, pas de système FR/EN existant). index.html porte les cartes et les sections ; projets/ contient les fiches ; projects.json fournit un catalogue miroir. Les scripts app.js, motion.js, cyber.js, v5.js et v6.js pilotent les interactions existantes. v7.js combine recherche et filtres ; v7.css ajoute les styles correspondants. Les liens utilisent des chemins relatifs.

Le CV fourni dans V6.2 est conservé octet pour octet. Aucun parcours professionnel n'a été reconstruit à partir d'informations extérieures au site.

## Sources et prudence éditoriale

| Sujet | Source exploitée | Qualification |
| --- | --- | --- |
| Nmap 04/05 | Fiches transmises par Aya | Réalisé selon compte rendu ; captures non jointes |
| Cloud | Compte rendu TP Cloud Sécurité, version (1) | TP réalisé ; SSRF théorique et IAM non revendiqué comme réalisé |
| Forensic | Rapport TP3 Digital Forensics | Récupération ciblée EXT4 ; comparaison NTFS limitée |
| CYBERNOVA | Compte rendu Aya / Ayman | Plan de mission et analyse académique ; pas audit de production |
| OSINT | Dossier collectif du 14/10/2026 | Synthèse anonymisée ; rapport brut exclu |
| IA | Compte rendu TD/TP IA cybersécurité | Régression sur données synthétiques |
| RSA | Compte rendu comparatif Fermat/Pollard | Petits modules pédagogiques ; pas cassage de RSA moderne |
| Notes Oracle / CrossKnowledge | Consignes pédagogiques | Ne prouvent pas une certification obtenue |

Les documents bruts de 5CIIR ne sont pas inclus. Pas de clés privées, de cartographie OSINT nominative, ni de faux screenshot. Les anciennes fiches sans nouvelle preuve sont conservées ; aucun nouveau résultat SOC/DevSecOps n'a été inventé. Le statut Réalisé porte sur le périmètre décrit, parfois un livrable de conception et non une implémentation.

## Vérifications effectuées

- Syntaxe des 6 fichiers JavaScript : node --check, sans erreur.
- 24 pages HTML ; 554 références locales (fichiers et ancres), sans cible manquante.
- 23 cartes et 23 entrées du catalogue, mêmes identifiants.
- CV identique à la base.
- Navigateur desktop : accueil et recherche Nmap observés ; combinaison Nmap + Étudié affiche aucun résultat, puis retour à tous les statuts affiche 3 projets.
- Un compteur hérité « Tous 18 » a été corrigé en « Tous 23 ».
- Contrôle mobile navigateur non finalisé : reprise du navigateur bloquée. CSS responsive présent, à recetter sur un vrai téléphone.
- Pas de test sur appareils réels, pas de validation automatique WCAG exhaustive et pas de vérification en ligne de chaque lien externe.
- Aucun scan de sécurité réel n'a été lancé par le site ou pour sa validation.

## Preuves à compléter

1. Captures de complétion des cinq rooms TryHackMe et sorties Nmap anonymisées.
2. Extraits Cloud / Forensic / IA / RSA relus et anonymisés avant mise en ligne.
3. Pour VPN, DMZ et énergie : contexte, configuration réellement réalisée et résultats.
4. Pour les contrôles CYBERNOVA : valider les dénominateurs, exceptions et exports avant toute conclusion définitive.
5. Recette sur téléphone : menu, tableaux défilants, CV, filtres, carrousel, mode recruteur et réduction des mouvements.

## Mise à jour GitHub Pages

Garder le dépôt existant. Sauvegarder sa version actuelle, puis remplacer les fichiers du site par le CONTENU du ZIP à la racine configurée pour Pages (index.html doit rester à ce niveau). Ne pas téléverser le ZIP comme page. Commit puis attendre le déploiement GitHub Pages. Conserver la configuration existante de domaine. Pour un hébergement sous un sous-chemin différent, ajuster les URL canonical/OG avant publication.

Cette livraison contient .nojekyll et conserve vercel.json. L'hébergement Vercel peut servir ce projet statique sans compilation, selon la configuration du projet existant.
