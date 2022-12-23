### ada-2022-project-nonansland22

### Datastory 

The website containing our datastory can be found [here](https://pauldfepfl.github.io/DatastoryNonNansLand/2022/12/21/datastory.html) 

# The evolution of women’s representation in the film industry

To follow this notebook, the datataset and the Supplement: Stanford CoreNLP-processed summaries need to be downloaded from https://www.cs.cmu.edu/~ark/personas/. These folders need to placed at the same level, in the the same directory of this notebook.

### Abstract 
The last decade has been marked by emancipating and feminist movements. While many inequalities subsist to this day, women’s rights have progressed, along with mindsets[1][2]. In this context, we are going to assess if before the last decade, a trend of improved women’s representation was translated in the film industry during the last fifty years, and how this representation itself has evolved (i.e., the way women are depicted, and their relative importance compared to male characters). Firstly, it would be interesting to study women’s representation across many movies using different characteristics throughout the last century, combining meta-datas about the movies, their characters, and their summaries’ language analysis. Then, we will study in more detail and compare different movie genres to further gain insight on women’s representation and evaluate its homogeneity across the film industry. Lastly, we will use the movies’ countries of origin to assess progress in this representation in different world regions.

 ### Research questions
How has the representation of female characters evolved in the film industry over time? 
A) Has the presence (eg. proportion) and attributes (eg. age) of female characters differed over time and how do they compare to male characters?
B) How has women’s representation evolved in some of the most mainstream genres, and how homogenous was this representation across genres throughout time? 
C) How are female characters depicted and how important are their roles relative to male characters using language analysis?
 
### Proposed additional datasets
 
**Stanford CoreNLP processed summaries**: Learning Latent Personas of Film Characters David Bamman et al. ran all the plot summaries through the Stanford Core NLP pipeline. They tagged and parsed the text to extract entities, and resolve coreference within the document. Using these processed XML files for each movie, we can extract language and look at descriptive words for each character to be able to assess female character representation compared to male characters. 
 
**Metacritic:** Metacritic website gathers critiques given by professional movie critics and computes them into a ‘metascore’. We can use this metascore to assess how movies with important and active main female characters were received by the society at the time the movie aired, contrarily to IMDB where the grades can be given years after the movies’ release.
 
**Wikidata:** We have an important amount of missing values in the character metadata in the ‘character name’ and/or gender. Those two as well as the release date for the movies are critical to assess women’s representation over time. We want to enrich our initial data set and retrieve those missing values to increase the number of movies and characters that can be part of the analysis. 
 
 
### Methods

**Step 1: Data pre-processing, dataset filtering and correction**

- Loaded and labeled the movie and character metadata and plot summaries.
- Intersection, using the wiki ID, the common feature of these three datasets, to extract the movies for which we have access to the data available on all three datasets.
- Profiling.
- Used wikidata to retrieve missing information such as gender, date of birth, characters'name.
- Filtered data: removed non-relevant columns, characters with missing features of interest, characters with aberant values succh as negative values for age.

**Step 2: Visualisation and exploratory data analysis**
- Looked at general aspects of women representation in the whole dataset. This includes various metrics such as age distribution or women to men ratios and proportions.
- After observing general tendencies, we splitted the data in decades, in order to assess an eventual evolution in the metrics observed previously.

**Step 3: Analysis by genre and comparison to the previously obtained results**
- Extracted a combination of three genres as independent as possible from each other and with a relative importance in the film industry due to a high movie count.
- Assessed if the temporal evolution observed previously is equally present and homogeneous across genres. Studied evolution of age and ratios.

**Step 4: Language analysis**
We aimed to determine how the female characters' representation itself evolved throughout time, in terms of their relative importance in the scenario.

- Used language analysis of the plot summaries over time (with Stanford CoreNLP processed summaries), by observing the evolution of agent verbs, patient verbs and attributes associated with female characters.
- Highlighted if the evolution is shared across the film industry or if different popular genres reveal different trends and evolutions.
- Vizualized qualitatively the results using wordclouds.

**Step 5*: geographical case study Hollywood vs Bollywood**
- Analyzed similar features studied on the overall population: Proportion of women and age distibution for Indian and American movies.
- Language analysis of Indian movies compared to US movies
- Vizualized qualitatively the results using wordclouds

**Step 6: Population's reception to women-empowering movies**
- Used metascore from metacritic to assess how movies with important and active main female characters were received by the society at the time the movie aired.
 
 
### Proposed timeline
 
#### P2
Week 1: Data pre-processing and data filtering for the analysis needs

Week 2: Exploratory data analysis, XML file extraction and README

Week 3: Language analysis, visualization and finalize README
 
#### P3
Week 1: Further analysis and Statistical test of P2 analysis 

Week 2: Case study (e.g., Hollywood vs Bollywood) and website

Week 3: Data story, website, and README
 
 
### Organization within the team
 
#### Team:
- Select together the subject with the highest potential and interests
- Data exploration 
- Understand formats, distributions, missing values of the data of each data frame individually. 
- Define research questions and feasibility
- Define pipeline and steps

#### Individual/pair:

Matthieu/Arnault:
- Data pre-processing and dataset filtering
- Genre selection and analysis. 
- XML extraction pipeline.
- Quantitative Language analysis and visualization

Matthieu: 
- Interactive plots and improved plot visualization 
- Wikidata
- Metacritic
- Hollywood vs Bollywood

Arnault:
- Wordcloud analysis
- Readme

Paul/Jules: 
- Visualisation and exploratory data analysis.
- Analysis on the general filtered dataset. 

Paul: 
- Website
- Profilling
- Plots designing
 
Jules: 
- Statistical tests to evaluate previous analysis and findings between male and female characters. 
- Redaction of datastory


### References
[1] Our Favorite Milestones for Women This Decade [WWW Document], n.d. . Ellevest. URL https://www.ellevest.com/magazine/disrupt-money/women-milestones-2010s (accessed 12.23.22).


[2] The 2010s the decade women fought back, Forbes. URL https://www.forbes.com/sites/lizelting/2019/12/20/the-2010s-the-decade-women-fought-back/?sh=68c5546421ad




