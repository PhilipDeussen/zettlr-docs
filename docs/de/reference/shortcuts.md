# Tastaturkürzel

Diese Seite enthält eine Auflistung aller Tastaturkürzel der App.

Um sich an die Tastaturkürzel einfacher zu erinnern haben wir uns einige Gedanken zu der Belegung dieser gemacht. Im Allgemeinen folgen wir den genannte Regeln, aber es gibt ein paar Ausnahmen.

1. **Geläufige Tastaturkürzel**: Einige der Tastaturkürzel sind so geläufig, dass sie nicht in unser System passen, aber jeder diese kennt. Ein Beispiel dafür ist das Einstellungs-Tastaturkürzel (`Cmd/Ctrl+,`), ein weiteres das Tastaturkürzel zum Beenden des Bearbeiten einer Fußnote. Wir versuchen so viele von diesen wie möglich zu verwenden, um einen reibungslosen Ablauf einzuhalten.
2. **Tastaturkürzel mit hoher Priorität**: Diese Tastaturkürzel wirst du _häufig_ verwenden. Allgemein sind dies `Cmd/Ctrl` und ein einzelner Buchstabe. Bei der Belegung versuchen wir uns an den englischen Bezeichnung der Funktion zu orientieren, die diese Kürzel ausführen (**N**ew, **R**emove, **F**ind, etc). Manchmal ist das allerdings nicht möglich, wie zum Beispiel beim ablenkungsfreien Modus, der mit `Cmd/Ctrl+J` gestartet wird, da `Cmd/Ctrl+D` bereits für den Editor verwendet wird.

3. **Alternative Aktionen**: Wir nehmen die semantische Bedeutung der `Alt`-Taste ernst. Aus diesem Grund kannst du ein Tastaturkürzel mit hoher Priorität nehmen und zusätzlich `Alt` verwenden und führst damit im Allgemeinen eine alternative Aktion mit demselben Ziel aus. Einige beachtenswerte Ausnahmen sind das Entwickler-Panel, das mit `Cmd/Ctrl+Alt+I` geöffnet wird, während `Cmd/Ctrl+I` den Text kursiv stellt. **Das betrifft _alle_ Aktionen, die du mit der Maus auslösen kannst. Alle alternativen Maus-Aktionen kannst du mit `Alt+Click` auslösen. Falls das gewünschte Ergebnis mit `Alt+Click` nicht eintrifft sollte `Ctrl+Click` ebenfalls funktionieren**.

4. **Alternative Ziele**: Falls du die gleiche Aktion mit einem anderen Ziel ausführen möchtest kannst du eine `Shift`-Taste benutzen. Für den Großteil der App gilt, dass `Shift`-Tastenkombinationen von der aktuell selektierten Datei zu dem aktuell selektierten Verzeichnis ändern. Die Suche besitzt ebenfalls dieses Verhalten (`Cmd/Ctrl+F` durchsucht die Datei, `Cmd/Ctrl+Shift+F` das gesamte Verzeichnis).

## Anwendungsweite Tastaturkürzel

* `Cmd/Ctrl+,`: Öffnet Einstellungen
* `Cmd/Ctrl+Alt+,`: Öffnet PDF-Export-Einstellungen
* `Cmd/Ctrl+Q`: App schließen
* `Cmd/Ctrl+N`: Erstellt eine neue Datei im aktuellen ausgewählten Verzeichnis. Falls keines ausgewählt sein sollte ist die Tastenkombination deaktiviert.  
* `Cmd/Ctrl+Shift+N`: Erstellt ein neues Verzeichnis im aktuell ausgewählten Verzeichnis. Falls keines ausgewählt sein sollte ist die Tastenkombination deaktiviert.
* `Cmd/Ctrl+O`: Blendet den Dialog zum Öffnen eines anderen Verzeichnisses an
* `Cmd/Ctrl+S`: Speichert die Datei. Zettlr speichert die Datien automatisch, aber einige fühlen sich besser, wenn sie die Option haben manuell zu speichern.
* `Cmd/Ctrl+E`: Öffnet den Export-Dialog zum Exportieren der aktuellen Datei. Falls keine ausgewählt sein sollte ist die Tastenkombination deaktiviert.
* `Cmd/Ctrl+R`: Umbennen der geöffneten Datei. Falls keine ausgewählt sein sollte ist die Tastenkombination deaktiviert.
* `Cmd/Ctrl+Shift+R`: Umbenennen des aktuellen Verzeichnisses. Falls keines ausgewählt sein sollte ist die Tastenkombination deaktiviert.
* `Cmd/Ctrl+Delete`: Löscht die aktuelle Datei. Falls keine ausgewählt sein sollte ist die Tastenkombination deaktiviert.
* `Cmd/Ctrl+Shift+Delete`: Löscht das aktuelle Verzeichnis. Falls keines ausgewählt sein sollte ist die Tastenkombination deaktiviert.
* `Cmd/Ctrl+Shift+F`: Fokussiert das globale Suchfeld
* `Cmd/Ctrl+Alt+L`: Schaltet das Theme zwischen hell und dunkel hin und her

* `Cmd/Ctrl+Alt+S`: Umschalten der Darstellung der Textausschnitte

* `Cmd/Ctrl+Shift+1`: Ein-/ausblenden des Seitenleisten-Modus um entweder die Datei-Liste oder die Baumansicht zu sehen. In dem erweiterten Seitenleisten-Modus deaktiviert.

* `Cmd/Ctrl+?`: Ein-/ausblenden der Seitenleiste für Anhänge

* `Cmd/Ctrl+[0-9]`: Öffnen des kürzlich verwendete Dokuments an den Stellen 0 bis 9 in der Liste kürzlich verwendeter Dokumente (Datei->Kürzlich verwendete Dokumente).

* `Cmd+Ctrl+F` (macOS) `F11` (windows/Linux): Ein-/ausschalten des Vollbildmodus

* `Cmd/Ctrl+W`: Schließen des Anwendungsfensters. Unter Windows und Linux schließt sich hiermit auch die App.

* `Cmd/Ctrl+M`: Verkleinert das Anwendungsfenster

* `F1`: Öffnet diese Dokumentation. Der Link wird in deinem Standard-Browser geöffnet.

**Falls der Debug-Modus eingeschaltet ist**

* `F5`: Neu laden der grafischen Oberfläche.
* `Cmd+Alt+I` (macOs) `Ctrl+Shift+I` (Windows/Linux): Öffnet die Chrome-Entwicklerwerkzeuge

## Textfeld-bezogene anwendungsweite Tastaturkürzel

* `Cmd/Ctrl+Z`: Rückgängig
* `Cmd/Ctrl+Shift+Z`: Wiederholen
* `Cmd/Ctrl+X`: Ausschneiden
* `Cmd/Ctrl+C`: Kopieren
* `Cmd/Ctrl+V`: Einfügen
* `Cmd/Ctrl+A`: Alles auswählen

## Editor-bezogene Tastaturkürzel

* `Cmd/Ctrl+Alt+C`: Kopiere als HTML. Falls etwas selektiert ist wird es in HTML umgewandelt und nicht als einfacher Text kopiert. Damit kannst du es zum Beispiel in Textverarbeitungsprogramme einfügen.
* `Cmd/Ctrl+Shift+C`: Ein-/auskommentieren des selektierten Textes (oder einen neuen HTML-Kommentar an der aktuellen Cursor-Position einfügen).
* `Cmd/Ctrl+X`: Ausschneiden. Falls der Fokus auf dem Editor liegt wird die aktuelle Auswahl ausgeschnitten. Falls nichts ausgewählt sein sollte wird **die gesamte Zeile** der aktuellen Cursor-Position ausgeschnitten.
* `Cmd/Ctrl+V`: Einfügen. Falls der Fokus auf dem Editor liegt und du gerade eine ganze Zeile ausgeschnitten hast, wird die das Ausgeschnitte in der Zeile über dem Cursor eingefügt. Falls die Zwischenablage formatierten Text enthält wird diese beibehalten.
* `Cmd/Ctrl+Shift+V`: Das gleiche wie oben, nur das hier die Formatierung des Textes nicht beibehalten wird.
* `Cmd/Ctrl+B`: Markierten Text fett stellen oder neue Zeichen für fette Formatierung einfügen.
* `Cmd/Ctrl+I`: Markierten Text kursiv stellen oder neue Zeichen für kursive Formatierung einfügen.
* `Cmd/Ctrl+K`: Neue Link-Vorlage einfügen oder den ausgewählten Text in die Linkunterschrift eines neuen Links umwandeln. Falls die Zwischenablage einen erkennbaren Link enthält wird auch das Ziel des Links gefüllt.
* `Cmd/Ctrl+F`: Öffnet das Such-Popup in dem aktuell fokussierten Editor (entweder der Haupteditor oder das Quicklook-Fenster).
* `Ctrl+Alt+F` (Windows/Linux) `Cmd+Alt+R` (macOS): Einfügen einer neuen Fußnote an der aktuellen Cursor-Position.
* `Cmd/Ctrl+L`: Neue ID mit dem Generator-Muster aus den Einstellungen generieren und an der aktuellen Cursor-Position einfügen.
* `Cmd/Ctrl+0`: Zurücksetzen der Schriftgröße auf die Standardeinstellung des Editors.
* `Cmd+Plus` (macOS) `Ctrl+Shift+Plus` (Windows/Linux): Schriftgröße des Editors erhöhen.
* `Cmd/Ctrl+Minus`: Schriftgröße des Editors verringern.
* `Tab`: Liste einrücken.
* `Shift-Tab`: Ausrücken einer Liste.
* `Shift-Enter`: Speichern des Referenztextes beim Bearbeiten einer Fußnote. Andernfalls verhindert es das automatische Einfügen eines neuen Listenelements.
* `Ctrl-Enter`: Neue Zeile unterhalb der aktuellen Cursor-Position einfügen und den Cursor am Anfang dieser positionieren.
* `Ctrl-Shift-Enter`: Neue Zeile oberhalb der aktuellen Cursor-Position einfügen und den Cursor am Anfang dieser positionieren.

## Tastaturkürzel des Tabelleneditors

Diese Tastaturkürzel funktionieren in jedem Tabelleneditor sobald du im Bearbeitungsmodus bist, den du aktivierst, indem du in die Tabelle klickst.

* `Tab`: Zur nächsten Zelle gehen. Falls die letzte Spalte aktiv ist, geht es in die erste Zelle der nächsten Zeile. Falls dein Cursor in der letzten Spalte der letzten Reihe ist wird automatisch eine neue Zeile hinzugefügt.
* `Shift-Tab`: Zur vorherigen Zelle gehen. Falls der Cursor in der ersten Spalte ist, geht dieser automatisch zur letzten Zelle der vorherigen Spalte.
* `Return`: Geht zur selben Spalte in der nächsten Zeile. Falls dein Cursor in der letzten Reihe ist wird automatisch eine neue Zeile hinzugefügt.
* `Arrow Up/Arrow Down`: Geht zur nächsten/vorherigen Reihe in der gleichen Spalte. Falls du in der ersten oder letzten Zeile bist werden keine neuen Zeilen hinzugefügt.
* `Arrow Left/Arrow Right`: Bewegt den Cursor nach links/rechts. Falls der Cursor am Anfang/Ende einer Zelle ist geht dieser zur vorherigen/nächsten Zelle.

## Tastaturkürzel für Vorschauen

* `Arrow Up`: Öffnet die vorherige Datei.
* `Arrow Down`: Öffnet die nächste Datei.
* `Cmd/Ctrl+Arrow Up`: Springt zum Anfang der Liste.
* `Cmd/Ctrl+Arrow Down`: JSpringt zum Ende der Liste.

## Popup-bezogene Tastaturkürzel

* `ESC`: Hat ein Textfeld innerhalb des Popups den Fokus lässt sich mit Escape das Popup schließen.

**Im Suchen-Popup des Haupteditors**

* `Return`: Solange das _search_-Textfeld den Fokus hat wird das Tastaturkürzel die nächste gefundene Stelle deines Suchworts auswählen. Solange das _replace_-Textfeld den Fokus hat wird es das nächste Vorkommen deines Suchtextes mit dem neuen Text ersetzen und automatisch zum nächsten Vorkommen gehen.
* `Alt+Return`: Solange das _replace_-Textfeld den Fokus hat will dieses Tastaturkürzel alle Vorkommen deines Suchtextes durch den neuen Text ersetzen. 
