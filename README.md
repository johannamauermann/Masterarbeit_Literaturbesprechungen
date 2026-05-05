# Masterarbeit im Fach Digitale Methodik in den Geistes- und Kulturwissenschaften (JGU Mainz/Hochschule Mainz)

Dieses Repository enthält Code und Daten der Masterarbeit:

**„Literaturbesprechungen in historischen Zeitungen:  
Korpusbildung und Analyse diachroner Entwicklungen mit LLMs und NLP-Methoden“**

## Forschungsfrage

Im Zentrum der Arbeit steht die Frage:

> Wie entwickeln sich Literaturrezensionen in der *Kölnischen Zeitung* im Verlauf des 19. Jahrhunderts?  
> Inwieweit können LLMs Korpusaufbau, -anreicherung und das Auffinden systematischer Muster unterstützen?

## Projekt-Website

Die begleitende Website zur Masterarbeit:  
🔗 https://johannamauermann.github.io/Masterarbeit_Literaturbesprechungen_Website/

---

## Inhalt des Repositories

### Notebooks

- **`finding_keywords.ipynb`**  
  Identifikation relevanter literaturbezogener Keywords auf Basis eines manuell erstellten Testdatensatzes (inkl. extrahierter Rezensionen).  
  Ziel: möglichst gute Balance zwischen *Precision* und *Recall*.

- **`evaluation_code_review_extraction.ipynb`**  
  Evaluationscode für die Extraktion von Rezensionen aus Zeitungstexten mittels LLMs (XML-Format) im Vergleich zu einer Ground Truth.

- **`annotation_evaluation_code.ipynb`**  
  Evaluation der Übereinstimmung von Metadaten- und Sentiment-Annotationen (Extraktion & Klassifikation) anhand einer Ground Truth.

- **`exploratory_analysis.ipynb`**  
  Explorative Visualisierungen auf Basis der durch LLMs angereicherten Rezensionen.

---

### Daten

- **`df_review_test.csv`**  
  Testdatensatz mit 20 Beispielen zur Erprobung der Rezensionsextraktion.

- **`full_dataset_part_1_with_model_extractions.csv`**  
- **`full_dataset_part_2_with_model_extractions.csv`**  
  Aufgeteiltes Gesamtdataset (insgesamt 1740 Einträge) inkl.  
  - Ground Truth (Rezensionen)  
  - Modelloutputs aus Prompt-Experimenten  

- **`all_reviews_with_metadata_sentiment.csv`**  
  Datensatz aller extrahierten Rezensionen (n = 633) inkl.  
  - Metadaten  
  - Sentiment-Klassifikation  
  - strukturierte XML-Ausgaben der Modelle  

---

### Prompts

- **`prompt_review_extraction`**  
  Finaler Prompt zur Extraktion von Rezensionen aus Zeitungstexten

- **`prompt_corpus_enrichment`**  
  Finaler Prompt zur Anreicherung des Korpus (Sentiment & Metadaten)

### AI model documentation sheet

- **`AI_model_documentation_sheet.pdf`**
  Zur Dokumentation der verwendeten Modelle, Biases, etc. (Template von Sarah Oberbichler; https://doi.org/10.5281/zenodo.15046713 ) 
