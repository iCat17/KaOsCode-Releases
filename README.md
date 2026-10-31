# KaOsCode Releases

Installationsdateien der Apps von KaOsCode: APKs für Android, für Benchly zusätzlich ein Installer für Windows.
Der Quellcode liegt nicht in diesem Repository.

*English version below.*

## Apps

| App | Beschreibung | Releases | Datenschutz |
|---|---|---|---|
| **Spectare PDF** | PDF-Viewer mit Dokumentenscanner | [Releases](https://github.com/iCat17/KaOsCode-Releases/releases?q=spectare) | Erhebt selbst keine Daten: keine Berechtigungen, kein Internetzugriff, keine Sicherung. Der optionale Scanner kommt aus den Google Play Services: Die Dokumente bleiben auf dem Gerät, Google erhält Nutzungsstatistiken zum Scanner |
| **Benchly** | Kursverläufe von Aktien, ETFs, Indizes und Krypto vergleichen | [Releases](https://github.com/iCat17/KaOsCode-Releases/releases?q=benchly) | Erhebt selbst keine Daten. Kurse werden direkt von Yahoo Finance geladen, dabei sieht Yahoo IP-Adresse und abgefragte Symbole. Bei der Suche nach einer WKN wird diese an OpenFIGI (Bloomberg) gesendet |
| **Arrowly** | Logikpuzzle: Pfeile in der richtigen Reihenfolge vom Feld schieben | [Releases](https://github.com/iCat17/KaOsCode-Releases/releases?q=arrowly) | Erhebt keine Daten: keine Berechtigungen, kein Internetzugriff; Spielstand nur auf dem Gerät |
| **FlexStock** | Inventar mit Barcode-Scanner, Fotos und Einkaufsliste | [Google Play](https://play.google.com/store/apps/details?id=com.kaoscode.flexstock) | Erhebt selbst keine Daten, das Inventar bleibt auf dem Gerät. Beim Barcode-Scan wird nur die Barcode-Nummer an öffentliche Produktdatenbanken (u. a. Open Food Facts, Google Books, UPCitemdb) gesendet, die dabei die IP-Adresse sehen. [Datenschutzerklärung](https://icat17.github.io/flexstock-privacy/) |

FlexStock gibt es nur bei Google Play, hier liegen keine Installationsdateien dafür.

## Installation (Android)

1. Unter **Releases** die neueste Version der App öffnen und die Datei `….apk` herunterladen.
2. Die Datei antippen. Android fragt beim ersten Mal, ob diese Quelle (z. B. Browser oder „Dateien“) Apps installieren darf: erlauben, zurück, **Installieren**.
3. Falls Google Play Protect warnt: **Trotzdem installieren**.

Ein Entwicklermodus ist nicht nötig.

## Installation (Windows, Benchly)

1. Unter **Releases** die neueste Benchly-Version öffnen und `benchly-….-setup.exe` herunterladen.
2. Die Datei ausführen. Der Installer ist nicht signiert, deshalb zeigt Windows „Der Computer wurde durch Windows geschützt“: **Weitere Informationen** → **Trotzdem ausführen**.
3. Optional prüfen: Die Ausgabe von `Get-FileHash .\benchly-….-setup.exe` (PowerShell) muss mit dem Inhalt der `.sha256`-Datei aus dem Release übereinstimmen.

Update: den neuen Installer herunterladen und ausführen, Vergleich und Einstellungen bleiben erhalten.

## Automatische Updates mit Obtainium

[Obtainium](https://github.com/ImranR98/Obtainium) installieren, dann **App hinzufügen**:
- **Quell-URL:** `https://github.com/iCat17/KaOsCode-Releases`
- **Release-Titel nach regulärem Ausdruck filtern:** `^Spectare` (bzw. der Name der gewünschten App)

## Kontakt

kaos-code@outlook.com

---

# KaOsCode Releases (English)

Installation files for KaOsCode's apps: APKs for Android, plus a Windows installer for Benchly.
The source code is not part of this repository.

Spectare PDF collects no data itself: no permissions, no internet access, no backup. The optional scanner is provided by Google Play Services: documents stay on the device, Google receives usage statistics about the scanner.
Benchly collects no data itself. Prices are loaded directly from Yahoo Finance, which sees your IP address and the requested symbols. When you search for a WKN, it is sent to OpenFIGI (Bloomberg).
Arrowly collects no data: no permissions, no internet access; game progress stays on the device.
FlexStock (inventory with barcode scanner, photos and shopping list) is only available on [Google Play](https://play.google.com/store/apps/details?id=com.kaoscode.flexstock), there are no installation files here. It collects no data itself, your inventory stays on the device. When you scan a barcode, only the barcode number is sent to public product databases (including Open Food Facts, Google Books, UPCitemdb), which see your IP address. [Privacy policy](https://icat17.github.io/flexstock-privacy/)

## Installation (Android)

1. Open the latest release of the app under **Releases** and download the `….apk` file.
2. Tap the file. On first use, Android asks whether this source (e.g. browser or "Files") may install apps: allow it, go back, tap **Install**.
3. If Google Play Protect shows a warning: **Install anyway**.

No developer mode required.

## Installation (Windows, Benchly)

1. Open the latest Benchly release under **Releases** and download `benchly-….-setup.exe`.
2. Run the file. The installer is not signed, so Windows shows "Windows protected your PC": **More info** → **Run anyway**.
3. Optional check: the output of `Get-FileHash .\benchly-….-setup.exe` (PowerShell) must match the content of the `.sha256` file in the release.

Update: download and run the new installer; your comparison and settings are kept.

## Automatic updates with Obtainium

Install [Obtainium](https://github.com/ImranR98/Obtainium), then **Add app**:
- **Source URL:** `https://github.com/iCat17/KaOsCode-Releases`
- **Filter release titles by regular expression:** `^Spectare` (or the name of the app you want)

## Contact

kaos-code@outlook.com
