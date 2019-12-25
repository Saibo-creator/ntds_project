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
  The dataset that we choose to use are __Player Transfer Data of nine majors European football leagues from 1992 to 2018__ :

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
Two possibilities:

__Players based network__: Each player is a node and the link could be "if two players played in a same team before".

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

- Is it possible to infer the wealth of a club by analyzing the patterns of transfers between it and other clubs

## Past projects

Projects from NTDS'18:
* [[report][r01], [slides][s01], [code][c01]] A Network Analysis of Movie Popularity
* [[report][r02], [slides][s02], [code][c02]] Learning US Senate voting behavior from bill sponsorship profiles
* [[report][r03], [slides][s03], [code][c03]] Retrieving the continent labels from the air routes structure
* [[report][r04], [slides][s04], [code][c04]] Evolution of the movie industry
* [[report][r05], [slides][s05], [code][c05]] A network tour to flight delay in the US
* [[report][r06], [slides][s06], [code][c06]] Flight network and airline alliances
* [[report][r07], [slides][s07], [code][c07]] Vote prediction of US Senators from graph properties
* [[report][r08], [slides][s08], [code][c08]] Spreading disease through the air
* [[report][r09], [slides][s09], [code][c09]] A Network Analysis of the 2018 FIFA World Cup
* [[report][r10], [slides][s10], [code][c10]] History of Movie Success through GSP
* [[report][r11], [slides][s11], [code][c11]] Music Genre Recognition
* [[report][r12], [slides][s12], [code][c12]] Finding Continents from a Flight Routes Network
* [[report][r13], [slides][s13], [code][c13]] Conversation starter using Wikipedia
* [[report][r14], [slides][s14], [code][c14]] Smooth Radio: Automatic playlist generation using signal graph processing
* [[report][r15], [slides][s15], [code][c15]] Movie Grossing Success Prediction with Convolutional Neural Networks on Graphs
* [[report][r16], [slides][s16], [code][c16]] How to invest in movies?
* [[report][r17], [slides][s17], [code][c17]] A Netflix Tour of Data Science — Film suggestion by diffusion on graphs
* [[report][r18], [slides][s18], [code][c18]] U.S. Senators: A Voting Pattern Study
* [[report][r19], [slides][s19], [code][c19]] A Data Study of Terrorism and its Tendencies
* [[report][r20], [slides][s20], [code][c20]] Spammer… Catch me if you can
* [[report][r21], [slides][s21], [code][c21]] Exposing the True Terrorist Network
* [[report][r22], [slides][s22], [code][c22]] Small Components' Analysis and Flight Delay Prediction
* [[report][r23], [slides][s23], [code][c23]] Minipedia
* [[report][r24], [slides][s24], [code][c24]] Wikipedia Analysis Using Keyword Based Graphs
* [[report][r25], [slides][s25], [code][c25]] Finding the Authors of a Terrorist Attack
* [[report][r27], [slides][s27], [code][c27]] How to beat terrorism efficiently: identification of set of key players in terrorist networks
* [[report][r28], [slides][s28], [code][c28]] A Network Topology Analysis of the Airline Industry
* [[report][r29], [slides][s29], [code][c29]] Predicting Terror Attacks — A Data Story
* [[report][r30], [slides][s30], [code][c30]] Free Music Alternative Playlists
* [[report][r31], [slides][s31], [code][c31], [proposal][p31]] Feminism in Hollywood
* [[report][r32], [slides][s32], [code][c32]] Genre Classification: A Transductive, Inductive and Deep Approach
* [[report][r33], [slides][s33], [code][c33]] Friends Will Be Friends: A Network Tour of Musical Friendship
* [[report][r34], [slides][s34], [code][c34]] Predicting the nature of terrorist attacks
* [[report][r36], [slides][s36], [code][c36]] Transitional playlists for new musical discoveries
* [[report][r37], [slides][s37], [code][c37]] A Wikipedia Tour of Death — or how University College Boat Club became popular
* [[report][r38], [slides][s38], [code][c38]] Tempering the Spread of Epidemics on Aerial Networks
* [[report][r40], [slides][s40], [code][c40]] Can we estimate the earnings of a movie?
* [[report][r42], [slides][s42], [code][c42]] Re-balancing flight routes inequalities
* [[report][r44], [slides][s44], [code][c44], [proposal][p44]] Voting patterns in the Swiss National Council
* [[report][r47], [slides][s47], [code][c47]] An overviews of intercontinental flight route connections
* [[report][r49], [slides][s49], [code][c49]] A Network Tour of Millenial Movies
* [[report][r50], [slides][s50], [code][c50]] Identifying Spammers on Social Networks
* [[report][r51], [slides][s51], [code][c51], [proposal][p51]] An exploratory study on the brain dysconnectome
* [[report][r52], [slides][s52], [code][c52]] Mood Changing Playlist Generator
* [[report][r54], [slides][s54], [code][c54]] Fight Against Terrorism

Projects from NTDS'17:
* [[proposal][01p], [analysis][01r], [slides][01s]] American Basketball Players
* [[proposal][02p], [analysis][02r], [slides][02s]] Graph-based Nutrition Guide
* [[proposal][03p], [analysis][03r], [slides][03s]] What Impacts the Success of a Movie?
* [[proposal][04p], [analysis][04r], [slides][04s]] Exploring the Crunchbase Dataset to Detect High Potential Startups
* [[proposal][05p], [analysis][05r], [slides][05s]] Beer Suggester
* [[proposal][06p], [analysis][06r], [slides][06s]] Swiss Political Survey
* [[proposal][07p], [analysis][07r], [slides][07s]] A StackOverflow Recommender System
* [[proposal][08p], [analysis][08r], [slides][08s]] Analysis of World Development Indicators as Predictors
* [[proposal][09p], [analysis][09r], [slides][09s]] Satellites Characterization – Clustering using Orbital Characteristics
* [[proposal][10p], [analysis][10r], [slides][10s]] Amazon Electronic Products – Network Analysis
* [[proposal][11p], [analysis][11r], [slides][11s]] GSP on the Digital Reconstruction of the Brain
* [[proposal][12p], [analysis][12r], [slides][12s]] Movie Recommendation
* [[proposal][13p], [analysis][13r], [slides][13s]] GraphLang
* [[proposal][14p], [analysis][14r], [slides][14s]] Buda + Pest = Budapest
* [[proposal][15p], [analysis][15r], [slides][15s]] Manifold Learning of Face Data
* [[proposal][16p], [analysis][16r], [slides][16s]] A Network Tour of the Tunisian and Egyptian Springs
* [[proposal][17p], [analysis][17r], [slides][17s]] StackOverflow Survey
* [[proposal][18p], [analysis][18r], [slides][18s]] Speech Recognition Challenge
* [[proposal][19p], [analysis][19r], [slides][19s]] Analysis of the Elite Football Transfer Market
* [[proposal][20p], [analysis][20r], [slides][20s]] Titanic
* [[proposal][21p], [analysis][21r], [slides][21s]] This is My Jam
* [[proposal][22p], [analysis][22r], [slides][22s]] A Network Tour of StackOverflow
* [[proposal][23p], [analysis][23r], [slides][23s]] Course Suggester
* [[proposal][24p], [analysis][24r], [slides][24s]] Spectral Analysis of 5000 Movies Network
* [[proposal][25p], [analysis][25r], [slides][25s]] Community Detection on the Wikipedia Hyperlink Graph
* [[proposal][26p], [analysis][26r], [slides][26s]] 3D Meshes of Facial Expression
* [[proposal][27p], [analysis][27r], [slides][27s]] Terrorist Attacks
* [[proposal][28p], [analysis][28r], [slides][28s]] Community Detection and Labelling in an Instagram Network
* [[proposal][29p], [analysis][29r], [slides][29s]] Graph-based Recommendation for lastFM 

[p31]: https://github.com/mdeff/ntds_2018/blob/master/projects/proposals/team_31.pdf
[p44]: https://github.com/mdeff/ntds_2018/blob/master/projects/proposals/team_44.pdf
[p51]: https://github.com/mdeff/ntds_2018/blob/master/projects/proposals/team_51.pdf

[r01]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_01.pdf
[r02]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_02.pdf
[r03]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_03.pdf
[r04]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_04.pdf
[r05]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_05.pdf
[r06]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_06.pdf
[r07]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_07.pdf
[r08]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_08.pdf
[r09]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_09.pdf
[r10]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_10.pdf
[r11]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_11.pdf
[r12]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_12.pdf
[r13]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_13.pdf
[r14]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_14.pdf
[r15]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_15.pdf
[r16]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_16.pdf
[r17]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_17.pdf
[r18]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_18.pdf
[r19]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_19.pdf
[r20]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_20.pdf
[r21]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_21.pdf
[r22]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_22.pdf
[r23]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_23.pdf
[r24]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_24.pdf
[r25]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_25.pdf
[r27]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_27.pdf
[r28]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_28.pdf
[r29]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_29.pdf
[r30]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_30.pdf
[r31]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_31.pdf
[r32]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_32.pdf
[r33]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_33.pdf
[r34]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_34.pdf
[r36]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_36.pdf
[r37]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_37.pdf
[r38]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_38.pdf
[r40]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_40.pdf
[r42]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_42.pdf
[r44]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_44.pdf
[r47]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_47.pdf
[r49]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_49.pdf
[r50]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_50.pdf
[r51]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_51.pdf
[r52]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_52.pdf
[r54]: https://github.com/mdeff/ntds_2018/blob/master/projects/reports/team_54.pdf

[s01]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_01.pdf
[s02]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_02.pdf
[s03]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_03.pdf
[s04]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_04.pdf
[s05]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_05.pdf
[s06]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_06.pdf
[s07]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_07.pdf
[s08]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_08.pdf
[s09]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_09.pdf
[s10]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_10.pdf
[s11]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_11.pdf
[s12]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_12.pdf
[s13]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_13.pdf
[s14]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_14.pdf
[s15]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_15.pdf
[s16]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_16.pdf
[s17]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_17.pdf
[s18]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_18.pdf
[s19]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_19.pdf
[s20]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_20.pdf
[s21]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_21.pdf
[s22]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_22.pdf
[s23]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_23.pdf
[s24]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_24.pdf
[s25]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_25.pdf
[s27]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_27.pdf
[s28]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_28.pdf
[s29]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_29.pdf
[s30]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_30.pdf
[s31]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_31.pdf
[s32]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_32.pdf
[s33]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_33.pdf
[s34]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_34.pdf
[s36]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_36.pdf
[s37]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_37.pdf
[s38]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_38.pdf
[s40]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_40.pdf
[s42]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_42.pdf
[s44]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_44.pdf
[s47]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_47.pdf
[s49]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_49.pdf
[s50]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_50.pdf
[s51]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_51.pdf
[s52]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_52.pdf
[s54]: https://github.com/mdeff/ntds_2018/blob/master/projects/slides/team_54.pdf

[c01]: https://github.com/illorens/Project_NTDS
[c02]: https://github.com/roman-bachmann/US-Senators
[c03]: https://github.com/AmauV/NTDS
[c04]: https://github.com/swouf/ntds_IMDb_team4
[c05]: https://github.com/yf0726/ntds_project
[c06]: https://github.com/nicolasFontbonne/Project_ntds
[c07]: https://github.com/magoncal/NTDS_Project
[c08]: https://github.com/dsalathe/group_ntds
[c09]: https://github.com/ProjectNTDS/Network_World_Cup_Analysis
[c10]: https://github.com/hugofluhr/Team10_ntds_2018
[c11]: https://github.com/angomez/ntds
[c12]: https://github.com/franckdess/NTDS_Project
[c13]: https://github.com/okhofsk/NTDS_Wikipedia
[c14]: https://github.com/padesplaces/ntds_project
[c15]: https://github.com/mcherep/ntds-epfl
[c16]: https://github.com/GentleDell/IMDb_movie_analysis
[c17]: https://github.com/PierreFourcade/A-Netflix-Tour-of-Data-Science---Film-suggestion-by-diffusion-on-graphs
[c18]: https://github.com/lkieliger/US-Senators
[c19]: https://github.com/AminMekacher/NTDS_Team19
[c20]: https://github.com/mfendri2/NTDS_Project_Team20
[c21]: https://github.com/sinyil/ntds_2018_Final_Project
[c22]: https://github.com/sami2310/NTDS_Project_team22
[c23]: https://github.com/Ivo-A/Team23_Wikipedia
[c24]: https://github.com/mattminder/wikilinks
[c25]: https://github.com/yusiZou/NTDS_project
[c27]: https://github.com/natbolon/terrorist_network_weaknesses
[c28]: https://github.com/rusucosmin/ntp
[c29]: https://github.com/Axeln78/TerrorAttacksNtds
[c30]: https://github.com/TTimTT/FMAP
[c31]: https://github.com/othmanbck/ntds_project_2018
[c32]: https://github.com/senakicir/ntds_project
[c33]: https://github.com/JCrobe/NTDS19_FWBF
[c34]: https://github.com/coencharles/NTDS_team34
[c36]: https://github.com/Team36-ntds2018/Project_free_music_archives_2018
[c37]: https://github.com/isabelaconstantin/wikinet
[c38]: https://github.com/montalex/NTDS_2018_Final_Project
[c40]: https://github.com/rocari96/NTDS-project
[c42]: https://github.com/VincentCoriou/Re-balancing-flight-routes-inequalities
[c44]: https://github.com/nikolaiorgland/conseil_national
[c47]: https://github.com/FrankSchmutz/NTDS2019FinalProject
[c49]: https://github.com/MilenaFilipovic/NTDS_Project_Team_49
[c50]: https://github.com/ilijagjorgjiev/project_ntds
[c51]: https://github.com/emullier/NTDS_team51_BrainNetworks
[c52]: https://github.com/rezaho/NetworkTour-of-DataScience
[c54]: https://github.com/mouadhhamdi/NTDS_Project

[01p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/basketball_players.pdf
[02p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/nutrition_guide.pdf
[03p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/movie_success.pdf
[04p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/crunchbase_startups.pdf
[05p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/beer_suggester.pdf
[06p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/swiss_politics.pdf
[07p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/stackoverflow_recommendation.pdf
[08p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/countries_development.pdf
[09p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/satellites.pdf
[10p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/amazon_products.pdf
[11p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/brain_network.pdf
[12p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/movie_recommendation.pdf
[13p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/graphlang.pdf
[14p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/road_network.pdf
[15p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/face_manifold.pdf
[16p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/arab_springs.pdf
[17p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/stackoverflow_survey.pdf
[18p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/speech_recognition.pdf
[19p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/football_transfers.pdf
[20p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/titanic.pdf
[21p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/jam.pdf
[22p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/stackoverflow_network.pdf
[23p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/course_suggester.pdf
[24p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/movie_network.pdf
[25p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/wikipedia_hyperlink.pdf
[26p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/facial_expression.pdf
[27p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/terrorist_attacks.pdf
[28p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/instagram_community.pdf
[29p]: https://github.com/mdeff/ntds_2017/blob/master/projects/proposals/lastfm_recommendation.pdf

[01s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/basketball_players.pdf
[02s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/nutrition_guide.pdf
[03s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/movie_success.pdf
[04s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/crunchbase_startups.pdf
[05s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/beer_suggester.pdf
[06s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/swiss_politics.pdf
[07s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/stackoverflow_recommendation.pdf
[08s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/countries_development.pdf
[09s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/satellites.pdf
[10s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/amazon_products.pdf
[11s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/brain_network.pdf
[12s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/movie_recommendation.pdf
[13s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/graphlang.pdf
[14s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/road_network.pdf
[15s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/face_manifold.pdf
[16s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/arab_springs.pdf
[17s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/stackoverflow_survey.pdf
[18s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/speech_recognition.pdf
[19s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/football_transfers.pdf
[20s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/titanic.pdf
[21s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/jam.pdf
[22s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/stackoverflow_network.pdf
[23s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/course_suggester.pdf
[24s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/movie_network.pdf
[25s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/wikipedia_hyperlink.pdf
[26s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/facial_expression.pdf
[27s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/terrorist_attacks.pdf
[28s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/instagram_community.pdf
[29s]: https://github.com/mdeff/ntds_2017/blob/master/projects/slides/lastfm_recommendation.pdf

[01r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/basketball_players
[02r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/nutrition_guide
[03r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/movie_success
[04r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/crunchbase_startups
[05r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/beer_suggester
[06r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/swiss_politics
[07r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/stackoverflow_recommendation
[08r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/countries_development
[09r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/satellites
[10r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/amazon_products
[11r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/brain_network
[12r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/movie_recommendation
[13r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/graphlang
[14r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/road_network
[15r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/face_manifold
[16r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/arab_springs
[17r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/stackoverflow_survey
[18r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/speech_recognition
[19r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/football_transfers
[20r]: https://github.com/zifeo/Titanic
[21r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/jam
[22r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/stackoverflow_network
[23r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/course_suggester
[24r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/movie_network
[25r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/wikipedia_hyperlink
[26r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/facial_expression
[27r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/terrorist_attacks
[28r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/instagram_community
[29r]: https://github.com/mdeff/ntds_2017/blob/master/projects/reports/lastfm_recommendation
