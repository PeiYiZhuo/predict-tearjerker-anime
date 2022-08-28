# predict-tearjerker-anime

One of the few pieces of media to have ever coaxed tears from me is Kyoto Animation's devastating 2008 anime series *Clannad: After Story*, a show that I enthusiatically recommend. I do so not in spite of the fact that it crushed my soul, mind you, but because of it. If anything, I consider an anime's ability to turn on the waterworks a marker of quality. Most of my favorite anime are considered tearjerkers (In addition to *Clannad: After Story*, *A Place Further than the Universe* and *Your Name* come to mind as notable examples.). Even if I do not tear up while watching them, a decent attempt on the part of an anime's creators garners enormous credit from me nonetheless. 

Given my affinity for the medium, it comes as no surprise that predicting tearjerker anime would be a fun project with which to advance my understanding of machine learning and scikit-learn. Using data scraped off of the website MyAnimeList, courtesy of [Marlesson](https://www.kaggle.com/datasets/marlesson/myanimelist-dataset-animes-profiles-reviews?select=animes.csv) and [Azathoth](https://www.kaggle.com/datasets/azathoth42/myanimelist?select=AnimeList.csv), I ...

1. Labeled each member of a set of 1690 anime, every one of which has at least 10 MyAnimeList reviews available, as a tearjerker or a non-tearjerker based on the simultaneous occurence within a single review of at least one word that connotes saddness and at least one word that conveys crying.
2. Used the total number of MyAnimeList users who reported they have watched or are planning to watch a particular anime and the studios that created said anime along with the score, number of episodes, synopsis, genre, and source of the anime as well as whether or not it was a TV show to predict the anime's tearjerker status using logistic regression.

My logistic regression model ultimately achieved an accuracy of 87% when it was evaluated using five-fold cross validation on the training set.

## Citations

Marlesson. (2020). *Anime Dataset with Reviews - MyAnimeList* [Data set]. Kaggle. https://www.kaggle.com/datasets/marlesson/myanimelist-dataset-animes-profiles-reviews

Matěj Račinský. (2018). <i>MyAnimeList Dataset</i> [Data set]. Kaggle. https://doi.org/10.34740/KAGGLE/DSV/45582
