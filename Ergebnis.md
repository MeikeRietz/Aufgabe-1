# Datenprozesse in der Stadtbibliothek Köln

Die Stadtbibliothek Köln ist eine der größten öffentlichen Bibliotheken Deutschlands. Täglich nutzen mehrere Tausend Bibliothekskunden die Einrichtungen der Stadtbibliothek Köln. Um die vielfältigen Dienstleistungen anzubieten, bedarf es enorme Ressourcen an Mitarbeitenden sowie technischer Ausstattung. So kommt es in unterschiedlichen Aufgabengebiete zu der Erfassung und Bearbeitung von Datenmassen.    
In diesem Repositorium werden vier dieser Aufgabengebiete gelistet und Aufkommen und Umgang mit den Daten kurz erläutert. Der letzte Datenprozess soll eingehend beleuchtet und Verbesserungspotential erkannt werden. 

**Inhalt:**  
[1. Kataloganreicherung durch Metadatenimporte](#Metadatenimporte)  
[2. Datenerfassung bei der Benutzeranmeldung](#Benutzeranmeldung)  
[3. Datenerfassung innerhalb der EDV: Inventar](#Inventar)  
[4. Archivierung von Bildmaterial](#Bildmaterial)  
[Quellen](#Quellen)



## 1. Kataloganreicherung durch Metadatenimporte <a name="Metadatenimporte" /></a>

Die Metadaten werden entweder über einen FTP-Server-Zugriff beim HBZ heruntergeladen oder durch die entsprechenden Dienstleister zugesandt. Mit der Software wfl-Load werden die Daten in ein dem Kalatog entsprechenden Format konvertiert. Mit der Software Tom21 können die Metadaten anschließend in den Katalog hochgeladen werden.   

Folgende Daten werden importiert: 

**- Daten der DNB (Reihe A, Reihe N, Reihe M, Reihe T):**  
Dabei handelt es sich um Katalogdatensätze, die wöchentlich durch das HBZ bereitgestellt werden. Die Reihe N beinhaltet Neuerscheinungen und noch unvollständige Datensätze. Diese Daten werden vor allem für die Lektoratsrecherchen und Bestellungen verwendet. Reihe A beinhaltet korrigierte Datensätze, die für die Bestandsrecherchen wichtig sind. Die Reihe M und Reihe T handelt es sich um Datensätze zu Musikalien und Musiktonträgern.¹ Alle Reihen werden in die "TFE", also in das Fremddatenübernahme-Tool des Katalogs geladen, wo sie für die Katalogisierung, für das Lektorat und die Erwerbung einsehbar sind. Die Änderungen aus Reihe A werden ins Live System übertragen.

**- Daten von Hugendubel:**  
Bei den Metadatenlieferungen der Firma Hugendubel handelt es sich um Datensätze zu bestellten DVDs und Blurays. Sie beinhalten neben zum Beispiel Titel, Schauspieler, Regisseur, Laufzeit und Sprachen eine kurze Zusammenfassung des Inhalts.

**- Daten der Divibib:**  
Die Daten der Divibib beinhalten alle Titel, die in der Onleihe durch die Stadtbibliothek Köln bereitgestellt werden. Dabei handelt es sich um eBooks, eAudios, eLearning und weitere Angebote. Außerdem wird nomatlich eine Liste von Medien erzeugt, die aus dem digitalen Angebot entfernt wurden. Diese Daten gleicht der Anbieter des Library Management Systems mit dem Live System ab. 

**- Munzinger-Daten** (Kataloganreicherungen, die auf das Munzinger-Archiv verweisen) 

**- Zukünfig:** Filmfried, OverDrive



## 2. Datenerfassung bei der Benutzeranmeldung <a name="Benutzeranmeldung" /></a>

Bei der **Benutzeranmeldung** werden folgende Daten in der Eingabemaske im Librabry Manegment System "Concerto" erfasst:  
- Name
- Geburtsdatum
- Geschlecht
- Adresse (Straße, Hausnummer, Postleitzahl)
- Optional: Telefonnummer, E-Mail-Adresse

Bei **Kindern und Jugendlichen** unter 18 Jahren:  
- Name, Geburtstdatum, Adresse der bürgenden Person oder der erziehungsberechtigten Person

**Dauermitglieder**:  
- IBAN zur Abbuchung des regelmäßigen Mitgliedsbeitrags 

Folgende Daten werden überprüft, aber nicht erfasst:  
- Bei Personen mit Anrecht auf Ermäßigung: Studierendenausweis, Ausbildungsnachweis, Köln-Pass, Schwerbehindertenausweis

Jeder Datensatz wird an eine 10-stellige Ausweisnummer geknüpft.

Weitere Informationen für Kundinnen und Kunden zur Anmeldung sind auf der Website der Stadtbibliothek Köln zu finden.²


## 3. Datenerfassung innerhalb der EDV: Inventar <a name="Inventar" /></a>

Die IT-Aufstellung der Stadtbibliothek Köln ist unabhängig vom Rechenzentrum der Stadt Köln, was bedeutet, dass eine hauseigene EDV-Abteilung das System wartet und betreut. Innerhalb dieser Abteilung wird mit dem Managementsystem OTRS⁴ gearbeitet, welches eine Strukturierung von eingehenden Daten innerhalb eines Ticketsystems ermöglicht.

Die EDV-Abteilung der Stadtbibliothek Köln betreibt über 1000 Endgeräte für Mitarbeiter und Bibliothekskunden. Dazu zählen zahlreiche Server, 350 Clients für Mitarbeiter und Kunden, über 30 Selbstbedienungsgeräte für Kundinnen und Kunden, mehrere Hundert Drucker, Bildschirme und vieles mehr. Die EDV-Abteilung ist verantwortlich für die Beschaffung, den Betrieb und die Weiterentwicklung (Austausch der Hardware bei Defekt oder falls veraltet) der Hardwarekomponenten.

Einen großen Bestandteil neben dem Ticketsystem ist also die Datenbank des Inventars. Hier wird die gesamte IT-Infrastruktur inventarisiert in den Gruppen:    

- Computer (Computer und Notebooks)
- Hardware (Monitore, RFID-Verbuchungsplatten, Handscanner, Magnetkartentastaturen, (Quittungs-)Drucker, iPads und Tablets, Server und Serverkomponenten, Ferseher und Screens etc.)
- Software (Concerto, Office 2016, Concerto, McAfee etc.)
- Netzwerk (Kundennetz, Bibliothektsnetz etc.)
- Standort (Zentralbibliothek (Abteilung Lektorat, etc.) o. Zweigstelle)

Alle Elemente lassen sich beliebig miteinander verknüpfen. Bei dem Datensatz eines regulären Bibliotheks-PCs werden folgende Daten erfasst:

- Name (PC-Kennung, Gliederungskürzel, Seriennumer, Anlagennummer)
- Verwendungsstatus (Produktiv/Außer Dienst)
- Anbieter (Herstellername)
- Model
- Beschreibung (Vermerk zum Lieferschein)
- Typ (Blibliotheks-PC/Kunden-PC)
- Seriennummer
- Betriebssystem
- CPU
- Arbeitspeicher
- Festplatte
- IP-Adresse
- Grafik Adapter
- Garantie Ablaufdatum
- Installationsdatum

Der Datensatz wiederum wird mit entsprechenden Hardware-, Software-, Netzwerk- und Standort-Einträgen verknüpft. 




## 4. Archivierung von Bildmaterial <a name="Bildmaterial" /></a>

Die Stadtbibliothek pflegt im Social Media Bereich folgende Kanäle: Twitter, Facebook, Instagram, YouTube und einen Blog bei Wordpress. Dies führt zwangsläufig dazu, dass Bild- und Videomaterial gesammelt wird, welches für die Social Media Kanäle, aber auch für die Website, Flyer, Plakate, Pressemeldungen etc. verwendet werden kann. 

Sowohl im Alltag, als auch bei stattfindenden Veranstaltungen, wird Bildmaterial von vielen verschiedenen Personen gesammelt und dezentral - meist lokal auf dem eigenen Büro-PC - abgelegt. Nur selten wird das Bidlmaterial auf dem zentralen NAS³, dem Dateiserver des Betriebs, gespeichert und so für alle Personen zugänglich gemacht. Selbst wenn das Bildmaterial auf dem Netzlaufwerk gespeichert wird, liegt keine einheitliche Struktur zur Ablage vor: Meist werden veranstaltungsbezogene Ordner erstellt, doch dort sind die Bilder selten durch einen speziellen Dateinamen gekennzeichnet oder geben Hinweise auf eine eventuell vorliegende Bildfreigabe. Denn diese ist notwendig, um Bilder konfliktfrei veröffentlichen zu dürfen.

An dieser Stelle ist eine Verbesserung der Situation unerlässlich. Wünschenswert wäre eine Software, die als Bildarchiv fungiert und somit ein gezieltes Suchen nach Bildmaterial möglich macht. Folgende Metadaten wären hierbei notwendig: Datum, Ort, Verschlagwortung (Bsp.: Vorlesen, 3D-Drucker, MINT, Interkulturell etc.), Bildfreigabe (ja, nein, beschränkt) und Autor. 

Denkbar wäre neben der Einigung auf eine einheitliche Ablagestruktur der Einsatz einer kostenpflichtigen Datenbank wie  _Cumulus_ der Firma _Canto_ ⁵.
  
  
  
  
**Quellen:** <a name="Quellen" /></a>  
¹ Deutsche Nationalbibliothek, _Metadienste_     URL:https://www.dnb.de/DE/Professionell/Metadatendienste/Metadaten/Nationalbibliografie/nationalbibliografie_node.html, abgerufen am 06.05.2020    
² Stadtbibliothek Köln, _Mitgliedschaft_     
URL:https://www.stadt-koeln.de/leben-in-koeln/stadtbibliothek/mitgliedschaft, abgerufen am 06.05.2020    
³ Wikipedia, _Network Attached Storage_    
URL:https://de.wikipedia.org/wiki/Network_Attached_Storage, abgerufen am 06.05.2020        
⁴ OTRS, _Produktwebsite_    
URL:https://otrs.com/de/home/, abgerufen am 06.05.2020        
⁵ Canto, _Cumulus_    
URL:https://www.canto.com/de/cumulus/, abgerufen am 06.05.2020

