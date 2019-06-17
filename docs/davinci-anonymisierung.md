# DAVINCI-Anonymisierung

Die folgenden Datentypen können zur Anonymisierung von Lehrer und Schülerdaten verwendet werden. Beim Importieren werden Name, E-Mail, Ort, Telefonnummer und Benutzerkennung anonymisiert.

## Zeilentyp „XT“

| Nr  | Typ | Bedeutung                                 |
| --- | --- | ----------------------------------------- |
| 1.  | C   | Zeilentyp XT – Lehrernamen Anonymisierung |
| 2.  | C   | Kürzel                                    |
| 3.  | C   | Vorname                                   |
| 4.  | C   | Nachname                                  |
| 5.  | C   | Mittelname                                |
| 6.  | C   | Titel                                     |
| 7.  | C   | Geschlecht \(„w“=weiblich, „m“=männlich\) |

## Zeilentyp „XS“

| Nr  | Typ | Bedeutung                                  |
| --- | --- | ------------------------------------------ |
| 1.  | C   | Zeilentyp XS – Schülernamen Anonymisierung |
| 2.  | C   | Vorname                                    |
| 3.  | C   | Nachname                                   |
| 4.  | C   | Mittelname                                 |
| 5.  | C   | Geschlecht \(„w“=weiblich, „m“=männlich\)  |


## Einfaches Schülernamen Format

Vereinfachter Datensatz für das Importieren vom Schülernamen aus einer Textdatei. Datensatz ohne Zeilentyp, Vornamen und Nachname durch Leerzeichen getrennt.

#### Beispiel
```
Albert Einstein
Robert Koch

```
