# Political Opinion Finder-2.0

Development repository for the second version of my social media opinion finder. It will have several notable improvement.

## Motivation

To make a revised version of [Political-Opinion-finder-1.0](https://github.com/philhabell/Political-Opinion-Finder) that is more versatile and usable so it can be used a product.

## Installation

Clone the repository, install [Python 3](https://www.python.org/downloads/) and the following Python libraries using `pip install`:
* `Tweepy` Twitter API library for accessing Twitter
* `pymongo` MongoDB library for using MongoDB
* `codecs` Encoding library for encoding the tweets
* `nltk` Natural language library for analysing meaning of tweets
* `tqdm`

Install the following from their `.whl` from the [Windows Binary](http://www.lfd.uci.edu/~gohlke/pythonlibs/) site using `pip install`:
* `numpy`
* `scipy`
* `scit_learn`
* `sklearn`

This is for Windows(I believe they work with normal `pip install` on Linux).

Create a JSON file with users MongoDB server credentials, use the [example](https://github.com/philhabell/Political-Opinion-Finder/blob/master/credentials/mongoCredentialsExample.json) file as a guide. If using a local server download [MongoDB](https://www.mongodb.com/download-center?jmp=nav) and leave `mongoURL` empty in the JSON file.

User must also create a JSON file with there [Twitter API](https://apps.twitter.com/) credentials, use the [example](https://github.com/philhabell/Political-Opinion-Finder/blob/master/credentials/apiCredentialsExample.json) file as a guide.


## Operation

Run the following in console/terminal:
``` 
python ./main.py
```
Then select what you would like to do from the menu presented to you.

On first run the program will download the necessary [NLTK data](http://www.nltk.org/data.html) (This may take some time).
It is advised to use `Gather tweets` option on first run so there are tweets in the database.
The calculation of twitter vs poll opinion difference does take a long time (can be hours on a slower system).

## Licence
Copyright (C) 2017 Philip Bell - All Rights Reserved
Unauthorized copying of this file, via any medium is strictly prohibited.

Proprietary and confidential.

Written by Philip Bell <philhabell@gmail.com>, March 2017.

**[Back to top](#political-opinion-finder)**