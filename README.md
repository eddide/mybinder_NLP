# Binder Badge
https://mybinder.org/v2/gh/eddide/mybinder_logreg/HEAD

# Dokumentation zur Ausführung
1. Aktivieren des Links zu Binder
2. Öffnen des Python-Notebooks "Installationen"
3. In der Toolbar unter "Kernel" "Restart & Run All" aktivieren. --> Bestätigen des Pop-up Fensters mit "Restart and Run All Cells"
4. Nach der erfolgreichen Ausführung Schließen des Python-Notenooks "Installationen"
5. Öffnen des Pyhton-Notebooks "Logistic Regression"
6. In der Toolbar unter "Kernel" "Restart & Run All" aktivieren. --> Bestätigen des Pop-up Fensters mit "Restart and Run All Cells"
7. Ergebnisse mit den unten beschriebenen Ergebnissen abgleichen.

# Natural Language Processing Projekt

Willkommen zum NLP Projekt des Kurses. In diesem NLP Projekt werden wir versuchen Yelp Reviews in 1 Stern oder 5 Sterne Kategorien zu klassifizieren. Dazu nutzen wir den Text ihrere Bewertung. Dieses Prozedere wird leichter sein als das der Lektion, da wir die Pipeline für komplexe Aufgaben verwenden werden. 

Wir nutzen [Yelp Review Daten von Kaggle](https://www.kaggle.com/c/yelp-recsys-2013).

Jede Beobachtung in dem Datensatz ist eine bestimmte Bewertung eines bestimmten Geschäfts durch einen bestimmten Nutzer.

Die "stars" Spalte beinhaltet die Anzahl der Sterne (1 bis 5) die der Bewerter dem Geschäft verliehen hat. In anderne Worten: Die Bewertung des Geschäfts durch den Autor. 

Die "cool" Spalte beinhaltet die Anzahl der "Cool"-Votes der Bewertung durch andere Nutzer.

Alle Bewertungen starten mit 0 "Cool"-Votes und es gibt nach oben kein Limit. Je mehr Leute die Bewertung "Cool" finden und sie so voten, desto höhere die Anzahl.

Für die "useful" (dt. nützlich) und "funny" (dt. witzig) Spalten gilt das gleiche.

## Anwendung
### Libraries Import
zuerst werden die relevanten Libraries importiert
- pandas
- numpy
- matplotlib
- seaborn
### Daten Import und Überprüfung
dann werden die Daten importiert und überprüft
- Anzeigen der Daten
- Information der Daten
- Beschreibung der Daten
### Explorative Datenanalyse
Verwendung unterschiedlicher Visualisierungen um die Daten zu erforschen
- FacetGrid
- Boxplot
- Histogramm
- Heatmap
### Datenvorbereitung
- Gruppieren der Daten
- Korrealtion der Daten prüfen
### NLP Klassifizierung
Anwenden der NLP Klassifizierung
- Erstellung eines DataFrames zur Vorhersage der Kategorien
- Nutzen des CountVectorizers von Scikitlearn
- Fitten und Transformieren des CountVectorizers auf die Prädiktoren
- Aufsplitten der Daten in Test und Trainingsdaten
- fiten des MultinomialNB auf die Trainingsdaten
- vorhgersagen der Testdaten
### Evaluation der Vorhersage
Evaluierung über den classification report.
Es sollten ähnliche Ergebnisse wie diese angezeigt werden:
- accuracy: 93%
- reall: 70 und 98%
- f1-score: 78 und 96%
