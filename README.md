= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = =
# **SMART CITIES - SICHERHEITSKONZEPT**


* 13.03.2025 - 1.0
  * Initiale Version

= = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = =

## **Inhalt**
### [1 Einleitung](#1-einleitung-1)
#### [1.1 Übersicht](#11-übersicht-1)
#### [1.2 Kolophon](#12-kolophon-1)
### [2 Architektur und Komponenten](#2-architektur-und-komponenten-1)
#### [2.1 Sensoren (und Aktoren)](#21-sensoren-und-aktoren-1)
#### [2.2 Datenübertragung](#22-datenübertragung-1)
#### [2.3 IoT- und Datenplattformen](#23-iot--und-datenplattformen-1)
#### [2.4 Smart City - Anwendungen](#24-smart-city--anwendungen)
### [3 Strategien und Handlungsempfehlungen](#3-strategien-und-handlungsempfehlungen-1)
#### [3.1 Bestehende Strategien und Handlungsempfehlungen im Überblick](#31-bestehende-strategien-und-handlungsempfehlungen-im-überblick-1)
#### [3.2 Technologieintegration als besondere Herausforderung](#32-technologieintegration-als-besondere-herausforderung-1)
#### [3.3 Kommunale Umsetzungshürden: Zwischen Anspruch und Realität](#33-kommunale-umsetzungshürden-zwischen-anspruch-und-realität-1)
### [4 Richtlinien und Standards](#4-richtlinien-und-standards-1)
#### [4.1 Richtlinien](#41-richtlinien-1)
#### [4.2 Standards](#42-standards-1)
### [5 Weiterführende Ressourcen und Tools](#5-weiterführende-ressourcen-und-tools-1)

***

## **1 Einleitung**
Mit der zunehmenden Digitalisierung gewinnen smarte Technologien eine immer größere Bedeutung für Städte, die ihre Effizienz steigern und ihre Dienstleistungen optimieren möchten. Dazu gehören Sensoren, urbane Datenplattformen und die Integration dieser Systeme in die alltäglichen Abläufe. Dieses Smart City Cybersecurity-Referenzkonzept (nachfolgend: SCCK) verfolgt das Ziel, eine umfassende Sammlung bewährter Ansätze, Standards und Ressourcen rund um Cybersecurity im Smart City-Kontext bereitzustellen. Darüber hinaus enthält es typische Beispiele und Angriffsszenarien für die einzelnen Systemkomponenten. Das SCCK richtet sich insbesondere an Smart City - Teams, die mit der Implementierung von Smart City - Lösungen beauftragt sind und an interessierte Nutzer, die ein besseres Verständnis entwickeln möchten.   

### 1.1 Übersicht
Das Sicherheitskonzept umfasst folgende Schwerpunkte: 

- _Architektur und Komponenten_: Analyse der Sicherheitsanforderungen auf den Ebenen der Sensoren, der Datenübertragung, den Plattformen und Cloud-Systeme und den Anwendungen 

- _Strategien_: Empfehlungen und Maßnahmen zur präventiven Absicherung von Smart City-Systemen. 

- _Richtlinien und Standards_: Auflistung relevanter nationaler und internationaler Sicherheitsstandards. 

- _Weiterführende Informationen_: Weiterführende Ressourcen und Informationen. 

### 1.2 Kolophon
- _Autoren_:  Dieses Konzept wurde in seiner ersten Fassung von einem interdisziplinären Team aus Expertinnen und Experten in den Bereichen Cybersecurity, Smart City-Technologien und kommunaler Verwaltung entwickelt. Die Federführung lag beim  Team Smart City der Stadt Osnabrück, und entstand in Zusammenarbeit mit der Zentrum für Digitalen Entwicklung GmbH, Westhausen. 

- _Mitreden und Mitgestalten_: Zukünftig soll das Dokument auf Basis von Ideen, Feedback und dem Austausch mit weiteren Expert:innen sowie interessierten Netzwerken und Fachgruppen kontinuierlich weiterentwickelt werden. Dadurch bleibt das Konzept nicht nur aktuell, sondern kann sich dynamisch an neue Herausforderungen, Technologien und Erkenntnisse anpassen. Das Sicherheitskonzept ist somit Teil eines kollaborativen Ansatzes, um die digitale Souveränität deutscher Smart Cities zu fördern. Interessierte Städte und Organisationen sind eingeladen, sich an der Weiterentwicklung zu beteiligen. openCode als Plattform wurden bewusst gewählt, da hier die Möglichkeit besteht, aktiv mitzuwirken, Vorschläge einzubringen und von den Erfahrungen anderer Städte zu profitieren.  

- _Finanzierung_: Die Finanzierung der ersten Version dieses Dokuments erfolgte durch eine Förderung des Programms „Modellprojekte Smart Cities“ des Bundesministerium für Wohnen, Stadtentwicklung und Bauwesen sowie der KfW.

- _Lizensierung_: Das Konzept steht unter der **Creative Commons Lizenz (CC BY oder CC BY-SA)**, was bedeutet, dass es frei genutzt, weitergegeben und angepasst werden darf, solange die ursprünglichen Autorinnen und Autoren (Stadt Osnabrück / Team Smart City und Zentrum für Digitale Entwicklung GmbH) genannt werden. Diese Lizenz gewährleistet Offenheit und fördert die Nutzung in einem kollaborativen Umfeld, mit dem Ziel, ein sicheres und nachhaltiges Smart City - Modell in Deutschland zu schaffen. 

***

## **2 Architektur und Komponenten**
In diesem Kapitel wird die typische Architektur von Smart City - Lösungen beschrieben, die von der Datenerfassung durch Sensoren bis zur Nutzung der Daten in spezifischen städtischen Anwendungen reicht. Die verschiedenen Systemkomponenten – Sensoren, Übertragungsinfrastrukturen, IoT-Plattformen und applikationsspezifische Smart City Anwendungen – bilden zusammen ein komplexes Netzwerk.  

Jede dieser Ebenen weist dabei eigene Anforderungen an Sicherheit und Zuverlässigkeit auf. Um den durchgängigen Schutz (sensibler) Daten sowie den unterbrechungsfreien Betrieb sicherzustellen, sind gezielte Sicherheitsmaßnahmen auf allen Ebenen der Architektur unerlässlich. Auf diese Weise können potenzielle Risiken frühzeitig erkannt, kritische Infrastrukturen wirksam geschützt und das Vertrauen in die digitalen Prozesse einer Smart City nachhaltig gestärkt werden. 

### 2.1 Sensoren (und Aktoren)
**_Was ist es?_**

Die erste Ebene in der Smart City - Systemwelt umfasst Geräte, die als Sensoren oder Aktoren fungieren können. Unter Sensoren versteht man im Kontext einer Smart City technische Mess- und Erfassungseinrichtungen, die physikalische oder umweltbezogene Größen aus der städtischen Umgebung aufnehmen, in digitale Daten umwandeln und für nachgelagerte Anwendungen bereitstellen. Dazu zählen beispielsweise Sensoren für Luftqualität, Lärmbelastung, Verkehrsdichte, Füllstände von Abfallbehältern oder Energieverbräuche. Während Sensoren Informationen erfassen und bereitstellen, setzen Aktoren diese Informationen in konkrete Aktionen um. Beispiele dafür sind unter anderem Systeme zur bedarfsgerechten Beleuchtungssteuerung, adaptive Verkehrsregelungen, automatische Bewässerungsanlagen in Grünflächen oder Heizungs-, Lüftungs- und Klimasysteme in öffentlichen Gebäuden. Hier beginnt die Interaktion der Smart City mit ihrer Umgebung. Die Datenübertragung findet hierbei in vielen Fällen drahtlos über Übertragungsinfrastrukturen wie LoRaWAN oder NB-IoT statt.

**_Technologien und ausgewählte Beispiele_**

1. _Sensoren_

- Typische Anwendungsfälle:  

  - **Umweltmonitoring**: Erfassen von Luftqualitätsdaten (z. B. CO₂, NOₓ), Lärmbelastung oder Feinstaubwerten 

  - **Energie- und Ressourcenmanagement**: Messen von Strom- und Wasserverbrauch in öffentlichen Gebäuden und Einrichtungen 

  - **Verkehrs- und Parkraumüberwachung**: Erkennen freier Parkplätze, Zählen von Fahrzeugen, Erhebung von Echtzeit-Verkehrsdaten 

  - **Personenzählung und Besucherströme**: Erfassen von Fußgängerbewegungen in Einkaufsstraßen, auf Plätzen oder in Veranstaltungsbereichen 

- Typische Technologien: 

  - **Optische Sensoren (z. B. Kameras)**: Erfassen visuelle Informationen zur Personen- oder Fahrzeugdetektion und können z. B. für Parkraum- oder Sicherheitsüberwachung eingesetzt werden 

  - **Infrarotsensoren**: Registrieren Wärmequellen und Bewegungen, beispielsweise zur automatischen Lichtsteuerung oder Personenzählung 

  - **Induktive Zähler**: Messen den Stromfluss in Leitungen oder erkennen metallische Objekte (Fahrzeuge) und werden häufig im Energiemanagement oder bei Ampelsteuerungen genutzt 

  - **Ultraschall-Sensoren**: Bestimmen Abstände durch Schallwellenreflexion und finden Anwendung bei Parkraumüberwachung, Füllstandsmessungen oder Verkehrssteuerungen 

  - **Chemische Sensoren**: Erfassen spezifische Schadstoffe (z. B. CO₂, NOₓ, Ozon) und andere Luftqualitätsparameter, um die Umweltsituation kontinuierlich zu überwachen 

- Besonderheit: Die einzelnen Sensoren sind in der Regel mit einem Übertragungsnetz verbunden, das die erhobenen Daten in Echtzeit an eine zentrale Plattform weiterleitet. Dort werden sie ausgewertet und für unterschiedliche Smart City-Anwendungen bereitgestellt – von der Verkehrssteuerung über das Energiecontrolling bis hin zur Umweltanalyse. 

2. _Aktoren_

- Typische Anwendungsfälle:  

  - **Ampel- und Verkehrssteuerung**: Automatische Anpassung von Ampelphasen basierend auf Verkehrsdaten 

  - **Straßenbeleuchtung**: Bedarfsorientierte Lichtregelung, z. B. abhängig von Helligkeit, Bewegungen oder Uhrzeit 

  - **Parkraummanagement**: Steuern von Schranken oder Parkbarrieren zur Regelung der Ein- und Ausfahrten und Parkraumbewirtschaftung 

  - **Gebäudeautomation**: Automatisierte Heizungs-, Lüftungs- und Klimasteuerung sowie Jalousien- oder Rolladensteuerung in öffentlichen Gebäuden 

- Typische Technologien: 

  - **Elektromechanische Aktoren**: Ermöglichen die physische Bewegung von Komponenten (z. B. Barrieren, Schranken) durch elektrische Signale 

  - **Leuchtdioden (LED)**: Dienen als zentrale Lichtquelle bei Straßen- und Gebäudebeleuchtung; sie zeichnen sich durch hohe Energieeffizienz und lange Lebensdauer aus 

  - **Hydraulische und pneumatische Systeme**: Kommen zum Einsatz, wenn größere Kräfte oder präzise Bewegungen benötigt werden, beispielsweise beim Heben und Senken von Brücken- oder Schrankenanlagen 

- Besonderheit: Aktoren reagieren in Echtzeit auf Daten, die von Sensoren erfasst und in zentralen Plattformen ausgewertet werden. So lassen sich städtische Infrastrukturen dynamisch an die aktuelle Situation anpassen – etwa durch das Umschalten einer Ampelphase bei hohem Verkehrsaufkommen oder die bedarfsgerechte Regulierung der Straßenbeleuchtung zur Steigerung von Energieeffizienz und Sicherheit.  

3. _Smartphone_

- Typische Anwendungsfälle:  

  - **Bürgerbeteiligung und Feedback**: Meldung von Störungen, Verschmutzungen oder Optimierungsvorschlägen für städtische Infrastruktur 

  - **Navigations- und Verkehrs-Apps**: Echtzeitinformationen über Staus, Baustellen oder freie Parkplätze 

  - **Standortbasierte Smart City Dienste**: Bereitstellung von Angeboten und Services abhängig vom aktuellen Aufenthaltsort 

  - **Umweltbeobachtung**: Erfassung und Meldung von Lärm-, Luft- oder anderen Umweltwerten durch integrierte Gerätesensorik 

- Typische Technologien: 

  - **Integrierte Sensorik (z. B. Kamera, Barometer, Gyroskop, Magnetometer)**: Können für Smart City-Anwendungen genutzt werden, eröffnen vielseitige Einsatzmöglichkeiten für Datenerfassung und Analyse, wie die Aufnahme von Zustandsberichten und Bildern im öffentlichen Raum 

  - **Ortungstechnologien (z.B. GPS, Galileo, GLONASS)**: Ermöglichen standortbasierte Anwendungen, z. B. Navigation, Geofencing oder ortsgebundene Bürgerinformationen 

  - **Mobile Datenübertragung (4G/5G)**: Sorgt für eine flächendeckende Konnektivität in Echtzeit und unterstützt damit zahlreiche Smart City-Anwendungen 

- Besonderheit: Smartphones fördern die direkte, wechselseitige Kommunikation zwischen Stadtverwaltung und Bürgerinnen und Bürgern. Sie ermöglichen die Einbindung der Stadtbevölkerung in Entscheidungsprozesse und sorgen für eine schnelle Rückmeldung von Informationen aus dem öffentlichen Raum. Dadurch entsteht eine dynamische Vernetzung, die Smart City - Dienste effizienter gestaltet und gleichzeitig die Partizipation in der Stadtgemeinschaft stärkt. 

4. _Intelligente Beleuchtung_

- Typische Anwendungsfälle: 

  - **Straßenbeleuchtung**: Dynamische Anpassung der Lichtintensität an Verkehrsaufkommen oder Umgebungshelligkeit 

  - **Signalleuchten in Notfällen**: Erhöhte Sichtbarkeit für Rettungskräfte und Bevölkerung in Krisensituationen 

  - **Öffentliche Plätze und Parks**: Bedarfsgesteuerte Beleuchtung zur Erhöhung der Aufenthaltsqualität und Sicherheit 
 

- Typische Technologien: 

  - **Bewegungssensoren**: Erfassen Personen- und Fahrzeugbewegungen und passen die Lichtstärke bedarfsgerecht an 

  - **Dämmerungssensoren**: Messen das Umgebungslicht und schalten das Licht bei Bedarf automatisch ein oder aus 

  - **Netzwerkfähige Steuerungssysteme**: Ermöglichen die zentrale Verwaltung, Fernüberwachung und -wartung der Beleuchtungseinrichtungen 

  - **LED-Technologie**: Bietet energieeffiziente, langlebige und flexible Beleuchtungslösungen für den städtischen Raum 

- Besonderheit: Durch eine nahtlose Integration in Smart City - Plattformen und andere urbane Systeme können Beleuchtungsanlagen gezielt und in Echtzeit gesteuert werden. Dies reduziert den Energieverbrauch, senkt Betriebskosten und erhöht gleichzeitig die Sicherheit und das Wohlbefinden der Bevölkerung. 

**_Typische Angriffsszenarien_**

In einer Smart City sammeln Sensoren und Aktoren kontinuierlich eine große Menge an städtischen Daten und führen wichtige Aktionen aus. Die hohe Vernetzung und der teils öffentliche Standort dieser Geräte machen sie zu einem möglichen Ziel für Cyberangriffe. Nachfolgend werden ausgewählte Angriffsszenarien beschrieben, die sowohl die Verfügbarkeit als auch die Integrität und Vertraulichkeit der Daten in einer Smart City gefährden können. Die Angriffsszenarien sind entsprechend ihrer Auftrittswahrscheinlichkeit und -häufigkeit aufgelistet. 

_1. Abhören und Abgreifen von Daten_

**Wahrscheinlichkeit**: Hoch 

**Beschreibung**: Drahtlose Sensoren und IoT-Geräte übertragen oft Daten über WLAN, Mobilfunk oder andere Funkstandards. Ohne ausreichende Verschlüsselungsmaßnahmen können Angreifer den Datenverkehr mit relativ geringem Aufwand abfangen.  

**Auswirkungen**: Kompromittierung sensibler Informationen, potenzieller Identitätsdiebstahl oder Auslesen von Zugangsdaten zu kritischen Stadtinfrastrukturen. 

_2. Firmware- und Software-Exploits_

**Wahrscheinlichkeit**: Hoch 

**Beschreibung**: Veraltete Firmware und nicht gepatchte Sicherheitslücken machen IoT-Geräte und Computer anfällig für Angriffe. Angreiferinnen und Angreifer nutzen diese gezielt aus, um Zugriff auf das Gerät oder das umgebende Netzwerk zu erlangen. 

**Auswirkungen**: Da Sicherheitsupdates nicht immer zeitnah durchgeführt werden, nutzen Angreiferinnen und Angreifer oft bekannte Schwachstellen aus, um unbefugt Kontrolle über das Gerät zu erlangen, Daten zu stehlen oder einen Einstiegspunkt für weiterführende Angriffe im gesamten Netz zu schaffen.  

_3. Manipulation und Spoofing von Sensordaten_

**Wahrscheinlichkeit**: Mittel bis hoch 

**Beschreibung**: Angreiferinnen und Angreifer fälschen Sensordaten oder ersetzen sie durch manipulierte Informationen, um beispielsweise Verkehrs- oder Umweltmessungen zu verfälschen.  

**Auswirkungen**: Fehlentscheidungen in städtischen Steuerungssystemen (z. B. falsche Ampelschaltungen oder ungenaue Luftqualitätsmessungen die zu Fehlentscheidungen im System führen) sowie Beeinträchtigungen in der öffentlichen Sicherheit.  

_4. Denial-of-Service (DoS) Angriffe_

**Wahrscheinlichkeit**: Mittel 

**Beschreibung**: DoS-Angriffe auf das Zugangsnetz oder bestimmte IoT-Geräte sind weniger häufig, aber effektiv, um städtische Dienste zu stören. Ziel ist es, den normalen Datenverkehr zu blockieren oder die Netzwerkressourcen zu überlasten, sodass Systeme für legitime Anfragen nicht mehr erreichbar sind.  

**Auswirkungen**: Störungen in städtischen Diensten (z. B. Verkehrsüberwachung) oder zeitweise Ausfälle von Smart City - Anwendungen und -Plattformen. 

_5. Bösartige Aktoren-Befehle_

**Wahrscheinlichkeit**: Mittel bis gering 

**Beschreibung**: Durch das gezielte Übernehmen von Steuerbefehlen können Angreiferinnen und Angreifer z. B. Ampelschaltungen, Schranken oder öffentliche Beleuchtung manipulieren. Diese gezielten Angriffe auf Aktoren erfordern in der Regel tiefergehendes Systemwissen und sind technisch aufwendig. Solche Angriffe können jedoch auftreten, wenn Schwachstellen im Zugangsnetzwerk bestehen. 

**Auswirkungen**: Potenzielle Gefährdung der öffentlichen Sicherheit, erhöhtes Unfallrisiko oder beträchtliche Sachschäden. 

_6. Physischer Zugriff und Sabotage_

**Wahrscheinlichkeit**: Gering 

**Beschreibung**: Sensoren und Aktoren sind oft im öffentlichen Raum installiert und damit potenziell physischen Angriffen und Beschädigungen ausgesetzt. Tatsächlich kommt es eher selten zu gezielten Angriffen oder Sabotageakten – auch weil Hersteller die eingesetzte Technik sicher vor Vandalismus gestalten und Städte entsprechende Vorkehrungen treffen. 

**Auswirkungen**: Schäden können zu Datenlücken, Fehlfunktionen oder einer kompletten Systemunterbrechung führen. Potenzielle Gefährdung der öffentlichen Sicherheit und erhöhtes Unfallrisiko in sicherheitskritischen Bereichen wie Verkehrsmanagement. Beträchtliche Sachschäden. 

### 2.2 Datenübertragung

**_Was ist es?_**

Die Datenübertragung bildet das Rückgrat der digitalen Infrastruktur in einer Smart City. Sie stellt die Verbindung zwischen Sensoren, Aktoren und den zentralen Systemen her, indem sie die erfassten Daten sicher und effizient weiterleitet. Während Sensoren physikalische und umweltbezogene Parameter messen und Aktoren darauf reagieren, ermöglicht die Datenübertragung den kontinuierlichen Austausch dieser Informationen zwischen den verschiedenen Ebenen der Smart City. 

Die Übertragung kann über eine Vielzahl von Technologien erfolgen, je nach Anwendungsfall, Reichweite, Energiebedarf und benötigter Bandbreite. Dabei reicht das Spektrum von drahtlosen Funktechnologien wie LoRaWAN, NB-IoT oder 5G, die für die großflächige Vernetzung von IoT-Geräten genutzt werden, bis hin zu kabelgebundenen Lösungen wie Glasfaser oder Ethernet, die für hochsichere und leistungsstarke Datenübertragungen in kritischen Infrastrukturen zum Einsatz kommen. 

Je nach Technologie unterscheidet sich nicht nur die Übertragungsgeschwindigkeit, sondern auch die Art und Weise, wie Daten gebündelt, gesichert und weiterverarbeitet werden. Um eine zuverlässige und sichere Kommunikation zwischen allen Smart City - Komponenten zu gewährleisten, müssen unterschiedliche Anforderungen an Latenz, Redundanz, Verschlüsselung und Resilienz berücksichtigt werden. 

**_Technologien und ausgewählte Beispiele_**

Die Datenübertragung in Smart Cities erfolgt über verschiedene Netzwerktechnologien, die je nach Anwendung spezifische Anforderungen an Reichweite, Bandbreite, Energieverbrauch und Latenz erfüllen müssen. Während einige Technologien für hohe Datenraten und niedrige Latenzen ausgelegt sind (z. B. Glasfaser, 5G), eignen sich andere für energieeffiziente Übertragungen mit geringen Datenmengen (z. B. LoRaWAN, NB-IoT). Die Auswahl der richtigen Technologie hängt von den jeweiligen Anwendungsfällen und weiteren Überlegungen z.B. zu Sicherheitsaspekten ab. 

Typische Anwendungsfälle: 

- **Echtzeit-Datenübertragung für kritische Anwendungen**: Verkehrssteuerung, Notfallkommunikation, Videoüberwachung 

- **Flächendeckende Vernetzung von IoT-Geräten**: Umweltmonitoring, Energiemanagement, smarte Bewässerungssysteme 

- **Datenkommunikation in hochfrequentierten Bereichen**: WLAN-basierte Besucherzählung, öffentliche Internetzugänge, Mobilitätslösungen 

- **Sichere und redundante Übertragung für resiliente Systeme**: Backup-Netzwerke für kritische Infrastrukturen, verschlüsselte Kommunikationskanäle 

Typische Technologien: 

- **Glasfasernetze – Höchste Bandbreite für datenintensive Anwendungen** 

  - Eigenschaften: Sehr hohe Datenraten, extrem niedrige Latenz, störungsresistent 

  - Einsatzbereiche: Vernetzung von Smart City - Datenzentren, Übertragung großer Datenmengen aus Videoüberwachungssystemen, Anbindung von Edge-Computing-Plattformen 

  - Besonderheit: Aufgrund der hohen Investitionskosten werden Glasfasernetze primär für Backbone-Infrastrukturen genutzt 

- **Mobilfunktechnologien (4G/5G) – Drahtlose Hochgeschwindigkeitsnetze**

  - Eigenschaften: Hohe Bandbreite, mittlere bis niedrige Latenz, flexibel einsetzbar 

  - Einsatzbereiche: Verkehrsmanagement (z. B. 5G-basierte Ampelschaltungen), Notfallkommunikation, IoT-gestützte Steuerung von Stadtbeleuchtung 

  - Besonderheit: 5G ermöglicht die Echtzeit-Kommunikation für vernetzte Fahrzeuge und intelligente Mobilitätslösungen 

- **WLAN (Wi-Fi) – Flexible Nahbereichsübertragung**

  - Eigenschaften: Mittelgroße Reichweite, hohe Bandbreite, nicht flächendeckend 

  - Einsatzbereiche: Luft- und Lärmmessung im urbanen Raum, Besucherzählung in Innenstädten, öffentlicher Internetzugang in Smart City - Zonen 

  - Besonderheit: Wird oft in Kombination mit Mobilfunk- oder Glasfasernetzen genutzt, um gezielte Netzabdeckung bereitzustellen 

- **NB-IoT (Narrowband IoT) – Energieeffiziente Kommunikation für vernetzte Sensoren**

  - Eigenschaften: Sehr geringer Energieverbrauch, tiefes Eindringen in Gebäude, niedrige Datenrate 

  - Einsatzbereiche: Wasserzähler, intelligente Stromnetze (Smart Metering), Gebäudeüberwachung 

  - Besonderheit: Ideal für Anwendungen, die eine langlebige Batterieversorgung und sporadische Datenübertragungen erfordern 

- **LoRaWAN (Long Range Wide Area Network) – Weitreichende, kostengünstige IoT-Kommunikation**

  - Eigenschaften: Sehr hohe Reichweite, extrem niedriger Energieverbrauch, geringe Datenrate 

  - Einsatzbereiche: Füllstandsensoren für Mülltonnen, Parkplatzüberwachung, Luftqualitätsmessungen 

  - Besonderheit: Ermöglicht den Betrieb von großen Sensornetzwerken ohne hohen Infrastrukturaufwand 

**_Typische Angriffsszenarien_**

In einer Smart City bildet die Datenübertragung das Bindeglied zwischen Sensoren, Aktoren und zentralen Systemen. Die ständige Vernetzung und der Austausch großer Datenmengen machen die Kommunikationswege anfällig für Angriffe, die Vertraulichkeit, Integrität und Verfügbarkeit der übertragenen Informationen gefährden können. Neben klassischen Cyberbedrohungen wie Abhören oder Datenmanipulation spielen auch gezielte Störungen und Überlastungsangriffe eine Rolle. 

Die nachfolgenden Angriffsszenarien sind entsprechend ihrer Wahrscheinlichkeit und potenziellen Auswirkungen geordnet und zeigen typische Bedrohungen für die Datenübertragung in Smart Cities auf. 

1. _Abhören und Mitlesen des Datenverkehrs_ 

**Wahrscheinlichkeit**: Hoch 

**Beschreibung**: Angreifer fangen Datenpakete ab, um sensible Informationen wie Standortdaten oder Benutzeraktivitäten auszuspähen. Besonders in unverschlüsselten Netzwerken ist dies ein gängiges Angriffsmuster. Öffentliche WLAN-Netzwerke oder unverschlüsselte IoT-Protokolle sind besonders anfällig. 

**Folgen**: Die Privatsphäre der Bürgerinnen und Bürger wird verletzt, und es können z.B. gezielte Bewegungsprofile erstellt werden. In sicherheitskritischen Bereichen wie Überwachungssystemen oder Zugangskontrollen kann ein solcher Angriff zur Kompromittierung der Stadtinfrastruktur führen. 

2. _Man-in-the-Middle (MitM)-Angriffe_

**Wahrscheinlichkeit**: Mittel bis hoch 

**Beschreibung**: Angreifer schalten sich zwischen die kommunizierenden Geräte, um den Datenverkehr abzufangen, zu manipulieren oder sich als legitime Partei auszugeben. Ohne Sicherheitsmaßnahmen wie TLS (Transport Layer Security) oder Ende-zu-Ende-Verschlüsselung sind viele Smart City - Systeme anfällig für diese Art von Angriff. 

**Folgen**: Verfälschte oder manipulierte Daten können zu Fehlentscheidungen in städtischen Systemen führen, etwa durch falsche Sensordaten für Verkehrsflussanalysen oder manipulative Eingriffe in Energiemanagementsysteme. 

3. _Jamming und Signalstörung_

**Wahrscheinlichkeit**: Mittel 

**Beschreibung**: Angreifer setzen Störsender ein, um drahtlose Kommunikation in Mobilfunk-, WLAN- oder IoT-Netzwerken gezielt zu unterbrechen oder zu blockieren. Besonders LPWAN-Technologien wie LoRaWAN oder NB-IoT sind anfällig für gezielte Signalstörungen. 

**Folgen**: Störungen in der Datenübertragung können den Betrieb kritischer Smart City - Dienste, wie die Verkehrssteuerung oder Notfallsysteme, erheblich beeinträchtigen 

### 2.3 IoT- und Datenplattformen

**_Was ist es?_**

IoT- und Datenplattformen bilden die zentrale Verarbeitungsebene in der Architektur einer Smart City. Sie empfangen, speichern und analysieren Daten aus vernetzten Sensoren und Aktoren, die über verschiedene Kommunikationsnetze übertragen werden. Diese Systeme wandeln Rohdaten in verwertbare Informationen um, die für städtische Entscheidungsprozesse, Automatisierung und übergreifende Analysen essenziell sind. 

In vielen Fällen übernehmen Edge-Systeme bereits eine Vorverarbeitung der Daten an der Quelle – etwa durch Filtern oder Verdichten von Sensormesswerten, bevor diese an zentrale Datenplattformen weitergeleitet werden. Die eigentliche Langzeitspeicherung, übergreifende Analyse und KI-gestützte Entscheidungsfindung erfolgen jedoch auf urbanen Datenplattformen und Cloud-Systemen. 

Durch den Einsatz leistungsfähiger Cloud-Technologien ermöglichen diese Plattformen eine skalierbare und effiziente Datenverarbeitung, die sowohl in Echtzeit als auch für langfristige Analysen genutzt werden kann. Dabei kommen verschiedene Sicherheitsmechanismen wie Zugriffskontrollen, Verschlüsselung und Redundanzstrategien zum Einsatz, um die Integrität, Verfügbarkeit und Vertraulichkeit der Daten zu gewährleisten. 

Diese Plattformen sind ein kritischer Bestandteil smarter Städte, da sie nicht nur Sensordaten bereitstellen, sondern auch als zentrale Schnittstelle zu weiteren städtischen Diensten wie GIS-Systemen und Smart City - Anwendungen dienen. 

**_Technologien und ausgewählte Beispiele_**

In Smart Cities kommen verschiedene IoT- und Datenplattformen zum Einsatz – oft auch mehrere parallel –, um die unterschiedlichen Anforderungen an Datenmanagement, Skalierbarkeit, Sicherheit und Interoperabilität zu erfüllen. Die Auswahl hängt dabei stark von den spezifischen Anwendungsfällen, der bestehenden IT-Infrastruktur und den gewünschten Integrationsmöglichkeiten ab. 

1. _IoT- Datenplattformen_ 
- **Beschreibung**: IoT-Datenplattformen verwalten die Vielzahl an verteilten IoT-Geräten, Sensoren und Aktoren und stellen sicher, dass die Daten zentral gesammelt und gespeichert werden. Sie bieten Speicherlösungen, die große Datenmengen sicher und effizient organisieren. 

- **Anwendungsfälle:** 

  - Verwaltung städtischer Infrastrukturen: Datenplattformen ermöglichen die zentrale Verwaltung von Verkehrssensoren, Wasser- und Energiezählern sowie Umweltsensoren und verbessern die Übersicht und Effizienz städtischer Dienste. 

  - Echtzeit-Überwachung und Wartung: Sensordaten liefern Hinweise auf Wartungsbedarf, z.B. bei Straßenbeleuchtung und Wasserleitungen, wodurch proaktive Instandhaltungsmaßnahmen unterstützt werden 

  - Netzwerk- und Gerätemanagement: Überwachung und Steuerung der Konnektivität und des Zustands der angebundenen IoT-Geräte und Sensoren zur zentralen Verwaltung von Netzwerktopologien, Optimierung von Datenflüssen und frühzeitigen Meldung von Ausfälle oder Störungen 

2. _Urbane Datenplattformen_

- **Beschreibung:** Diese Plattformen führen Datenströme aus verschiedenen Quellen zusammen, um diese zu kombinieren und zu verschneiden und so einheitliche Datensätze für spezielle Anwendungen bereitzustellen. Sie sind entscheidend für städtische Digitalisierungsprojekte, da sie eine zentrale Informationsbasis schaffen, die für weitere Anwendungen genutzt werden kann. 

- **Anwendungsfälle:**

  - Intersektorale Datenanalysen: Integrierte Daten aus Bereichen wie z.B. Verkehr, Energie, Umwelt und Gesundheitswesen werden analysiert, um übergreifende Muster zu erkennen und nachhaltige städtische Entscheidungen zu fördern 

  - Datenbereitstellung für Smart City - Apps: Bürgerinnen und Bürger nutzen Apps, die in Echtzeit Informationen wie Verkehrsstaus, Luftqualität und Lärmbelastung anzeigen, basierend auf integrierten Datensätzen aus verschiedenen städtischen Sensoren 

  - Optimierung des öffentlichen Transports: Daten aus Verkehrssensoren und Fahrzeugortungssystemen werden zusammengeführt, um die Effizienz und Pünktlichkeit des öffentlichen Nahverkehrs zu verbessern 

3. _Urbane Datennutzung und Interoperabilität_

- **Beschreibung:** Urbane Datennutzung und Interoperabilität ermöglichen den Austausch und die Integration städtischer Daten über verschiedene Systeme und Anwendungen hinweg. Sie schaffen vernetzte Datenökosysteme, indem sie offene Schnittstellen und standardisierte Datenformate bereitstellen. Open Data - Portale spielen hierbei eine zentrale Rolle, indem sie Verwaltungsdaten, Sensordaten und Analyseergebnisse öffentlich zugänglich machen. 

- **Anwendungsfälle:** 

  - Offene Dateninfrastruktur: Open Data - Portale ermöglichen den freien Zugang zu städtischen Daten aus Bereichen wie Verkehr, Energie und Umwelt und fördern dadurch Innovationen und datenbasierte Entscheidungen 

  - Dateninteroperabilität und API-Management: Schnittstellen erleichtern den Datenaustausch zwischen städtischen Systemen, externen Anwendungen und Forschungseinrichtungen, um eine einheitliche, vernetzte Nutzung städtischer Informationen zu ermöglichen 

  - Digitale Zwillinge: Durch die Kombination von Echtzeit- und historischen Daten lassen sich virtuelle Stadtmodelle erstellen, die für Simulationen und optimierte Planungsprozesse genutzt werden können 

**_Typische Angrufsszenarien_**

IoT- und Datenplattformen sind ein zentrales Element der Smart City - Infrastruktur und daher ein attraktives Ziel für Cyberangriffe. Auf diesen Plattformen laufen sensible Daten aus verschiedenen Quellen zusammen, die für die Steuerung und Überwachung städtischer Systeme entscheidend sind. Die typischen Angriffsszenarien umfassen folgende Bedrohungen: 

1. _Unbefugter Zugriff und Datenabfluss_

**Wahrscheinlichkeit**: Hoch 

**Beschreibung**: Angreiferinnen oder Angreifer können versuchen, sich Zugang zur Datenplattform zu verschaffen, um auf vertrauliche Informationen zuzugreifen oder Daten zu stehlen. Eine der häufigsten Bedrohungen, da Fehlkonfigurationen, schwache Authentifizierung oder Insider-Bedrohungen immer wieder Sicherheitslücken schaffen. 

**Folgen**: Unbefugter Zugriff kann dazu führen, dass sensible Daten veröffentlicht oder manipuliert werden, was das Vertrauen der Bürgerinnen und Bürger in die Smart City - Systeme untergräbt und rechtliche Konsequenzen nach sich ziehen kann. 

2. _Datenmanipulation und Integritätsverletzungen_

**Wahrscheinlichkeit**: Mittel bis Hoch 

**Beschreibung**: Angreiferinnen oder Angreifer können versuchen, Daten in der Plattform zu manipulieren, um fehlerhafte Informationen zu erzeugen oder unerwünschte Aktionen auszulösen. Da Smart City - Systeme Daten aus verschiedenen Quellen zusammenführen, entstehen potenzielle Angriffspunkte, an denen Manipulationen vorgenommen werden können. 

**Folgen**: Falsche oder manipulierte Daten können zu unkoordinierten Aktionen in Smart City - Diensten führen, was die Sicherheit und Effizienz gefährdet und sogar die öffentliche Ordnung beeinträchtigen kann. Besonders problematisch ist dies, wenn falsche Daten die Entscheidungsprozesse in städtischen Systemen wie Verkehrssteuerung oder Energieverteilung beeinflussen. 

3. _Ransomware-Angriffe auf zentrale Systeme_

**Wahrscheinlichkeit**: Mittel bis Hoch 

**Beschreibung**: Ransomware-Angriffe verschlüsseln die Daten in der Plattform und machen sie unzugänglich, bis ein Lösegeld gezahlt wird. Diese Angriffe auf kritische Infrastrukturen sind in den letzten Jahren stark angestiegen, insbesondere bei Kommunen und öffentlichen IT-Systemen. 

**Folgen**: Die Blockade von Daten kann den Betrieb vieler städtischer Systeme lahmlegen, was zu erheblichen finanziellen und logistischen Schäden führen kann.  

4. _Angriffe auf Datenplattformen_

**Wahrscheinlichkeit**: Mittel 

**Beschreibung**: Angreifer überlasten die zentrale Datenplattform mit Anfragen oder Attacken, um deren Verfügbarkeit zu beeinträchtigen. Dadurch wird verhindert, dass legitime Anfragen verarbeitet werden. Technisch einfach durchzuführen, aber Plattformen haben oft Schutzmechanismen wie Rate Limiting oder DDoS-Schutz. 

**Folgen**: Ein DoS-Angriff auf die Datenplattform kann kritische städtische Dienste wie Verkehrsmanagement, Energieversorgung und öffentliche Sicherheit stören und somit massive Auswirkungen auf das tägliche Leben in der Stadt haben. 

### 2.4 Smart City- Anwendungen
_**Was ist es?**_ 

Smart City - Anwendungen bilden die oberste Ebene der städtischen Digitalinfrastruktur. Im Gegensatz zu urbanen Datenplattformen, die eine Vielzahl unterschiedlicher Datenquellen zusammenführen, sind diese Anwendungen meist auf spezifische Anwendungsfälle ausgerichtet. Sie nutzen gezielt ausgewählte Daten aus Sensoren, Kommunikationsnetzen oder urbanen Datenplattformen, um daraus visuelle, analytische oder interaktive Lösungen zu entwickeln. 

Diese Anwendungen dienen vor allem der Datenaufbereitung und Entscheidungsunterstützung – etwa durch Dashboards, Monitoring-Tools oder spezialisierte Analyse- und Steuerungssysteme. Sie ermöglichen Stadtverwaltungen, Versorgungsbetrieben und weiteren Akteuren, Echtzeitinformationen zu erfassen, Muster zu erkennen und fundierte Maßnahmen abzuleiten. 

In einigen Bereichen gehen Smart City - Anwendungen über die reine Datenvisualisierung hinaus und übernehmen erste automatisierte Funktionen – etwa in der dynamischen Verkehrssteuerung, ressourcenschonenden Energienutzung, adaptiven Beleuchtungssystemen oder der automatisierten Bewässerung städtischer Grünflächen. 

_**Technologien und ausgewählte Beispiele**_

- Typische Anwendungsfälle: 

  - **Verkehrsmanagement**: Optimierung des Verkehrsflusses durch Echtzeit-Daten aus Sensoren und KI-gestützte Prognosen (z. B. intelligente Ampelsteuerung, dynamische Fahrspurempfehlungen) 

  - **Energie- und Ressourcensteuerung**: Automatisierte Regulierung von Straßenbeleuchtung, intelligentes Energiemanagement in öffentlichen Gebäuden und Integration erneuerbarer Energien 

  - **Umwelt- und Klimamanagement**: Überwachung von Luftqualität, Lärm- und Wetterdaten mit automatisierten Reaktionsmechanismen wie smarten Bewässerungssystemen oder Hitzeaktionsplänen 

  - **Bürgerinteraktion und urbane Services**: Digitale Plattformen für Bürgerbeteiligung, Smart City-Apps für Meldesysteme (z. B. kaputte Straßenlaternen) oder öffentliche Informations-Displays 

- Typische Technologien: 

  - **Datenanalyse und Visualisierung**: Ermöglicht die Erfassung, Verarbeitung und Darstellung städtischer Daten in Echtzeit, z.B. durch Business Intelligence Lösungen & IoT-Dashboards, Geoinformationssysteme (GIS), KI-gestützte Mustererkennung & Prognosen 

  - **Automatisierung und Steuerung**: Umfasst Technologien zur intelligenten Steuerung städtischer Prozesse und Infrastrukturen. Dazu gehören: 

  - **Edge Computing & IoT-Controller**: Lokale Verarbeitung und Echtzeit-Steuerung von Smart City-Geräten, z. B. für adaptive Verkehrsregelung, smarte Beleuchtung oder Umweltmonitoring 

  - **Regelbasierte Automatisierungssysteme**: Steuert urbane Infrastruktur auf Basis vordefinierter Regeln (z. B. Beleuchtung, Bewässerung, Verkehrssteuerung)., z. B. für intelligente Straßenbeleuchtung, smarte Bewässerungssysteme oder optimierte Ampelsteuerung 

  - **Cloud-gestützte Automatisierung**: Steuerung über zentrale Plattformen und KI-optimierte Prozesse, z. B. für energieeffizientes Gebäudemanagement oder intelligente Verkehrsflusssteuerung 

  - **Urbane Datennutzung und Interoperabilität**: Ermöglicht die Vernetzung städtischer Systeme, die Bereitstellung und Nutzung urbaner Daten sowie die Integration verschiedener Anwendungen in die Smart City - Infrastruktur, z. B. durch API-Plattformen und Open Data-Portale, Smart City - Apps und Bürgerplattformen.

**_Typische Angriffsszenarien_**

Die IoT- Anwendungen in Smart Cities sind ein attraktives Ziel für Angriffe, da sie eine direkte Schnittstelle zwischen Nutzenden und städtischen Systemen darstellen. Die häufigsten Szenarien gefährden die **Sicherheit, Integrität und Verfügbarkeit** dieser Anwendungen. 
1. _Angriffe auf Drittanbieter-Integrationen_

**Wahrscheinlichkeit**: Hoch 

**Beschreibung**: Unsichere APIs oder Schnittstellen von Drittanbietern werden als Angriffsvektor genutzt, um Daten zu kompromittieren oder falsche Informationen einzuschleusen. 

**Folgen**: Verfälschte Daten führen zu fehlerhaften Prognosen, ineffektiven Stadtsteuerungen und potenziellen Sicherheitsrisiken. 

2. _Ausnutzung von Schwachstellen in IoT-Anwendungen_

**Wahrscheinlichkeit**: Hoch 

**Beschreibung**: Sicherheitslücken in mobilen oder webbasierten Anwendungen ermöglichen Angreiferinnen oder Angreifer unbefugten Zugriff auf städtische Systeme oder Daten. 

**Folgen**: Datenlecks, Identitätsdiebstahl oder unautorisierte Steuerung kritischer Dienste wie Ampelanlagen oder Umweltüberwachungssysteme. 

3. _Manipulation von Berechnungen und Entscheidungsprozessen_

**Wahrscheinlichkeit**: Mittel 

**Beschreibung**: Angreiferinnen oder Angreifer manipulieren Daten oder Analyse-Algorithmen, um falsche Ergebnisse zu erzeugen und Entscheidungen zu beeinflussen. 

**Folgen**: Fehlentscheidungen bei der Verkehrssteuerung, Umweltmaßnahmen oder Energienutzung, was zu ineffizienten oder riskanten Maßnahmen führen kann. 

4. _Denial-of-Service-Angriffe (DoS) auf Anwendungen_

**Wahrscheinlichkeit**: Mittel 

**Beschreibung**: Angreifer überlasten Server, sodass Bürgerinnen und Bürger oder städtische Mitarbeitende nicht auf wichtige Dienste zugreifen können. 

**Folgen**: Ausfälle von Parkraum- und Verkehrsmanagement, digitale Bürgerdienste oder Smart City-Verwaltungsportale. Kritische Infrastrukturen wie Notruf-Apps oder Frühwarnsysteme können ebenfalls betroffen sein. 

***

## 3 Strategien und Handlungsempfehlungen

Die Sicherheit von Smart City-Infrastrukturen ist ein komplexes Thema, für das bereits zahlreiche fundierte Empfehlungen existieren. Anstatt diese erneut zusammenzufassen, verweist dieses Kapitel gezielt auf bestehende Ressourcen und ergänzt diese um praxisnahe Betrachtungen. 

Ein zentrales Referenzdokument ist die BSI-Handlungsempfehlung für Smart Cities, die einen umfassenden Sicherheitsansatz über den gesamten Lebenszyklus smarter Infrastrukturen hinweg bietet. Sie liefert klare Vorgaben zur sicheren Planung, Implementierung und zum Betrieb von IoT-Infrastrukturen in Städten. Die darin enthaltenen Prinzipien und Maßnahmen werden allen Smart City – Akteuren empfohlen. 

Ergänzend zu den bestehenden Empfehlungen widmet sich dieses Kapitel spezifischen Herausforderungen in Bezug auf Technologieintegration und Interoperabilität sowie dem Übertrag in die kommunale Praxis. und Praxisaspekten der Cybersicherheit in Smart Cities.  

### 3.1 Bestehende Strategien und Handlungsempfehlungen im Überblick


| Publikation | Hrsg. | Erschienen | Sprache | Einordnung |
| ----------- | ----- | ---------- | ------- | ---------- |
|[Smart Cities/ Smart Regions Informationssicherheit für IoT- Infrastrukturen- Handlungsempfehlungen](https://www.bsi.bund.de/SharedDocs/Downloads/DE/BSI/SmartCity/Handlungsempfehlungen_Smart_City.pdf?__blob=publicationFile&v=3) | BSI | 2022 | deutsch | *Must Read* Richtet sich an Kommunen und kommunale Unternehmen, die IoT-Projekte initiieren und betreiben; Fokus auf den Aufbau und Ausbau sicherer IoT-Infrastrukturen; Handlungsempfehlungen entlang des Lebenszyklus einer IoT-Infrastruktur |
|[Making smart cities cybersecure - Ways to address distinct risks in an increasingly connected urban future](https://www.deloitte.com/de/de/services/risk-advisory/research/smart-cities-cyber-security.html) | Deloitte | 2019 | Englisch |  *Read* Bietet ein Rahmenwerk für Managementstrategien zur Gewährleistung von Sicherheit, Verfügbarkeit, Vertraulichkeit, Integrität und Elastizität in vernetzten städtischen Systemen |
|[Resilienz in der Smart City - Wie Kommunen besser mit Krisen umgehen und proaktiv eine nachhaltige Zukunft gestalten können](https://www.smart-city-dialog.de/resilienz-der-smart-city-wie-kommunen-besser-mit-krisen-umgehen-koennen) | BBSR | 2023 | deutsch | *Information* Setzt auf ein Resilienzkonzept für krisenfeste Städte; Digitalisierung und Cybersicherheit als Schlüssel; Schutz kritischer Infrastruktur und Anpassungsfähigkeit im Fokus; Handlungsempfehlungen zur Stärkung durch Feedback-Loops, Modularität, Diversität, Redundanz; konkrete Praxisbeispiele |

### 3.2 Technologieintegration als besondere Herausforderung
Die Integration verschiedener Technologien ist für den Betrieb einer Smart City essenziell – sie ist aber auch eine der größten sicherheitstechnischen Schwachstellen. Unterschiedliche Hersteller, uneinheitliche Standards und nicht durchgängig abgesicherte Schnittstellen erhöhen das Risiko für Datenverluste, Manipulationen und unautorisierten Zugriff. 

Zentrale Herausforderungen in Bezug auf Cybersecurity: 

- **Unsichere Schnittstellen und API-Schwachstellen**: Viele Smart City - Dienste greifen auf offene APIs und externe Datenquellen zurück. Unzureichend gesicherte Schnittstellen sind häufige Angriffspunkte für Man-in-the-Middle-Angriffe, unautorisierte Zugriffe oder Datenmanipulationen. Fehlende Authentifizierungs- und Verschlüsselungsmechanismen gefährden die Integrität der übermittelten Informationen. 

- **Interoperabilität & Sicherheitslücken durch heterogene Systeme**: Smart Cities setzen eine Vielzahl an Technologien ein, die oft aus unterschiedlichen Ökosystemen stammen. Nicht standardisierte Sicherheitsmechanismen führen zu Inkompatibilitäten, die Angreifer gezielt ausnutzen können. Beispielsweise sind unterschiedliche Verschlüsselungsstandards oder Authentifizierungsverfahren eine potenzielle Schwachstelle. 

- **Datenkonsistenz & Integrität in vernetzten Systemen**: Smart Cities aggregieren Daten aus unterschiedlichen Quellen, von Sensoren über Verwaltungsplattformen bis hin zu Drittanbietern. Datenmanipulation kann zu falschen Entscheidungen führen, Sicherheitsprozesse untergraben oder automatisierte Abläufe sabotieren. 

- **Abhängigkeit von proprietären Lösungen vs. Open Source**: Proprietäre Smart City-Plattformen versprechen eine bessere Wartung und höhere Sicherheit, können aber zur Blackbox für Sicherheitsprüfungen werden und verhindern unabhängige Audits. Open-Source-Lösungen bieten Transparenz und mehr Flexibilität, benötigen aber zusätzliche Sicherheitsmaßnahmen und kontinuierliche Wartung, um Schwachstellen zu minimieren. 

- **Fehlende Sicherheitsupdates und Patch-Management**: Unterschiedliche Systeme mit variierenden Update-Zyklen stellen ein erhebliches Risiko dar. Ungepatchte Sicherheitslücken in IoT-Geräten oder Plattformen können als Einfallstor für Cyberangriffe dienen und ganze Infrastrukturen kompromittieren. 

Cybersecurity muss daher bereits bei der Planung von Technologieintegrationen berücksichtigt werden. Sichere APIs, standardisierte Verschlüsselung und eine durchgehende Überprüfung der Datenintegrität sind essenziell, um Angriffsflächen zu minimieren. 

### 3.3 Kommunale Umsetzungshürden: Zwischen Anspruch und Realität
Die sichere Gestaltung von Smart Cities scheitert in der Praxis oft nicht an fehlenden Konzepten, sondern an strukturellen und organisatorischen Hürden. Fachkräftemangel, unklare Zuständigkeiten, fehlende Budgets und komplexe Abstimmungsprozesse machen es Kommunen schwer, Cybersicherheit konsequent umzusetzen. 

Ein zentrales Problem: Viele Smart City - Projekte starten als Pilotvorhaben ohne langfristige Sicherheitsstrategie. Sicherheitsmaßnahmen werden oft punktuell integriert, statt systematisch in den Regelbetrieb überführt zu werden. Gleichzeitig bleibt Cybersicherheit häufig eine untergeordnete Priorität in der Förderlogik, da Programme eher technische Innovationen als deren nachhaltige Absicherung unterstützen. Die Realität zeigt, dass Cybersicherheit nicht allein durch technische Lösungen erreicht wird. Es braucht klare Verantwortlichkeiten, durchgehende Sicherheitsrichtlinien und eine bessere Vernetzung der relevanten Akteure. 

Viele bestehende Strategien geben sinnvolle Handlungsempfehlungen – doch die eigentliche Herausforderung liegt in der praktischen Umsetzung. Was heute fehlt, ist eine realistische Diskussion darüber, wie Cybersicherheit unter den tatsächlichen Rahmenbedingungen deutscher Kommunen langfristig verankert werden kann. Dabei kommen drei zentrale Ansatzpunkte für eine realistische Cybersicherheitsstrategie in Betracht: 

- **Sicherheit als Standard**: Sicherheitsanforderungen dürfen nicht erst nachträglich ergänzt werden. Cybersicherheit muss verbindlich in Ausschreibungen, Verträge und Betriebskonzepte integriert sein – nicht als Sonderaufgabe, sondern als selbstverständlicher Bestandteil smarter Stadtentwicklung. 

- **Strategische Verankerung**: Viele Kommunen setzen bereits auf Insellösungen – etwa verschlüsselte IoT-Kommunikation oder sicherheitszertifizierte Cloud-Dienste. Doch diese Maßnahmen greifen nur, wenn sie Teil einer gesamtstädtischen Sicherheitsstrategie sind, die Verwaltung, Stadtwerke, externe Lösungsanbieter und IT-Dienstleister gemeinsam tragen. 

- **Einbindung und Weiterentwicklung durch die Community**: Cybersicherheit ist kein statisches Konzept, sondern ein sich ständig weiterentwickelndes Feld. Kommunen brauchen den Austausch mit anderen Städten, IT-Sicherheitsforschung und Open Source/Open Data -Initiativen, um langfristig widerstandsfähig zu bleiben. Der Dialog zwischen technischen, rechtlichen und organisatorischen Akteuren ist dabei dringend geboten.

***

## **4 Richtlinien und Standards**
Diese Abschnitt verweist auf bewährte Richtlinien und Standards für die Sichheit in Smart Cities. Die aufgeführten Vorgaben bieten eine Grundlage für den Schutz digitaler Infrastrukturen und lassen sich flexibel auf txpische Herausforderungen in urbanen Kontext anwenden.
### 4.1 Richtlinien
**_Datenschutz- Grundverordnung_**

[Die Datenschutz-Grundverordnung (DSGVO)](https://dsgvo-gesetz.de/) hat erhebliche Auswirkungen auf Smart City - Lösungen, da sie den Umgang mit personenbezogenen Daten strikt regelt. In einer Smart City werden viele Daten über Sensoren, urbane Datenplattformen und andere digitale Infrastrukturen erfasst und der Datenschutz ist immer mitzudenken.  

Für Smart City-Lösungen bedeutet dies: 

- **Datensparsamkeit**: Nur die minimal notwendigen Daten dürfen erhoben und verarbeitet werden 

- **Sicherheitsvorkehrungen**: Es müssen technische und organisatorische Maßnahmen getroffen werden, um die Sicherheit der Daten zu gewährleisten und unbefugten Zugriff zu verhindern 

- **Transparenz**: Bürger müssen darüber informiert werden, welche Daten von ihnen erfasst werden und zu welchem Zweck 

- **Rechte der Betroffenen**: Bürger haben das Recht, Auskunft über ihre Daten zu verlangen, diese zu korrigieren, löschen zu lassen oder deren Verarbeitung einzuschränken 

Die Nichteinhaltung der DSGVO kann zu erheblichen Strafen führen und das Vertrauen der Bürger in Smart City-Projekte untergraben. Daher ist die Integration von Datenschutz in alle Phasen der Konzeption und Umsetzung solcher Lösungen unerlässlich. 

**_CER und NIS-2_**

Die [CER-Richtlinie (Critical Entities Resilience Directive)](https://eur-lex.europa.eu/legal-content/DE/TXT/PDF/?uri=CELEX:32022L2557) und die [NIS2-Richtlinie](https://eur-lex.europa.eu/eli/dir/2022/2555) sind zwei separate, aber eng miteinander verknüpfte EU-Richtlinien, die darauf abzielen, die Cybersecurity und Cyberresilienz kritischer Infrastrukturen in Europa zu stärken. Beide traten im Oktober 2024 in Kraft und ergänzen sich in ihrer Ausrichtung auf physische und digitale Bedrohungen. 

- **NIS2-Richtlinie**: Diese Richtlinie zielt darauf ab, die Cybersicherheit in einer Vielzahl von Sektoren, einschließlich digitaler Infrastrukturen, Energie, Gesundheitswesen und öffentlichen Verwaltungen, zu verbessern. Sie erfordert robuste Cybersicherheitsmaßnahmen, umfassendes Risikomanagement, sowie Meldepflichten bei Sicherheitsvorfällen. NIS2 legt den Schwerpunkt auf den Schutz digitaler Systeme und den Aufbau von widerstandsfähigen IT-Strukturen in kritischen Sektoren 

- **CER-Richtlinie**: Im Gegensatz dazu fokussiert die CER-Richtlinie auf die physische Resilienz kritischer Infrastrukturen gegenüber einer Reihe von Bedrohungen wie Naturkatastrophen, Terroranschlägen, Insider-Bedrohungen oder Sabotage. Sie deckt 11 Sektoren ab, darunter Energie, Transport, Bankwesen und öffentliche Verwaltung. Diese Richtlinie verlangt von den betroffenen Organisationen, ihre physischen und digitalen Risiken zu identifizieren und Maßnahmen zu ergreifen, um ihre Infrastruktur vor Störungen zu schützen.  

Zusammen bieten NIS2 und CER einen umfassenden Rahmen zur Sicherung kritischer Infrastrukturen in Smart Cities, sowohl gegen physische als auch cyberbezogene Bedrohungen. 

_**Open Data Richtlinie**_

Die [Open Data Richtlinie der EU](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=LEGISSUM:4405374), auch bekannt als die Richtlinie über offene Daten und die Weiterverwendung von Informationen des öffentlichen Sektors, hat erhebliche Auswirkungen auf Smart Cities, da sie den freien Zugang zu und die Wiederverwendung von öffentlichen Daten fördert. Im Kontext von Smart Cities bedeutet dies, dass große Mengen an urbanen Daten, die durch Sensoren und digitale Plattformen gesammelt werden, offen zugänglich gemacht werden müssen, um Transparenz, Innovation und Bürgerbeteiligung zu fördern. 

Die Bereitstellung von offenen Daten stellt für Smart Cities jedoch auch eine Cybersecurity-Herausforderung dar. Einerseits muss der freie Zugang zu nicht personenbezogenen Daten gewährleistet werden, andererseits müssen sensible Informationen wie personenbezogene Daten und sicherheitskritische Infrastrukturen geschützt werden. Die Open Data Richtlinie erfordert daher ein feingliedriges Sicherheitsmanagement, um sicherzustellen, dass die Freigabe von Daten nicht zu potenziellen Angriffsflächen führt. 

- **Datensicherheit**: Um die Datensicherheit zu gewährleisten, müssen Smart Cities strikte Zugriffskontrollen und Anonymisierungsverfahren implementieren, bevor Daten veröffentlicht werden 

- **Transparenz und Sicherheit**: Der Spagat zwischen Transparenz und Cybersecurity erfordert die Einhaltung von Sicherheitsstandards, die sicherstellen, dass die Integrität und Verfügbarkeit der Daten gewährleistet bleiben, während gleichzeitig offene Datenplattformen betrieben werden 

- **Angriffsrisiken**: Offene Datenportale können potenziell von Cyberangreifern ausgenutzt werden, um Schwachstellen in den städtischen Infrastrukturen zu identifizieren. Daher müssen Städte, die Open Data bereitstellen, geeignete Cybersicherheitsmaßnahmen treffen, wie etwa die regelmäßige Überprüfung der veröffentlichten Datensätze und die Integration von Risikobewertungen. 

Insgesamt müssen Smart Cities beim Umgang mit Open Data stets ein ausgewogenes Verhältnis zwischen der Förderung von Offenheit und Innovation und dem Schutz ihrer kritischen Infrastrukturen finden. 

### 4.2 Standards
**_BSI-Grundschutz_**

Der [BSI IT-Grundschutz](https://www.bsi.bund.de/DE/Themen/Unternehmen-und-Organisationen/Standards-und-Zertifizierung/IT-Grundschutz/it-grundschutz_node.html) ist ein umfassendes Sicherheitskonzept, das vom [Bundesamt für Sicherheit in der Informationstechnik (BSI)](https://www.bsi.bund.de/SharedDocs/Downloads/DE/BSI/Grundschutz/Hilfsmittel/Profile/Basis_Absicherung_Kommunalverwaltung.html) entwickelt wurde, um Organisationen dabei zu unterstützen, ihre IT-Systeme systematisch und effizient zu schützen. Es bietet eine strukturierte Methodik, mit der Sicherheitsrisiken identifiziert und geeignete Schutzmaßnahmen implementiert werden können. Der IT-Grundschutz umfasst dabei Module für unterschiedliche Szenarien, von der Netzwerksicherheit über physische Sicherheitsmaßnahmen bis hin zur Reaktion auf Sicherheitsvorfälle. 

Für Smart Cities ist der IT-Grundschutz besonders relevant, da sie stark auf vernetzte Infrastrukturen, IoT-Geräte und urbane Datenplattformen angewiesen sind. Der IT-Grundschutz bietet einen systematischen Rahmen, um diese komplexen Systeme abzusichern. Im Kontext von Smart Cities sind folgende Aspekte besonders wichtig: 

**_ISO und DIN_**

Internationale Standards wie ISO und nationale Normen wie DIN bieten strukturierte Rahmenwerke, um die Sicherheit und Effizienz moderner Smart City-Systeme zu gewährleisten. Sie definieren Anforderungen und Best Practices, die es Städten ermöglichen, ihre digitalen Infrastrukturen und IoT-Systeme sicher und zukunftsfähig zu gestalten. Eine gute Übersicht über relevante Standards in diesen Bereichen sind im Folgenden zusammengetragen: 

|Norm|Rahmen|
|-|-|
|DIN|[Nationale Normen und Standards](https://www.din.de/de/forschung-und-innovation/themen/smart-cities/normen-und-standards/nationale-normen-und-standards) für Smart City u.a. für Urbane Digitale Zwillinge, Offene Urbane Datenplattformen|
|ISO|u.a Standards zu Informationssicherheitsmanagement (ISO/IEC 27001), der auch für den BSI- Grundschutz relevant ist|

***

## 5 **Weiterführende Ressourcen und Tools**
Dieser Abschnitt enthält eine Auswahl an Ressourcen und weiterführenden Informationen, die für Smart Cities hilfreich sein können. Das Angebot in diesem Bereich wächst kontinuierlich, und Ergänzungen werden gerne aufgenommen. Hinweise bitte über die Kommentierung. 

| Titel | Link |
| --------------------------- | ------|
| Allianz für Cybersicherheit | [ACS - Allianz für Cyber Sicherheit -ACS](https://www.allianz-fuer-cybersicherheit.de/Webs/ACS/DE/Home/home_node.html)
| Pilotprojekt Sicherkommunal BSI & Sachsen- Anhalt | [Mehr IT- Sicherheit für kommunen- Kommune21 online Kommune21 - E-Government, Internet und Informationstechnik](https://www.kommune21.de/k21-meldungen/mehr-it-sicherheit-fuer-kommunen-2/) |
| Hessen | [Aktionsprogramm Kommunale Cybersicherheit Hessen 3C CyberCompetenceCenter](https://hessen3c.de/unsere-leistungen/aktionsprogramm-kommunale-cybersicherheit-akc) |
| Cybersicherheitskompass für kommunen (beta) | [Cybersicherheitskompass BETA 0.9](https://cybersicherheitskompass.de/) |
| Rolle der Verwaltungsspitze in der Informationssicherheit (Dt. Städtetag) | [Informationssicherheit für die Verwaltungsspitzen von Städten und Gemeinden](https://www.staedtetag.de/files/dst/docs/Publikationen/Weitere-Publikationen/2022/papier-rolle-der-verwaltungsspitze-in-der-Informationssicherheit.pdf) |
| Whitepaper zum BSI- Projekt "safe hAAven 5G++" | [Cybersicherheit-in-deutschen-Smart-Cities-2024 11.pdf](https://zde-akademie.de/wp-content/uploads/2024/11/Cybersicherheit-in-deutschen-Smart-Cities-2024_11.pdf) |

