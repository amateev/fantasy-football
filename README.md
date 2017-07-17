# Implemented three scraping techniques:

### 1. cool way

* nightmare.js - headless browser to tackle content loaded in via js
* cheerio - to parse the html returned from nightmare

### 2. not cool way

copy and paste content into excel 

1. split the data on delimiters using text to columns 
2. select content and transpose it
3. manually join each team's schedule via cut and paste in excel

### 3. really not cool way

manually create a csv file (ex. offense-rankings.csv)

it might have been faster to implement a nightmare script for num 2 and 3 but whatev

# current formulas

wide receivers: 
=0.25*('offensive line rankings'!B2)+0.75*(32-'defense rankings'!B2+1)

running backs:
=0.75*('offensive line rankings'!B2)+0.25*('defense rankings'!B2)

# Steals I think

hunter henry		
zach ertz

john brown	
cameron merideth		
Tyrell Williams - Los Angeles Chargers	
Marquise Goodwin - San Francisco 49ers
Marqise Lee - Jaguars

leg blount
dalvin cook

immediate to do 
-----
* might want to switch o line rankings to https://www.fantasypros.com/2017/07/nfl-offensive-line-rankings-and-fantasy-impact/ OR add that in with profootball to see which one is better

* be sure to import as 2017 data - have a year column for everything

* implement promises with scrape.js

* implement rate limiting with scrape.js

* import mockdraftable player links

* create teams table

* import nfl-schedule-2017.csv

* import offense-rankings.csv

* delete duplicate games in nfl-schedule-2017 table

* need to use the schedule to really deep dive into who the weekly winners are and if there's a streak of having a really good opportunity (ex. weeks 1-6 use ameer abdullah and then it's downhill for him so trade him away then)

* need to add qb rankings to wide receivers and wide receiver rankings to rbs (opens up rb lanes)

