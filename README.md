# Machine Learning Analyses – Wire Solutions

Deze repository bevat het volledige Jupyter Notebook, de dataset en ondersteunende code die zijn gebruikt voor de machine-learninganalyses binnen het data-onderzoek voor Wire Solutions.  
Het notebook combineert zowel **supervised learning (tekstclassificatie)** als **unsupervised learning (topic modelling)** in één geïntegreerd bestand.

## Doel van de analyses

Het doel van dit onderzoek is om te beoordelen in hoeverre machine learning waarde kan toevoegen binnen de servicedeskprocessen van Wire Solutions. De analyses richten zich op twee vragen:

1. **Supervised learning:**  
   Kunnen incidenten met een ontbrekende afdelingsregistratie automatisch worden aangevuld op basis van de incidentbeschrijving?

2. **Unsupervised learning:**  
   Welke thema’s ontstaan vanzelf binnen de incidentbeschrijvingen, en sluiten deze aan op de bestaande categorisatie?

De resultaten helpen om:
- de geschiktheid van tekstclassificatie binnen servicedeskdata te beoordelen,  
- te begrijpen welke inhoudelijke probleemgroepen (topics) in de incidentbeschrijvingen voorkomen,  
- inzicht te krijgen in de beperkingen en mogelijkheden van ML binnen operationele IT-processen.

---

## Inhoud van de notebook

Het notebook bevat onder andere:

### 🔷 Supervised Learning (Tekstclassificatie)
- Inladen en opschonen van tekstdata  
- TF-IDF vectorisatie  
- Train-test-splitsing (80/20)  
- Logistic Regression-model voor afdelingsvoorspelling  
- Evaluatie met accuracy, precision, recall en F1-score  
- Confusion matrix en interpretatie  
- Drempelanalyse (thresholding) voor modelzekerheid  
- Toepassing op incidenten met onbekende afdelingscode  

### 🔷 Unsupervised Learning (Topic Modelling)
- Tekstopschoning + stopwoordenlijst  
- Tokenisatie en document-term matrix (CountVectorizer)  
- LDA-model met 4 topics  
- Topwoorden per topic  
- Dominant topic per incident  
- Mapping naar interpreteerbare topiclabels  
- Export voor verdere analyse in Power BI  

Het notebook ondersteunt daarmee zowel de kwantitatieve conclusies uit het hoofdrapport als de thematische inzichten die in de servicedeskanalyse zijn gebruikt.

---

## Installatie

Installeer de benodigde pakketten met:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
