# Explorative Datenanalyse der Kriminalität in Chicago

## Projektdetails

### Autoren
* Ian Altenau
* Sakhr Al-Absi
* Sam Bokai

### Vorläufige Liste zu untersuchender Forschungsfragen:
* "Wann und wo komme ich mit mit einer Straftat am besten davon?"
* "Welche Straftaten passieren am häufigsten? Wann und wo?"
* Korrelation zwischen Häuslicher Gewalt und Geburtenraten
* "Wie effektiv sind die Ermittlungsbehörden?"
* Vorhersage von Kriminalitätswellen, Radikalisierung der Bevölkerung oder konkreten Straften

### Datenquellen
* [Offizielle Daten der Stadverwaltung Chicago - 'Crimes 2001 to present'](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-present/ijzp-q8t2)

## Erste Schritte

### Voraussetzungen
* Klone dieses Projekt

    ```bash
    git clone https://github.com/sambokai/Chicago-Crime-EDA.git
    ```


* Installiere [Anaconda](https://www.anaconda.com/download) oder [Miniconda](https://conda.io/miniconda.html)
    * Überprüfe die erfolgreiche Installation mit `conda -V`


* Lade einen Chicago-Crime Datensatz zur Analyse herunter
    * Lade die CSV Datei von der offiziellen Webseite der Stadtverwaltung Chicagos herunter. Nutze hierfür die [Datenquellen](#datenquellen)
    * Speichere die CSV als `crimes.csv` im Ordner `data` dieses Projekts. Erstelle vorher den Ordner `data` im Stammverzeichnis, falls benötigt.
  
### Einrichtung der Entwicklungsumgebung


Erstelle ein [Conda Environment](https://conda.io/docs/user-guide/concepts.html) mit den benötigten Packages. Diese sind in der Datei `environment.yml` dieses Projekts definiert. [Offizielle Dokumentation](https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file)

```bash
conda env create -f environment.yml # Erstelle ein Environment mithilfe der environment.yml dieses Projektes
conda info -e # Liste alle installierten Environments auf um zu überprüfen ob das Environment korrekt installiert wurde
```

Aktiviere das zuvor installierte Environment
* Unter MacOS / Linux, im Terminal: `source activate chicago-crime`
* Unter Windows, im Anaconda Prompt: `activate chicago-crime`

Überprüfe die Aktivierung. 
```bash
conda info # Der Wert von `active environment` sollte `chicago-crime` sein.
```

### Starten des Notebooks / Jupyter Labs
Starte [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/)
````bash
jupyter lab
````

In Jupyter führe den Schritt `Load Data` des Notebooks aus um zu überprüfen, ob der Chicago-Crime Datensatz korrekt installiert wurde.