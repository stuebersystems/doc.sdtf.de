# Zeilenaufbau

Eine Schuldatentransferdatei ist eine zeilenorientierte ANSI-Textdatei. Schuldatentransferdateien sollten die Endung .TXT haben. Die Datenfelder einer Zeile bzw. eines Datensatzes haben eine variable Länge und werden durch Semikolons getrennt. Das erste Feld enthält den Zeilentyp der angibt, wie die
restlichen Datenfelder der Zeile interpretiert werden sollen. Ist das erste Datenfeld leer, so handelt es sich um eine Kommentarzeile.

Die Felder entsprechen dem sog. System Data Format (SDF), d.h. bei einem Semikolon, Komma, Sonderzeichen oder einem Leerzeichen im String wird der String in Hochkommata gesetzt, z.B. das Klassenkürzel “HB 00“ wird

```
...;“HB 00“;...
```

und nicht

```
...;HB 00;...
```

geschrieben.

Nicht unterstützte Felder werden leer übertragen (zwei Semikolons ohne Zwischenraum). Leere Felder hinter dem letzten nichtleeren Feld können wahlweise auch entfallen. Das Schuldatentransferformat ist als allgemeines programmunabhängiges Austauschformat für Schuldaten entwickelt worden. Es müssen nicht alle Zeilentypen in einer Schuldatentransferdatei vorkommen. Programme die dieses Format einlesen, sollten angemessen auf fehlende Informationen reagieren. 

| Zeilentyp | Datentypen             |
| --------- | ---------------------- |
| (leer)    | Kommentarzeile         |
| K         | Klassendaten           |
| L         | Lehrerdaten            |
| R         | Raumdaten              |
| F         | Fachdaten              |
| V         | Versionsangaben        |
| U         | Veranstaltungen        |
| T         | Stundentafeln          |
| A         | Abteilungen            |
| S         | Lehrer-Soll-Schlüssel  |
| P         | Schüler                |
| D         | MAGELLAN Datawarehouse |
| Z         | Zeitraumdaten          |

Wegen evtl. Referenzen zwischen den Datensätzen, z.B. nimmt der Datensatz K1 durch die Klassenraumangabe Bezug auf Raumdaten des Typs R1, sollte unbedingt folgende Reihenfolge der Datensatztypen in der Schuldatentransferdatei eingehalten werden: W, S, A, R, F, L, T, K, C, U, P. Ein U1-Datensatz muss z.B. unmittelbar von seinen entsprechenden U2, U3, U4, U5, U6-Datensätzen gefolgt werden.

Die V-Datensätze werden ausschließlich für das Vertretungsarchiv (.dar-Datei) und die D-Datensätze werden ausschließlich für das MAGELLAN-Datawarehouse exportiert. Analoges gilt für andere Datentypen. Andernfalls können die Daten beim Importieren von einer Schuldatentransferdatei in eine Plandatei vom Konvertierungsprogramm möglicherweise nicht vollständig rekonstruiert werden.

| Abkürzung | Bedeutung                     |
| --------- | ----------------------------- |
| C         | Zeichenfolge                  |
| N         | Ganze Zahl (integer)          |
| R         | Kommazahl: Trennzeichen Komma |
| D         | Datum JJJJMMTT                |
| <leer>    | leeres Feld „;;“              |