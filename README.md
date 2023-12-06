# Rodecaster-Pro-1-mAirlist-Konfiguration
Hier möchte ich meine Konfiguration mit euch teilen in der ich mAirList mit dem Rodecaster Pro 1 erfolgreich betreibe. 
# Rodecaster-Pro-1-mAirlist-Konfiguration
Hier möchte ich meine Konfiguration mit euch teilen in der ich mAirList mit dem Rodecaster Pro 1 erfolgreich betreibe. 

Inhalt Liesmich.txt
Stellt vor dem Import der Dateien und Funktionen sicher, das ihr die MIDI Funktion eures Rodecasters aktiviert habt!

RodeCasterPro1 Einrichtung für mAirList als EINZELSENDEPLATZ
Audiokonfiguration bitte der PDF entnehmen!
Dies sind meine Einstellungen der MIDI Steuerungen für das Rode Rodecaster Pro1 in mAirList 7.
ACHTUNG: Bestimmte Remote Befehle funktionieren erst ab der Version 7.1.5 mit Snapshot Build 5234 (oder höher)
Daher vor Einrichtung auf Updates überprüfen.
Ob alle Einstellungen in der V6 auch anwendbar sind kann ich nicht zu 100% garantieren.
///////////

Ihr müsst lediglich alle ini und mls Dateien 1:1 Importieren. 
Funktion und Workflow findet ihr dann ebenfalls in den beiliegenden PDFs.

///////////

Schritt 1:
mls Scripte importieren in Hintergrundscipte von mAirList:
mAirList Konfiguration/Hintergundscripte:
Quell-Ordner .../mAirListconfigs of Rodecaster Pro1/Backgroundscipts/
- MidiFaderStartPlayerA.mls
- MidiFaderStartPlayerB.mls
- MidiFaderStartCart1.mls

Schritt 2:
ini Fernsteuerungen einzeln importieren in Fernsteuerungsübersicht von mAirList:
mAirList Konfiguration/Fernsteuerungen:
Quell-Ordner .../mAirListconfigs of Rodecaster Pro1/Remotecommands/ 		///WICHTIG REIHENFOLGE BEACHTEN!
- MidiFaderstartRemotePlayerA.ini
- MidiFaderstartRemotePlayerB.ini
- MidiFaderstartRemoteCart1.ini
- MidiRemoteRodecaster1General.ini

Diese Reihenfolge und Separierung der Faderstartfunktion ist wichtig und ist Teil der Funktion
die den Faderstart ein und ausschalten kann.
Danach muss in der Fernsteuerung folgende Reihenfolge stehen: 
[ ] MIDI 					///Inhalt: MidiFaderstartRemotePlayerA.ini
[ ] MIDI 					///Inhalt: MidiFaderstartRemotePlayerB.ini
[ ] MIDI 					///Inhalt: MidiFaderstartRemoteCart1.ini
[X] MIDI 					///INhalt: MidiRemoteRodecaster1General.ini

Solltet ihr noch andere Fernsteuerungen besitzen, diese bitte an Ende der Liste ziehen.

Schritt 3:
Erweiterte Buttons importieren: 
mAirList GUI/Bildschirmobjekte:
Quell-Ordner .../mAirListconfigs of Rodecaster Pro1/Screenobjekts/
- AdvacedButtonPlayerFaderStartA.ini
- AdvacedButtonPlayerFaderStartB.ini
- AdvacedButtonPlayerFaderStartCart1.ini

RADIOTOM
https://laut.fm/hitradiotom
