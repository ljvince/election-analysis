# election-analysis -- module 3 challenge
## the purpose of this election audit analysis: 

#### The purpose of this project is using a Python 3 environment coding and function to create and adding more data to complete the require of the election commission, which is "the voter turnout for each county", "the percentage of votes from each county out of the total count", and " the county with the highest turnout".
#### During this project we cloud even visualize more data from our coding. However, the purpose for this challenge is to use python 3 and python function and method to catch data from CSV in order to get the result that we need.

## Results: 



#### 1.pre-work 
<img width="864" alt="Screen Shot 2022-06-13 at 11 48 32 PM" src="https://user-images.githubusercontent.com/106010498/173755800-21a7f0ef-939c-47ad-9ff7-80c0a1eb9600.png">

###### First of all, set environment, index, list and dictionary up.
    I add dependencies and set up the file-loading-path and file-saving-path.
    
    Initialize the total number of votes 
    
    make list of candidate and county
    
    make dictionary of candidate and county 
    
    set up winner candidate, initialize the winner candidate count and percentage
    
    also set up the winner county, initialize the winner county count and percentage

###### this couple set up will help me to finish the rest of project 


#### 2.Total votes

<img width="742" alt="Screen Shot 2022-06-13 at 11 48 51 PM" src="https://user-images.githubusercontent.com/106010498/173757757-68c85e47-2943-4def-bbe1-1a0e70c14f05.png">

###### next, using for look and if then function to create the total votes and catch value for the list and dictionary of candidate and county that i create in the first step.

    Open and reader the file that we need with csv.reader()
    
    in this case using a for loop, to get the total voter with 
    total_voter = total_voter + 1
    
    and using if then function to append the each name on our dataset to our dictionary with
    
    get the each candidate_voter of each name on our dataset 
    
    at the meanwhile, i also need to append the each county and get the each county votes 
    
 <img width="420" alt="Screen Shot 2022-06-14 at 11 48 07 PM" src="https://user-images.githubusercontent.com/106010498/173761168-f567303b-5802-416b-afa5-5005d0b43b84.png">
 
The total voter = 369,711
 
###### in this for loop , i get more value of the index, list and dictionary.
###### I will using the index, list and dictionary to make next result.




#### 3.The number of votes and the percentage of total votes for each county
####                              &
####         Which county had the largest number of votes?

<img width="906" alt="Screen Shot 2022-06-13 at 11 48 59 PM" src="https://user-images.githubusercontent.com/106010498/173762033-0292ef44-df67-41eb-9de5-5111ea34378b.png">

    using for loop to get the county total votes of each county 
    
    and using the function (couty_total / total votes * 100) to make the percentage of each county,
    
    in this loop using if then function to get the value of the largest number of county voter, county name and the percentage.

<img width="246" alt="Screen Shot 2022-06-15 at 12 00 56 AM" src="https://user-images.githubusercontent.com/106010498/173763384-58d4b5c6-5955-43bd-b2ec-90265dfe7317.png">

###### County Votes:
###### Jefferson: 10.5% (38,855)
###### Denver: 82.8% (306,055)
###### Arapahoe: 6.7% (24,801)
###### --------------------------
###### largest county:
###### Largest County Turnout: Denver
###### largest turnout votes: 306,055
###### largest turnout percentage: 82.8%





####               4.The number of votes and the percentage of the total votes each candidate 
####                                                   &
####   Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

<img width="768" alt="Screen Shot 2022-06-13 at 11 49 04 PM" src="https://user-images.githubusercontent.com/106010498/173765082-adf134fa-0d4d-436b-933d-e05493c264d6.png">

    using the same idea of for loop  and if then function, but different index, list and dictionary to get the each candidate's percentage and votes, and also get the winner candidate' name, count and percentage.
    
<img width="275" alt="Screen Shot 2022-06-15 at 12 12 35 AM" src="https://user-images.githubusercontent.com/106010498/173765933-619a0671-cb7e-46d8-8229-95159ce3d260.png">

###### Charles Casper Stockham: 23.0% (85,213)
###### Diana DeGette: 73.8% (272,892)
###### Raymon Anthony Doane: 3.1% (11,606)
###### -------------------------
###### Winner: Diana DeGette
###### Winning Vote Count: 272,892
###### Winning Percentage: 73.8%



## Election-Audit Summary: 
#### This script going through with Python 3 environment, reader from CSV file, it can be used for any election. 
#### please pay attention on blow rule to modify this script in order to using in different commission
###### rule 1: change file's path when you loading and saving a different commission;
###### rule 2: you dataset(.xlsx .cvs or etc.) may have different value on row[1] and row[2], make sure you put this correct :
    candidate_name = row["the row number of your date-set of candidate name"]
    county_name = row["the row number of your date-set of county name"]
###### rule 3: if you need the more result instead of candidate and county for example (area, city, age group，gender).
###### you might want to create a new list and dictionary and flow this coding for loop and if then function to get the result that you wand
    for example
    city_option = []
    city_votes = {}
    lrg_city = ""
    lrg_city_count = 0
    lrg_city_percentage = 0
    (and follow the next for loop and if then function .......)
###### rule 4: If you have any question, please ask an expert or google-fu it.
