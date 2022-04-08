# Intent and Slots Datasets
This repository contains the two famouse datasets namely ATIS and SNIPS used for benchmarking models on Intent Classification and Slot Filling tasks. In this repostory, I've changed the data format, making it common for both of them. The data scheme is the following:
```json
[
  {
    "utterance": "on april first i need a flight going from phoenix to san diego", 
    "slots": "O B-depart_date.month_name B-depart_date.day_number O O O O O O B-fromloc.city_name O B-toloc.city_name I-toloc.city_name", 
    "intent": "flight"
   },
   "..."
]
```
Basically, the data scheme is an array of dictionaires, where each dictionary is an element of the dataset.

## ATIS 
ATIS dataset has been taken from Microsof CNTK: https://github.com/Microsoft/CNTK/tree/master/Examples/LanguageUnderstanding/ATIS/Data. It is split in training and test sets containing 4978 and 893 examples, respetively. 
## SNIPS
SNIPS dataset has been taken from the GitHub repo: https://github.com/ZhenwenZhang/Slot_Filling 
