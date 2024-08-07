# BUILD - Dokument

Author: Dana
Created: August 7, 2024

Voraussetzungen: Windows- oder Linux-System mit Entwicklungsumgebung, Python und Jupyter

1. Google Cloud Developer Account erstellen und lokal anmelden, dabei den Schritten unter [Google Cloud Environment](https://cloud.google.com/vertex-ai/docs/start/cloud-environment?hl=de) bis Schritt 5 folgen.
2. Zip-Ordner mit Bausteinen vom BSI, Kreuzreferenztabellen und das Grundschutzkompendium herunterladen. (Wichtig: Bald kommen neue Bausteine vom BSI heraus, diese haben wir nicht getestet)
    - Links: [Zip-Ordner](https://www.bsi.bund.de/SharedDocs/Downloads/DE/BSI/Grundschutz/IT-GS-Kompendium_Einzel_PDFs_2023/Zip_Datei_Edition_2023.html), [Kreuzreferenztabelle](https://www.bsi.bund.de/SharedDocs/Downloads/DE/BSI/Grundschutz/Kompendium/krt2023_Excel.html), [Grundschutzkompendium](https://www.bsi.bund.de/SharedDocs/Downloads/DE/BSI/Grundschutz/Kompendium/IT_Grundschutz_Kompendium_Edition2023.pdf?__blob=publicationFile&v=4#download=1)
3. Google Storage Bucket erstellen: [Anleitung](https://cloud.google.com/storage/docs/creating-buckets?hl=de)
4. Die Bausteine als PDFs in den Storage Bucket hochladen.
5. In die Konsole von Google Cloud Shell folgenden Befehl mit dem eigenen Namen vom Storage Bucket eingeben: `gsutil ls gs://test_bucket_teamprojekt/` um eine Liste der Ressourcen zu erhalten, die dem Prozess bereitgestellt werden müssen.
6. Die dadurch generierten Links aller Baustein-Dateien in eine txt-Datei im Hauptordner speichern und `file_path` mit dem Dateipfad der erstellten txt-Datei ersetzen.
7. GitHub-Repository klonen.
8. Pfad zum eigenen Ordner mit Excel-Datei für Kreuzreferenztabelle im Code bei [3] ändern. Eventuell `r` vor den Pfad setzen:
    
    ![BUILD%20-%20Dokument%2026ea99e537dc488ea7ec59d4093b08ba/Untitled.png](BUILD%20-%20Dokument%2026ea99e537dc488ea7ec59d4093b08ba/Untitled.png)
    
9. `pip install -r requirements.txt` im Jupyter Notebook ausführen, um Requirements zu installieren.
10. Eigene Project ID vom Google Cloud Project im Code bei [3] ändern. Die Project ID findet man bei seinen Projekten unter [Google Cloud Console](https://console.cloud.google.com/).
11. Cloud Shell aktivieren (Icon ganz links):
    
    ![BUILD%20-%20Dokument%2026ea99e537dc488ea7ec59d4093b08ba/Untitled%201.png](BUILD%20-%20Dokument%2026ea99e537dc488ea7ec59d4093b08ba/Untitled%201.png)
    
12. Jupyter Server neu starten.
13. Import-Codeblock testen, um zu überprüfen, ob alle Installationen in der richtigen Version vorhanden sind. Falls nicht, per `pip install ...` im Notebook korrigieren.
14. Gefahrenliste im Notebook mit der aus dem Grundschutzkompendium PDF abgleichen und gegebenenfalls aktualisieren.
15. "Run ALL" ausführen (kann lange dauern).

Wichtige Tipps:

- Vor "Run ALL" sollten alle Dateien gespeichert sein.
- Python installiert.
- Eventuell VSC als Administrator neu öffnen.
- Eventuell folgendes in Windows-Konsole eingeben: `gcloud auth application-default login`.