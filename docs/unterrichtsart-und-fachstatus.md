# Unterrichtsart und Fachstatus

Die Datensätze U1, T1, P1 und in den D-Datensätzen enthalten die Felder „Unterrichtsart“ bzw. „Fachstatus“. Lassen Sie diese Felder leer oder achten Sie darauf, dass diese Felder die korrekten in
DAVINCI verwendeten Schlüssel (NICHT die Kürzel) enthalten.

In DAVINCI kann man unter `Extras > Schlüsselverzeichnisse` Fachstatus und Unterrichtsarten definieren
und zwar je Eintrag „Kürzel“ und „Schlüssel“. Beide Schlüsselverzeichnisse werden NICHT als Stammdaten im Schuldatentransferformat übertragen. Die Standardvorgaben in DAVINCI sollten vom Benutzer nicht geändert werden, da andernfalls Fachwahlüberprüfungen und amtliche Statistiken nicht mehr korrekt funktionieren. Die am häufigsten verwendeten Vorgabeschlüssel sind:

Fachstatus:

Schlüssel | Bedeutung
--------- | ---------
Standard  | Standardeinstellung
AufgestGK | Aufgestockter Grundkurs
1PF       | 1. Prüfungsfach
2PF       | 2. Prüfungsfach
3PF       | 3. Prüfungsfach
4PF       | 4. Prüfungsfach
Befreit   | Vom Unterrcht befreit
Freiw     | Freiwilliger Unterricht
Wahlb     | Wahlbereich

Unterrichtsart:

Schlüssel | Bedeutung
--------- | ---------
Kurs      | Standardeinstellung
GK        | Grundkurs
LK        | Leistungskurs