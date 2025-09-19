# Amazon-Bewertungen Sentiment-Analyse und Klassifikationsmodell

Dieses Projekt wurde entwickelt, um die Produktbewertungen von **Kozmos**, einem Unternehmen für Heimtextilien und Alltagsbekleidung auf Amazon, zu analysieren. Ziel ist es, die Kundenzufriedenheit zu messen, Rückmeldungen zur Produktverbesserung zu erhalten und Verkaufsstrategien zu optimieren.

## Projektziel

Durch die Analyse von Amazon-Kundenbewertungen sollen:

- Die Kundenzufriedenheit gemessen werden  
- Rückmeldungen für die Produktentwicklung gewonnen werden  
- Eine automatische Sentiment-Klassifizierung erfolgen  
- Verkaufsstrategien optimiert werden  

## Datensatz

Der Datensatz besteht aus folgenden Variablen:

| Variable | Beschreibung |
|----------|-------------|
| **Review** | Text der Produktbewertung |
| **Title** | Kurzer Titel der Bewertung |
| **HelpFul** | Anzahl der Personen, die die Bewertung hilfreich fanden |
| **Star** | Sternebewertung des Produkts (1-5) |

## Projektablauf

### 1. Textvorverarbeitung
- Umwandlung in Kleinbuchstaben  
- Entfernung von Satzzeichen  
- Entfernung numerischer Werte  
- Stopwords-Filterung  
- Filterung seltener Wörter (weniger als 1000 Vorkommen)  
- Lemmatization (Wortstamm-Reduktion)  

### 2. Textvisualisierung
- **Bar Plot**: Häufigkeitsanalyse der meistgenutzten Wörter  
- **Word Cloud**: Visuelle Darstellung der Wörter in den Bewertungen  

### 3. Sentiment-Analyse
- Einsatz von NLTK **SentimentIntensityAnalyzer**  
- Berechnung der Polaritätsscores  
- Positive/Negative-Kennzeichnung basierend auf dem Compound-Score  
- Automatische Sentiment-Klassifizierung  

### 4. Vorbereitung für Maschinelles Lernen
- Aufteilung der Daten in Trainings- und Testset  
- Text-Vektorisierung mit **TfidfVectorizer**  
- Umwandlung in numerische Repräsentationen  

### 5. Modellentwicklung

#### Logistische Regression
- Training und Test des Modells  
- Leistungsbewertung  
- Cross-Validation Analyse  
- Vorhersagetest auf zufälligen Stichproben  

#### Random Forest
- Ansatz des Ensemble Learning  
- Modellvergleich  
- Bewertung der Genauigkeit (Accuracy)  

## Ergebnisse
- Zwei verschiedene ML-Modelle wurden entwickelt  
- Vergleich der Modellleistung  
- Aufbau eines automatischen Sentiment-Klassifizierungssystems  
- Echtzeit-Vorhersage von Kundenbewertungen implementiert  
