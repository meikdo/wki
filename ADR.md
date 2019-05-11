## Entwurfsentscheidungen 
----
### ADR01 Clean Architecture als Makroarchitektur
Kontext
Das Projekt soll in möglichst sauberer Arbeitsteilung umgesetzt werden. Es kommen verschiedene Backendtechnologien in verschiedenen Umgebungen zum Einsatz.

### Entscheidungsbeschreibung
Als Makroarchitektur des Projekts wird Clean Architecture eingesetzt.

### Konsequenzen
Die saubere Schichtung in Clean Architecture erleichtert die Zusammenarbeit. Die verschiedenen Umgebungen können durch Austausch von Gatewayimplementierungen realisiert werden.

### Status
Akzeptiert

----

ADR02 Filter für Parkmöglichkeiten innerhalb der App & App-Einstellungen
### Kontext
Das Parkmöglichkeitenangebot muss nach Bedarf und Wünschen gefiltert werden können.

### Entscheidungsbeschreibung
Es gibt grundlegende und nur über die App-Einstellungen veränderliche Filter, wie zum Beispiel: behindertengerecht oder Aufladestation für Elektrofahrzeuge.
Jedoch gibt es zusätzlich noch die Option bei der Parkmöglichkeitensuche eben diese Filter einmalig für eine Suche anzuwenden und noch mehr Filter auszuwählen, wie zum Beispiel: Familienparkplatz oder Video-überwacht.

### Konsequenzen
Auch bei jedem Neustart der App sind die Filter die in den App-Einstellungen angewendet wurden aktiv.

### Status
Akzeptiert
