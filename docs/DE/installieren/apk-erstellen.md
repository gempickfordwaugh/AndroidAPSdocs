# AndroidAPS installieren - App erstellen

Dieser Artikel ist in zwei Teile geteilt.
* Im "Überblick" werden die wichtigsten Schritte kurz zusammengefasst
* In der "Schritt für Schritt Anleitung" wird detailiert auf die einzelnen Punkte mithilfe von Screenshots eingegangen. Aufgrund der Weiterentwicklung von Android Studio oder Nutzung von eines anderen Betriebssystem (Windows, Linux, Mac OS), kann es sein, dass die Screenshots nicht identisch mit dem sind, was du siehst. Bei großeren Veränderungen oder fehlenden, bzw. falschen Informationen wäre es hilfreich, dies den Entwicklern in der Facebookgruppe 'Android APS' oder in den Gitter Chats [Android APS](https://gitter.im/MilosKozak/AndroidAPS) oder [AndroidAPSwiki](https://gitter.im/AndroidAPSwiki/Lobby) mitzuteilen, sodass das Wiki stets aktuell ist.   


## Überblick

Kurzfassung der wichtigsten Schritte.

* Installiere git
* Installiere and konfiguriere Android Studio.
* Nutze git clone, um den Quellcode von AndroidAPS auf Github zu downloaden. 
* Öffne das gedownloadete Projekt in Android Studio. 
* Erstelle die signierte APK.
* Schicke die erstellte APK an dein Smartphone.


## Schritt für Schritt Anleitung

Detailierte Beschreibung der notwendigen Schritte

* Installiere git
  * [Windows](https://gitforwindows.org/)
  * [Mac OS X](http://sourceforge.net/projects/git-osx-installer/)
  * Linux - installiere einfach ein 'Package Git' über einen 'Package Manager' deiner Linux-Distribution
* Installiere [Android Studio](https://developer.android.com/studio/install.html).
* Konfiguriere Android Studio gleich beim ersten Öffnen des Programms.

Wähle "Do not import settings", da bisher keine Einstellungen vorgenommen wurden.
![Screenshot 1](../../images/Installation_Screenshot_01.png)

Klicke auf "Next".
![Screenshot 2](../../images/Installation_Screenshot_02.png)

Wähle "Standard" Installation und klicke auf "Next".
![Screenshot 3](../../images/Installation_Screenshot_03.png)

Wähle "Intellij" als "UI theme" (Benutzeroberfläche) und klicke auf "Next".
![Screenshot 4](../../images/Installation_Screenshot_04.png)

Klicke auf "Next" in dem Fenster "Verify Settings".
![Screenshot 5](../../images/Installation_Screenshot_05.png)

The Android emulator (to emulate the smartphone on your PC or Mac) is not used to build the APK.
Du kannst auf 'Finish' klicken, um die Installation zu beenden und die vorgeschlagene Dokumentation bei Bedarf später lesen.

![Screenshot 6](../../images/Installation_Screenshot_06.png)

Android Studio lädt einige benötigte Software-Komponenten herunter.
Du kannst auf 'Show Details' klicken um zu sehen was passiert, aber das ist nicht relevant für den weiteren Verlauf.
![Screenshot 7](../../images/Installation_Screenshot_07.png)
![Screenshot 8](../../images/Installation_Screenshot_08.png)

Wenn der Download beendet ist, klicke auf "Finish".
![Screenshot 9](../../images/Installation_Screenshot_09.png)

* Herzlichen Glückwunsch, jetzt hast du die Android Studio soweit fertig installiert und kannst mit dem "Cloning" des Quellcodes beginnen. Hier ist allerdings auch ein guter Zeitpunkt, um Pause zu machen.


* Nutze "git clone" in Android Studio wie in dem folgendem Screenshot angegeben. Wähle "Check out project from Version Control" und "Git" aus.
![Screenshot 10](../../images/Installation_Screenshot_10.png)
![Screenshot 11](../../images/Installation_Screenshot_11.png)

Gib die URL der Hauptseite des AndroidAPS Repositorys ("https://github.com/MilosKozak/AndroidAPS") an und klicke auf "Clone".
![Screenshot 13](../../images/Installation_Screenshot_13.png)

Android Studio fängt an das Projekt zu kopieren/"clonen". Klicke nicht auf "Background".
![Screenshot 14](../../images/Installation_Screenshot_14.png)

Beende "checkout from version control", indem du auf "Yes" klickst und das Projekt öffnest.
![Screenshot 15](../../images/Installation_Screenshot_15.png)

Nutze den Standard "default gradle wrapper" und klicke auf "OK".
![Screenshot 16](../../images/Installation_Screenshot_16.png)

Lese und schließe den "Tip of the Day", indem du auf "close" klickst.
![Screenshot 17](../../images/Installation_Screenshot_17.png)

* Perfekt, du hast jetzt eine Kopie des Quellcodes in Android Studio erstellt. Weiter geht es mit mit dem Kompilieren der APK. 
* Als nächstes wird dich eine Fehlermeldung erwarten. Glücklicherweise schlägt Android Studio gleich die Lösung vor: 

Klicke auf "Install missing platform(s) and sync project", da Android Studios noch einige Komponenten installieren muss.
![Screenshot 18](../../images/Installation_Screenshot_18.png)

Akzeptiere die Lizenzvereinbarung, indem du auf "Accept" und "Next" klickst.
![Screenshot 19](../../images/Installation_Screenshot_19.png)

Wie beschrieben, einfach warten, bis die Installation abgeschlossen ist.
![Screenshot 20](../../images/Installation_Screenshot_20.png)

Ist diese abgeschlossen, dann klicke wieder auf "Finish". 
![Screenshot 21](../../images/Installation_Screenshot_21.png)

Und dann wird wohl wieder der nächste Fehler auf dich zukommen... Klicke auf “Install Build Tools and sync project”  um die fehlenden "Tools" zu installieren.
![Screenshot 22](../../images/Installation_Screenshot_22.png)

Warte, bis die "Tools" fertig installiert sind.
![Screenshot 23](../../images/Installation_Screenshot_23.png)

Sobald sie fertig installiert sind, klicke auf "Finish".
![Screenshot 24](../../images/Installation_Screenshot_24.png)

Und der nächste Fehler tritt auf. Klicke einfach wieder auf "Install missing platform(s) and sync project".
![Screenshot 25](../../images/Installation_Screenshot_25.png)

Warte, bis die Installation abgeschlossen ist.
![Screenshot 26](../../images/Installation_Screenshot_26.png)

Sobald sie fertig ist, klicke auf "Finish".".
![Screenshot 27](../../images/Installation_Screenshot_27.png)

Und so geht es weiter: Klicke auf "Install Build Tools and sync project" um den Fehler zu beheben und die "Tools" zu installieren.
![Screenshot 28](../../images/Installation_Screenshot_28.png)

Warte, bis die "Tools" fertig installiert sind.
![Screenshot 29](../../images/Installation_Screenshot_29.png)

Sobald sie fertig installiert sind, klicke auf "Finish".
![Screenshot 30](../../images/Installation_Screenshot_30.png)

Sieht so aus, als ob wir die Fehlermeldungen hinter uns haben :). Zeit für eine Trinkpause?!
![Screenshot 31](../../images/Installation_Screenshot_31.png)

Nun wird von Android Studios empfohlen,"Gradle Plugin" auf Version 4.4 zu aktualisieren. Für den Fall, dass du die AndroidAPS App mit einer Version älter als Android APS 2.0 oder ein 'release candidate'(RC)Version bauen willst, dann klicke NICHT auf "Update", sondern auf "Remind me tomorrow", ansonsten wird die App nicht kompiliert werden können. 
Für AndroidAPS ist es kein Nachteil oder Unterschied, mit einer älteren Version von 'Gradle' gebaut zu werde. "Gradle" ist nur dafür da, den "Build Process" zu kontrollieren. Wenn du eine Version von AndroidAPS 2.0 oder größer bauen willst, könntest du dennoch auf Version 4.4 aktualisieren. 

![Screenshot 32](../../images/Installation_Screenshot_32.png)

Der Prozess läuft weiter...
![Screenshot 33](../../images/Installation_Screenshot_33.png)

Perfekt, der erste "Build Prozess" ist jetzt fertig.
![Screenshot 34](../../images/Installation_Screenshot_34.png)

Als nächstes, gehe zum "Build" Menü und "Generate Signed APK". Es ist notwenig, die App digital zu signieren, da Android aus Sicherheitsgründen nur signierten Quellcode akzeptiert. Falls dich das Thema interessiert, findest du [hier](https://developer.android.com/studio/publish/app-signing.html#generate-key) mehr.
![Screenshot 39](../../images/Installation_Screenshot_39.png)

Wähle "App" aus und klicke auf "Next".
![Screenshot 40](../../images/Installation_Screenshot_40.png)

Klicke auf "Create new..." um einen "Keystore" zu erstellen. Dieser ist nichts anderes als ein Ordner, indem die Informationen deiner Signatur der App gespeichert ist. Diese ist verschlüsselt und mit Passwörtern versehen. Du solltest dich an den Dateipfad ("Key store path") und die Passwörter erinnern. Falls du diese vergessen hast, ist es aber auch nicht weiter tragisch, da du sonst einfach einen neuen "Keystore" erstellen kannst.
![Screenshot 41](../../images/Installation_Screenshot_41.png)

* Fülle die Informationen in den nächsten Textfeldern aus.
  * "Key store path": Der Ort, an dem der Keystore gespeichert wird
  * "Password": Um sicher zu gehen, dass du das richtige Passwort eingibst, das du gerne hättest, ist es notwendig, dass Passwort zwei mal einzugeben, in "Password" und "Confirm", was so viel wie "bestätigen" bedeutet.
  * "Alias": ist der Name für die Verschlüsselung. Du kannst ihn stehen lassen, wie vorgegeben oder jeden beliebigen anderen Namen geben.
  * "(key) Password": hier gibst du das Passwort für die Verschlüsselung selber ein. Das Passwort muss wieder in "Cofirm" ein zweites Mal eingetragen werden
  * "Validity": Übersetzt bedeutet das "Gültigkeit". Du kannst die "25 years" so stehen lassen
  * Du bist nur verpflichtet, "First and Last Name" ("übersetzt: Vor- und Nachname") auszufüllen, kannst aber auch den Rest ergänzen.
Klicke danach auf "OK".
![Screenshot 42](../../images/Installation_Screenshot_42.png)

Fülle die Informationen von dem Keystore, den du gerade erstellt hast, aus  und klicke auf "Next".
![Screenshot 43](../../images/Installation_Screenshot_43.png)

Wähle "full" in dem "Flavors" Menü aus, um die vollständige AndroidAPS App zu erstellen und klicke auf V1 "Jar Signature" (V2 ist optional) und klicke auf "Finish".
Folgende Informationen könnten später für dich nützlich sein:
* "Release" solltest du immer lassen, "Debug" ist nur für Programmierer, um Fehler zu finden.
* Wähle den "Flavour", den du kompilieren möchtest:
  * full: Gesamte App (inkl. open loop, closed loop, Smartwatch-Steuerung)
  * openloop (dieser gibt nur temporäre Basalraten-Vorschläge, die nur manuell auszuführen sind)
  * pumpcontrol (kein Loop, mit dieser kann man die Pumpe über die App bedienen)
  * nsclient (hier werden z.B. die Daten eines anderen Nutzers dargestellt und Careportal-Einträge können hinzugefügt werden)

![Screenshot 44](../../images/Installation_Screenshot_44.png)

Im event log sollte jetzt angezeigt werden, dass die signierte APK erfolgreich generiert wurde.
![Screenshot 45](../../images/Installation_Screenshot_45.png)

Klicke auf "locate" im "event log".
![Screenshot 46](../../images/Installation_Screenshot_46.png)

Es sollte sich ein Datei Manager öffnen. Dies könnte bei dir anders aussehen (dieser Screenshot wurde mit einem Linux-PC gemacht). In Windows wird sich der "Explorer" öffnen, in Mac OS X der "Finder". Egal in welchem Datei Manager sollte jetzt eine APK sichtbar sein. Diese ist aber unglücklicherweise NICHT die, die wir suchen, diese ist nur die "wear-release.apk".
![Screenshot 47](../../images/Installation_Screenshot_47.png)

Um zu der gesuchten APK zu gelangen, musst du zu dem Ordner AndroidAPS/app/full/release gehen und nach der "app-full-release.apk" Datei Ausschau halten. Das ist deine noch nicht installierte AndroidAPS App.
Der nächste Schritt ist es also, die APK an das Smartphone zu senden. Dafür gibt es verschiedene Möglichkeiten, wie Email, Bluetooth, Cloud Upload. 
![Screenshot 48](../../images/Installation_Screenshot_48.png)

Für Gmail und jede andere Methode auch, ist es Vorausetzung, dass das Installieren von unbekannten Apps für diese Quellen erlaubt ist. Dies kannst du in "Einstellungen- unbekannte Apps installieren" ändern.
![Screenshot 49](../../images/Installation_Screenshot_49.png)

Klicke dort auf "aus dieser Quelle zulassen". Nach der Installation ist es empfehlenswert dies aus Sicherheitsgründen wieder rückgängig zu machen.
![Screenshot 50](../../images/Installation_Screenshot_50.png)

Der letzte Schritt ist es, auf die APK Datei zu klicken und die App zu installieren. Sollte es nicht funktionieren, kann es sein, dass sich eine ältere Version mit einem anderen "Key"/einer anderen Signatur auf dem Handy befindet, sodass man diese erst deinstallieren muss, aber zuerst die Einstellung der App exportieren sollte.

Herzlichen Glückwunsch, du hast es geschafft! Nun kannst du AndroidAPS starten und einrichten. 

Maybe someone could add a link to the next step
