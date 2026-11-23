# Documentation technique — PlantEvo Viewer

**Projet** : Brief 01 — Digital Farming School
**Auteure** : VIEGNEKOU Koffi Bogar
**Date** : 16–23 novembre 2026

## 1. Contexte et objectif
Site statique pour une exposition sur l'agriculture. Présente l'évolution
de l'appareil végétatif et des modes de reproduction de 6 groupes :
Algues → Mousses → Fougères → Gymnospermes → Graminées → Dicotylédones.

## 2. Environnement de travail
| Élément | Choix |
|---------|-------|
| Éditeur | Visual Studio Code |
| Versionnement | Git + GitHub |
| Maquettage | Figma |

## 3. Maquettage (C2N1)
Prototype Figma : [lien](https://www.figma.com/proto/h0WmQ5x4TfDukXe8zusdwk/VIEGNEKOU-Figma?page-id=0%3A1%3Fnode-id%3D62-235&p=f&viewport=140%2C131%2C0.09&t=fS6ZLEK8NcdKYnWL-1&scaling=min-zoom&content-scaling=fixed&node-id=1-2)

## 4. Architecture
Voir l'arborescence détaillée dans le `README.md` :
index.html, pages/ (6 fiches), css/style.css, images/, data/releves.csv,
js/ (facultatif), docs/.

## 5. Navigation (2 niveaux)
Accueil → ancre `#cartes` → 6 cartes → pages → retour au menu.

## 6. Balises sémantiques
`header`, `nav`, `main`, `section`, `figure`, `figcaption`, `footer`, `aside`.

## 7. CSS
- Variables `:root` (couleurs, espacements, polices)
- Grid (6 → 3 → 1 colonnes)
- Media queries 900 px / 600 px
- Un seul fichier CSS commenté

## 8. Responsive
| Écran | Cartes | Grille |
|-------|--------|--------|
| > 900 px | 6 | 3 |
| 600–900 px | 3 | 1 |
| < 600 px | 2 | 1 |

## 9. Fonctionnalités
- Menu statique 6 liens
- Retour au menu
- Ratio 80/20 (contenu/illustration)
- Images avec `alt` + `<figcaption>`
- Relevés GPS (`data/releves.csv`)

## 10. Optimisation des images
Redimensionnement 1200 px max, JPEG q80 ou WebP, poids < 200 ko.
Outil : https://squoosh.app/

## 11. Contenu agronomique (AG1/AG6)
Fil rouge : sortir de l'eau = 4 problèmes résolus
(soutien, dessiccation, reproduction hors eau, transport).

## 12. Données SIG (SIGTD1)
WGS 84 (collecte, EPSG:4326) / UTM 30 N (analyse, EPSG:32630).
Voir `dictionnaire_donnees.md`.

## 13. Tests
Navigation, responsive, `alt`, liens : OK.

## 14. Compétences couvertes
CIN1, C2N1, C3N1, AG1, AG6, SIGTD1.

## 15. Améliorations possibles
Carte `<map>`, schémas SVG, galerie photos, filtre par groupe.