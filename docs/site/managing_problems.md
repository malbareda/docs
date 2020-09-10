Aquesta pàgina et guiarà a l'hora de Crear i Afegir nous problemes.


# Crear nous problemes

## Categoria

Pensa en la Categoria que vols posar al problema. 

Primers passos es per problemes que es puguin resoldre sense bucles (per tant, han de tenir casos de prova individuals!). 
Iniciació per problemes molt senzills que no tinguin cap estructura de dades, com arrays.
Aprenentatge és si el problema es pot resoldre amb relativament poques linies, va d'un sol concepte, i la dificultat del problema està més en l'implementació que no en pensar el que s'ha de fer. Aprenentatge poden ser casos molt bàsics (invertir una string) o força complexes (implementar Dijkstra). Sempre que es compleixin aquestes condicions. Aprenentatge seria el típic exercici de 2-3p a un examen.
Competitius son problemes que podrien estar en un concurs. Tenen un enunciat, s'ha d'interpretar, s'ha de pensar, s'ha de resoldre, poden haver-hi més d'un concepte, etc. La dificultat pot ser molt variable.

No feu servir la resta de les categories. Especialment no feu servir la categoria Negra sense consultar-ho amb l'admin (Marc) abans

## Punts

Decidir els punts del problema és una de les parts més dificils de fer el problema. Mira problemes similars en dificultat al teu i posa uns punts equivalents. La majoria de problemes tindran entre 3 i 15 punts. Pensa molt detingudament si vas a posar més de 15 punts a un problema. 


## Nombre de casos de Prova

Idealment un problema hauria de tenir uns 15-20 casos de prova força exhaustius, dels quals uns 3-5 haurien de ser públics (i per tant penjats a l'enunciat) i la resta privats. Haurien d'estar dividits en un mínim de 2 parelles d'arxius entrada/sortida, un per als casos públics i un per als casos privats. Idealment s'hauria de tenir una parella per als públics, i després una altra per cada 10 casos privats. Si es fan casos amb molts casos de prova (més de 10.000) no s'hauria de fer servir la retroacció per no col·lapsar el jutge ni les pantalles dels docents que mirin enviaments al problema.

## Format dels casos de Prova

El jutge bàsicament el que fa es canviar l'entrada i sortida estandard del problema amb fitxers i executar, i després comparar el fitxer de sortida amb el fitxer de respostes esperades. Això fa que realment el jutge NO sap quina entrada es correspón a cada sortida. Per tal de que ho sàpiga (i per tant, pugui informar a l'usuari de quina entrada té malament) s'han de fer els problemes amb un format especial.

Formats acceptats:

### Estàndard

una línea d'entrada es correspón a una línea de sortida. Per tant, els casos de prova tindran n línies de sortida i n o n+1 línies d'entrada. el +1 es degut a que la majoria de problemes solen tenir una primera linea que indica quants casos hi ha.

Aquest cas el tracta el jutge automàticament i no cal fer res

Un exemple seria https://joder.ga/problem/compteambelveri  (1 entrada / 1 sortida)  

### Relació fixa

n línees d'entrada es correspón a m línees de sortida, sent n i m valors fixos i un dels dos sent 1. Per exemple, cada cas son sempre 2 linees d'entrada i 1 de sortida, o 5 i 1, o 1 i 4. També es te en consideració el +1 per la primera linea que indica quants casos hi ha.

No funciona si tant l'entrada com la sortida son més d'una línea. si son 4 linies cada entrada i 2 cada sortida el programa no té forma de saber si son 4-2 o 2-1. Com a consell intenteu que la sortida sigui sempre una línea, excepte en exercicis de matrius.

Aquest cas el tracta el jutge automàticament i no cal fer res

Un exemple seria https://joder.ga/problem/colarse (3 entrades / 1 sortida)

### STOP al final

És exactament igual que l'estàndard o la relació fixa, pero en comptes de tenir una linea al principi que indica quants casos hi ha, hi ha una al final amb una entrada ja acordada que indica que s'acaba l'execució i no s'ha de processar

Aquest cas s'ha d'indicar a l'hora de penjar els casos de prova!

Un exemple seria https://joder.ga/problem/7segments

### Cada cas té linies indicades

És un problema que segueix la seguent casuística.
"El primer nombre n indica el nombre de casos. Després hi haura n casos. En cada cas, el primer nombre, k, indica les linies que hi ha. Després hi haura k línies detallant el cas." La sortida SEMPRE es d'una sola linea.

Aquest cas s'ha d'indicar a l'hora de penjar els casos de prova!

Un exemple seria https://joder.ga/problem/pozoluna (molt clar)  o https://joder.ga/problem/torniquet (hi ha 2 números a la línea pero el que val per al sistema d'ajuda és el primer) o https://joder.ga/problem/buscamines (aquest és de matrius i bàsicament m'obliga a crear el número L per al sistema d'ajuda)

### Cas individual

Quan el problema no segueix cap dels casos anteriors, es pot fer cada cas individual. En aquest sentit, cada cas seria un fitxer d'entrada/sortida diferent. 
Aquest cas s'ha d'indicar a l'hora de penjar els casos de prova!

Un exemple seria https://joder.ga/problem/barrethogwarts (és un problema massa introductori per tenir bucle d'entrada i s'ha de fer en casos anteriors) https://joder.ga/problem/blackfriday (els exercicis de matrius solen donar problemes) o https://joder.ga/problem/consellescolar (els problemes a on el nombre de línies de la sortida es variable sempre son casos irregulars)

### Cas Irregular

Quan el problema no segueix cap dels casos anteriors

**NO pots activar el sistema d'ajuda en un cas Irregular, i ha de tenir un Checker sense retroacció (generalment el de només profes)**

# Afegir un Problema
ves a [dmoj.ca/admin](https://dmoj.ca/admin), i fes servir les teves credencials.
Aleshores, fes click al botó _Add_ en el menú _Problems_ 

![](http://i.imgur.com/RFPQaUi.png)

Això obrirà l'editor de problemes. Fes servir un codi (únic per a cada problema) i un títol per al problema. **AFEGEIX-TE COM A AUTOR O NO PODRAS EDITAR EL PROBLEMA**

![](http://i.imgur.com/bPlNZUR.png)

Aquí pots fer l'enunciat del problema. El jutge fa servir Markdown amb Latex. Tens un exemple de problema estàndard [aqui](https://github.com/malbareda/docs/blob/master/sample_files/problema_aireacondicionat.md.txt) i tens un template que mostra totes les opcions del Markdown [aqui](https://raw.githubusercontent.com/DMOJ/docs/master/sample_files/problem_markdown_example.md.txt).

En el 95% de problemes copiar l'estàndard i canviar el text i l'imatge serà més que suficient.

Hi ha moltes opcions per a configurar el teu problema. Parlem de les més importants

Publicy Visible: True
Manually Managed: False (si no el jutge no funcionaria!)
Problem Types: Els que creguis convenients. Un com a mínim. No afegeixis tipus nous
Problem Categories: El que s'ha dit a la part de categories
Allows Partial Points: True (si es fa servir la retroacció)
Time Limit: No més de 5 segons
Memory Limit: Ser generós. Si no la Màquina Virtual de Java es pot quedar sense espai. Els 64 MB que posen com exemple son suficients per el 99% de problemes (a no ser que vulguis fer un problema a on vulguis jugar amb el límit de memòria)


Un cop acabat guarda el problema i el pots veure en el lloc

![](http://i.imgur.com/ZgO5xcY.png)

## Editar Casos de Prova
Internament el jutge fa servir YAML, però hi ha una interficie que et genera el YAML automàticament. Pots llegir més sobre el YAML aquí [here](/judge/problem_format.md).

En la pàgina del problema, un cop creat, ves a  _Edit test data_ que obrirà l'editor dels casos de prova

![](http://i.imgur.com/eDWEEJk.png)

En l'editor has de pujar un arxiu zip que contingui els casos de prova. Cada cas de prova son dos arxius de text, un amb l'entrada i un amb la sortida. Generalment voldras un cas de prova (i per tant una parella d'arxius diferent) per cada 10 casos.

La convenció es que els arxius d'entrada acabin amb `.in` i els de sortida amb `.out` però **no** és necessari.

Per exemple, un problema amb codi de `testp1`, podria tenir 4 arxius en el zip, `testp1.1.in`,`testp1.1.out`, `testp1.2.in`,`testp1.2.out` .

![](http://i.imgur.com/w5ytsgi.png)

En Checker tens 3 opcions

- Standard: Si vols desactivar totalment el sistema d'ajuda o tens casos de prova amb més de 10.000 casos
- Linea a Linea (només profes): Si vols que els professors puguin veure els errors i l'entrada, o si els teus casos de prova són Irregulars com s'explica més amunt
- Linea a Linea amb Retroacció: Si vols activar el Sistema d'Ajuda. Els problemes haurien de tenir aquest Checker gairebé sempre.

A Format de Casos de Prova has d'activar un dels següents

- Estàndard/fixe: Si el teu format és Estàndard o Relació Fixa
- STOP al final: Si el teu format és STOP al final
- Linies per cada cas: Si el teu format és Cada cas té linies indicades
- Casos individuals: Si el teu format és Cas individual

**seleccionar el format incorrecte farà que el sistema d'ajuda dongui errors!**

Has d'afegir tants casos de prova (add case) com fitxers tinguis.

Per cada cas de proves hauras d'afegir una puntuació per a que es pugui calcular parcialment.

D'aquesta forma, si el teu problema val 20 punts i té 3 casos que pesen 1, 2 i 7 punts, un ususari que tingui els primers casos correctes tindrà (1 + 2) / (1 + 2 + 7) * 20 punts.

## Enviar el Problema
Un cop has acabat, pots donar a Submit i el problema quedarà obert. Recorda que pots editar-lo si hi ha cap error i que pots fer servir els comentaris per fer qualsevol aclariment. El problema no serà públic fins que un veterà l'hagi verificat.
