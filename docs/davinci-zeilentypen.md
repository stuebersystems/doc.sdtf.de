# DAVINCI-Zeilentypen

## Zeilentyp “A1”

| Nr  | Typ | Bedeutung                                  |
| --- | --- | ------------------------------------------ |
| 1.  | C   | Zeilentyp A1 – Abteilungsdaten (Teamdaten) |
| 2.  | N   | ID                                         |
| 3.  | C   | Abteilungskürzel                           |
| 4.  | C   | Bemerkung                                  |

## Zeilentyp “B1”

| Nr  | Typ | Bedeutung                        |
| --- | --- | -------------------------------- |
| 1.  | C   | Zeilentyp B1 – Aufsichtsbereiche |
| 2.  | N   | ID                               |
| 3.  | C   | Kürzel                           |
| 4.  | C   | Bezeichnung                      |
| 5.  | N   | Anzahl der Räume                 |
| 6.  | C   | Raumkürzel 1                     |
| 7.  | C   | Raumkürzel 2                     |
| :   | :   | :                                |

## Zeilentyp “B2”

| Nr  | Typ | Bedeutung                                           |
| --- | --- | --------------------------------------------------- |
| 1.  | C   | Zeilentyp B2 – Aufsichtsbereiche                    |
| 2.  | N   | ID                                                  |
| 3.  | C   | Kürzel                                              |
| 4.  | N   | Anzahl der Aufsichtstermine                         |
| 5a  | N   | Tag (Montag “1”..”7”Sonntag)                        |
| 5b  | N   | Stunde (Startposition in Einheiten)                 |
| 5c  | N   | WochenNr (0..56, relativ zum Anfangsdatum U0.Feld2) |
| 5d  | N   | WochenNr (0..56, relativ zum Anfangsdatum U0.Feld2) |
| 5e  | C   | Lehrerkürzel                                        |
| 6a  | N   | Tag (Montag “1”..”7”Sonntag)                        |
| 6b  | N   | Stunde (Startposition in Einheiten)                 |
| 6c  | N   | WochenNr (0..56, relativ zum Anfangsdatum U0.Feld2) |
| 6d  | N   | WochenNr (0..56, relativ zum Anfangsdatum U0.Feld2) |
| 6e  | C   | Lehrerkürzel                                        |
| :   | :   | :                                                   |

## Zeilentyp “F1”

| Nr  | Typ | Bedeutung                                                                               |
| --- | --- | --------------------------------------------------------------------------------------- |
| 1.  | C   | Zeilentyp F1 – Fachdaten                                                                |
| 2.  | N   | ID                                                                                      |
| 3.  | C   | Fachkürzel                                                                              |
| 4.  | C   | Bezeichnung                                                                             |
| 5.  | C   | Statistikschlüssel                                                                      |
| 6.  | N   | Kategorie (<leer> = keine Angabe, 0 = Fremdsprache usw.                                 |
| 7.  | N   | Aufgabenbereich (<leer> = keine Angabe, 0 = Sprachlich, lit.-künstlerisch, ..5 = Sport) |

## Zeilentyp “F2”

| Nr  | Typ | Bedeutung                                                                  |
| --- | --- | -------------------------------------------------------------------------- |
| 1.  | C   | Zeilentyp F2 – Fach-Sperrungen (nur bis DAVINCI 5, abn Version 6 siehe F9) |
| 2.  | C   | Fachkürzel                                                                 |
| 3.  | N   | Anzahl der Termine                                                         |
| 4a  | N   | Tag (1=Montag...7=Sonntag)                                                 |
| 4b. | N   | Absolute Position (1, 2, 3, ...)                                           |
| 4c. | N   | Dauer in Einheiten (1, 2, 3, ...)                                          |
| 4d  | N   | Absolute Wochennummer (0, 1, 2, 3...)                                      |
| 5a  | N   | Tag (1=Montag...7=Sonntag)                                                 |
| :   | :   | :                                                                          |

## Zeilentyp “F3”

| Nr  | Typ | Bedeutung                |
| --- | --- | ------------------------ |
| 1.  | C   | Zeilentyp F3 – Fachdaten |
| 2.  | N   | ID                       |
| 3.  | C   | Fachkürzel               |
| 4.  | N   | Anzahl der Räume         |
| 5.  | C   | Fachraum 1               |
| 6.  | C   | Fachraum 2               |
| :   | :   | :                        |

## Zeilentyp “F9”

| Nr  | Typ | Bedeutung                                                       |
| --- | --- | --------------------------------------------------------------- |
| 1.  | C   | Zeilentyp F9 – Fach Zeitpräferenzen                             |
| 2.  | N   | ID                                                              |
| 3.  | C   | Fachkürzel                                                      |
| 4.  | N   | Anzahl der Zeitpräferenzen                                      |
| 5a  | C   | Typ (Sperrung oder Kernzeit)                                    |
| 5b  | N   | Periodisch (0=false, 1=true)                                    |
| 5c  | C   | Name                                                            |
| 5d  | C   | Start-Zeitpunkt (im Format „yyyymmddhhmm“)                      |
| 5e  | C   | End-Zeitpunkt (im Format „yyyymmddhhmm“)                        |
| 5f  | C   | Tages Start-Zeitpunkt (im Format „hhmm“)                        |
| 5g  | C   | Tages End-Zeitpunkt (im Format „hhmm“)                          |
| 5h  | C   | Wochen Start-Zeitpunkt (0=keinen Angabe, 1=Montag, 2=Dienstag…) |
| 5j  | C   | Wochen End-Zeitpunkt (0=keinen Angabe, 1=Montag, 2=Dienstag…)   |
| 5k  | C   | Wochen Start-Zeitpunkt (0=keinen Angabe, 1=Montag, 2=Dienstag…) |
| 5l  | R   | Wert                                                            |
| 5m  | C   | Zeitpräferenzkategorie.Kürzel                                   |
| 5n  | C   | Team.Kürzel                                                     |
| 5o  | N   | Ganztägig (0=false, 1=true)                                     |
| 5p  | N   | SystemCreated (0=false, 1=true)                                 |
| 6a  | C   | Typ (Sperrung oder Kernzeit)                                    |
| 6b  | N   | Periodisch (0=false, 1=true)                                    |
| :   | :   | :                                                               |

## Zeilentyp “K1”

| Nr  | Typ | Bedeutung                                                    |
| --- | --- | ------------------------------------------------------------ |
| 1.  | C   | Zeilentyp K1 – Klassendaten                                  |
| 2.  | N   | ID                                                           |
| 3.  | C   | Klassenkürzel                                                |
| 4.  | C   | Bezeichnung                                                  |
| 5.  | C   | Abteilungskennzeichen                                        |
| 6.  | C   | Klassenlehrer.Kürzel 1                                       |
| 7.  | C   | Klassenlehrer.Kürzel 2                                       |
| 8.  | C   | Klassenraum.Kürzel                                           |
| 9.  | N   | Wochentaganzahl                                              |
| 10. | N   | Schüleranzahl                                                |
| 11. | C   | Stundentafel                                                 |
| 12. | C   | Integrierte Klasse.Kürzel                                    |
| 13. | N   | Stufe (1, 2, ..., 13)                                        |
| 14. | N   | Kursmodus (0=Standard, 1=Kurse, 2=Leistungs- und Grundkurse) |
| 15. | C   | Perioden.Kürzel                                              |
| 16. | C   | Schulnummer                                                  |
| 17. | C   | Merkmale                                                     |
| 18. | C   | Assoziierte Klasse.Kürzel                                    |
| 19. | C   | Gebäude.Kürzel                                               |
| 20. | C   | Bildungsgang.Kürzel                                          |
| 21. | C   | Schulform.Kürzel                                             |
| 22. | C   | Schulstelle.Kürzel                                           |
| 23. | C   | Klassenmerkmal.Kürzel                                        |

## Zeilentyp “K2”

| Nr  | Typ | Bedeutung                                                                     |
| --- | --- | ----------------------------------------------------------------------------- |
| 1.  | C   | Zeilentyp K2 – Klassen Sperrungen (nur bis DAVINCI 5, abn Version 6 siehe F9) |
| 2.  | C   | Klassenkürzel                                                                 |
| 3.  | N   | Anzahl der Termine                                                            |
| 4a  | N   | Tag (1=Montag...7=Sonntag)                                                    |
| 4b  | N   | Absolute Position (1, 2, 3, ...)                                              |
| 4c  | N   | Dauer in Einheiten (1, 2, 3, ...)                                             |
| 4d  | N   | Absolute Wochennummer (0, 1, 2, 3...)                                         |
| 5a  | N   | Tag (1=Montag...7=Sonntag)                                                    |
| :   | :   | :                                                                             |

## Zeilentyp “K9”

| Nr  | Typ | Bedeutung                                                       |
| --- | --- | --------------------------------------------------------------- |
| 1.  | C   | Zeilentyp K9 – Klassen Zeitpräferenzen                          |
| 2.  | N   | ID                                                              |
| 3.  | C   | Klassenkürzel                                                   |
| 4.  | N   | Anzahl der Zeitpräferenzen                                      |
| 5a  | C   | Typ (Sperrung oder Kernzeit)                                    |
| 5b  | N   | Periodisch (0=false, 1=true)                                    |
| 5c  | C   | Name                                                            |
| 5d  | C   | Start-Zeitpunkt (im Format „yyyymmddhhmm“)                      |
| 5e  | C   | End-Zeitpunkt (im Format „yyyymmddhhmm“)                        |
| 5f  | C   | Tages Start-Zeitpunkt (im Format „hhmm“)                        |
| 5g  | C   | Tages End-Zeitpunkt (im Format „hhmm“)                          |
| 5h  | C   | Wochen Start-Zeitpunkt (0=keinen Angabe, 1=Montag, 2=Dienstag…) |
| 5j  | C   | Wochen End-Zeitpunkt (0=keinen Angabe, 1=Montag, 2=Dienstag…)   |
| 5k  | R   | Wert                                                            |
| 5l  | C   | Zeitpräferenzkategorie.Kürzel                                   |
| 5m  | C   | Team.Kürzel                                                     |
| 5n  | N   | Ganztägig (0=false, 1=true)                                     |
| 5o  | N   | SystemCreated (0=false, 1=true)                                 |
| 6a  | C   | Typ (Sperrung oder Kernzeit)                                    |
| 6b  | N   | Periodisch (0=false, 1=true)                                    |
| :   | :   | :                                                               |

## Zeilentyp “L1”

| Nr  | Typ | Bedeutung                                         |
| --- | --- | ------------------------------------------------- |
| 1.  | C   | Zeilentyp L1 – Lehrerdaten                        |
| 2.  | N   | Lehrer-ID                                         |
| 3.  | C   | Lehrerkürzel                                      |
| 4.  | C   | Nachname                                          |
| 5.  | C   | Vorname                                           |
| 6.  | C   | Bemerkung                                         |
| 7.  | N   | Max. Springstunden                                |
| 8.  | N   | Wochentage                                        |
| 9.  | C   | Raum                                              |
| 10. | C   | Schulnummer                                       |
| 11. | C   | Titel                                             |
| 12. | C   | Lehrerart.Kurzel                                  |
| 13. | N   | Geschlecht (0=unbestimmt, 1=männlich, 2=weiblich) |
| 14. | C   | Handy                                             |
| 15. | C   | Email                                             |

## Zeilentyp “L2”

| Nr  | Typ | Bedeutung                             |
| --- | --- | ------------------------------------- |
| 1.  | C   | Zeilentyp L2 – Lehrer Sperrungen      |
| 2.  | C   | Lehrerkürzel                          |
| 3.  | N   | Anzahl der Termine                    |
| 4a  | N   | Tag (1=Montag...7=Sonntag)            |
| 4b  | N   | Absolute Position (1, 2, 3, ...)      |
| 4c  | N   | Dauer in Einheiten (1, 2, 3, ...)     |
| 4d  | N   | Absolute Wochennummer (0, 1, 2, 3...) |
| 4e  | N   | Zeitschiene (A, B, C, …)              |
| 5a  | N   | Tag (1=Montag...7=Sonntag)            |
| :   | :   | :                                     |

## Zeilentyp “L3”

| Nr  | Typ | Bedeutung                    |
| --- | --- | ---------------------------- |
| 1.  | C   | Zeilentyp L3 – Lehrer Fächer |
| 2.  | N   | Lehrer-ID                    |
| 3.  | C   | Lehrerkürzel                 |
| 4.  | N   | Anzahl der Fächer            |
| 5.  | C   | Fachkürzel 1                 |
| 6.  | C   | Fachkürzel 2                 |
| :   | :   | :                            |

## Zeilentyp “L4”

| Nr  | Typ | Bedeutung                             |
| --- | --- | ------------------------------------- |
| 1.  | C   | Zeilentyp L4 – Lehrer Abteilungsdaten |
| 2.  | N   | Lehrer-ID                             |
| 3.  | C   | Lehrerkürzel                          |
| 4.  | N   | Anzahl der Abteilungen                |
| 5.  | C   | Abteilung 1                           |
| 6.  | C   | Abteilung 2                           |
| :   | :   | :                                     |

## Zeilentyp “L5”

| Nr  | Typ | Bedeutung                            |
| --- | --- | ------------------------------------ |
| 1.  | C   | Zeilentyp L5 – Lehrerdaten           |
| 2.  | N   | ID                                   |
| 3.  | C   | Lehrerkürzel                         |
| 4.  | N   | Anzahl der Schlüssel                 |
| 5.  | C   | Soll-Schlüssel Kürzel                |
| 6.  | C   | Soll-Schlüssel Bezeichnung           |
| 7.  | C   | Soll-Schlüssel Schlüsseltyp/Operator |
| 8.  | R   | Soll-Schlüssel Stundenanzahl         |
| 9.  | C   | Soll-Schlüssel Bemerkung             |
| 10. | C   | Soll-Schlüssel Kürzel                |
| 11. | C   | Soll-Schlüssel Bezeichnung           |
| 12. | C   | Soll-Schlüssel Schlüsseltyp/Operator |
| 13. | R   | Soll-Schlüssel Stundenanzahl         |
| 14. | C   | Soll-Schlüssel Bemerkung             |
| :   | :   | :                                    |

## Zeilentyp “L6”

| Nr  | Typ | Bedeutung                                    |
| --- | --- | -------------------------------------------- |
| 1.  | C   | Zeilentyp L6 – Lehrerfehlzeiten (nur Export) |
| 2.  | C   | Lehrerkürzel                                 |
| 3.  | C   | Startdatum/-zeit nach ISO8601                |
| 4.  | C   | Enddatum/-zeit nach ISO8601                  |
| 5.  | C   | Fehlgrund Kürzel                             |
| 6.  | C   | Bemerkung                                    |


## Zeilentyp “L9”

| Nr  | Typ | Bedeutung                                                                        |
| --- | --- | -------------------------------------------------------------------------------- |
| 1.  | C   | Zeilentyp L9 – Lehrer Zeitpräferenzen                                            |
| 2.  | N   | ID                                                                               |
| 3.  | C   | Lehrerkürzel                                                                     |
| 4.  | N   | Anzahl der Zeitpräferenzen                                                       |
| 5a  | C   | Typ (Sperrung oder Kernzeit)                                                     |
| 5b  | N   | Periodisch (0=false, 1=true)                                                     |
| 5c  | C   | Name                                                                             |
| 5d  | C   | Start-Zeitpunkt (im Format „yyyymmddhhmm“)                                       |
| 5e  | C   | End-Zeitpunkt (im Format „yyyymmddhhmm“)                                         |
| 5f  | C   | Tages Start-Zeitpunkt (im Format „hhmm“)                                         |
| 5g  | C   | Tages End-Zeitpunkt (im Format „hhmm“)                                           |
| 5h  | C   | Wochen Start-Zeitpunkt (0=keinen Angabe, 1=Montag, 2=Dienstag…)                  |
| 5j  | C   | Wochen End-Zeitpunkt (0=keinen Angabe, 1=Montag, 2=Dienstag…)                    |
| 5k  | R   | Wert                                                                             |
| 5l  | C   | Zeitpräferenzkategorie.Kürzel                                                    |
| 5m  | C   | Team.Kürzel                                                                      |
| 5n  | N   | Ganztägig (0=false, 1=true)                                                      |
| 5o  | N   | SystemCreated (0=false, 1=true)                                                  |
| 6a  | C   | Typ (Sperrung oder Kernzeit)                                                     |
| 6b  | N   | Periodisch (0=false, 1=true)                                                     |
| :   | :   | :                                                                                |

## Zeilentyp “P1”

| Nr  | Typ | Bedeutung                                                                                                                                                                                                                                                                                  |
| --- | --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1.  | C   | Zeilentyp P1 – Schülerdaten                                                                                                                                                                                                                                                                |
| 2.  | N   | Schüler-ID                                                                                                                                                                                                                                                                                 |
| 3.  | C   | Jahrgangs Kürzel (Klassen Kürzel)                                                                                                                                                                                                                                                          |
| 4.  | C   | Nachname                                                                                                                                                                                                                                                                                   |
| 5.  | C   | Vorname                                                                                                                                                                                                                                                                                    |
| 6.  | N   | Geschlecht (0=unbestimmt, 1=männlich, 2=weiblich)                                                                                                                                                                                                                                          |
| 7.  | C   | Geburtsdatum im Format JJJJMMTT                                                                                                                                                                                                                                                            |
| 8.  | C   | Email                                                                                                                                                                                                                                                                                      |
| 9.  | C   | Schluessel (der Fachkombination)                                                                                                                                                                                                                                                           |
| 10. | C   | Matrikelnummer                                                                                                                                                                                                                                                                             |
| 11. | C   | Schulnummer                                                                                                                                                                                                                                                                                |
| 12. | C   | Tutor (Lehrer Kürzel)                                                                                                                                                                                                                                                                      |
| 13. | C   | Custom-ID einer externen Anwendung                                                                                                                                                                                                                                                         |
| 14. | N   | Zeitraum-ID des 1. Halbjahres                                                                                                                                                                                                                                                              |
| 15. | N   | Zeitraum-ID des 2. Halbjahres                                                                                                                                                                                                                                                              |
| 16. | N   | Zeitraum-ID des 3. Halbjahres                                                                                                                                                                                                                                                              |
| 17. | N   | Zeitraum-ID des 4. Halbjahres                                                                                                                                                                                                                                                              |
| 18. | N   | Zeitraum-ID des 5. Halbjahres                                                                                                                                                                                                                                                              |
| 19. | N   | Zeitraum-ID des 6. Halbjahres                                                                                                                                                                                                                                                              |
| 20. | N   | Anzahl der Fachwahlen/Kurse                                                                                                                                                                                                                                                                |
| 21. | C   | Fachkürzel                                                                                                                                                                                                                                                                                 |
| 22. | N   | Kursnummer<br>„-1“ = der Schüler ist einem Fach in der Fachwahl zugeordnet<br>(Leerzeichen) = der Schüler ist einem Fach aber keinem Kurs zugeordnet<br>„0“ = der Schüler ist in diesem Fach einem Kurs zugeordnet<br>„1“ und höher = der Schüler ist in diesem Fach einem Kurs zugeordnet |
| 23. | C   | Unterrichtsart Kürzel (Kurs=Kurs, GK=Grundkurs, LK=Leistungskurs)                                                                                                                                                                                                                          |
| 24. | C   | Fachstatus Kürzel                                                                                                                                                                                                                                                                          |
| 25. | C   | Kursmerkmale der Schülerfachwahl (jahrgangsübergreifend)                                                                                                                                                                                                                                   |
| 26. | C   | Kursmerkmale des Kurses (im aktuellen Jahrgang)                                                                                                                                                                                                                                            |
| 27. | C   | Fachschwerpunkt                                                                                                                                                                                                                                                                            |
| 28. | N   | Pflichtstunden                                                                                                                                                                                                                                                                             |
| 29. | N   | Stunden tatsächlich (nicht in MAGELLAN verfügbar)                                                                                                                                                                                                                                          |
| 30. | C   | Halbjahre 6 Zeichen im Format „111100“, wobei 0=false und 1=true. Dieses Feld unterscheidet Kurswahlen von Veranstaltungen: Falls leer, dann handelt es sich um eine Veranstaltung, sonst um eine Kurswahl.                                                                                |
| 31. | C   | Soll-Stunden gemäß Stundentafel des Jahrgangs (nicht in MAGELLAN verfügbar)                                                                                                                                                                                                                |
| 32. | C   | Fachkürzel                                                                                                                                                                                                                                                                                 |
| 33. | N   | Kursnummer<br>„-1“ = der Schüler ist einem Fach in der Fachwahl zugeordnet<br>(Leerzeichen) = der Schüler ist einem Fach aber keinem Kurs zugeordnet<br>„0“ = der Schüler ist in diesem Fach einem Kurs zugeordnet<br>„1“ und höher = der Schüler ist in diesem Fach einem Kurs zugeordnet |
| 34. | C   | Unterrichtsart Kürzel (Kurs=Kurs, GK=Grundkurs, LK=Leistungskurs)                                                                                                                                                                                                                          |
| 35. | C   | Fachstatus Kürzel                                                                                                                                                                                                                                                                          |
| 36. | C   | Kursmerkmale der Schülerfachwahl (jahrgangsübergreifend)                                                                                                                                                                                                                                   |
| 37. | C   | Kursmerkmale des Kurses (im aktuellen Jahrgang)                                                                                                                                                                                                                                            |
| 38. | C   | Fachschwerpunkt                                                                                                                                                                                                                                                                            |
| 39. | N   | Pflichtstunden                                                                                                                                                                                                                                                                             |
| 40. | N   | Stunden tatsächlich (nicht in MAGELLAN verfügbar)                                                                                                                                                                                                                                          |
| 41. | C   | Halbjahre 6 Zeichen im Format „111100“, wobei 0=false und 1=true                                                                                                                                                                                                                           |
| 42. | C   | Soll-Stunden gemäß Stundentafel des Jahrgangs (nicht in MAGELLAN verfügbar)                                                                                                                                                                                                                |
| :   | :   | :                                                                                                                                                                                                                                                                                          |

## Zeilentyp “R1”

| Nr  | Typ | Bedeutung                            |
| --- | --- | ------------------------------------ |
| 1.  | C   | Zeilentyp R1 – Raumdaten             |
| 2.  | N   | ID                                   |
| 3.  | C   | Raumkürzel                           |
| 4.  | C   | Langname / Informationsfeld          |
| 5.  | C   | Abteilung                            |
| 6.  | N   | Raumkapazität                        |
| 7.  | C   | Gebäude                              |
| 8.  | N   | <In aktueller Version nicht benutzt> |
| 9.  | N   | Raumart.Kürzel                       |
| 10. | C   | Lehrer.Kürzel (Betreuer)             |

## Zeilentyp “R2”

| Nr  | Typ | Bedeutung                                                                  |
| --- | --- | -------------------------------------------------------------------------- |
| 1.  | C   | Zeilentyp R2 – Raum Sperrungen (nur bis DAVINCI 5, abn Version 6 siehe F9) |
| 2.  | C   | Raumkürzel                                                                 |
| 3.  | N   | Anzahl der Termine                                                         |
| 4a  | N   | Tag (1=Montag...7=Sonntag)                                                 |
| 4b  | N   | Absolute Position (1, 2, 3, ...)                                           |
| 4c  | N   | Dauer in Einheiten (1, 2, 3, ...)                                          |
| 4d  | N   | Absolute Wochennummer (0, 1, 2, 3...)                                      |
| 5a  | N   | Tag (1=Montag...7=Sonntag)                                                 |
| :   | :   | :                                                                          |

## Zeilentyp “R9”

| Nr  | Typ | Bedeutung                                                       |
| --- | --- | --------------------------------------------------------------- |
| 1.  | C   | Zeilentyp R9 – Raum Zeitpräferenzen                             |
| 2.  | N   | ID                                                              |
| 3.  | C   | Raumkürzel                                                      |
| 4.  | N   | Anzahl der Zeitpräferenzen                                      |
| 5a  | C   | Typ (Sperrung oder Kernzeit)                                    |
| 5b  | N   | Periodisch (0=false, 1=true)                                    |
| 5c  | C   | Name                                                            |
| 5d  | C   | Start-Zeitpunkt (im Format „yyyymmddhhmm“)                      |
| 5e  | C   | End-Zeitpunkt (im Format „yyyymmddhhmm“)                        |
| 5f  | C   | Tages Start-Zeitpunkt (im Format „hhmm“)                        |
| 5g  | C   | Tages End-Zeitpunkt (im Format „hhmm“)                          |
| 5h  | C   | Wochen Start-Zeitpunkt (0=keinen Angabe, 1=Montag, 2=Dienstag…) |
| 5j  | C   | Wochen End-Zeitpunkt (0=keinen Angabe, 1=Montag, 2=Dienstag…)   |
| 5k  | R   | Wert                                                            |
| 5l  | C   | Zeitpräferenzkategorie.Kürzel                                   |
| 5m  | C   | Team.Kürzel                                                     |
| 5n  | N   | Ganztägig (0=false, 1=true)                                     |
| 5o  | N   | SystemCreated (0=false, 1=true)                                 |
| 6a  | C   | Typ (Sperrung oder Kernzeit)                                    |
| 6b  | N   | Periodisch (0=false, 1=true)                                    |
| :   | :   | :                                                               |

## Zeilentyp “S1”

| Nr  | Typ | Bedeutung                            |
| --- | --- | ------------------------------------ |
| 1.  | C   | Zeilentyp S1 – Lehrer-Soll-Schlüssel |
| 2.  | C   | Kürzel                               |
| 3.  | C   | Langname                             |
| 4.  | C   | Schlüsseltyp                         |

## Zeilentyp “T1”

| Nr  | Typ | Bedeutung                        |
| --- | --- | -------------------------------- |
| 1.  | C   | Zeilentyp T1 – Stundentafeldaten |
| 2.  | N   | ID                               |
| 3.  | C   | Stundentafel Kürzel              |
| 4.  | C   | Stundentafel Bezeichnung         |
| 5.  | C   | Profil.Kürzel                    |
| 6.  | C   | Bildungsgang.Kürzel              |
| 7.  | N   | Jahrgangsstufe                   |
| 8.  | N   | Anzahl der Einträge/Fächer       |
| 9a  | C   | Fachkürzel                       |
| 9b  | C   | Unterrichtsart.Kürzel            |
| 9c  | R   | Soll                             |
| 9d  | R   | Soll-Min                         |
| 9e  | R   | Soll-Max                         |
| 9f  | R   | Differenz                        |
| 9g  | R   | Wertfaktor                       |
| 9h  | R   | Bemerkung                        |
| 9i  | R   | Unterrichtsform.Kürzel           |
| 9j  | R   | Unterrichtskategorie.Kürzel      |
| 9k  | R   | Lehrbereich.Kürzel               |
| 10a | C   | Fachkürzel                       |
| 10b | C   | Unterrichtsart.Kürzel            |
| 10c | R   | Soll                             |
| 10d | R   | Soll-Min                         |
| 10e | R   | Soll-Max                         |
| 10f | R   | Differenz                        |
| 10g | R   | Wertfaktor                       |
| 10h | R   | Bemerkung                        |
| 10i | R   | Unterrichtsform.Kürzel           |
| 10j | R   | Unterrichtskategorie.Kürzel      |
| 10k | R   | Lehrbereich.Kürzel               |
| :   | :   | :                                |

## Zeilentyp “U0”

| Nr  | Typ | Bedeutung                                                         |
| --- | --- | ----------------------------------------------------------------- |
| 1.  | C   | Zeilentyp U0 - Zeitrahmen                                         |
| 2.  | D   | Anfangsdatum des Plans im Format JJJJMMTT                         |
| 3.  | D   | Enddatum des Plans im Format JJJJMMTT                             |
| 4.  | D   | Anfangsdatum des Gültigkeitszeitraums im Format JJJJMMTT          |
| 5.  | D   | Enddatum des Gültigkeitszeitraums im Format JJJJMMTT              |
| 6.  | C   | Wochenbezogener Unterricht (W=Ja, sonst=Nein)                     |
| 7.  | C   | Ferienwochen (X=markiert, - = nicht markiert), wenn Feldnr.3=W    |
| 8.  | N   | Positionen je Tag                                                 |
| 9.  | N   | Einheiten je Position                                             |
| 10. | N   | Von Tag (1=Montag...7=Sonntag)                                    |
| 11. | N   | Bis Tag (1=Montag...7=Sonntag)                                    |
| 12. | N   | Minuten je Einheit                                                |
| 13a | C   | Uhrzeit der 1. Position, z.B. 8:00                                |
| 13b | C   | Uhrzeit der 2. Position                                           |
| :   | :   | :                                                                 |
| :   | C   | Uhrzeit der <Feld 5>. Position (Anzahl siehe „Positionen je Tag“) |

## Zeilentyp “UA”

| Nr  | Typ                            | Bedeutung                          |
| --- | ------------------------------ | ---------------------------------- |
| 1.  | C                              | Zeilentyp UA – Zeitrahmen          |
| 2.  | N                              | Positionen je Tag                  |
| 3.  | N                              | Einheiten je Position              |
| 4.  | N                              | Minuten je Einheit                 |
| 5a  | C                              | Uhrzeit der 1. Position, z.B. 8:00 |
| 5b  | C                              | Uhrzeit der 2. Position            |
| :   | :                              | :                                  |
| C   | Uhrzeit der <Feld 5>. Position |

## Zeilentyp “UC”

| Nr  | Typ | Bedeutung                                     |
| --- | --- | --------------------------------------------- |
| 1.  | C   | Zeilentyp UC – Veranstaltungsdaten            |
| 2.  | N   | Laufende Block-/Veranstaltungsnummer          |
| 3.  | C   | DAVINCI Veranstaltungs GUID                   |
| 4.  | C   | Kundenspezifische ID                          |
| 5.  | C   | "E"=einmaliger Kurs, sonst wöchentlicher Kurs |
| 6.  | C   | Veranstaltungsart                             |
| 7.  | N   | Kundenspezifisches Provider Kennzeichen       |

## Zeilentyp “U1”

| Nr  | Typ | Bedeutung                                                                                |
| --- | --- | ---------------------------------------------------------------------------------------- |
| 1.  | C   | Zeilentyp U1 – Veranstaltungsdaten                                                       |
| 2.  | N   | Laufende Block-/Veranstaltungsnummer                                                     |
| 3.  | C   | Klassen-/Jahrgangskürzel (bei mehr als einer Klasse für Kurs wird zusätzlich U6 erzeugt) |
| 4.  | C   | Lehrerkürzel                                                                             |
| 5.  | C   | Unterrichtsart-Kürzel                                                                    |
| 6.  | C   | Fachstatus-Kürzel                                                                        |
| 7.  | C   | Fach-/Kursbezeichnung für die Anzeige                                                    |
| 8.  | C   | Raumkürzel des Vorgaberaums oder Variablenbezeichner                                     |
| 9.  | R   | Dauer (Stundenanzahl)                                                                    |
| 10. | C   | Bemerkung                                                                                |
| 11  | R   | Klassenfaktorzähler                                                                      |
| 12  | R   | Klassenfaktornenner                                                                      |
| 13  | R   | Lehrerfaktorzähler                                                                       |
| 14  | R   | Lehrerfaktornenner                                                                       |
| 15. | N   | Schüleranzahl                                                                            |
| 16. | N   | Tagesposition                                                                            |
| 17. | N   | Eckstunde (Optionsnr. “1”..”4”)                                                          |
| 18. | C   | Periodenkürzel                                                                           |
| 19. | N   | Schema - *unbenutzt!*                                                                    |
| 20. | C   | Zeitschiene (X, Y, A, B...)                                                              |
| 21. | C   | Wochenfaktor automatisch berechnen (N=Nein, sonst=Ja);                                   |
| 22. | C   | Klassenfaktor ist Lehrerfaktor (N=Nein, sonst=Ja);                                       |
| 23. | C   | VeranstaltungsNr.                                                                        |
| 24. | C   | Blockbezeichner                                                                          |
| 25. | C   | Fach-Schlüssel                                                                           |
| 26. | R   | Lehrer-Ist                                                                               |
| 27. | R   | Klassen-Ist                                                                              |
| 28. | D   | VonDatum                                                                                 |
| 29. | D   | BisDatum                                                                                 |
| 30. | C   | Fachkürzel                                                                               |
| 31. | C   | Schulnummer                                                                              |
| 32. | C   | Merkmale (Kursplan)                                                                      |
| 33. | C   | Differenzierung                                                                          |
| 34. | C   | Intern                                                                                   |
| 35. | C   | Unterrichtsform.Kuerzel                                                                  |
| 36. | C   | Schulform.Kuerzel                                                                        |
| 37. | C   | Kategorie.Kuerzel                                                                        |
| 38. | C   | Merkmal.Kuerzel                                                                          |
| 39. | N   | Kursnummer                                                                               |
| 40. | N   | Kurs-Index (eindeutiger Index des Kurse im Plan, nur für DAVINCI Export)                 |

## Zeilentyp “U2”

| Nr  | Typ | Bedeutung                                                                      |
| --- | --- | ------------------------------------------------------------------------------ |
| 1.  | C   | Zeilentyp U2 – Veranstaltungsdaten (nur bis DAVINCI 5, für DAVINCI 6 siehe U8) |
| 2.  | N   | Laufende Block-/Veranstaltungsnummer                                           |
| 3.  | N   | Anzahl der gesetzten Termine                                                   |
| 4a  | N   | Tag (Montag “1”..”7”Sonntag)                                                   |
| 4b  | N   | Stunde (Startposition in Einheiten)                                            |
| 4c  | R   | Dauer                                                                          |
| 4d  | C   | Raumkürzel                                                                     |
| 4e  | C   | Lehrerkürzel                                                                   |
| 4f  | C   | Stunde fix “f” oder variabel “v”                                               |
| 5a  | N   | Tag (Montag “1”..”7”Sonntag)                                                   |
| 5b  | N   | Stunde (Startposition in Einheiten)                                            |
| 5c  | R   | Dauer                                                                          |
| 5d  | C   | Raumkürzel                                                                     |
| 5e  | C   | Lehrerkürzel                                                                   |
| 5f  | C   | Stunde fix “f” oder variabel “v”                                               |
| :   | :   | :                                                                              |

## Zeilentyp “U4”

| Nr  | Typ | Bedeutung                                |
| --- | --- | ---------------------------------------- |
| 1.  | C   | Zeilentyp U4 – Veranstaltungsdaten       |
| 2.  | N   | Laufende Block-/Veranstaltungsnummer     |
| 3.  | N   | Anzahl der Vorgaberäume in der Raumliste |
| 4.  | C   | Raumkürzel 1                             |
| 5.  | C   | Raumkürzel 2                             |
| :   | :   | :                                        |

## Zeilentyp “U5”

| Nr  | Typ | Bedeutung                               |
| --- | --- | --------------------------------------- |
| 1.  | C   | Zeilentyp U5 – Veranstaltungsdaten      |
| 2.  | N   | Laufende Block-/Veranstaltungsnummer    |
| 3.  | C   | Wochen (X=markiert, - = nicht markiert) |

## Zeilentyp “U6”

| Nr  | Typ | Bedeutung                                                                          |
| --- | --- | ---------------------------------------------------------------------------------- |
| 1.  | C   | Zeilentyp U6 – Veranstaltungsdaten<br>(wird nur bei mehr als einer Klasse erzeugt) |
| 2.  | N   | Laufende Blocknummer                                                               |
| 3.  | N   | Anzahl der Klassen                                                                 |
| 4.  | C   | Klassenkürzel 1                                                                    |
| 5.  | C   | Klassenkürzel 2                                                                    |
| :   | :   | :                                                                                  |

## Zeilentyp “U7”

| Nr  | Typ | Bedeutung                                     |
| --- | --- | --------------------------------------------- |
| 1.  | C   | Zeilentyp U7 – Termindaten                    |
| 2.  | C   | Block-ID der Veranstaltung (Blockbezeichnung) |
| 3.  | N   | Anzahl der Termine                            |
| 4a  | C   | DAVINCI Termin GUID                           |
| 4b  | C   | Kundenspezifische Termin ID                   |
| :   | :   | :                                             |

## Zeilentyp “U8”

| Nr  | Typ | Bedeutung                                                                             |
| --- | --- | ------------------------------------------------------------------------------------- |
| 1.  | C   | Zeilentyp U8 – Termindaten                                                            |
| 2.  | C   | Block-ID der Veranstaltung (Blockbezeichnung)                                         |
| 3.  | N   | Anzahl der Termine                                                                    |
| 4.  | C   | Start-Zeitpunkt (im Format „yyyymmddhhmm“)                                            |
| 5.  | C   | Ende-Zeitpunkt (im Format „yyyymmddhhmm“)                                             |
| 6.  | N   | Wochentag (0=keine Angabe, 1=Montag, 2=Dienstag,…)                                    |
| 7.  | N   | Schiene (0='A', 1='B', 2='C', 3='D', 4='E', 5='X', 6='Y')                             |
| 8.  | R   | Solldauer in Minuten                                                                  |
| 9.  | C   | Block-ID des Termins (Blockbezeichnung des Termins)                                   |
| 10. | C   | Lehrerkürzel (wenn der Termin mehrere Lehrer hat, wird hier nur der erste ausgegeben) |
| 11. | C   | Raumkürzel (wenn der Termin mehrere Räume hat, wird hier nur der erste ausgegeben)    |
| 12. | C   | Stunde fix “f” oder variabel “v”                                                      |
| 13. | C   | Bemerkung                                                                             |
| 14. | C   | Start-Zeitpunkt (im Format „yyyymmddhhmm“)                                            |
| 15. | C   | Ende-Zeitpunkt (im Format „yyyymmddhhmm“)                                             |
| 16. | N   | Wochentag (0=keine Angabe, 1=Montag, 2=Dienstag,…)                                    |
| 17. | N   | Schiene (0='A', 1='B', 2='C', 3='D', 4='E', 5='X', 6='Y')                             |
| 18. | R   | Solldauer in Minuten                                                                  |
| 19. | C   | Block-ID des Termins (Blockbezeichnung des Termins)                                   |
| 20. | C   | Lehrerkürzel (wenn der Termin mehrere Lehrer hat, wird hier nur der erste ausgegeben) |
| 21. | C   | Raumkürzel (wenn der Termin mehrere Räume hat, wird hier nur der erste ausgegeben)    |
| 22. | C   | Stunde fix “f” oder variabel “v”                                                      |
| 23. | C   | Bemerkung                                                                             |
| :   | :   | :                                                                                     |

## Zeilentyp “V1”

| Nr  | Typ | Bedeutung                                                          |
| --- | --- | ------------------------------------------------------------------ |
| 1.  | C   | Zeilentyp V1 – Versionsangaben                                     |
| 2.  | C   | Version des Datenformats dieser Datei                              |
| 3.  | C   | Name des erzeugenden Applikation, z.B. „DAVINCI6“ oder „MAGELLAN6“ |
| 4.  | C   | Version der erzeugenden Applikation                                |

## Zeilentyp “W1”

| Nr  | Typ | Bedeutung                               |
| --- | --- | --------------------------------------- |
| 1.  | C   | Zeilentyp W1 – Periodenschema           |
| 2.  | N   | ID                                      |
| 3.  | C   | Kürzel                                  |
| 4.  | C   | Bezeichnung                             |
| 5.  | N   | Faktor Zähler                           |
| 6.  | N   | Faktor Nenner                           |
| 7.  | N   | Faktor2 Zähler                          |
| 8.  | N   | Faktor2 Nenner                          |
| 9.  | C   | Wochen (X=markiert, - = nicht markiert) |

## Zeilentyp “Z1”

| Nr  | Typ | Bedeutung                                                             |
| --- | --- | --------------------------------------------------------------------- |
| 1.  | C   | Zeilentyp Z1 – Zeitraumdaten                                          |
| 2.  | N   | ID                                                                    |
| 3.  | C   | Kürzel                                                                |
| 4.  | C   | Bezeichnung                                                           |
| 5.  | D   | VonDatum im Format JJJJMMTT                                           |
| 6.  | D   | BisDatum im Format JJJJMMTT                                           |
| 7.  | N   | Aktueller Zeitraum (0=nein, 1=ja), nur ein Zeitraum kann aktuell sein |