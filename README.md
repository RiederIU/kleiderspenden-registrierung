# Kleiderspenden-Registrierung
Eine responsive Webanwendung (Single-Page-Application) zur Erfassung von Kleiderspenden.<br>
Entwickelt für die Fallstudie des fiktiven Kleiderspenden e.V.

## Umgesetzte Funktionen
### 1. Kernfunktionen & SPA-Architektur
* **SPA-Routing:** Clientseitige Navigation implementiert. Die Menü-Links führen nun zu dynamischen Unterseiten ohne Neuladen der Seite.
* **Informationsseiten:** 5 vollständige Unterseiten (Über uns, Kontakt, Impressum, Datenschutz, AGB) mit transparenten Quellennachweisen für KI-generierte Inhalte.
* **Globale Navigation:** Eine übersichtliche Kopfzeile mit lokal eingebundenem Logo, das als funktionaler Home-Button dient, sowie eine dynamische Menü-Markierung zur Orientierung.
* **Spendenformular:** Erfassung von Spendenart, Krisengebiet und Übergabeart (Geschäftsstelle oder Abholung)
* **Bestätigungsansicht:** Übersichtliche Zusammenfassung aller erfassten Daten mit Zeitstempel nach erfolgreicher Registrierung
* **Echtzeit-Validierung:** Das Formular prüft bei der Eingabe automatisch, ob die Postleitzahl für das Sammelfahrzeug aus genau 5 Ziffern besteht und mit "12" beginnt. Der Absende-Button wird bei ungültiger Eingabe gesperrt.

### 2. Barrierefreiheit (Accessibility & Usability)
* **Screenreader-Unterstützung:** Automatisches Fokus-Management bei der Bestätigungsansicht und beim Seitenwechsel für eine verbesserte Zugänglichkeit.
* **Auto-Scroll (Viewport-Reset):** Die Seite scrollt beim Wechseln der Unterseiten automatisch nach oben, um das Navigationsverhalten einer klassischen Webseite zu emulieren.
* **Visuelles Feedback:** Hover-Effekte bei Formularelementen zur besseren Orientierung.

### 3. Responsive Design
* **Mobile Optimierung:** Logo-Größe und Vereinsname werden auf Mobilgeräten verkleinert, damit das Hamburger-Menü nicht mehr in die nächste Zeile umbricht.
* **Flexibles Layout:** Die Benutzeroberfläche passt sich mithilfe von CSS-Flexbox und Bootstrap automatisch an alle Bildschirmgrößen an. Dies umfasst einen Sticky Footer für ein sauberes Layout bei kurzen Inhalten.

### 4. Sicherheit & Code-Qualität
* **IT-Sicherheit (SRI-Hashes):** Das Bootstrap-Framework ist mit Subresource Integrity (SRI) abgesichert, um die Manipulation von CDN-Ressourcen zu verhindern.
* **Robuste Validierung:** Button-Sperre berücksichtigt alle Validierungszustände (null, false, true).
* **Dokumentation:** Vollständige Überarbeitung der Code-Kommentare mit Fokus auf Architektur und Geschäftslogik statt reiner Code-Übersetzung.

## Verwendete Technologien
* HTML5 / CSS3
* Vue.js 3 (via CDN eingebunden)
* Bootstrap 5.3.8 (via CDN eingebunden, mit SRI-Hashes abgesichert)

## Ausführung des Projekts
Um die Anwendung zu starten, laden Sie die Dateien dieses Repositories (`index.html` und `logo.png`) herunter und **speichern Sie zwingend beide Dateien im selben Ordner**.<br>
Öffnen Sie anschließend die `index.html` in einem aktuellen Webbrowser (z. B. Chrome, Firefox oder Edge). Es ist keine weitere Installation notwendig.

## Hinweise zur Transparenz (KI-Nutzung)
Alle Informationstexte (Über uns, Kontakt, Impressum, Datenschutz, AGB) sowie das Logo wurden für diese Fallstudie am 05.03.2026 mithilfe von KI (Google Gemini) generiert.<br>
Die Quellen sind transparent direkt auf den jeweiligen Seiten sowie im Footer vermerkt.
