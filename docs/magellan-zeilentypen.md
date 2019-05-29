# MAGELLAN Datawarehouse Zeilentypen

## Zeilentyp “D1”

Nr | Typ | Bedeutung
-- | --- | ---------
1. | C   | Zeilentyp D1 – Lehrerdaten - MAGELLAN Datawarehouse
2. | N   | Lehrer-ID
3. | C   | Lehrer- Kürzel
4. | C   | Lehrer-Nachname
5. | C   | Lehrer-Vorname

## Zeilentyp “D2”

Nr | Typ | Bedeutung
-- | --- | ---------
1. | C   | Zeilentyp D2 – Klassendaten - MAGELLAN Datawarehouse
2. | R   | Klassen-ID
3. | C   | Klassen- Kürzel
4. | R   | Klassen-Ist
5. | C   | Klassen-Merkmal

## Zeilentyp “D3”

Nr  | Typ | Bedeutung
--- | --- | ---------
1.  | C   | Zeilentyp D3 – Termine - MAGELLAN Datawarehouse
2.  | D   | ZeitpunktDatum
3.  | T   | ZeitpunktUhrzeit
4.  | R   | DauerSchulStd
5.  | N   | DauerMinuten
6.  | C   | Klassen-ID
7.  | C   | Lehrer- ID
8.  | C   | Fach-Kürzel
9.  | C   | Fach-Schlüssel
10. | C   | Fach-Unterrichtsart
11. | C   | Fach-Status
12. | N   | KursNr
13. | C   | VeranstaltungsNr

## Zeilentyp “D4”

Nr  | Typ | Bedeutung
--- | --- | ---------
1.  | C   | Zeilentyp D4 – Veranstaltungen - MAGELLAN Datawarehouse
2.  | C   | Klassen-ID
3.  | C   | Lehrer- ID
4.  | C   | Fach-Kürzel
5.  | C   | Fach-Schlüssel
6.  | C   | Fach-Unterrichtsart-Schlüssel
7.  | C   | Fach-Status-Schlüssel
8.  | I   | KursNr
9.  | R   | Soll
10. | R   | Soll2
11. | R   | KlassenIst
12. | R   | LehrerIst
13. | I   | D4-Block-ID, falls vorhanden, sonst leer
14. | C   | Block-ID, falls vorhanden, sonst leer
15. | C   | Bemerkung aus der Stundentafel
16. | C   | Bemerkung
17. | C   | „Beifach“, falls es sich um Beifach handelt, leer sonst

## Zeilentyp “D5”

Nr | Typ | Bedeutung
-- | --- | ---------
1. | C   | Zeilentyp D5 – Lehrer-Soll-Berechnung - MAGELLAN Datawarehouse
2. | N   | Lehrer-ID
3. | N   | Position
4. | C   | Soll-Schlüssel-Kürzel
5. | C   | Soll-Schlüssel-Typ
6. | N   | Dauer
7. | C   | Bemerkung

## Zeilentyp „D6“

Nr  | Typ | Bedeutung
--- | --- | ---------
1.  | C   | Zeilentyp D6 – Veranstaltungen - MAGELLAN Datawarehouse
2.  | C   | Klassen-ID
3.  | C   | Lehrer-ID
4.  | C   | Fach-Kürzel
5.  | C   | Fach-Schlüssel
6.  | C   | Unterrichtsart-Schlüssel
7.  | C   | Fachstatus-Schlüssel
8.  | I   | KursNr
9.  | R   | Soll der Klasse, der Stundentafel
10. | R   | Soll2 Solländerung, bzw- Differenz der Stundentafel
11. | R   | KlassenIst
12. | R   | LehrerIst
13. | I   | D6-ID
14. | I   | D6-Block-Nr., falls vorhanden, sonst leer
15. | C   | Block-ID, falls vorhanden, sonst leer
16. | C   | Soll-Bemerkung aus der Stundentafel
17. | C   | Bemerkung aus der Veranstaltungsliste
18. | C   | Bemerkung: Beifach
19. | C   | Unterrichtsform
20. | I   | Schüleranzahl
21. | C   | Kategorie
22. | I   | Klassenverband (1=ja, 0=nein)