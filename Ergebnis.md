# Datenprozesse in der Stadtbibliothek Köln

In der Stadtbibliothek Köln kommt es in unterschiedlichen Aufgabengebiete zu der Erfassung und Bearbeitung von Datenmassen.
In diesem Repositorium werden drei verschiedene dieser Stellen gelistet und kurz erörtert. Der letzte Datenprozess soll eingehend beleuchtet und Verbesserungspotential erkannt werden. 



## 1. Kataloganreicherung durch Metadatenimporte 

Folgende Daten werden in den Katalog der Stadtbibliothek Köln importiert

- Daten der DNB (Reihe A, Reihe N, Reihe M, Reihe T)
Dabei handelt es sich um Katalogdatensätze, die wöchentlich durch das HBZ bereitgestellt werden. Die Reihe N beinhaltet Neuerscheinungen und noch unvollständige Datensätze. Diese Daten werden vor allem für die Lektoratsrecherchen und Bestellungen verwendet. Reihe A binhaltet korrigierte Datensätze, die für die Bestandsrecherchen wichtig sind. Die Reihe M und Reihe T handelt es sich um Datensätze zu Musikalien und Musiktonträgern.¹ Alle Reihen werden in die "TFE", als in das Fremddatenübernahme-Tool des Katalogs geladen, wo sie für die Katalogisierung, für das Lektorat und die Erwerbung einsehbar sind. Die Änderungen aus Reihe A werden ins Live System übertragen.

- Daten von Hugendubel 
Bei den Metadatenlieferungen der Firma Hugendubel handelt es sich um Datensätze zu bestellten DVDs und Blurays. Sie beinhalten neben zum Beispiel Titel, Schauspieler, Regisseur, Laufzeit und Sprachen eine kurze Zusammenfassung des Inhalts.

- Daten der Divibib 
Die Daten der Divibib beinhalten alle Titel, die in der Onleihe durch die Stadtbibliothek Köln bereitgestellt werden. Dabei handelt es sich um eBooks, eAudios, eLearning und weitere Angebote. Außerdem wird nomatlich eine Liste von Medien erzeugt, die aus dem digitalen Angebot entfernt wurden. Diese Daten gleicht der Anbieter des Library Management Systems mit dem Live System ab. 

- Munzinger-Daten (Kataloganreicherungen, die auf das Munzinger-Archiv verweisen) 

Zukünfig: Filmfried, OverDrive



## 2. Datenerfassung bei der Benutzeranmeldung 

Bei der Benutzeranmeldung werden folgende Daten in der Eingabemaske im Librabry Manegment System "Concerto" erfasst
- Name
- Geburtsdatum
- Geschlecht
- Adresse (Straße, Hausnummer, Postleitzahl)
- Optional: Telefonnummer, E-Mail-Adresse

Bei Kindern und Jugendlichen unter 18 Jahren:
- Name, Geburtstdatum, Adresse der bürgenden Person oder der erziehungsberechtigten Person

Dauermitglieder:
- IBAN zur Abbuchung des regelmäßigen Mitgliedsbeitrags 

Folgende Daten werden überprüft, aber nicht erfasst:
- Bei Personen mit Anrecht auf Ermäßigung: Studierendenausweis, Ausbildungsnachweis, Köln-Pass, Schwerbehindertenausweis

Jeder Datensatz wird an eine 10-stellige Ausweisnummer geknüpft.

Weitere Informationen für Kundinnen und Kunden zur Anmeldung sind auf der Website der Stadtbibliothek Köln zu finden.²


## 3. Archivierung von Bildmaterial

Die Stadtbibliothek pflegt im Social Media Bereich folgende Kanäle: Twitter, Facebook, Instagram, YouTube und einen Blog bei Wordpress. Dies führt zwangsläufig dazu, dass Bild- und Videomaterial gesammelt wird, welches für die Social Media Kanäle, aber auch für die Website, Flyer, Plakate, Pressemeldungen etc. verwendet werden kann. 

Sowohl im Alltag, als auch bei stattfindenden Veranstaltungen, wird Bildmaterial von vielen verschiedenen Personen gesammelt und dezentral - meist lokal auf dem eigenen Büro-PC - abgelegt. Nur selten wird das Bidlmaterial auf dem zentralen NAS³, dem Dateiserver des Betriebs, gespeichert und so für alle Personen zugänglich gemacht. Selbst wenn das Bildmaterial auf dem Netzlaufwerk gespeichert wird, liegt keine einheitliche Struktur zur Ablage vor: Meist werden veranstaltungsbezogene Ordner erstellt, doch dort sind die Bilder selten durch einen speziellen Dateinamen gekennzeichnet oder geben Hinweise auf eine eventuell vorliegende Bildfreigabe. Denn diese ist notwendig, um Bilder konfliktfrei veröffentlichen zu dürfen.

An dieser Stelle ist eine Verbesserung der Situation unerlässlich. Wünschenswert wäre eine Software, die als Bildarchiv fungiert und somit ein geziletes Suchen nach Bildmaterial möglich macht. Folgende Metadaten wären hierbei notwendig: Datum, Ort, Verschlagwortung (Bsp.: Vorlesen, 3D-Drucker, MINT, Interkulturell etc.), Bildfreigabe (ja, nein, beschränkt) und Autor. 

Denkbar wäre neben der Einigung auf eine einheitliche Ablagestruktur der Einsatz einer kostenpflichtigen Datenbank wie  _Cumulus_ der Firma _Canto_⁴.






¹https://www.dnb.de/DE/Professionell/Metadatendienste/Metadaten/Nationalbibliografie/nationalbibliografie_node.html
²https://www.stadt-koeln.de/leben-in-koeln/stadtbibliothek/mitgliedschaft
³https://de.wikipedia.org/wiki/Network_Attached_Storage
⁴https://www.canto.com/de/cumulus/

