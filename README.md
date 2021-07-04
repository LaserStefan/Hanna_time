# Analysis of Tweets for the #IchBinHannah Campaign

Authors: #IchBinHanna Research Collective
(in alphabetic order: David Adler, Migle Bareikyte, Elen Le Foll, Christian Funk, Stefan Laser, Jana Lasser)

This is part of a collaborative project that sits at the intersection of campaigning and doing (computational) social science research. Other output of the #IchBinHanna Research Collective [is stored here](https://github.com/LaserSteff/IchbinHanna).

[![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

## Data  

### Included Datasets
* **#IchBinHanna**: This hashtag refers to "Hanna" from a [video](https://www.bmbf.de/de/media-video-16944.html) published by the German ministry for education and research back in 2018. In a cartoon film, the Ministry of Education thus introduces the background and alleged advantages of the fixed-term regulations in the German academic system, following the career of a fictitious doctoral student in biology, Hanna. In June 2021, the video was "rediscovered" and caused a wave of activity under the #IchBinHannah hashtag on Twitter. We used various lower and upper case versions and the Hanna/h combination in our query.

The dataset was downloaded using twarc (see section [Getting data from Twitter](#getting-data-from-twitter)). The respecitve query is stored in the folder ```query```.

We store only the Tweet IDs and Conversation IDs of the Tweets and conversations that were included in the data analysis. We do not store full tweets, due to restrictions in the Twitter terms of use. Using the Tweet IDs stored in ```data/tweet-IDs```, you can "rehydrate" the corresponding tweets, using for example [twarc](https://scholarslab.github.io/learn-twarc/06-twarc-command-basics#rehydrate-a-dataset) by typing  

```twarc2 hydrate tweet_ids.txt > tweets_hydrated.jsonl```  

in your command line. Similarly, by using the [twarc conversations](https://twarc-project.readthedocs.io/en/latest/twarc2/#conversations) utility, you can retrieve all Tweets belonging to a converation ID  

```twarc2 conversations conversation_ids.txt conversations.jsonl```

## Frequency plot
The plot [displayed for public exploration](https://lasersteff.github.io/Hanna_time/) was created using plotly. Check the Jupyter notebook ```plotly_interactive_time``` to access the code. The plot is stored in the ```index.html``` file.
