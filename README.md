# Forensics et Analyse de Vulnérabilités (FAV)

[← Tous les cours de MaletYon](https://github.com/maletyon) · [Livre (PDF)](FAV_main.pdf) · [Présentations](Présentation/) · [Fiches par chapitre](fiches/) · [Corrigés](correction/README.md)

**UE MSN-2S3-SEC07** · Master Professionnel en Sécurité des Systèmes Numériques · Semestre 3
Chaire UNESCO d'Afrique Centrale ACCES-TIC, sous la tutelle académique de l'École Nationale Supérieure Polytechnique de l'Université de Yaoundé I
Auteur : MINKA MI NGUIDJOÏ Thierry Emmanuel, enseignant-chercheur (LIMSI, ENSPY) · contact : maletyon@proton.me · année académique 2026-2027

> *Expliquer l'incident, empêcher le suivant : de la trace à la correction vérifiée.*

L'investigation numérique explique un incident ; l'analyse de vulnérabilités empêche le suivant. Le cours enseigne les deux dans une même démarche : recueillir et préserver la preuve, examiner un disque, une mémoire et une capture réseau, bâtir une chronologie, puis remonter de la trace à la faille qui a permis l'attaque, la coter, la prioriser et vérifier sa correction. Chaque conclusion sépare la constatation de l'analyse et reçoit une cote OUI / NON / NEK ; l'incertitude d'une enquête se mesure par μ, U et H, selon le programme de l'auditologie. Le cours s'appuie sur les normes ISO/IEC 27037 à 27043, le NIST SP 800-86, CVSS v4.0, EPSS, le catalogue KEV et la loi camerounaise n° 2010/012. Deux cas forment le fil rouge : NYANGA CRÉDIT (Bafoussam) et SOLITRANS LOGISTIQUE (Douala). L'exploitation des failles n'y est pas enseignée : elle relève de l'UE MSN-2S3-SEC03.

## Ce que contient ce dépôt

| Élément | Où | Description |
|---|---|---|
| Le livre du cours | [`FAV_main.pdf`](FAV_main.pdf) | Traité complet (prologue, 16 chapitres, annexes), compilé depuis [`FAV_main.tex`](FAV_main.tex) |
| Les présentations | [`Présentation/`](Présentation/) | 16 présentations PowerPoint : vision d'ensemble et 15 séances de 2 heures, avec notes du présentateur |
| Les fiches d'exercices | [`fiches/`](fiches/) | 17 fiches de 40 questions au format texte, à distribuer en attendant l'ouverture de NDAP SUKULU |
| Le livret de correction | [`correction/`](correction/) | Accès réservé : voir la page du dossier |
| Les sources LaTeX | `front/`, `partie0/` à `partie6/`, `annexes/`, `bibliographie/`, `figures/`, [`Style_FAV.sty`](Style_FAV.sty) | Sources du livre |

## Organisation du cours (30 heures, 15 séances de 2 heures)

Les 30 heures sont consacrées au cours magistral. Les travaux dirigés (fiches, exercices de fin de chapitre) et les travaux pratiques (dix laboratoires) se font à la maison, sur NDAP SUKULU.

| Partie | Chapitres | Fichiers |
|---|---|---|
| **Prologue** | 0. La nuit du 14 mars à Bafoussam | [`partie0/`](partie0/) |
| **I. Fondements** | 1. L'investigation numérique · 2. La preuve numérique et la chaîne de possession | [`partie1/`](partie1/) |
| **II. Méthode : examiner les supports** | 3. Acquérir et préserver · 4. L'analyse du disque · 5. L'analyse de la mémoire · 6. L'analyse du réseau · 7. Chronologie et corrélation | [`partie2/`](partie2/) |
| **III. Cadre normatif et juridique** | 8. Normes et droit de l'investigation | [`partie3/`](partie3/) |
| **IV. Pratique : les vulnérabilités** | 9. Qu'est-ce qu'une vulnérabilité · 10. Identifier les vulnérabilités sans les exploiter · 11. Gérer les vulnérabilités · 12. De l'artefact à la vulnérabilité | [`partie4/`](partie4/) |
| **V. Défis avancés** | 13. Anti-forensique, nuage et conteneurs · 14. L'enquête intégratrice · 15. Le rapport et le témoignage | [`partie5/`](partie5/) |
| **VI. Recherche** | 16. Mesurer l'incertitude d'une enquête | [`partie6/`](partie6/) |
| **Annexes** | A. Glossaire · B. Outils · C. Modèles de documents · D. Textes et normes · E. Bibliographie commentée · F. Contacts | [`annexes/`](annexes/) |

## NDAP SUKULU, la salle de classe compagnon

*Ndap sukulu* signifie « la salle de classe » en bassa, et *Malet Yon* « ton enseignant ». NDAP SUKULU est l'environnement d'évaluation du cours : une fiche de 20 questions tirées d'une banque de 100 par chapitre, et dix laboratoires pratiques, minutés et en nombre de tentatives limité. Le code de cours est **MSN-2S3-SEC07**. La présentation complète figure au début du livre.

| Utilisation | Où |
|---|---|
| En ligne | `https://maletyon.github.io/cours-fav/ndap-sukulu/` |
| Sur un ordinateur, sans Internet | archive téléchargeable dans [`ndap-sukulu/`](ndap-sukulu/) |
| Sur un téléphone (fiches seulement) | `https://maletyon.github.io/cours-fav/ndap-sukulu/telephone/` |
| Si votre réseau bloque `github.io` | adresse de secours `https://raw.githack.com/MaletYon/cours-fav/main/ndap-sukulu/`, ou [archive à télécharger](https://github.com/MaletYon/cours-fav/raw/main/ndap-sukulu/NDAP_SUKULU_FAV_ordinateur.zip) pour travailler hors ligne |

La connexion se fait avec le matricule et le mot de passe remis par l'enseignant. Les copies sont remises à l'enseignant sous forme d'un fichier chiffré ; il les corrige et publie les résultats, que chacun consulte dans l'application. Le mode d'emploi complet, pour l'étudiant et pour l'enseignant, est dans [`ndap-sukulu/README.md`](ndap-sukulu/README.md). Les fiches de 40 questions au format texte restent disponibles dans [`fiches/`](fiches/).

| Lab | Sujet | Chapitre |
|---|---|---|
| FAV-LAB-01 | Chaîne de possession et scellés | 2 |
| FAV-LAB-02 | Duplication et hachage | 3 |
| FAV-LAB-03 | Disque : système de fichiers et artefacts | 4 |
| FAV-LAB-04 | Mémoire : processus et connexions | 5 |
| FAV-LAB-05 | Réseau : l'exfiltration | 6 |
| FAV-LAB-06 | Chronologie unifiée | 7 |
| FAV-LAB-07 | Lire un résultat de balayage | 10 |
| FAV-LAB-08 | Coter : CVSS v4.0, EPSS, KEV | 9 |
| FAV-LAB-09 | Prioriser et suivre la remédiation | 11 |
| FAV-LAB-10 | Enquête intégratrice | 12, 14 |

## Sources de recherche

Le cours s'appuie sur deux prépublications de l'auteur, déposées sur HAL : *Vers l'auditologie* (`hal-05701007`) et *Modelling Epistemic Uncertainty in IS Audit* (`hal-05701270`). Les autres travaux cités comme « en préparation » ne sont pas encore publiés.

## Compiler le livre

Avec une distribution LaTeX : `pdflatex FAV_main`, `biber FAV_main`, `makeindex FAV_main`, puis deux fois `pdflatex FAV_main`.
Les présentations se régénèrent avec `python Présentation/_sources/run.py FAV all` (Python 3 et python-pptx).

## Normes et documents sous licence

Les normes ISO et les autres documents sous licence cités dans le cours **ne sont pas fournis** dans ce dépôt. Les noms d'organisations, de personnes, les adresses et les montants des cas sont fictifs ; les adresses IP appartiennent aux plages réservées à la documentation.

## Licence

Contenu pédagogique : [CC BY-NC-SA 4.0](LICENSE.md). Code du générateur de présentations : MIT. Voir [`LICENSE.md`](LICENSE.md).
