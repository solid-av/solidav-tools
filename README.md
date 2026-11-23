# solidAV Tools

Fertige Apps von solidAV Medientechnik für Livestream und Veranstaltungstechnik (macOS mit Apple-Chip und Windows 10/11, 64 Bit).

| App | Wofür |
|---|---|
| **solidAV Launcher** | Startpunkt: installiert, aktualisiert und startet alle anderen Tools |
| Decks | Stream-Deck-Steuerung für vMix, ATEM, Analog Way und die eigenen Tools |
| Speaker Timer | Countdown mit Ampel, Ablauf und Nachricht an den Speaker |
| Overlay | Bauchbinden, Sendelogo und Grafiken per NDI/OMT |
| Bridge | Kreuzschiene NDI · OMT · DeckLink |
| LipSync | Bild/Ton-Versatz am vMix-Ausgang messen |

## Installation – Mac (Apple-Chip, M1 oder neuer)

1. Unter **Releases** die neueste `solidAV-Launcher-…-mac-arm64.zip` laden und doppelklicken.
2. `solidAV Launcher.app` in den Ordner **Programme** ziehen.
3. Erster Start: Die App ist nicht von Apple beglaubigt. macOS meldet beim ersten Öffnen, dass sie nicht geprüft werden kann.
   Dann **Systemeinstellungen › Datenschutz & Sicherheit** öffnen, unten bei „solidAV Launcher“ auf **Trotzdem öffnen** klicken und bestätigen.
   (Alternativ im Terminal: `xattr -dr com.apple.quarantine "/Applications/solidAV Launcher.app"`)
4. Im Launcher bei jedem gewünschten Tool auf **Installieren** klicken. Updates erscheinen dort automatisch.
5. Beim ersten Start eines Tools nach dem Zugriff auf das **lokale Netzwerk** gefragt: **Erlauben** (sonst werden keine NDI/OMT-Quellen gefunden).

## Installation – Windows 10/11 (64 Bit)

1. Unter **Releases** die neueste `solidAV-Launcher-Setup-…-win-x64.exe` laden und starten.
2. Die Apps sind nicht signiert. Windows zeigt „Der Computer wurde durch Windows geschützt“: auf **Weitere Informationen › Trotzdem ausführen** klicken.
3. Im Launcher bei jedem gewünschten Tool auf **Installieren** klicken (landet unter `%LOCALAPPDATA%\Programs\solidAV`). Updates erscheinen dort automatisch.
4. Beim ersten Start eines Tools fragt die Windows-Firewall nach Netzwerkzugriff: **Private Netzwerke** erlauben (sonst keine NDI/OMT-Quellen).

Ohne Installer: `solidAV-Launcher-…-win-x64.zip` entpacken und `solidAV Launcher.exe` starten.

## Was zusätzlich nötig ist

- **NDI:** die kostenlosen NDI Tools von ndi.video (bringen die NDI-Bibliothek mit, auf Windows die „NDI Runtime“). OMT ist in den Apps enthalten.
- **Bridge mit SDI:** Blackmagic Desktop Video (Treiber für DeckLink-Karten bzw. UltraStudio).
- **Stream Deck (Decks):** Die Elgato-Stream-Deck-App muss geschlossen sein, solange Decks läuft.
