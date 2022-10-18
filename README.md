# WHAT ABOUT SHARKS?

<center>
<img src=./images/jaws-movie-poster.jpg alt=“shark_title” width=“400”/>
</center>

## Abstract
This project is about exploring the Global Shark Attacks dataset, which can be downloaded at kaggle.com 

The dataset is filled with recorded shark attacks by the Shark Research Institute, whose objective is to give a better understanding of our relationship with those animals and minimize the risk of the interactions.

## Data Cleaning
Since the dataset is really dirty we will focus on the following data:
- Year of the attack
- Month of the attack
- Sex of the victim
- Fatality of the attack
- Age of the victim
- Species of the shark

The focus of the cleaning has been put into getting the species of the shark as clean as possible.

## Hypothesis

### 1) Men are more prone to get attacked by a shark than Women
The first hypothesis revolves around determining what sex is attacked the most by the sharks.

For proving it we have plotted the year of the attacks vs. the age of the victim and highlighting the sex of the victim.

We can easily check that out hypothesis was correct, and as extra information we can notice that most of the victims are around 20 years old or younger.

This dataset has way more records in the recent years generating some bias on the data, but that was expected.

<center>
<img src=./images/year_vs_age_sex.png width=“400”/>
</center>

### 2) In the recent years the fatality has decreased as there is a general better access to sanity.

In the plot below we have the same scatter plot comparing the year of the attacks vs. the age of the victim but this time the fatality is highlighted.

We can check that most of the deaths are distributed towards the oldest data even though most of the records are more recent, as we expected. But that could be because only fatal attacks were recorded and simple injuries were ignored.

<center>
<img src=./images/year_vs_age_fatality.png width=“400”/>
</center>

### 3) Fatal attacks are performed by greater shark species
After filtering the data so we only keep the records where the shark species is explicitely stated and confirmed we have plotted the attacks by species.

In the following figure we can check that bigger species account for the majority of the aggressions, with the white shark standing out by a great amount.
<center>
<img src=./images/total_attacks_fatality.png width=“400”/>
</center>

To determine the most dangerous species we have plotted the ratio of fatality over the attacks recorded and the tier list is as follows:

More than 25% of the Tiger Shark attacks end in death, closely followed by the Bull Shark, the White Shark, the Oceanic Whitetip Shark and the Blue Shark.

### Top dangerous sharks
    1) Tiger Shark
    2) Bull Shark
    3) White Shark
    4) Oceanic Whitetip Shark
    5) Blue Shark
    6) Bronze Whaler Shark
    7) Hammerhead Shark
    8) Mako Shark
    9) Nurse Shark
    10) Blacktip Shark
    11) Wobbegong Shark
    12) Raggedtooth Shark
    13) Spinner Shark
    14) Lemon Shark

<center>
<img src=./images/fatality_ratio.png width=“400”/>
</center>

Now for extra insights we will show the distribution of the attacks by year by the top 5 most deadly species.

One surprising thing is the increase of the representation in the attacks of the Bull Shark and the Tiger Shark in the recent years.

<center>
<img src=./images/kde1_attacks_year_top5.png width=“400”/>
</center>

<center>
<img src=./images/kde2_attacks_year_top5.png width=“400”/>
</center>

In the following figures we can notice how younger people suffer more attacks.

<center>
<img src=./images/kde1_attacks_victim_age_top5.png width=“400”/>
</center>

<center>
<img src=./images/kde2_attacks_victim_age_top5.png width=“400”/>
</center>

And finally we have plotted the distribution of the fatal attacks by year for all the species. It is surprising that the Blue Shark and the Bronze Whaler Shark only have fatal attacks around the 1960s and in the following years no more fatal incidents are recorded.


<center>
<img src=./images/kde_fatal_attacks_year.png width=“400”/>
</center>


## Conclusion
As we had supposed, we have verified that men are attacked more usually by sharks (1:10 ratio aprox). We also have checked that the fatality of the incident has decreased in the recent years and discovered what are the most deadly species.

One last thing to notice is that the White Shark seems over represented in this dataset. It may be because it is one of the most well known shark species and when most people are attacked by a big shark they assume it is a one of them.