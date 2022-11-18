### ada-2022-project-nonansland22

# The evolution of women’s representation in the film industry

### Abstract 
The last decade has been marked by emancipating and feminist movements. While many inequalities subsist to this day, women’s rights have progressed, along with mentalities. In this context, one could assess if before the last decade, a trend of improved women’s representation was translated in the film industry during the last fifty to a hundred years, and how this representation itself has evolved (i.e., the way women are depicted, and their relative importance compared to male characters). Firstly, it would be interesting to study women’s representation across many movies using different characteristics throughout the last century, combining meta-datas about the movies, their characters, and their summaries’ language analysis. Then, one could study in more detail and compare different movie genres to further gain insight on women’s representation and evaluate its homogeneity across the film industry. Lastly, one could use the movies’ countries of origin to assess progress in this representation in different world regions.

 ### Research questions
How has the representation of female characters evolved in the film industry over time ? 
A) Has the presence (eg. proportion) and attributes (eg. age) of female characters differ over time and how do they compare to male characters ?
B) How has women’s representation evolved in some of the most mainstream genres, and how homogenous was this representation across genres throughout time? 
C) How are female characters depicted and how important are their roles relative to male characters using language analysis?
 
### Proposed additional datasets
 
**Stanford CoreNLP processed summaries**: Learning Latent Personas of Film Characters David Bamman et al. ran all the plot summaries through the Stanford Core NLP pipeline. They tagged and parsed the text to extract entities, and resolve coreference within the document. Using these processed XML files for each movie, we can extract language and look at descriptive words for each character to be able to assess female character representation compared to male characters. 
 
**Metacritic:** Metacritic website gathers critiques given by professional movie critics and computes them into a ‘metascore’. We can use this metascore to assess how movies with important and active main female characters were received by the society at the time the movie aired, contrarily to IMDB where the grades can be given years after the movies’ release.
 
**Wikidata:** We have an important amount of missing values in the character metadata in the ‘character name’ and/or gender. Those two as well as the release date for the movies are critical to assess women’s representation over time. We want to enrich our initial data set and retrieve those missing values to increase the number of movies and characters that can be part of the analysis. 
 
 
### Methods
 
First, we properly loaded and labeled the movie and character metadata and plot summaries. Then, using the wiki ID, the common feature of these three datasets, we made an intersection to extract the movies for which we have access to the data available on all three datasets. This enabled linking all characters to the movie’s specifics and extracting language analysis from the plot summaries about each character. Finally, we used each dataset to extract the most relevant genres, the specifics of each character, and their importance and attributes. 
 
Using the obtained filtered movie metadata dataset, before looking at evolution through time we looked at general aspects of women representation in the whole dataset. This includes various metrics such as age distribution or women to men presence ratio. After observing general tendencies, we splitted the data in decades, in order to assess an eventual evolution. In a further analysis, we wanted to extract a combination of three genres as independent as possible from each other, with a relative importance in the film industry with a high movie count. Then, one could assess if the temporal evolution observed previously is equally present and homogeneous across genres.
 
Furthermore, we aimed to determine how the female characters' representation itself evolved throughout time, in terms of their relative importance in the scenario. To do so, we used language analysis of the plot summaries over time (with Stanford CoreNLP processed summaries), by observing the evolution of agent verbs, patient verbs and attributes associated with female characters. 
 
Lastly, we assessed if the change in women’s representation is progressive or if we notice any significant gap. We can also highlight if the evolution is shared across the film industry or if different popular genres have other impacts and evolutions. 
 
 
 
 
 
 
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
Select together the subject with the highest potential and interests

Data exploration 

Define research questions and feasibility

Define pipeline and steps
 
#### Individual/pair:
Understand formats, distributions, missing values and correlations of the data of each data frame individually.

Exploratory data analysis and visualization.

Filter and transform the data from each dataset. Extract features and descriptive values from relevant variables of each data frame individually.

Language and XML extraction pipeline.

Analysis and selection of relevant genres. Data analysis across time  for the selected genre.

Language analysis for Female character’s specificities extraction relative to male characters across time in the film industry.

Visualize summaries language extraction to evaluate the quantity of attributes, relevance, role, and impact of female characters compared to male ones.

Statistical tests to evaluate previous analysis and findings between male and female characters.

Relevant plots to visualize women’s representation evolution in the film industry and its possible similarity across popular and independent genres.

Case study eg. Hollywood vs Bollywood 

Website
 
 
 
### Questions for TAs
 
Is it correct to separate the different genres the way we did? 

Is it correct to divide by decade or should we use another timescale?


