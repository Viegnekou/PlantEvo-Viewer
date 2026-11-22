# PlantEvo-Viewer

Site web statique racontant l'évolution des végétaux (de l'eau à la terre), réalisé dans le cadre du Brief 01 - Digital Farming School.

## Technologies utilisées
- HTML5 (balises sémantiques)
- CSS3 (Flexbox, Grid, Responsive Design)
- Aucun framework (conforme aux consignes)

## Structure du projet

PlantEvo-Viewer/
│
├── index.html                
├── algues.html                 
├── mousses.html                
├── fougeres.html               
├── coniferes.html              
├── graminees.html              
├── dicotyledones.html          
│
├── css/
│   └── style.css             
│
├── images/                    
│   ├── algues.jpg
│   ├── algues2.jpg
│   ├── mousses.jpg
│   ├── mousses2.jpg
│   ├── fougeres.jpg
│   ├── fougeres2.jpg
│   ├── coniferes.jpg
│   ├── coniferes2.jpg
│   ├── GraminéAppareil.png
│   ├── hero-foret.jpg
│   ├── carte-repartition.svg  
│   │
│   └── galerie/                
│       ├── Logo.png
│       ├── Page de garde.png
│       ├── Dico Appareil.png
│       ├── Dicotyledone.png
│       ├── ImageGraminé.png
│       ├── photo-1.jpg
│       ├── photo-2.jpg
│       ├── photo-3.jpg
│       ├── ... (jusqu'à photo-8.jpg)

├── docs/                       
│   ├── maquette-figma.png   
│   └── rapport-sig.pdf         
│
└── README.md   
                
- `index.html` : Page d'accueil avec le menu et la galerie.
- `algues.html`, `mousses.html`, `fougeres.html`, `coniferes.html`, `graminees.html`, `dicotyledones.html` : Les 6 pages groupes.
- `css/style.css` : Feuille de style unique.
- `images/` : Photos de terrain et carte SVG.

## Données SIG
La carte de répartition a été générée avec QGIS.
- **Projection** : WGS 84 / EPSG:4326
- **Fond de carte** : OpenStreetMap
- **Auteur** : VIEKNEKOU Koffi Bogar

##  Auteur
- VIEKNEKOU Koffi Bogar
- Digital Farming School - 2026