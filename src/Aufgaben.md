# Übung WID 4 - CSS Grid

Grids werden genutzt, um die Grobstruktur einer App zu definieren und mithilfe von CSS zu fixieren. Apps haben meist eine oder mehrere Kopfzeilen (header-Element), einen Bereich für den Hauptinhalt (main-Element), eine oder mehrere Seitenleisten (aside-Element) und manchmal eine Fusszeile (footer-Element). Deren Anordnung und Position sollte mit einem CSS Grid festgelegt werden, bevor die weitere Ausgestaltung erfolgt!

In dieser Sandbox ist ein einfaches Grid bereits vordefiniert, mit welchem du im Folgenden experimentieren kannst. Die zwei Backup-Dateien (App_backup und style_backup) kannst du nutzen, um den ursprünglichen Zustand wiederherzustellen (kopiere in dem Fall den Code aus den Dateien in die App.js bzw. die style.css)

## Experimente:

Falls du bereits eine Idee hast, wie dein Grid aussehen soll, kannst du versuchen diese umzusetzen. Andernfalls findest du hier einige Anregungen (und Tipps):

### Kein Footer:

Falls du keinen Footer benötigst, solltest du diesen entfernen und mehr Platz für andere Elemente schaffen. Entferne den Footer aus der App.js und passe im CSS `grid-template-rows` an - du hast eine Zeile weniger im Grid. Entferne auch den Selektor und die dazu gehörenden Deklarationen.

### Seitenleiste rechts:

Vielleicht möchtest du die Seitenleiste lieber auf der rechten Seite platzieren? Vertausche die Reihenfolge vom aside- und main-Element in der App.js und passe dann auch `grid-template-columns` im CSS an.

### Zwei Header:

Manche Apps haben einen Header (Logo, Text) und darunter eine weitere Header-Zeile als Toolbar für Werkzeuge.
Füge in der App.js unter dem header-Element einen weiteren Header (oder ein div) ein. Passe das Grid im CSS Code an - du hast jetzt eine weiter Zeile (row) in `grid-template-rows`.

### Zwei Seitenleisten:

Du benötigst ein weiteres aside-Element in der App.js. Die Anzahl deiner Spalten in `grid-template-columns` ändert sich dadurch und muss angepasst werden.

### Elemente (vertikal) mittig in der Seitenleiste platzieren:

Hierfür kannst du Flexbox benutzen. Lösche den Text "Sidebar" im aside-Element und platziere dort ein div-Element (Elternelement) sowie ein weiteres Element als Kind (z.B. ein p-Element mit Text). Dem Elternelement weist du jetzt Flexbox-Stile zu. Du benötigst `display: flex`, `flex-direction: column`, `justify-content: center` sowie `height: 100%` damit Flexbox die ganze Seitenleiste vertikal ausfüllt (zu 100%).
