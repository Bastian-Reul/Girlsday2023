# Girlsday2023
Dieses Projekt wurde für den Girlsday der WHS 2023 erstellt und dieses repository richtet sich auch an dessen Teilnehmerinnen. Das Projekt richtet sich an Einsteiger in Bezug zu Hard- und Software.

Als Hauptbestandteil der Hardware wurde ein Bananapi M2 Zero eingesetzt. Dieser ist einer der wenigen momentan verfügbaren SingleBoard Computer, welche momentan im regulären Handel lieferbar sind. (Stand April 2023)

Mit eurem MagicMirror habt ihr eine Micro-SD Karte (welche in dem Bananapi eingesteckt ist) bekommen. Auf dieser Micro-SD Karte befindet sich das gesammte Betriebssystem eures MagicMirrors und auch alle Dateien für den Betrieb und die Konfiguration des MagicMirrors.

## Installation bei euch zu Hause (WLAN Verbindung hat geklappt) ##
Wenn man Girlsday alles glatt gelaufen ist, habt ihr schon im Labor eure WLAN Daten in den MagicMirror eingegeben, er verbindet sich direkt mit eurem WLAN zuhause und der MagicMirror funktioniert einfach. Dies erkennt ihr daran, dass er euch zum Beispiel den aktuellen Wetterbericht oben rechts in der Ecke anzeigt. Desweiteren zeigt der MagicMirror unten rechts (schwer erkennbar, soll im regulären Betrieb aber halt auch nicht stören) seine IP Adresse an. Diese ist bei euch vermutlich in der Art: **192.168.1.23** oder **192.168.0.125** oder **192.168.178.23**. Die letzten beiden Zahlenblöcke können bei euch abweichen, aber die vorderen beiden sollten höchstwahrscheinlich **192.168** sein. 

Mit Hilfe dieser IP Adresse könnt ihr euch über einen Computer mit einem SSH Programm (SSH Client, bspw. [Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)) mit dem MagicMirror verbinden. 
### Um Putty auf einem Windows Rechner zu installieren ### 
* geht auf die verlinkte Seite
* Sektion **Package files** -> **MSI (‘Windows Installer’)**
* Die .msi Datei für **64-bit x86:** herunterladen

Mit dieser Datei könnt ihr putty auf eurem **Windows** Rechner installieren. Solltet ihr einen Mac haben, müsst ihr wen fragen, der sich damit auskennt. Aber auch für Apple Betriebssysteme gibt es **SSH Clients**

## Installation bei euch zu Hause (WLAN Verbindung hat **nicht** geklappt) ##
Ok, da ist was schiefgelaufen, ist kein Beinbruch, jetzt muss aber ein wenig "gebastelt" werden. Wenn der MagigMirror schon läuft, steckt den USB On the Go (UBS-OTG) Adapter in die mittlere Micro-USB Buchse
![USB-OTG Buchse](/BPI-M2_zero_11_USB-OTG.png?raw=true "USB-OTG Buchse")

An diesen Adapter könnte ihr jetzt eine USB Tastatur und eine USB Maus anschließen. Anschließend könnt ihr aus dem Programm, welches sonst immer im Vollbildmodus im Vordergrund läuft verlassen, und eure WLAN Verbindung bei euch zuhause einrichten.
Bedenkt hierbei: Durch die Spiegelfolie ist das Bild sehr dunkel. Das eigentliche MagicMirror Programm ist genau für diesen Zweck entworfen worden, und arbeitet mit sehr hohen Kontrasten und Helligkeiten. Um das WLAN zu konfigurieren, müsst ihr das MagicMirror Programm jedoch verlassen und auf das gewöhnliche Betriebssystem wechseln. Falls ihr hier nicht genug erkennen könnt, versuch eure Arbeitsumgebung möglichst dunkel zu gestalten. Licht aus, Rollos herunterfahren, etc.
Das WLAN Menü findet ihr oben rechts im ARMBIAN Betriebssystem.


## Betriebssystem ##
Als Betriebssystem kommt ein für den Bananapi angepasstes ARMBIAN zum Einsatz. Armbian ist eine Abwandlung des Betriebssystems Debian, welches für den Betrieb mit einem ARM Prozessor (welcher auf dem Bananapi sitzt) angepasst ist.

## Konfiguration des MagicMirrors ##
Die Hauptdatei an der ihr änderungen an eurem MagicMirror vornehmen könnt, ist die Datei /home/bastian/MagicMirror/config/config.js
Wenn ihr diese Datei mit dem Tetxteditor nano per ssh öffnet, könnt ihr hier euren MagicMirro nach euren Bedürfnissen anpassen.
