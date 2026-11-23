# Dictionnaire de données — `data/releves.csv`

| Colonne | Type | Obligatoire | Règle | Exemple |
|---------|------|-------------|-------|---------|
| `ID` | texte | oui | Identifiant unique, format `E8-XX` | `E8-01` |
| `Groupe` | liste | oui | algues, mousses, fougères, gymnospermes, graminées, dicotylédones | `Mousses` |
| `Espece` | texte | non | Nom scientifique si connu, sinon `Inconnue` | `Polypodiacées` |
| `Statut` | liste | oui | Trouvé / Non trouvé / À vérifier | `Trouvé` |
| `Longitude` | décimal | oui | Degrés décimaux, 6 décimales, négatif à l'ouest | `-5.225756` |
| `Latitude` | décimal | oui | Degrés décimaux, 6 décimales, positif au nord | `6.890899` |
| `Precision_m` | décimal | oui | Précision GNSS (m) | `8` |
| `Date_heure` | date | oui | `AAAA-MM-JJ HH:MM:SS` | `2026-11-21 11:01:22` |
| `Observateur` | texte | oui | Nom de l'apprenant | `VIEGNEKOU KOFFI BOGAR` |
| `Remarque` | texte | non | Appareil végétatif/reproducteur, état | `...` |
| `Milieu` | texte | oui | Milieu d'observation | `ombre, tronc` |
| `Photo_1` | texte | oui | Chemin relatif vers la photo principale | `photos/E8-01_1.jpg` |
| `Photo_2` | texte | non | Photo secondaire | `photos/E8-01_2.jpg` |
| `Photo_3` | texte | non | Photo tertiaire | `photos/E8-01_3.jpg` |

## Systèmes de référence
- **Collecte** : WGS 84 — `EPSG:4326`
- **Analyse** : UTM 30 N — `EPSG:32630`
- **Règle** : degrés décimaux, point comme séparateur

## Règle d'or
Un identifiant unique (`ID`) relie point GPS + photo(s) + échantillon.