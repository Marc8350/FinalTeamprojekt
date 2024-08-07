# Designentscheidungen

**Begründung der Designentscheidungen für das Projekt**

Bei der Planung und Umsetzung unseres Projekts haben wir mehrere bedeutende Designentscheidungen getroffen, um Effizienz, Flexibilität und Benutzerfreundlichkeit zu gewährleisten. Diese Entscheidungen umfassen die Wahl der Programmiersprache, die Nutzung von Notebooks, die Kombination von Skripten und objektorientierter Programmierung, die Auswahl der Google Gemini API sowie Überlegungen zur zukünftigen Verbesserung.

**1. Wahl der Programmiersprache**

Unsere erste wesentliche Entscheidung betraf die Programmiersprache. Wir haben uns für Python entschieden, da es eine Fülle hervorragender Bibliotheken bietet, die uns die Implementierung vieler Funktionen erleichtern. Insbesondere die API-Zugriffe sind in Python relativ einfach zu handhaben. Darüber hinaus ist die OWL-Ready-Bibliothek, die wir verwendet haben, genau auf unsere Aufgabe zugeschnitten – das Erstellen einer Ontologie-Datei im OWL-Format.

**2. Verwendung von Notebooks**

Ein weiterer zentraler Aspekt unseres Designs ist die Nutzung von Notebooks. Wir sehen unser Artefakt als Baukasten, der als Grundlage für andere Projekte dienen kann. Notebooks sind besonders hilfreich, wenn man mit Prompt Engineering arbeitet, da sie es ermöglichen, Ergebnisse zu speichern und leicht auf Variablen zuzugreifen, ohne Anfragen erneut ausführen zu müssen. Dies wäre in einem klassischen Skript weniger effizient.

**3. Mischform aus Skript und objektorientierter Programmierung**

Wir haben eine Kombination aus Skript- und objektorientierter Programmierung gewählt, da dies gut zu unserem Workflow passte. Ausgangspunkt war der Prozess, den wir aus dem Process Mining abgeleitet haben. Diesen Prozess haben wir automatisiert und darauf aufbauend die Funktionen für den Baukasten entwickelt.

**4. Verwendung der Google Gemini API**

Die Google Gemini API wurde aufgrund ihrer gut dokumentierten Unterstützung für PDF-Dokumente gewählt, was uns die Notwendigkeit ersparte, das Format-Handling selbst zu übernehmen. Zum Zeitpunkt der Entwicklung bot Google Gemini das größte Kontextfenster, was uns die Arbeit mit längeren Dokumenten ermöglichte. Ein weiterer Vorteil war der Sign-up Bonus von 300 Dollar Rechenguthaben, wodurch das Projekt kostenfrei umgesetzt werden konnte. Allerdings führte die Nutzung der Google Gemini API dazu, dass wir auf die Google Cloud zurückgreifen mussten, was zusätzliche Komplexität und potenzielle Fehlerquellen mit sich brachte.

**Probleme und zukünftige Verbesserungen**

Während der Entwicklung stießen wir auf einige Herausforderungen, insbesondere bei der Textkodierung aufgrund der Eigenheiten von Protégé. Künftig würden wir wahrscheinlich eher eine herkömmliche Grafendatenbank wie Neo4j verwenden, um diese Probleme zu vermeiden. Außerdem würden wir Redundanzen einbauen und verschiedene APIs nutzen, da mittlerweile mehrere Dienste Dateien hochladen können. Zudem würden wir für unseren Google Gemini Developer-Account eine höhere Sicherheitsfreigabe beantragen, um weniger Anfragen blockiert zu bekommen.

Abschließend würden wir die Anwendung als Web-Anwendung entwickeln und ein agentisch implementiertes Qualitätsmanagement entwickeln, das auf einem Server läuft. Dies würde die aufwendigsten Schritte – den Setup-Prozess und die Qualitätssicherung – deutlich vereinfachen und somit die Benutzerfreundlichkeit weiter erhöhen.