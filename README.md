# Deutsche Raspberry-Pi-FAQ

Diese FAQ ist entstanden aus dem Wunsch, häufig gestellte Fragen (vor allem in der [Facebook-Gruppe "Raspberry Pi Deutschland"](https://www.facebook.com/groups/rpi.de/?ref=group_cover)) an zentraler Stelle zu sammen und zu beantworten. 

### Mitmachen!

Die Beiträge werden vom Pi-and-More-Team und anderen Freiwilligen redaktionell betreut, um die Qualität sicherzustellen. Beitragen kann aber jeder, dazu gibt es zwei Möglichkeiten:

 - Durch Pull-Requests. Interessierte Benutzer können das [https://github.com/PiAndMore/faq](Repository, in dem die Inhalte liegen,) auf Github clonen, die Inhalte in ihrer Kopie die Repositories bearbeiten, und uns dann einen Pull-Request schicken. Wir akzeptieren den Pull-Request, wenn er inhaltlich und vom Format her passt.

 - Benutzern, die regelmäßig Beiträge beisteuern möchten, geben wir eine Schreibberechtigung für das Github-Repository.

Tipp: Beide Bearbeitungsmöglichkeiten stehen dir auch direkt im Browser zur Verfügung: Klick auf die README.md-Datei und dann oben auf "bearbeiten". 


### Formatierungshinweise

Die ganze FAQ ist derzeit bewusst als eine lange Seite gestaltet - so bleibt sie schnell durchsuchbar. Sie soll bewusst keine vollständigen Tutorials etc. wiedergeben, die weitere Unterabschnitte oder separate Seiten erfordern würden. Auf solche Inhalte auf externen Seiten sollte mit Links verwiesen werden. Daher benutzen wir auch derzeit bewusst keine Wiki-Software.

Links sollten nicht kommentarlos eingefügt werden, dies hilft gerade Anfängern nicht. Wenn möglich, sollte auf deutsche Seiten verwiesen werden.

# Fragen und Antworten

## Wie stelle ich Fragen?

Wenn du eine Frage in einer Facebook-Gruppe oder einem Forum stellen möchtest, beachte bitte die folgenden Tipps:

 * Versuche zunächst, eine Antwort auf deine Frage **selbst zu finden** und schau, ob die Frage schoneinmal gestellt wurde:
    - Bei Google
    - In der Suchfunktion der unten verlinkten Foren und Facebook-Gruppen
    - In diesem Dokument (aber wenn du schon hier bist, hast du das wahrscheinlich schon getan)
 * Formuliere deine Frage möglichst **präzise**. (Verständliche Sprache und die Benutzung von Satzzeichen sollten dabei selbstverständlich sein!)
 * Stelle **genau eine Frage** pro Beitrag. 
 * Beschreibe, welche **Lösungsansätze** du bereits ausprobiert hast, und warum diese nicht funktioniert haben. 
 * Poste **Code und Konfigurationsdateien,** die du erstellt hast oder an denen du Änderungen durchgeführt hast. **Benutze dazu nicht Facebook,** sondern stell deinen Code auf http://pastebin.com/ und füge dann den Link in deiner Frage ein. Dies stellt sicher, dass Formatierungen im Code erhalten bleiben.
 * Bekommst du **Fehlermeldungen,** so gib sie im genauen Wortlaut wieder oder poste Screenshots!
 * Gehe auf die **Antworten** ein, die du erhältst - das hilft bei der Lösungssuche und steigert die Motivation deiner Helfer, dir auch beim nächsten Problem zur Seite zu stehen.

## Was brauche ich zum Einstieg?

- Einen ersten Einstieg, auf Englisch aber gut bebildert, bietet der offizielle Hardware-Guide:  https://www.raspberrypi.org/learning/hardware-guide/
- Eine Liste kompatibler Hardware, insbesondere SD-Karten, gibt es auf http://elinux.org/RPi_VerifiedPeripherals

## Wie stelle ich meine config.txt ein?

Siehe http://elinux.org/RPiconfig

## Wie installiere ich das Betriebssystem?

TODO

## Was sollte ich als Mediacenter verwenden?

TODO

## Meine Videos ruckeln! 

Du brauchst vielleicht (abhängig von deinem Videomaterial) die Lizenzen für MPEG 2 und VC-1. [(Für Hintergründe siehe hier.)](http://www.heise.de/hardware-hacks/meldung/Raspberry-Pi-MPEG-2-und-VC-1-Lizenzen-erhaeltlich-1676076.html) Du kannst diese Lizenzen auf https://raspberrypi.org erwerben.

## Wie kann ich Retrogames auf dem Pi spielen?

TODO


## Wie kann ich regelmäßig mein Programm ausführen lassen?

Dazu legst du einen sogenannten Cron-Job an. Cron ist ein Service, mit dem man zeitgesteuert oder auch beim Hochfahren des Pis Programme oder Skripte ausführen lassen kann. 

Informationen zur Einrichtung von [Dirk Handzik](https://www.facebook.com/notes/raspberry-pi-deutschland/vom-umgang-mit-cron/800791183304213) und [bei ubuntuusers.de](https://wiki.ubuntuusers.de/Cron/) (die Einrichtung über die GUI ist auf dem Pi je nach Betriebssystem u.U. nicht so durchführbar!).

**Tipp: Wenn dein Cronjob nicht funktioniert, liegt es häufig daran, dass Pfade nicht gefunden werden oder dass der Cronjob unter dem falschen Benutzer gestartet wurde (siehe [hier](https://wiki.ubuntuusers.de/Cron/#Haeufige-Fehler)).** 

## Ich würde gerne das Windows-Programm X auf dem Pi laufen lassen.

Ja, es gibt [Windows für den Pi](https://developer.microsoft.com/de-de/windows/iot). Nein, es ist nicht das Windows, was du von deinem PC kennst. Die allermeiste Software wird **nicht** auf deinem Pi laufen! Software, die auf Windows 10 IoT läuft, ist speziell dafür angepasst. Wenn das nicht explizit auf der Website der Software o.ä. steht, dann wird sie **nicht** auf dem Pi laufen!

In [diesem Artikel](https://www.golem.de/news/windows-10-iot-ausprobiert-finales-windows-auf-dem-raspberry-pi-2-1508-115747.html) findest du auch einen Vergleich von Windows 10 Iot zu dem "echten" Windows auf dem PC. Du wirst sehen, dass es sehr viele Unterschiede gibt.

## Aber es gibt doch Wine!

Mit Wine und QEMU lassen sich einige wenige [Programme auf dem Pi ausführen](http://www.forum-raspberrypi.de/Thread-raspbian-windowsprogramme-ausfuehren-mit-qemu-und-wine), aber die Ausführung ist sehr langsam. Das reicht für [Druckertreiber](https://www.lhinderberger.de/pi/2016/01/27/raspberry-pi-binary-x86-drivers.html) ([Kauf-Artikel bei c't](https://www.heise.de/ct/ausgabe/2015-18-Binaere-x86-Linux-Treiber-auf-dem-Raspi-nutzen-2766560.html)), aber nicht für größere Anwendungen. 

## Ich möchte gerne meinen Drucker XY mit dem Pi betreiben

Die erste Wahl sind die Treiber, die bei Raspbian mitgeliefert werden. Um einen Drucker zu installieren, installiert man zunächst CUPS (mit sudo apt-get install cups) und richtet dann den Drucker über den Webbrowser des Pis auf http://localhost:631/ ein. Eine ausführlichere Anleitung, die auch die Freigabe des Druckers im Netz behandelt, findet sich [bei Raspberry Pi Geek](http://www.raspberry-pi-geek.de/Magazin/2013/05/Raspberry-Pi-als-Datei-und-Drucker-Server/(offset)/2) und auch im [Elektronik-Kompendium](https://www.elektronik-kompendium.de/sites/raspberry-pi/2007081.htm). 


## Wie lese ich die GPIOs aus?

Wichtig: GPIOs akzeptieren nur 3,3V-Signale. 
 
- Englische Erklärung: https://www.raspberrypi.org/blog/using-the-gpio/
- GPIO-Belegung und maximale Stromstärken, die die GPIO-Pins liefern können: http://elinux.org/RPi_Low-level_peripherals

# Projekte

TODO

# Community

## Welche Foren und Communities gibt es?

 - [Facebook-Gruppe "Raspberry Pi Deutschland"](https://www.facebook.com/groups/rpi.de/?ref=group_cover)
 - [Facebook-Gruppe "TVHeadend Deutschland"](https://www.facebook.com/groups/tvheadend.de/)
 - [Facebook-Gruppe "Raspbery ZeroBOY Projekt"](https://www.facebook.com/groups/gameboyzeromod/)
 - [Facebook-Gruppe "Projekt Smart Mirror"](https://www.facebook.com/groups/248735748896945/)
 - [Facebook-Gruppe "Einplatinencomputer"](https://www.facebook.com/groups/577888222399762/)

## Welche Magazine, Bücher, Lektüre gibt es?

### Deutsch
- [Raspberry PI Geek](http://www.raspberry-pi-geek.de/Magazin) 

### Englisch

- [The MagPI](https://www.raspberrypi.org/magpi/) - kostenlos als PDF


# Offene Themen
Für die hier aufgelisteten Fragen freuen wir uns über eine gut formulierte Antwort von dir. Bitte verschiebe die Frage mit ihrer Antwort dann in den entsprechenden Abschnitt oben.
## Wie baue ich einen Magic Mirror?

## Ich will einen PI in mein Auto einbauen
http://www.st.com/content/ccc/resource/technical/document/application_note/1f/d7/fc/6d/2e/27/48/98/CD00181783.pdf/files/CD00181783.pdf/jcr:content/translations/en.CD00181783.pdf

## Wie baue ich mir einen eigenen Ablilight-Klon?
http://www.forum-raspberrypi.de/Thread-tutorial-ambi-tv-ambilight-fuer-hdmi-quellen



