# Pax-agreements-and-conflictivity
Relating the number of peace agreements signed and their date to the conflict rate

**Conflictivitat i acords de pau**

Hem seguit la metodologia de Hans Rosling de The best stats you've ever seen, una TED Talk:

https://youtu.be/hVimVzgtD6w

que presenta l'evolució global d'una variable, l'esperança de vida, definida per països i regions. Representa l'evolució temporal de la variable, que en aquest cas creix, i canvia de paradigma: de família llarga i vida curta, a família curta i vida llarga. La idea és desenvolupar la visualització de manera que aquest fet quedi patent per a l'espectador.

El resultat és un vídeo mp4 de 41,7 Mb pax-c.mp4 que per requeriment de Github (< 25 Mb) hem hagut de comprimir com a pax-c.7z.

El que hem fet és gastar les dades de la data base de https://www.peaceagreements.org/ d'acords de pau, i deduir del seu ritme de signatura per un mateix país la conflictivitat que pot estar present: ningú que no tingui conflictes signarà un tractat de pau innecessari. Quan hi ha conflictivitat o guerres, eventualment apareixen acords de pau; quan la conflictivitat és baixa els acords són duradors, mentre que si és alta, són efímers.

Les idees surten de la mateixa base de dades, que en trenta-dos anys (entre 1990 i 2021) registra 1915 acords de pau, un 10% signats per un mateix país el mateix dia. En un món sense conflictes, els acords de pau són poc freqüents; diguem menys de 100 en trenta-dos anys. Hem pensat mesurar la conflictivitat com proporcional a la inversa dels dies entre dos acords successius del mateix país.

Respecte a les dades, hi ha dues versions disponibles en format csv, el fitxer
‘pax_corpus_1915_agreements_07-12-21.csv',
de 13 columnes, i el fitxer
‘pax_data_1915_agreements_07-12-21.csv'
de 267 columnes. Triem el primer, que inclou les dades necessàries; el segon afegeix dades majoritàriament administratives.

Només emprem les dades de dates, país i regió. D'aquí es dedueixen altres dades, com a any de signatura o dies entre acords successius del mateix país. Hem tractat les dades en Excel i creat un nou fitxer csv: paxc2.csv.

Podem crear un índex de conflictivitat d'un país que sigui invers a la durada en dies dels seus acords de pau. En la base de dades hi ha registrats diversos acords o acords d'un país en el mateix dia (a vegades sis), o en diversos dies successius: un 10,65% en el mateix dia i un 23,5% en un període de cinc dies successius. Els hem eliminat, mantenint l'última data, considerant que reflecteixen el mateix conflicte.

L'índex apareix com '1000/ dies_entre_acords' al fitxer. Hem comprovat succintament que l'índex és adequat, per exemple, per als països on és major que 100. El coeficient '1000/dies_entre_acords' l'hem representat entre els anys 1990 i 2021, on les regions de la database han sigut representades per diferents colors, i la mida de cada punt, representa el nombre d'acords de pau signat pel país en els trenta-dos anys: com més acords, més conflicte.

El que podem concloure és que es manté globalment el nivell de conflictivitat, canviant d'escenari i protagonistes de tant en tant. 

Si representem el valor de l'índex en funció de la data per al conjunt de totes les dades, podria ser confús: hi ha massa detall. Per això, presentem una animació d'any en any, on es comprova com evoluciona la conflictivitat anual per regions i països.

Visualitzacions interactives

Les visualitzacions interactives estan internament en JavaScript, han estat desenvolupades amb la llibreria Plotly de Python i la sortida és format html: incloses en qualsevol format text es converteixen en imatges no interactives. Han de ser vistes amb un browser (com Firefox) i són d'una grandària sobre 3,5 Gb, per la qual cosa GitHub deixa baixar-los, però no obrir-los en la mateixa web de GitHub. Són els fitxers HTML d'aquesta carpeta i tots ells (els fitxers HTML) han de deixar-se en la mateixa carpeta, si volem obrir-los des del fitxer VisualitzacioInteractiva .html, que explica el contingut de cadascun.


La base de dades té uns drets de còpia Creative Commons, https://creativecommons.org/licenses/by-nc-sa/4.0/


Referencies:
https://www.peaceagreements.org/search?SearchForm%5Bregion%5D=&SearchForm%5Bcountry_entity%5D=&SearchForm%5Bname%5D=&SearchForm%5Bcategory_mode%5D=any&SearchForm%5Bagreement_text%5D=&s=Search+Database

-	Bell, Christine, Sanja Badanjak, Juline Beujouan, Robert Forster,Tim Epple,
Astrid Jamar, Kevin McNicholl, Sean Molloy, Kathryn Nash, Jan Pospisil,
Robert Wilson, Laura Wise (2021):
PA-X Codebook, Version 5. Political Settlements Research Programme,
University of Edinburgh, Edinburgh. www.peaceagreements.org
-	Bell, C. and Badanjak, S. (2019):
‘Introducing PA-X: A new peace agreement database and dataset’, Journal of Peace Research, 56 (3).
-	Dr. Nualart: Les visualitzacions de les dades de la mateixa web


**Conflictividad y acuerdos de paz**

Hemos seguido la metodología de Hans Rosling de The best stats you'viene ever seen, una TED Talk:

https://youtu.be/hvimvzgtd6w

que presenta la evolución global de una variable, la esperanza de vida, definida por países y regiones. Representa la evolución temporal de la variable, que en este caso crece, y cambia de paradigma: de familia larga y vida corta, a familia corta y vida larga. La idea es desarrollar la visualización de forma que este hecho quede patente para el espectador.

El resultado es un video mp4 de 41,7 Mb pax-c.mp4 que por requerimiento de Github (< 25Mb) hemos debido comprimir como pax-c.7z.

Lo que hemos hecho es usar los datos de la base de datos de https://www.peaceagreements.org/ de acuerdos de paz, y deducir de las  diferencias de fecha de firma en días, para un mismo país, la conflictividad que puede estar presente: nadie que no tenga conflictos firmará un tratado de paz innecesario. Cuando hay conflictividad o guerras, eventualmente aparecen acuerdos de paz; cuando la conflictividad es baja los acuerdos son duraderos, mientras que si es alta, son efímeros.

Las ideas salen de la misma base de datos, que en treinta y dos años (entre 1990 y 2021) registra 1915 acuerdos de paz, un 10% firmados por un mismo país el mismo día. En un mundo sin conflictos, los acuerdos de paz serian poco frecuentes; digamos menos de 100 en treinta y dos años. Hemos pensado medir la conflictividad como una variable proporcional a la inversa de los días entre dos acuerdos sucesivos del mismo país.

Respecto a los datos, hay dos versiones disponibles en formato csv, el fichero
‘pax_corpus_1915_agreements_07-12-21.csv',
de 13 columnas, y el fichero
‘pax_data_1915_agreements_07-12-21.csv'
de 267 columnas. Elegimos el primero, que incluye los datos necesarios; el segundo añade datos mayoritariamente administrativos y excesivos para un no experto.

Solo empleamos los datos de fechas, país y región. De aquí se deducen otros datos, como año de firma o días entre acuerdos sucesivos del mismo país. Hemos tratado los datos en Excel y creado un nuevo fichero csv: paxc.csv.

Podemos crear un índice de conflictividad de un país que sea inverso a la duración en días de sus acuerdos de paz. En la base de datos hay registrados varios acuerdos o acuerdos de un país en el mismo día (a veces seis), o en varios días sucesivos: un 10,65% en el mismo día y un 23,5% en un periodo de cinco días sucesivos. Los hemos eliminado, manteniendo la última fecha, considerando que reflejan el mismo conflicto.

El índice aparece como '1000/ días_entre_acuerdos' en el fichero csv. Hemos comprobado sucintamente que el índice es adecuado, por ejemplo, para los países donde es mayor que 100. 

Si representamos el valor del índice en función de la fecha para el conjunto de todos los datos, podría ser confuso: hay demasiado detalle. Por ello presentamos una animación de año en año, donde se comprueba cómo evoluciona la conflictividad anual por regiones y países, donde las regiones de la base de datos han sido representadas por diferentes colores, y el número de acuerdos de paz firmado por el país en los treinta y dos años, representado por el tamaño de cada punto; ya que más acuerdos de paz sugieren más conflicto. 

Lo que podemos concluir es que se mantiene globalmente el nivel de conflictividad, cambiando de escenario y protagonistas de tanto en tanto.


Visualizaciones interactivas

Las visualizaciones interactivas están internamente en JavaScript, han sido desarrolladas con la librería Plotly de Python y la salida es formato html: incluidas en cualquier formato texto se convierten en imágenes no interactivas. Deben ser vistas con un browser (como Firefox) y son de un tamaño sobre 3,5 Gb, por lo que GitHub deja bajarlos, pero no abrirlos en la propia web de GitHub. Son los ficheros HTML de esa carpeta y todos ellos (los ficheros HTML) deben dejarse en la misma carpeta, si queremos abrirlos desde el fichero VisualitzacioInteractiva.html, que explica el contenido de cada uno.


La base de datos tiene unos derechos de copia Creative Commons, https://creativecommons.org/licenses/by-nc-sa/4.0/


Referencias:
https://www.peaceagreements.org/search?SearchForm%5Bregion%5D=&SearchForm%5Bcountry_entity%5D=&SearchForm%5Bname%5D=&SearchForm%5Bcategory_mode%5D=any&SearchForm%5Bagreement_text%5D=&s=Search+Database

-	Bell, Christine, Sanja Badanjak, Juline Beujouan, Robert Forster,Tim Epple,
Astrid Jamar, Kevin McNicholl, Sean Molloy, Kathryn Nash, Jan Pospisil,
Robert Wilson, Laura Wise (2021):
PA-X Codebook, Version 5. Political Settlements Research Programme,
University of Edinburgh, Edinburgh. www.peaceagreements.org
-	Bell, C. and Badanjak, S. (2019):
‘Introducing PA-X: A new peace agreement database and dataset’, Journal of Peace Research, 56 (3).
-	Dr. Nualart: Visualizaciones en la misma web.


Interactive visualizations

The interactive visualizations are internally in JavaScript, have been developed with Python's Plotly library and the output is html format: included in any text format they become non-interactive images. They need to be viewed with a browser (like Firefox) and are about 3.5 Gb in size, so GitHub lets you download them, but not open them on GitHub's own website. They are the HTML files in that folder and all of them (the HTML files) must be left in the same folder, if we want to open them from the VisualitzacioInteractiva.html file, which explains the content of each one.



**Conflicts and Peace Agreements**

We have followed Hans Rosling's methodology from The best stats you've ever seen, a TED Talk:

https://youtu.be/hvimvzgtd6w

which presents the global evolution of a variable, life expectancy, defined by countries and regions. It represents the temporal evolution of the variable, which in this case grows, and changes paradigm: from long family and short life, to short family and long life. The idea is to develop the visualization in a way that makes this fact clear to the viewer.

The result is a 41.7 Mb mp4 video pax-c.mp4 that by Github requirement (< 25Mb) we had to compress as pax-c.7z.

What we have done is to use the data from the https://www.peaceagreements.org/ database of peace agreements, and deduce from the differences in the date of signature in days, for the same country, the conflictuality that may be present: no one who has no conflicts will sign an unnecessary peace treaty. When there is conflict or war, peace agreements eventually appear; when conflict is low, agreements are long-lasting, while if it is high, they are ephemeral.

The ideas come from the same database, which in thirty-two years (between 1990 and 2021) records 1915 peace agreements, 10% signed by the same country on the same day. In a world without conflict, peace agreements would be rare; let's say less than 100 in thirty-two years. We have thought of measuring conflict as a variable proportional to the inverse of the number of days between two successive agreements in the same country.

Regarding the data, there are two versions available in csv format, the file
‘pax_corpus_1915_agreements_07-12-21.csv',
of 13 columns, and the file
‘pax_data_1915_agreements_07-12-21.csv'
with 267 columns. We chose the former, which includes the necessary data; the latter adds mostly administrative data excessive for a non-expert.

We only use the data for dates, country and region. Other data, such as year of signature or days between successive agreements in the same country, can be derived from this. We have processed the data in Excel and created a new csv file: paxc.csv.

We can create a conflict index for a country that is inverse to the duration in days of its peace agreements. In the database there are several agreements or settlements of a country on the same day (sometimes six), or on several successive days: 10.65% on the same day and 23.5% over a period of five successive days. We have eliminated them, keeping the last date, considering that they reflect the same conflict.

The index appears as '1000/ days_between_agreements' in the csv file. We have succinctly checked that the index is appropriate, for example, for countries where it is greater than 100. 

If we plot the index value as a function of date for the set of all data, it could be confusing: there is too much detail. We therefore present an animation from year to year, showing how the annual conflictivity evolves by region and country, where the regions of the database have been represented by different colors, and the number of peace agreements signed by the country over the thirty-two years, represented by the size of each dot; since more peace agreements suggest more conflict. 

What we can conclude is that the level of conflict is maintained globally, changing scenario and protagonists from time to time. 

The database is copyrighted Creative Commons, https://creativecommons.org/licenses/by-nc-sa/4.0/.

