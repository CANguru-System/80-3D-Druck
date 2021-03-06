# 80-3D-Druck
 3D-Druckdateien für ausgewählte Hardwarekomponenten
    
Es ist sicherlich wünschenswert, für die Weichensteuerung einen Antrieb einsetzen zu können, der die Weiche langsam umstellt und unter der Weiche eingebaut werden kann, ohne große Löcher in Weichenauflage sägen zu müssen. Dafür wird ein sehr kleines und flaches Servo mit Linearantrieb benötigt.
Auf dem Markt findet man dazu keine große Auswahl. Ich habe mir das Servo VS-19 Pico Linear Servo ausgesucht, das von der Firma Robotshop angeboten wird.  
![Linear Servo VS-19 Pico](https://github.com/CANguru-System/80-3D-Druck/blob/master/Bilder/Bild04.PNG)  
Zusammen mit der Halterung steht das Servo etwa 4 mm über (besser unter) der Weiche hervor. Da wir unter die Gleise eine 5 mm starke Matte aus Schrittschalldämmung legen, reicht es, hier einen kleinen Ausschnitt vorzunehmen.   
Bevor wir uns das Ergebnis anschauen, will ich ein paar Hinweise geben, wie die Halterungen für die Weichen mit Hilfe eines 3D-Druckers entstanden sind.
Als erste Aufgabe ist die Frage zu klären, welche Entwurfssoftware will ich einsetzen. Ich habe mich für **TinkerCAD** entschieden und das aus diversen Gründen. Mit dessen schlichtem Klötzchenkonzept gelingt ein Design auch einem nicht sehr Geübten recht schnell. Somit ist es leicht bedienbar, im Browser sowie auf einer App unter iOS verfügbar und zudem ist es kostenlos. Sicherlich ist die Auswahl auch eine Geschmacksfrage, aber ich bin mit diesem Werkzeug sehr zufrieden. Beim Entwurf einer Halterung oder irgendeinem anderen Objekt ist es sehr wichtig zu bedenken, dass man in einem dreidimensionalen Raum arbeitet, bei dem Überhänge an Objekten nur sehr begrenzt möglich sind. Denn der Drucker kann sein flüssiges Filament natürlich nicht freischwebend platzieren, sondern er möchte es möglichst nur stapeln. Dabei führen in vielen Fällen einfache Lageveränderungen des Objektes zum Ziel. Was eben noch in der Luft schwebte, liegt durch eine 90 Grad-Drehung des Objekts plötzlich auf dem Tisch des Druckers auf.  
Wenn man sich dann mit der Klötzchenwelt von TinkerCAD angefreundet und sein Objekt entworfen hat, muss man es nun „slicen“ lassen. Denn die stl-Entwurfsdatei kann der Drucker nicht verarbeiten. Vielmehr benötigt er eine Datei, die das Objekt nun in Schichten darstellt. Dazu nutze ich **Ultimaker Cura**, auch kostenlos. Hier ist nicht viel zu tun. Dieses Programm erzeugt daraus eine auf den 3D-Drucker abgestimmte gcode-Datei, die der 3D-Drucker verarbeiten kann. Da ich den Drucker über ein USB-Kabel mit dem PC verbunden habe, kann ich aus Ultimaker Cura den Druckprozess direkt starten. Und dann heißt es warten. Denn, obwohl der Druckkopf stetig hin und her flitzt, dauert es doch eine Weile, bis auch ein kleines Objekt entstanden ist. Hinzu kommt aber noch, dass der erste Entwurf in der Regel nicht der letzte ist. Bis alles genau so ist, wie man sich das vorstellt, und auch passgenau ist, dreht man doch die ein oder andere Runde im Entwurfsprozess.  
So sieht die Halterung aus:  
![Halterung für das Linear Servo VS-19 Pico](https://github.com/CANguru-System/80-3D-Druck/blob/master/Bilder/Bild01.PNG)  
Und so in TinkerCAD:
![TinkerCAD](https://github.com/CANguru-System/80-3D-Druck/blob/master/Bilder/Bild02.PNG)  
Unter der Weiche sieht man die eingebaute Halterung mit dem Servo:  
![Eingebautes Linear Servo](https://github.com/CANguru-System/80-3D-Druck/blob/master/Bilder/Bild03.PNG)   
Und hier nur das Servo:  
![Linear Servo VS-19 Pico](https://github.com/CANguru-System/80-3D-Druck/blob/master/Bilder/Bild04.PNG)   
Hier noch mal die Erklärung der Parameter, die mit dem CANguru-Server eingestellt werden können:  
![Parameter fuer das Linear Servo](https://github.com/CANguru-System/80-3D-Druck/blob/master/Bilder/Bild05.PNG)   
Hier die Weiche kurz vor dem Einbau. Die Stromversorgung für die LED wird von der Servoversorgung abgenommen. Das sind dann nur 3,3 Volt und die LED hat auch keine große Strahlkraft; aber sie leuchtet und wieder ein paar Kabel weniger!  
![Anschluesse an das Linear Servo](https://github.com/CANguru-System/80-3D-Druck/blob/master/Bilder/Bild06.JPG)   
Diese Halterung passt für alle Märklin C-Gleis geraden Weichen, Bogenweichen sowie Doppelkreuzungsweichen.  
![Sicherung fuer den Hebel](https://github.com/CANguru-System/80-3D-Druck/blob/master/Bilder/Bild07.JPG)   
Vorsichtshalber habe ich noch eine kleine Drahtsicherung an den Servoskopf angebracht, damit der Hebel auf keinen Fall abrutschen kann.  
Viel Spaß damit!  
