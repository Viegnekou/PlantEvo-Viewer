# 🗺️ Rapport SIG — Positions des espèces observées

**Auteure** : VIEGNEKOU KOFFI BOGAR
**Outil** : QGIS [version]

## 1. Objectif
Cartographier les 6 points GPS et produire une carte intégrable au site.

## 2. Systèmes de référence
| Usage | EPSG |
|-------|------|
| Collecte | 4326 (WGS 84) |
| Analyse | 32630 (UTM 30 N) |

## 3. Données
Voir `data/releves.csv` (6 points E8-01 → E8-06).

## 4. Contrôle qualité
- Degrés décimaux, point séparateur ✅
- Latitude +, longitude − ✅
- Précision : 4 à 8 m (⚠️ E8-01 à 8 m > seuil 5 m)
- 1 ID unique par point ✅

## 5. Cartographie QGIS
1. Ajouter couche texte délimité → `releves.csv` (séparateur `;`)
2. X = Longitude, Y = Latitude, CRS = 4326
3. Reprojeter en 32630
4. Symbologie par groupe
5. Étiquettes `ID`
6. Fond OSM
7. Composeur de cartes → export PNG
8. Intégrer `images/carte_releves.png` au site

## 6. Intégration HTML
```html
<figure>
  <img src="images/carte_releves.png" alt="Carte des positions GPS">
  <figcaption>Carte des relevés E8-01 à E8-06</figcaption>
</figure>