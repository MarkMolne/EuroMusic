# EuroSongs: Music without Boundaries
#### Aquesta ha estat la meva primera pàgina web creada des de zero mitjançant el llenguatge HTML, CSS i JS.
#### Si vols veure el resultat final fes [click aquí](https://markmolne.github.io/EuroMusic/index.html)


## Els Objectius
   Per a elaborar aquesta pàgina vaig establir uns objectius, que conjuntament amb els que els professors demanaven en les tramesses van estar els següents:
   1. Aprendre a fer servir els llenguatges de HTML, CSS i JS
   2. Entendre el funcionament del GIT, GITHUB i GITCola
   3. Saber elaborar cartografia mitjançant LeafLet
   4. Elaborar un cercador a partir d'una API
   5. Apendre a introduir una cartografia elaborada en QGIS dintre d'una pàgina web


## La temàtica
Se'ns va proposar que la tèmatica de la pàgina web fos lliure, per tant vaig decidir elaborar-la sobre Eurovision ja que és un tema molt fàcil de trobar informació per elaborar la pagina web amb continguts veridics i entretinguts i que alhora permet elaborar cartografia tant a nivell local com europea.


## Les dades
Per tal de obtindre les dades s'han fet servir tres tipus de fonts principals
* Pàgines web relacionades amb Eurovision com poder ser [WiwiBlogs](https://wiwibloggs.com/) o [Eurovision-Spain](https://eurovision-spain.com/).
* Les wikipedies realacionades amb totes les edicions del Festival
* La pàgina web oficial, [Eurovision.tv](https://eurovision.tv/)

La API es va elaborar a partir de la base de dades de [AudioBD](https://www.theaudiodb.com/)


## Metodologia per elaborar la cartografia
Per elaborar la cartografia es van seguir els següents passos:
1. Discriminar, de la capa de paisos europeus, tots aquells que no han participat en el Festival.
2. Realitzar un joint amb les dades de cada pais sobre el nombre de victories i els anys en que van guanyar alhora que una fotografia del representant de cada pais en el 2021.
3. Representar el mapa mitjançant un esquema de colors on el pais amb més victories reb un color daurat, el segons es representat en color plata, el tercer color bronze i la resta juguen amb una escala de blaus.
4. Pel que fa a la capa de punts, que son els indrets on s'ha realitzat el Festival, al no trobar cap capa ja realitzada, es va digitalitzar de manera manual tots els teatres i estadis on s'ha duut a terme.
5. Es va afegir un SVG personalitzat per a representar els punts. 
6. Fer un joint amb les dades que es volien representar
7. Alhora d'exportar es va decidir les dades que es volien representar en el PopUp, una llegenda desplegable on es poden activar o desactivar les diverses capes del mapa i la realització de clusters de punts per a una correcta visualització d'aquestos.

Es pot veure el resultat del mapa final fent [click aquí](https://markmolne.github.io/EuroMusic/winnerchart.html)
