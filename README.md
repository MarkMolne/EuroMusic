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


## Metogologia per a l'elaboració de la pàgina web
Alhora de crear la pagina web es va seguir la següent metodologia:

0. _Passos previs_ : Elaborar una layout en brut per a l'organització de les pàgines i quantes d'hauran de crear. Retallar imatges amb el mateix format i organitzar un esquema de colors. També es va crear un logo per a la pagina.
1. _Creació de la pàgina principal_ : 
   1. Creació del document HTML
   2. Elaboració del Head
   3. Inserció del Body amb el Banner, on hi trobem el logo, i la barra de navegació on es troben els       botons per anar a la resta de seccions de la web
   4. Creació de dues columnes, la de l'esquerra amb la presentació de la pàgina web i una descripció del Festival, i la de la dreta amb les ultimes noticies. Tenen una miga del 60% i 35% respectivament
   5. Elaboració d'un footer que serà comú en totes les pàgines
2. _Creació del CSS_ :
Mentre es creava la pàgina principal, es va elaborar també de manera paral·lela l'arxiu CSS que dona estil a tota la pàgina web. Es van introduir els estils de tots els diferents elements del HTML per a que coincidicin en estil totes les pàgines, com per exemple la mida de la lletra dels diferents apartats, la font de lletra, el tamany de les capceleres, la justificació del text, etc...
3. _Elaboració de la pagina de noticies_:
Seguint l'estructura de totes les pàgines trobem una pagina de noticies amb una columna principal amb la redacció de noticies amb un titol, subtítol, imatge i redacció, i a la dreta un time-line de twitter amb un recopilatori de tuits sobre Eurovision. Acaba amb un footer.
4. _Elaboració de la pagina del TOP12_:
En aquesta pàgina ens trobem dues columnes d'igual mida amb 12 divisions que representen el meu top12 de cançons d'Eurovisión i dintre de cada divisió hi ha el títol de la cançó, el representatn i l'any, una explicació del perqué de la posició i un iframe d'Spotify que dona opció de escoltar 30 segons de la cançó. Al igual que les altres, acaba amb el footer.
5. _Elaboració d'un mapa amb LeafLet_:
Aquesta pàgina mostra un mapa elaborat amb llenguatge JS i realitzat a través de LeafLet amb un total de 49 punts que mostren les 49 arenes on s'ha fet el Festival, posteriorment aquest mapa ha estat millorat tal i com es pot veure en l'apartat de _Metodologia per elaborar la cartografia_. 
6. _Realització del about me_:
L'ultima pàgina, igual que la resta compta amb un banner i una barra de navegació. Compta amd dues columnes, una de principal amb una presentació personal i la justificació del projecte i a la columna dreta enllaços a les meves xarxes socials, una fotografia personal i un formulari per a posar-se en contacte en mi.


## Metodologia en l'elaboració del motor de cerca amb una API
Tal i com s'ha dit anteriorment, aquest motor de cerca està vinculat amb la base de dades de [AudioBD](https://www.theaudiodb.com/) el qual ens proporciona informació sobre diverses caracteristiques dels cantants o grups del que es realitza una busqueda. 
En aquest cas s'ha creat una pàgina nova d'html i js i s'ha introduit la taula en format html i el JSON que proveia la API. 
A partir d'un fetch s'ha indicat que es mostri certa informació cada cop que es busca l'artista, en aquest cas es mostra el nom, l'any de neixament de la carrera musical, el pais, el genere musical i la discografia.
Tot queda tancat amb el mateix footer que la resta de pagines.



## Metodologia per elaborar la cartografia
Per elaborar la cartografia es van seguir els següents passos:
1. Discriminar, de la capa de paisos europeus, tots aquells que no han participat en el Festival.
2. Realitzar un joint amb les dades de cada pais sobre el nombre de victories i els anys en que van guanyar alhora que una fotografia del representant de cada pais en el 2021.
3. Representar el mapa mitjançant un esquema de colors on el pais amb més victories reb un color daurat, el segons es representat en color plata, el tercer color bronze i la resta juguen amb una escala de blaus.
4. Pel que fa a la capa de punts, que son els indrets on s'ha realitzat el Festival, al no trobar cap capa ja realitzada, es va digitalitzar de manera manual tots els teatres i estadis on s'ha duut a terme.
5. Es va afegir un SVG personalitzat per a representar els punts. 
6. Fer un joint amb les dades que es volien representar
7. Alhora d'exportar es va decidir les dades que es volien representar en el PopUp, una llegenda desplegable on es poden activar o desactivar les diverses capes del mapa i la realització de clusters de punts per a una correcta visualització d'aquestos.

Totes aquestes tasques s'han elaborat a patir del programari de QGIS amb el complement de QGIS2WEB el qual ens ajudava a exportar el mapa i vincular-lo amb un iframe al html de la pagina dessitjada. 
Alhora de penjaro al repositori l'unic canvi que s'ha realitzat ha estat la substitució del enllaç local pel del repositori que consta amb el nom_de_la_carpeta/nom_de_arxiu.html

Es pot veure el resultat del mapa final fent [click aquí](https://markmolne.github.io/EuroMusic/winnerchart.html)

## Conclusions del treball i fets a millorar de la pàgina web
Elaborar aquesta pàgina web ha estat un repte personal el qual ha suposat molt de esforç en la busqueda de material per a poder completar la pàgina web completa. El més complicat va ser començar des de 0 l'inici de la pàgina però alhora es satisfactori veure com poc a poc pren la forma que desitjes. 
Un fet a millorar ha de ser el responsive de certes seccions de la web, i igual actualitzar una mica el disseny a que sigui més "modern". Encara així resto molt satisfet de la feina realitzada.

