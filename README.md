# Dataset and project ideas for NTDS'19

## A word on data preparation

For all datasets, some degree of pre-processing is needed before obtaining usable data.
That is inherent to the work of a data scientist, and will mostly involve the following steps.

1. **Data acquisition.**
   Raw data may need to be (i) collected via a web API, (ii) collected by scraping a website, or (iii) already collected and packaged (for example in a CSV file).
2. **Data importation.**
   Raw data needs to be imported in a pandas DataFrame, where rows will be nodes of the network, and columns will be features (or characteristics or attributes) of those nodes.
3. **Data cleaning.**
   This step varies a lot from dataset to dataset.
   In the context of the course, it will mostly consist in reducing the size of the network so that it can be processed in a reasonable amount of time.
   The less packaged the raw data, the more cleaning will be necessary.
4. **Network creation.**
   The network structure may either be (i) given to you as an adjacency matrix, (ii) given to you as an edge list, or (iii) inferred from raw data.

While those steps are necessary for every dataset, the amount of pre-processing will however vary.
If a dataset requires raw data to be collected or the network to be created, that will be indicated in the datset description.
So if you are a beginner and do not feel confident, choose a dataset that requires little pre-processing.
If you feel confident, be adventurous!
Keep in mind that the amount of work generally trades with flexibility: well packaged data usually serves a single task and may restrict your creativity.

## Selecting a dataset

We encourage teams to choose a dataset and problematic that inspire them.
While we provide a [list of datasets](#proposed-datasets), we encourage motivated teams to look for their own data.
That is especially relevant to PhD students who want to apply the knowledge acquired in this course to their research problems.

---

## Project Proposal Group 23

- A Network Tour of Football Transfer

- Group 23:Saibo Geng,Olavo, Xiao Zhou  

- December 2019
- Presentation
  - Soccer is a very popular sport in Europe. At the same time, this attractive event has triggered a series of economic effects each year. During the transfer window, a lot of soccer players transfer from original club to another, which affect both the performance and economic condition of different clubs.
    According to statistics, the European football market is now estimated to be worth €25.5 billion. Upon this, we wonder the connection of this large amount of trade and the features that can influence the transfers. %Therefore, the trade of soccer players is a great potential for 
  - The goal of the project is to exploit the connection of the soccer player transfers among clubs in different European leagues. The analysis will be implemented in the network approach. During the project, we will create a graph based on the transfer of soccer players and exploit the data with tools like clustering, dimensionality reduction, classification, etc.

- Dataset
  The dataset that we choose to use are __Player Transfer Data of nine majors European football leagues from 1992 to 2018__ :[data](https://github.com/ewenme/transfers/tree/master/data)

  

   -  English Premier League
-  English Championship 
-  dutch eredivisie
-  french ligue 1
-  german bundesliga
-  italian serie A
-  portugese liga nos
-  spanish primera division
-  russian premier liga

Each dataset include features like:__club name,	player, name,	age,	position,	club involved name,	fee	transfer movement,	fee cleaned	league name,	year__

We may merge these data into a single dataset and proceed analysis in \textbf{European scale}, or pick a single league and proceed more fine grained analysis.

Besides, the __FIFA score data__ will also probably be used.

## Network


__Clubs based network__: Each club represents a node and the link would represent a transfer(transfers ) between two clubs and the weight could be for example the transfer fee amount or the number of transfers.
    
The tools that we choose to use:
__clustering (spectral clustering, k-means)
dimensionality reduction (PCA, MDS, LLE, ISOMAP, Laplacian eigenmaps, t-SNE)__



## Research Questions

In terms of the standard data exploration, some interesting questions would be:

- In the European context, which clubs mainly serve other clubs with players, and which ones get transferences from smaller clubs?

- Which countries have clubs that receive more players from abroad and which countries more often use their internal market?

In terms of the analysis of the structure of the network, we would like to investigate:

- Which clubs occupy the center of the European football transfer market, and which of them are more peripheric?

- Are there clusters of clubs that trade mainly with each other (in terms of number of players / fees)?

We would like to performe some classification task, such as for example (need to rewrite / more ideas):



