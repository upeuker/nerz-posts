---
layout: post
title:  "Rahmenwerk auf Eclipse-PHOTON-Basis"
categories: rahmenwerk
---

## Rahmenwerk auf Eclipse-PHOTON-Basis

Das Rahmenwerk steht in der Developer-Version in einer neuen Version auf der Basis der Eclipse Version 4.8 (PHOTON) zur Verfügung.

Die Quellen stehem im [NERZ-Repository](https://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.rw) zur Verfügung.

Die aktuelle BETA-Version steht als Updateseite unter:

[http://www.bitctrl.de/projekte/rw3.3/updatesite/](http://www.bitctrl.de/projekte/rw3.3/updatesite/)

Die jeweils aktuellen BETA-Pakete sind verfügbar für:

- **Windows 64-Bit** [DOWNLOAD](https://http://www.bitctrl.de/projekte/rw3.3/products/de.bsvrz.buv.rw-win32.win32.x86_64.zip),
- **Windows 32-Bit** [DOWNLOAD](https://http://www.bitctrl.de/projekte/rw3.3/products/de.bsvrz.buv.rw-win32.win32.x86.zip),
- **Linux GTK** [DOWNLOAD](https://http://www.bitctrl.de/projekte/rw3.3/products/de.bsvrz.buv.rw-linux.gtk.x86_64.tar.gz) und
- **Mac OS X** [DOWNLOAD](https://http://www.bitctrl.de/projekte/rw3.3/products/de.bsvrz.buv.rw-macosx.cocoa.x86_64.tar.gz)

Zum Erstellen der Software sind eine aktuelle Maven-Version und ein Git-Client erforderlich.

````
git clone http://gitlab.nerz-ev.de/ERZ/RW_de.bsvrz.buv.rw.git
cd RW_de.bsvrz.buv.rw
mvn clean verify
````

Das erstellte Software-Paket findet sich im target-Verzeichnis des Unterprojekts de.bsvrz.buv.rw.tycho.product. 


## Plugins

Alle Standard-Plugins des Rahmenwerk 3 sind kompatibel mit dieser
Rahmenwerk-Version.

Insbesondere sind das die Plugins aus den NERZ-Projekten:

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

Der aktuelle Stand aus dem "develop"-Branch wird auf der Updateseite:

[http://www.bitctrl.de/projekte/lose_rw3.0/updatesite/](http://www.bitctrl.de/projekte/lose_rw3.0/updatesite/)

bereitgestellt.

## Java-Version

Das Rahmenwerk ist Java-8-kompatibel, d.h. es wurden noch keine neueren Java-Mittel eingesetzt.

Das Rahmenwerk ist auch mit Java 9/10 ausführbar, dazu sollte in der Datei "rahmenwerk.ini" der VM-Parameter:

````
--add-modules=ALL-SYSTEM
````

ergänzt werden, da einige Plugins Pakete verwenden, die in neueren Java-Versionen als Modul explizit eingebunden werden müssen.
