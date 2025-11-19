# ⚖️ Gesetzliche Grundlagen zur Barrierefreiheit

Diese Richtlinien fassen die Kernanforderungen der **WCAG (Web Content Accessibility Guidelines) nach Level AA** zusammen, die zur Erfüllung der gesetzlich geforderten Barrierefreiheit herangezogen werden sollen.

---

## 📅 Gesetzliche Grundlage & Richtlinien

* **Gültigkeit:** Das Gesetz ist gültig seit dem **28.06.2025**.
* **Gesetzestext:** [Richtlinie (EU) 2019/882 (Europäischer Rechtsakt zur Barrierefreiheit)](https://eur-lex.europa.eu/eli/dir/2019/882/oj?locale=de)
* **Umsetzung:** Zur Erreichung der gesetzlich geforderten Barrierefreiheit sollen die **[WCAG Richtlinien (Level AA)](https://www.w3.org/Translations/WCAG20-de/WCAG20-de-20091029/)** herangezogen werden.

---

## 🎯 Die 4 Prinzipien der WCAG (Level AA)

### 1. Wahrnehmbar

**Du musst Inhalte so gestalten, dass Benutzer sie wahrnehmen können.**

* **1.1 Textalternativen:** **Stelle** Textalternativen für alle Nicht-Text-Inhalte zur Verfügung, so dass diese in andere vom Benutzer benötigte Formen geändert werden können (z.B. Großschrift, Braille, Symbole oder einfachere Sprache).
* **1.2 Zeitbasierte Medien:** **Stelle** Alternativen für zeitbasierte Medien (Audio, Video) zur Verfügung.
* **1.3 Flexibilität:** **Erstelle** Inhalte, die auf verschiedene Arten dargestellt werden können (z.B. mit einfacherem Layout), ohne dass Informationen oder Strukturen verloren gehen.
* **1.4 Unterscheidbarkeit:** **Mache** es für den Benutzer leichter, Inhalte zu sehen und zu hören, einschließlich der Trennung zwischen Vordergrund und Hintergrund.

### 2. Bedienbar

**Du musst sicherstellen, dass Benutzende Komponenten der Benutzeroberfläche und Navigation bedienen können.**

* **2.1 Tastaturbedienung:** **Sorge** dafür, dass alle Funktionalitäten von der Tastatur aus verfügbar sind.
* **2.2 Ausreichend Zeit:** **Gib** den Benutzern ausreichend Zeit, Inhalte zu lesen und zu benutzen.
* **2.3 Anfallprävention:** **Gestalte** Inhalte nicht auf Arten, von denen bekannt ist, dass sie zu Anfällen führen (z.B. Blinken).
* **2.4 Navigation:** **Stelle** Mittel zur Verfügung, um Benutzer dabei zu unterstützen zu navigieren, Inhalte zu finden und zu bestimmen, wo sie sich befinden.

### 3. Verständlich

**Du musst Inhalte und Bedienungsinformationen verständlich machen.**

* **3.1 Lesbarkeit:** **Mache** Textinhalte lesbar und verständlich.
* **3.2 Vorhersehbarkeit:** **Sorge** dafür, dass Webseiten vorhersehbar aussehen und funktionieren.
* **3.3 Eingabeunterstützung:** **Hilf** den Benutzern dabei, Fehler zu vermeiden und zu korrigieren.

### 4. Robust

**Du musst Inhalte robust genug machen, damit sie von einer großen Auswahl an Benutzeragenten, einschließlich assistierender Techniken, zuverlässig interpretiert werden können.**

* **4.1 Kompatibilität:** **Maximiere** die Kompatibilität mit aktuellen und zukünftigen Benutzeragenten, einschließlich assistierender Techniken.

---

Möchtest du, dass ich die WCAG-Prinzipien weiter in spezifische Kriterien (z.B. 1.4.3 Kontrast (Minimum)) aufschlüssele?


# ♿ Barrierefreie Gestaltung eines Website-Prototyps

Diese Anweisungen dienen dazu, sicherzustellen, dass das Design **deines** Website-Prototyps die grundlegenden Kriterien für **Web-Barrierefreiheit (Accessibility)** erfüllt.

---

## 🎨 Design & Visuelle Elemente

### 1. Farbkontrast und Farbwahl

* **Kontrastverhältnis:** **Stelle** einen **ausreichenden Farbkontrast** zwischen Schrift und Hintergrund sicher.
    * *Tipp:* Oft genügt eine leichte Helligkeitsveränderung der Farben, um die Kontraste zu gewährleisten. Es muss nicht automatisch alles komplett anders sein.
* **Farbspektren:** **Plane** für interaktive Elemente wie Hover-Zustände (Hoverstates) **mehrere Abstufungen einer Farbe (4+)** ein.
* **Kontrastierende Kombinationen:** **Kombiniere** Farbkontraste gegebenenfalls auch basierend auf ihren Abstufungen.
* **Funktionale Farben:** Die **Primärfarbe** muss nicht immer die Farbe für z.B. Buttons sein. (Beispiel: nutze ein knalliges Orange und die direkte Kontrastfarbe Blau.)
* **Free Tools zur Farbwahl**  
[ColourContrustChecker](https://colourcontrast.cc/)  
[Accessible color palette generator](https://venngage.com/tools/accessible-color-palette-generator)
[WhoCanUse](https://www.whocanuse.com/)

### 2. Typografie und Lesbarkeit

* **Schriftarten:** **Verwende** **gut lesbare Schriftarten**, idealerweise **serifenlose** ohne Verzierungen (z.B. Arial).
* **Texthierarchie:** **Etabliere** eine **einfache, konstante Texthierarchie** und ein **logisches Layout**.
    * **H1-Überschriften:** Die $\mathbf{H1}$ sollte als die größte und wichtigste Headline **klar als erstes ersichtlich** sein.
* **PDF-Optimierung (Indesign-Hinweis):** Für optimale Reader-Funktionen digitaler PDFs müssen Textfelder im InDesign **alle verkettet** sein.

---

## 🖼️ Medien & Interaktion

### 3. Grafiken und Bilder

* **Informative Bilder:** **Optimiere** Grafiken und Bilder mit $\mathbf{ALT-Texten}$ (Alternativtexte).
    * Der $\mathbf{ALT-Text}$ muss eine **kurze Beschreibung** dessen sein, was auf dem Bild zu sehen ist, zur **optimalen Reader-Funktion** digitaler PDFs.
* **Dekorative Bilder:** Wenn Grafiken **rein dekorativ** zum Einsatz kommen, werden sie im Web **als solche definiert** und von Screenreadern **übersprungen** (d.h. der ALT-Text bleibt leer oder wird auf `alt=""` gesetzt).

### 4. Videos und Audio

* **Untertitel:** **Füge** für den gesprochenen Text in Videos stets **Untertitel** (Captions) hinzu.

---
