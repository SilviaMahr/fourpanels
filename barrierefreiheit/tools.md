# 🛠️ WCAG AA-Check: Tools & Vorgehen (Single Source of Truth)

Dieses Dokument legt die vier kostenlosen, standardisierten Tools und den genauen Ablauf fest, mit denen die Barrierefreiheit unserer Produktivversion getestet wird.

---

## 1. Auswahl der kostenlosen Tools

Wir verwenden eine Kombination aus automatisierten Scannern, Browser-Erweiterungen und den Standardfunktionen der Browser, um eine umfassende Abdeckung zu gewährleisten.

| Tool | Kategorie | Fokus |
| :--- | :--- | :--- |
| 1. **Google Lighthouse** | Integriertes Dev-Tool | Automatisierter Audit (Performance, SEO, **Accessibility**) |
| 2. **WAVE Web Accessibility Evaluation Tool** | Browser-Erweiterung & Online-Service | Visuelles Feedback, detaillierte Fehlerzuordnung |
| 3. **DevTools (Standard-Browser)** | Integriertes Dev-Tool | Manuelle Prüfung von Fokus, Kontrast und Semantik |
| 4. **Standard-Browser-Vorlesefunktion** | Integrierte Funktion | Prüfung der Semantik und Lesefolge (Screenreader-Simulation) |

---

## 2. ⚙️ Schritt-für-Schritt-Anleitung: Durchführung des WCAG AA-Checks

Führe diese Schritte in der folgenden Reihenfolge für alle relevanten Seiten der Webanwendung durch.

### Schritt 1: Automatisierter Audit mit Lighthouse

Die Lighthouse-Analyse bietet einen schnellen ersten Überblick über größere, leicht identifizierbare Probleme (z. B. unzureichende Kontraste, fehlende ALT-Texte).

1.  Öffne die zu testende Seite im **Google Chrome Browser**.
2.  Öffne die Entwickler-Tools (**DevTools**) über $\text{F12}$ oder rechte Maustaste $\rightarrow$ **Untersuchen**.
3.  Wechsle zum Tab **Lighthouse**.
4.  Wähle unter **Kategorien** nur **Accessibility** aus und wähle den Modus **Desktop** oder **Mobile** (je nach Testfokus).
5.  Klicke auf **Generate report**.
6.  **Ziel:** Der generierte **Accessibility Score** sollte so hoch wie möglich sein. **Prüfe und dokumentiere** alle aufgedeckten Probleme unter der Überschrift "Accessibility" und "Best Practices".

---

### Schritt 2: Visuelle und detaillierte Fehleranalyse mit WAVE

Das WAVE-Tool (Web Accessibility Evaluation Tool) bettet Icons direkt in die Seite ein, um visuell zu zeigen, wo Barrierefreiheitsprobleme (z. B. fehlende Formular-Labels oder Überschriften-Skipping) vorliegen.

1.  Installiere die **WAVE Browser-Erweiterung** (z. B. für Chrome oder Firefox).
2.  Öffne die zu testende Seite.
3.  Klicke auf das **WAVE-Icon** in der Browserleiste.
4.  **Ablauf:** Die Seite wird überlagert. **Arbeite** die linke Navigationsleiste ab:
    * **Errors/Kontrastfehler:** Identifiziere alle rot markierten Fehler (Errors) und die Kontrastfehler.
    * **Alerts:** Prüfe alle orange markierten Warnungen (Alerts), die potenzielle Probleme darstellen könnten.
    * **Structure:** Kontrolliere die **Überschriften-Hierarchie** und die **ARIA-Attribute** über den Reiter **Structure** oder **Details**.

---

### Schritt 3: Manuelle Interaktion und Fokus-Prüfung (DevTools)

Hierbei wird die **Tastaturbedienbarkeit** (WCAG 2.1.1) und die **Fokus-Sichtbarkeit** (WCAG 2.4.7) getestet.

1.  **Fokus-Sichtbarkeit:**
    * **Schließe** die DevTools und die WAVE-Ansicht.
    * Navigiere durch die gesamte Seite **ausschließlich** mit der $\text{Tabulator-Taste}$ ($\text{TAB}$).
    * **Prüfe:** Ist der aktive Fokus (der blaue oder farbige Rahmen) **jederzeit klar und deutlich** sichtbar?

2.  **Kontrast-Check für nicht-Text-Elemente:**
    * Öffne die DevTools. Wechsle zum Tab **Elements**.
    * Wähle interaktive Komponenten (Buttons, Links) oder Grafiken aus.
    * **Nutze** den **CSS-Inspektor** (Styles-Tab), um sicherzustellen, dass interaktive Grafiken und Schaltflächen ein **Kontrastverhältnis von mindestens 3:1** zum Hintergrund aufweisen (WCAG 1.4.11).

3.  **Semantik-Check (DevTools)**
    * Wechsle in den **Elements**-Tab.
    * **Prüfe** kritische Bereiche: Sind Links wirklich als `<a href="...">` definiert und Buttons als `<button>`?
    * **Stelle sicher**, dass keine falschen HTML-Elemente für ihre Funktion verwendet werden (z. B. ein `<div>` anstelle eines Buttons).

---

### Schritt 4: Lesefolge- und Semantik-Check mit der Vorlesefunktion

Dieser Schritt simuliert die Nutzung durch einen Screenreader, ohne dass ein vollständiger Screenreader installiert werden muss. Es geht darum, die **logische Lesefolge** der Seite zu bestätigen.

1.  **Aktivierung:** Nutze die in deinem Standard-Browser integrierte Funktion **"Laut vorlesen"** (z. B. in Edge, Firefox oder Safari).
2.  **Start:** Wähle den Anfang der Hauptseite oder der relevanten Sektion aus und starte die Vorlesefunktion.
3.  **Prüfung der Lesefolge:**
    * **Höre genau zu:** Werden Abschnitte, Überschriften und Listenelemente in einer **logischen, verständlichen Reihenfolge** vorgelesen?
    * **Prüfe:** Werden Elemente, die im Design rein dekorativ sind (z. B. Trennlinien), vom Programm **übersprungen**?
    * **Stelle sicher:** Werden **ALT-Texte** an der korrekten Stelle im Textfluss vorgelesen?

---

Möchtest du eine Vorlage für die Dokumentation der gefundenen Fehler hinzufügen, die dein Team verwenden kann?
