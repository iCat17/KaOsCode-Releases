# KaOsCode Releases

Installationsdateien der Apps von KaOsCode: APKs für Android, für Benchly zusätzlich ein Installer für Windows.
Der Quellcode liegt nicht in diesem Repository.

*English version below.*

## Apps

| App | Beschreibung | Releases | Datenschutz |
|---|---|---|---|
| **Spectare PDF** | PDF-Viewer mit Dokumentenscanner | [Releases](https://github.com/iCat17/KaOsCode-Releases/releases?q=spectare) | Erhebt selbst keine Daten, keine Sicherung. Ins Internet geht Spectare nur bei „Nach Updates suchen“ (nach Rückfrage): Dann fragt die App GitHub nach der neuesten Version, dabei sieht GitHub die IP-Adresse. Der optionale Scanner kommt aus den Google Play Services: Die Dokumente bleiben auf dem Gerät, Google erhält Nutzungsstatistiken zum Scanner |
| **Benchly** | Kursverläufe von Aktien, ETFs, Indizes und Krypto vergleichen | [Releases](https://github.com/iCat17/KaOsCode-Releases/releases?q=benchly) | Erhebt selbst keine Daten. Kurse werden direkt von Yahoo Finance geladen, dabei sieht Yahoo IP-Adresse und abgefragte Symbole. Bei der Suche nach einer WKN wird diese an OpenFIGI (Bloomberg) gesendet. Bei „Nach Updates suchen“ fragt die App GitHub nach der neuesten Version, dabei sieht GitHub die IP-Adresse |
| **Arrowly** | Logikpuzzle: Pfeile in der richtigen Reihenfolge vom Feld schieben | [Releases](https://github.com/iCat17/KaOsCode-Releases/releases?q=arrowly) | Erhebt keine Daten: keine Berechtigungen, kein Internetzugriff; Spielstand nur auf dem Gerät |
| **Bonly** | Kassenbons auslesen, Preise über alle Läden vergleichen und Angebote prüfen | [Releases](https://github.com/iCat17/KaOsCode-Releases/releases?q=bonly) | Erhebt selbst keine Daten: Die Bons bleiben auf dem Gerät, die Texterkennung läuft dort, Sicherungen nur als Datei, die du selbst ablegst. Ins Internet geht Bonly nur bei der optionalen Suche nach Packungsgrößen (standardmäßig aus): Dann gehen Namen von den Bons und die Kette an Open Food Facts und bei „Im Web nachsehen“ an Google, die dabei die IP-Adresse sehen |
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

Update: ab Benchly 1.5.0 in der App unter Einstellungen → **Nach Updates suchen** (auch in der Android-APK). Sonst den neuen Installer herunterladen und ausführen. Vergleich und Einstellungen bleiben erhalten.

## Updates (Android)

Spectare ab 1.4.1 und Benchly ab 1.5.0 suchen auf Wunsch selbst nach Updates.

- **Spectare:** ⋮ → Über Spectare → **Nach Updates suchen** zeigt eine neue Version an und öffnet den Download im Browser. Vor dem Installieren prüft **Heruntergeladene APK prüfen**, ob die Datei von KaOsCode signiert ist. Der Fingerabdruck steht auch im Dialog und unten auf jeder Release-Seite.
- **Benchly:** Einstellungen → **Nach Updates suchen** lädt die neue APK und öffnet den Android-Installer.

Daten und Einstellungen bleiben bei Updates erhalten.

## Automatische Updates mit Obtainium

[Obtainium](https://github.com/ImranR98/Obtainium) installieren, dann **App hinzufügen**:
- **Quell-URL:** `https://github.com/iCat17/KaOsCode-Releases`
- **Release-Titel nach regulärem Ausdruck filtern:** `^Spectare` (bzw. der Name der gewünschten App)

## Unterstützen

Wer die Entwicklung der Apps unterstützen möchte, kann das freiwillig über [Ko-fi](https://ko-fi.com/kaoscode) tun.

## Kontakt

kaos-code@outlook.com

---

# KaOsCode Releases (English)

Installation files for KaOsCode's apps: APKs for Android, plus a Windows installer for Benchly.
The source code is not part of this repository.

Spectare PDF collects no data itself, no backup. It only goes online when you check for updates (after confirming): the app then asks GitHub for the latest version, which sees your IP address. The optional scanner is provided by Google Play Services: documents stay on the device, Google receives usage statistics about the scanner.
Benchly collects no data itself. Prices are loaded directly from Yahoo Finance, which sees your IP address and the requested symbols. When you search for a WKN, it is sent to OpenFIGI (Bloomberg). When you check for updates, the app asks GitHub for the latest version, which sees your IP address.
Arrowly collects no data: no permissions, no internet access; game progress stays on the device.
Bonly (reads receipts, compares prices across all stores and checks offers) collects no data itself: receipts stay on the device, text recognition runs there, and backups are only files you store yourself. Bonly only goes online for the optional pack size lookup (off by default): then names from your receipts and the chain are sent to Open Food Facts, and to Google when you tap "Look it up on the web", which see your IP address.
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

Update: from Benchly 1.5.0 on, in the app under Settings → **Check for updates** (also in the Android APK). Otherwise download and run the new installer. Your comparison and settings are kept.

## Updates (Android)

Spectare from 1.4.1 and Benchly from 1.5.0 can check for updates on request.

- **Spectare:** ⋮ → About Spectare → **Check for updates** shows a new version and opens the download in your browser. Before installing, **Check downloaded APK** verifies that the file was signed by KaOsCode. The fingerprint is also shown in the dialog and at the bottom of every release page.
- **Benchly:** Settings → **Check for updates** downloads the new APK and opens the Android installer.

Data and settings are kept when updating.

## Automatic updates with Obtainium

Install [Obtainium](https://github.com/ImranR98/Obtainium), then **Add app**:
- **Source URL:** `https://github.com/iCat17/KaOsCode-Releases`
- **Filter release titles by regular expression:** `^Spectare` (or the name of the app you want)

## Support

If you'd like to support the development of the apps, you can make a voluntary contribution via [Ko-fi](https://ko-fi.com/kaoscode).

## Contact

kaos-code@outlook.com
