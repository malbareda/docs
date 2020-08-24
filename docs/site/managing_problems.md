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

Un exemple seria TODO

### Relació fixa

n línees d'entrada es correspón a m línees de sortida, sent n i m valors fixos. Per exemple, cada cas son sempre 2 linees d'entrada i 1 de sortida, o 5 i 2, o 1 i 4. També es te en consideració el +1 per la primera linea que indica quants casos hi ha

Aquest cas el tracta el jutge automàticament i no cal fer res

Un exemple seria TODO

### STOP al final

És exactament igual que l'estàndard o la relació fixa, pero en comptes de tenir una linea al principi que indica quants casos hi ha, hi ha una al final amb una entrada ja acordada que indica que s'acaba l'execució i no s'ha de processar

Aquest cas s'ha d'indicar a l'hora de penjar els casos de prova!

Un exemple seria TODO

### Cada cas té linies indicades

És un problema que segueix la seguent casuística.
"El primer nombre n indica el nombre de casos. Després hi haura n casos. En cada cas, el primer nombre, k, indica les linies que hi ha. Després hi haura k línies detallant el cas." La sortida SEMPRE es d'una sola linea.

Aquest cas s'ha d'indicar a l'hora de penjar els casos de prova!

Un exemple seria TODO

### Cas individual

Quan el problema no segueix cap dels casos següents, es pot fer cada cas individual. En aquest sentit, cada cas seria un fitxer d'entrada/sortida diferent. 
Aquest cas s'ha d'indicar a l'hora de penjar els casos de prova!

Un exemple seria TODO

### Cas Irregular

És un problema que segueix la seguent casuística.
"El primer nombre n indica el nombre de casos. Després hi haura n casos. En cada cas, el primer nombre, k, indica les linies que hi ha. Després hi haura k línies detallant el cas." La sortida SEMPRE es d'una sola linea.

Aquest cas s'ha d'indicar a l'hora de penjar els casos de prova!

Un exemple seria TODO


# Afegir un Problema
ves a [dmoj.ca/admin](https://dmoj.ca/admin), i fes servir les teves credencials.
Aleshores, fes click al botó _Add_ en el menú _Problems_ 

![](http://i.imgur.com/RFPQaUi.png)

This is will open up the main problem editor. To start, you should provide a problem code (must be unique site-wide),
and a title for your problem. **Make sure to mark yourself as an author**, as otherwise you will be locked out of your problem.

![](http://i.imgur.com/bPlNZUR.png)

Here you may edit your problem statement. The DMOJ features a rich Markdown-based syntax, with custom extensions for LaTeX-based display
math, and Mathjax-based inline math. See [this template](https://raw.githubusercontent.com/DMOJ/docs/master/sample_files/problem_markdown_example.md.txt) for a full feature example (you may copy/paste
its content into your editor).

There are many options controlling your problem described in the editor, that you may use to customize the execution of your problem.

Once you are done preparing your statement, click the _Save_ button, then scroll up to the top of the page and
click the _View on Site_ button.

![](http://i.imgur.com/ZgO5xcY.png)

## Editing Test Data
Internally, the DMOJ uses a YAML-based format for describing problem data, which you may read about [here](/judge/problem_format.md).
The site provides an interface for managing problem data, removing the need to drop down to YAML configuration for most problems.

On the problem page, click the _Edit test data_ link, which will open up the test data editor.

![](http://i.imgur.com/eDWEEJk.png)

In the editor, you must first upload a zip archive containing the input/output data used for your problem. The typical convention
is to use text files ending with a `.in` extension for input files, and `.out` for output files, with the 
testcase number embedded in the filename.

For example, for a problem with a code of `testp1`, a the first test case would be named `testp1.1.in`,
with an output file `testp1.1.out`.

Using this format is **not** necessary &mdash; the judge will accept any filenames &mdash; but using it will allow the test data
editor to autocomplete paths, saving some manual input.

![](http://i.imgur.com/w5ytsgi.png)

There are many other options, but for most problems only one more is necessary: the per-case point value. If partial points
are enabled in the problem statement editor, then a user's score on the problem is equal to the 
sum of the point values of the cases they got right divided by the total sum of case point values, multiplied by the number of
points the problem is worth.

For example, if your problem is worth 100 points and has 3 cases weighted 1/2/7 points respectively, a user who gets the first
two cases correct and then fails the last one will have a score of (1 + 2) / (1 + 2 + 7) &times; 100 = 30 points, out of 100.

## Submitting a Problem
After you have created your test data, you should head back to the problem and click the _Submit solution_ button. If at any point in
time you need to update your data, you may do so from the test data editor, and it will update automatically.
