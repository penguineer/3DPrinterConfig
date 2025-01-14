# Netz39 -- Konfigurationen für die 3D-Drucker
Dieses Repository enthält die aktuellen config-files für die [Netz39- Drucker](https://www.netz39.de/wiki/internal:inventory:tools:3d_printer).

Für den aktuellen Delta-Drucker (Anycubic Kossel Linear Plus) wird [PrusaSlicer](https://www.prusa3d.com/de/page/prusaslicer_424/) genutzt.
Für die momentan stillgelegten Drucker wurde [Cura](https://ultimaker.com/en/products/cura-software) verwendet.

## PrusaSlicer (Delta-Drucker "Anycubic Kossel Linear Plus")
  * [PrusaSlicer](https://www.prusa3d.com/de/page/prusaslicer_424/) auf deinem Rechner installieren
  * Konfig-Datei für den Drucker reinladen (hier `anycubic_kossel_linear_plus_n39_config.ini`)
  * Im `NETZ39`-WLAN den Octoprint-Service des Druckers in PrusaSlicer einbinden:
    * Seitenreiter 'Druckeinstellungen' -> Zahnradsymbol 'Physischen Drucker bearbeiten'
      * Host Typ: OctoPrint
      * IP:  siehe [Wiki](https://wiki.netz39.de/internal:inventory:tools:3d_printer:anycubic_kossel_linear_plus)
      * API Key: siehe [Wiki](https://wiki.netz39.de/internal:inventory:tools:3d_printer:anycubic_kossel_linear_plus)
      * möglicherweise muss 'CA-Zertifikat ignorieren' angewählt werden (unter Windows)
      * mit Button 'Test' die Verbindung testen
  * CAD importieren
  * 'Slice'-Button drücken
  * 'Zum Drucker senden'-Button drücken


## Cura (Anet-A8 oder Tevo-Tarantula)
Zum Hinzufügen eines Drucker-Profils zu Cura reicht es aus, die entsprechende ProjectFile-Datei (*.3mf) mit Cura zu öffnen. In einem Auswahlfenster wird gefragt, ob ihr einen neuen Drucker hinzufügen möchtet. Das hinterlegte 3D-Objekt in dem ProjektFiles ist der [Calibration Cube](https://www.thingiverse.com/thing:1278865).