---
layout: post
title:  "Bereitstellung der Los E - Plugins im NERZ-Repository"
categories: rahmenwerk
---

## Publikation

Die bisher zentral über eine Updateseite im Projekt "Los E" bereitgestellten
Plugins für das Rahmenwerk 3 wurden im NERZ-Repository als einzelne Projekte
angelegt.

Im Detail sind das:

- [Anlagenstatus](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.anlagenstatus)
- [Archivverwaltung](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.ars)
- [Archiv-Export](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.ars.export)
- [Engstellenverwaltung](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.baueditor)
- [Benutzerverwaltung](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.benutzervew)
- [Betriebsmeldungsverwaltung](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.bmvew)
- [Darstellungsobjekte](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.dobj)
- [Datenflussüberwachung](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.dafluss)
- [Darstellungsobjekt-Editor](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.doeditor)
- [Vorpositionierer](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.dopositionierer)
- [Ereigniskalender](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.ereigniskal)
- [Konfigurationsassistent](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.konfigass)
- [Konfigurationseditor](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.konfigeditor)
- [MQ Ganglinien](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.mq.ganglinien)
- [Netzdarstellung](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.netz)
- [Parametrierung](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.param)
- [Protokolle und Auswertungen](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.pua)
- [Rahmenwerk-Erweiterungen BitCtrl](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.rw.bitctrl)
- [RDS-Editor](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.rdseditor)
- [Selektionstransfer](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.selektion)
- [Simulation](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.sim)
- [Startstopp](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.startstopp)
- [Streckenprofil](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.streckenprofil)
- [Systemkalender](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.syskal)
- [Teil-Konfigurations-Assistenten](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.tka)
- [TMC-Editor](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.tmceditor)
- [Umfassende Datenanalyse](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.uda)
- [Verkehrsmeldungen-Detail](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.verkehrsmeldung.detail)

Ein "Plugin-Projekt" setzt sich wie folgt zusammen:

- ein oder mehrere Plugins, die die Funktionalität realisieren
- ein oder mehrere Features, die die Plugins bereitstellen
- eine Updatseite, über die die erzeugten Features und/oder Plugins zur
  Installation zur Verfügung gestellt werden können.

Die aus aktuellen "develop"-Branch erstellten Updateseiten der jeweiligen Projekte werden unter den im Projekt definierten URL http://bitctrl/projekte/rw_plugins/XXXX publiziert.

Die einzelnen Updateseiten sollten verwendet werden, wenn Plugins entwickelt werden, die von einem der oben genannten Plugins anghängig sind.


Aus den publizierten einzelnen Updateseiten wird die bisherige Gesamtupdateseite konstruiert:

[http://www.bitctrl.de/projekte/lose_rw3.0/updatesite/](http://www.bitctrl.de/projekte/lose_rw3.0/updatesite/)

Die Gesamt-Updateseite sollte in Produkten und/oder Installationen zur Installation und zum Update zum Einsatz kommen.

## Plugin bauen

Zum Erstellen eines Plugins sind eine aktuelle Maven-Version und ein Git-Client erforderlich.

Die Vorgehensweise ist im Folgenden beispielhaft am Plugin "Teilkonfigurations-Assistenten" dargestellt.

````
git clone http://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.plugin.tka.git
cd RW_de.bsvrz.buv.plugin.tka
mvn clean verify
````

Die erstellte Updateseite ist als ZIP-Archiv im "target"-Verzeichnis des Updatesite-Unterprojekts zu finden.

## Ausblick

Die Erstellung und Publikation der Updateseiten sollte zeitnah auf den NERZ ausgelagert werden.
