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





## Betriebssystem ##
Als Betriebssystem kommt ein für den Bananapi angepasstes ARMBIAN zum Einsatz. Armbian ist eine Abwandlung des Betriebssystems Debian, welches für den Betrieb mit einem ARM Prozessor (welcher auf dem Bananapi sitzt) angepasst ist.
