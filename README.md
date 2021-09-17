# Election_Analysis

## Project Overview
A Colorado Board of Elections employee gave the following tasks to complete the election audit of a recent local congressional election.

1. How many votes were cast in this congressional election?
2. Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
3. Which county had the largest number of votes?
4. Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
5. Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

## Resources
- Data Source: election_results.csv
- Software: Python 3.9, Visual Studio Code 1.60.1

## Election Audit Results
The analysis of the election show that:
1. There were 369,711 votes cast in the election.
2. The county results were:
    - Jefferson County accounted for 10.5% of the vote and 38,855 number of votes.
    - Denver County accounted for 82.8% of the vote and 306,055 number of votes.
    - Arapahoe County accounted for 6.7% of the vote and 24,801 number of votes.
4. The county with the largest number of votes was:
    - Denver County, which accounted for 82.8% of the vote and 306,055 number of votes.
6. The candidate results were:
    - Charles Casper Stockham received 23.0% of the vote and 85,213 number of votes.
    - Diana DeGette received 73.8% of the vote and 272,892 number of votes.
    - Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.
7. The winner of the election was:
    - Diana DeGette, who received 73.8% of the vote and 272,892 number of votes.

## Election Audit Summary

The election audit was completed by writing python script in Microsoft Visual Studio Code. The biggest advantage of using these sources is that we were able to write a sript that is not project-specific. In other words, we can run the same audit for any election in any county with minimal effort or time because the code would only need a few modifications. For example, with a new CSV file containing election results we could simply:
1.  Verify or update the name of the file in the `file_to_load` line (9).
2.  Verify or update where the candidates & county names are located in the file for the `candidate_name` and the `county_name` lines in the script (47 & 50).

Finally, if the new CSV file contains other election data (e.g. demographic), we could simply replace the `county_name` lines in the code with a new measure (e.g. age, gender, etc.) by updating lines 22 & 50 (to define and locate the new measure) and replace `county_name` with the new defined meaasure in the `for` loop (beginning in 67).  
