# Gesetz  
gültig seit 28.6.2025  
[Gesetzestext](https://eur-lex.europa.eu/eli/dir/2019/882/oj?locale=de)  
Damit die gesetzlich geforderte Barrierefreiheit erreicht wird, sollen die [WCAG Richtlinien (Level AA)](https://www.w3.org/Translations/WCAG20-de/WCAG20-de-20091029/) herangezogen werden.  
**1 Wahrnehmbar**  
1.1 Stellen Sie Textalternativen für alle Nicht-Text-Inhalte zur Verfügung, so dass diese in andere vom Benutzer benötigte Formen geändert werden können, wie zum Beispiel Großschrift, Braille, Symbole oder einfachere Sprache.  
1.2 Stellen Sie Alternativen für zeitbasierte Medien zur Verfügung.  
1.3 Erstellen Sie Inhalte, die auf verschiedene Arten dargestellt werden können (zum Beispiel mit einfacherem Layout), ohne dass Informationen oder Strukturen verloren gehen.  
1.4 Machen Sie es für den Benutzer leichter, Inhalte zu sehen und zu hören, einschließlich der Trennung zwischen Vordergrund und Hintergrund.  
**2 Bedienbar**  
2.1 Sorgen Sie dafür, dass alle Funktionalitäten von der Tastatur aus verfügbar sind.  
2.2 Geben Sie den Benutzern ausreichend Zeit, Inhalte zu lesen und zu benutzen.  
2.3 Gestalten Sie Inhalte nicht auf Arten, von denen bekannt ist, dass sie zu Anfällen führen.  
2.4 Stellen Sie Mittel zur Verfügung, um Benutzer dabei zu unterstützen zu navigieren, Inhalte zu finden und zu bestimmen, wo sie sich befinden.  
**3 Verständlich**  
3.1 Machen Sie Textinhalte lesbar und verständlich.  
3.2 Sorgen Sie dafür, dass Webseiten vorhersehbar aussehen und funktionieren.  
3.3 Helfen Sie den Benutzern dabei, Fehler zu vermeiden und zu korrigieren.  
**4 Robust**  
4.1 Maximieren Sie die Kompatibilität mit aktuellen und zukünftigen Benutzeragenten, einschließlich assistierender Techniken.  

Gerne, hier ist die Anleitung im Markdown-Format, die auf deinen Vorgaben basiert und diese strukturiert darstellt, wie ein barrierefreier Prototyp für eine Website gestaltet werden muss.

# ♿ Barrierefreie Gestaltung eines Website-Prototyps

Diese Anweisungen dienen dazu, sicherzustellen, dass das Design **deines** Website-Prototyps die grundlegenden Kriterien für **Web-Barrierefreiheit (Accessibility)** erfüllt.

---

## 🎨 Design & Visuelle Elemente

### 1. Farbkontrast und Farbwahl

* **Kontrastverhältnis:** **Stelle** einen **ausreichenden Farbkontrast** zwischen Schrift und Hintergrund sicher.
    * *Tipp:* Oft genügt eine leichte Helligkeitsveränderung der Farben, um die Kontraste zu gewährleisten. Es muss nicht automatisch alles komplett anders sein.
* **Farbspektren:** **Plane** für interaktive Elemente wie Hover-Zustände (Hoverstates) **mehrere Abstufungen einer Farbe (4+)** ein.
* **Kontrastierende Kombinationen:** **Kombiniere** Farbkontraste gegebenenfalls auch basierend auf ihren Abstufungen.
* **Funktionale Farben:** Die **Primärfarbe** muss nicht immer die Farbe für z.B. Buttons sein. (Beispiel: Headspace nutzt ein knalliges Orange und die direkte Kontrastfarbe Blau.)

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

--
