# Machine Learning Analyses – Wire Solutions

Deze repository bevat het Jupyter Notebook dat is gebruikt voor de
machine-learninganalyses binnen het dataonderzoek voor Wire Solutions.
De analyses zijn uitgevoerd ter ondersteuning van het onderzoeksrapport
en dienen als inhoudelijke verdieping van de servicedeskanalyse.

Het notebook combineert zowel supervised als unsupervised machine
learning op basis van incidentbeschrijvingen.

## Doel van de analyses

Het doel van de machine-learninganalyses is om te verkennen in hoeverre
tekstuele incidentdata aanvullende inzichten kan bieden bij de analyse
van servicedeskprocessen.

De analyses richten zich op twee vragen:

1. **Supervised learning**  
   In hoeverre is het mogelijk om incidenten met ontbrekende
   afdelingsinformatie automatisch te classificeren op basis van
   hun tekstbeschrijving?

2. **Unsupervised learning**  
   Welke inhoudelijke thema’s komen vanzelf naar voren in de
   incidentbeschrijvingen, en hoe verhouden deze zich tot de bestaande
   incidentcategorieën?

De resultaten worden gebruikt om verschillen in complexiteit tussen
incidentcategorieën beter te begrijpen en dienen niet als zelfstandig
beslissingsmodel.

---

## Inhoud van het notebook

Het notebook bevat onder andere:

### Supervised learning (tekstclassificatie)
- Voorbewerking en opschoning van tekstdata  
- Omzetting van tekst naar numerieke kenmerken (TF-IDF)  
- Training van een classificatiemodel  
- Evaluatie van de resultaten op hoofdlijnen  
- Verkennende toepassing op incidenten met ontbrekende categorie  

### Unsupervised learning (topic modelling)
- Tekstopschoning en tokenisatie  
- Topic modelling met LDA  
- Identificatie van dominante thema’s per incident  
- Interpretatie van topics op inhoudelijk niveau  
- Gebruik van de resultaten ter verdieping van de analyse in Power BI  

---

## Dataset

De gebruikte dataset is niet opgenomen in deze repository in verband met
vertrouwelijkheid. Het notebook toont de volledige analysemethodiek en
kan worden uitgevoerd met een vergelijkbare datasetstructuur.

---

## Technische omgeving

De analyses zijn uitgevoerd met Python en gangbare data-analysebibliotheken,
waaronder pandas, scikit-learn, matplotlib en Jupyter Notebook.
