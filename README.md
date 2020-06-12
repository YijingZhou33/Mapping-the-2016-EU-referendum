# Mapping the 2016 EU referendum
This project contains code to make three different kinds of general election maps which are geographically realistic maps, equally-sized hex maps and interactive maps based on two variables: election results and first party. 

## Installation
For static maps using **matplotlib** and **geopandas**.

For interactive maps using **altair**.

Note that user may not need to install altair module firstly because `pip install altair` has been embedded in the Jupyter Notebook.

## How to use
Run the `Mapping the 2016 EU referendum.ipynb` and all the data needed are stored in `/data`.

## Things you may want to know

**What is constituency?**

The Parliament of United Kingdom has 650 constituencies across the country, and each constituency elects one **Member of Parliament (MP)**. 

**Why hex map?**

It belongs to **contiguous cartograms** that maintain topological aspects as much as possible. For example, if two areas share a common border, it will maintain the border at the expense of shape of areas. The classic hex map is widely used in plotting election results to trade geographic accuracy for equalizing the importance of each constituency in UK.  

**How about election results?**

Election results combined with first party's attitude could be divided into 5 circumstances:
1. Seats won by pro-Brexit parties, where they also received most votes;
2. Seats won by pro-Brexit parties, where pro-referendum parties received more votes;
3. Seats won by pro-referendum parties, where they also received most votes;
4. Seats won by pro-referendum parties, where pro-Brexit parties received more votes;
5. Seats won by pro-referendum Speaker

## Further study

Currently, hex maps are only static and I cannot find a suitable module with python to create an interactive version. Most of them are produced by JavaScript, which needs to be explored later.  

## Data source and useful links

* Estimated leave vote in each constituency:
    
    https://docs.google.com/spreadsheets/d/1wTK5dV2_YjCMsUYlwg0l48uWWf44sKgG8uFVMv5OWlA/edit#gid=893960794

* Seats taken by different parties in the 2017 General Election:
    
    https://commonslibrary.parliament.uk/research-briefings/cbp-7979/

* UK hex map: 
    
    https://odileeds.org/projects/petitions/?241584

* Some much more dedicated versions:
    
    https://ukandeu.ac.uk/five-charts-that-explain-how-leave-won-and-remain-lost/
    
    https://www.theguardian.com/politics/ng-interactive/2016/jun/23/eu-referendum-live-results-and-analysis
