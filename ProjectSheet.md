# Project Sheet: Titel des Projekts

Team-Mitglieder:

* Finn Ferchau, ferchaufi91987@th-nuernberg.de
* Sascha Stelzl, stelzlsa95750@th-nuernberg.de
* Lukas Müller, muellerlu93279@th-nuernberg.de

## Motivation / Szenario

* Worum geht es in Ihrem Projekt?
    In unserem Projekt möchten wir Essays aus IELTS Writing Tasks automatisch bewerten. Dabei sollen sowohl die Scores der Essays vorhergesagt als auch die Essays bestimmten Kategorien zugeordnet werden. Die Kategorisierung erfolgt basierend auf der jeweiligen Fragestellung.

* Was ist Ihre Motivation?
    Wir möchten Studierenden, die sich auf den Test vorbereiten, dabei helfen, ihre Texte bereits bewerten zu lassen, um eventuell Fehlerquellen aufzudecken.

* Welches Szenario wollen Sie betrachten?
    Wir betrachten das Szenario von Studierenden, die sich auf den IELTS-Test vorbereiten und ihre Schreibfähigkeiten gezielt verbessern möchten.

* Gibt es vielleicht sogar einen hypothetischen Kunden, für den Ihr Anwendungsfall relevant wäre?
    Zwar haben wir keinen direkten Kunden, jedoch richten wir uns an Studierende, die den IELTS-Test absolvieren möchten.

* Welche Fragestellungen würden Sie gern beantworten?
    Wir möchten folgende Fragen beantworten: Wie gut ist mein Essay? Passt mein Essay zu anderen Essays, die dieselbe Fragestellung behandeln?

## Daten

Wir benutzen ein vorgefertigtes Dataset von HuggingFace (https://huggingface.co/datasets/chillies/IELTS-writing-task-2-evaluation). Zu jeder Fragestellung gibt es die Antwort im Form des Essays.
Die Scores zur Bewertung schlüsseln sich dabei in Coherence und Cohesion, Lexical Resource und Grammatical Range and Accuracy auf. Daraus berechnet sich der sogenannte Overall Band Score.

## Vorgehen

Sofern Sie schon Ideen dazu haben:

* Was für ML-Modelle wollen Sie trainieren?
    Für Automated Essay Scoring planen wir folgende Modelle zu trainieren:
    - Herkömmliche Modelle wie Lineare Regression 
    - Transformer wie BERT
    - Classification oder Regression
    
    Für das Clustering möchten wir folgende Methoden verwenden:
    - K-Means
    - Hierarchical Clustering

* Wie wollen Sie vorgehen?
    Unser Vorgehen gliedert sich in folgende Schritte:
    1. Data Cleaning
    2. Statistische Analyse durchführen, um den Datensatz besser kennenzulernen und zu verstehen
    3. Trainieren von herkömmlichen Modellen, um einen Vergleichswert zu haben (Vergleichsmodelle: LineareRegression, LogistischeRegression, SVM)
    4. Trainieren des BERT-model 
    5. Aufbauen des Clusters

* Welche statistischen Analysen können Sie sich vorstellen durchführen, um erste interessante Informationen und Zusammenhänge zu finden?
    Wir planen folgende statistische Analysen durchzuführen:
    1. Die Korrelation zwischen Textlänge und Bandscore untersuchen
    2. Den Einfluss der Wortvielfalt auf die Bewertungskriterien analysieren
    3. Die Verteilung der Vokabeln für die einzelnen Fragestellungen ermitteln
    4. Gibt es Unterschiede in dem Anspruch, an den Schreiber, der Teilbewertungen.
    5. Die Schwierigkeit der verschiedenen Fragestellungen vergleichen
    6. Die Korrelation zwischen speziellen Wörtern und dem Overall Band Score untersuchen
