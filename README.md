# Election-Analysis
## Overview of Election Audit:
Purpose of this audit is to get a summary of the election results.

Mainly to get the following:

    - Total votes.
    
    - Votes per county.
    
    - County with the largest vote turnout.
    
    - Count of votes for each candidate that took part in the election.
    
    - Percentage of votes compared to the total votes for each of the candidates.
    
    - Finally, get the winning canditate name, vote count and percentage.
    
The screen shot below displays the results that were saved in a text file using python code:

![Election Results Summary](/analysis/Results.PNG)

## Election-Audit Results:

  - Total number of votes casted were: 369,711
  
  This number is obtained by having a variable in the code that adds one to itself each time code loops through a row of the data: total_votes = total_votes + 1
  
  - There are 3 counties. Below is the number of votes per county and the percentage of total votes for each county in the precinct:
  
  Jefferson: 10.5% (38,855)
  
  Denver: 82.8% (306,055)
  
  Arapahoe: 6.7% (24,801)
  
  - Based on the analysis Denver had the largest number of votes.
  
  - There are 3 canditates. Below is a summary of total votes each candidate received and the percentage of total votes.
  
  Charles Casper Stockham: 23.0% (85,213)
  
  Diana DeGette: 73.8% (272,892)
  
  Raymon Anthony Doane: 3.1% (11,606)
  
  - Based on the above analysis the winning candidate was Diana DeGette with a total of 272,892 votes and 73.8% of the total votes.
  
  ## Election Audit Summary
  The script can be used for any election that has more that 3 candidates and/or more than 3 county. 
  
  The way the code is written it loops, it will work for as many candidates and as many county. For loops are used, as well as lists and dictionaries, which means that both of them can have more that 3 items added to them.
  
  In the event the county name or candidate name is not in the same column as the ones in the excel files. The user can change the code by simply changing the index of the column in the following lines: 
  
    candidate_name = row[2] - in this case candidate name is in the 3rd column.
   
    county_name = row[1] - in this case county name is in the 2nd column.
    
  In order to simplify the code, it can be modified so that all the print statements are placed in the same section for both candidate and county summary.
  
  The code can also be modified by having a disctionary that stores both the candidate names and count as well as county names and count. The code would then need to loop through the dictionary to provide the output summary of the winning candidate and the county with the most votes. This will eliminate some of the for loops as well as if statements.
  
  
  
  
  
