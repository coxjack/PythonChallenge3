## Election Analysis
Challenge 3 for Butler Data Science

## 1. Overview of Election Audit
### 
* The goal of this module is to assist a Colorado board of elections with their audit of a congressional precinct. In our audit we were asked to tabulate the following:
	1. Total number of votes cast
	2. A complete list of candidates who received votes
	3. Total number of votes each candidate received
	4. Percentage of votes each candidate won
	5. The winner of the election based on popular vote

## 2. Election Audit Results
### 
* How many votes were cast in this congressional election?
	- Total Votes: 369,711
* Breakdown of the number of votes and the percentage of total votes for each county in the precinct
	- County Votes:
	Jefferson: 10.5% (38,855);
	Denver: 82.8% (306,055);
	Arapahoe: 6.7% (24,801)
* Which county had the largest number of votes?
	- Largest County Turnout: Denver
* Breakdown of the number of votes and the percentage of the total votes each candidate received
	- Candidate Votes:
	Charles Casper Stockham: 23.0% (85,213);
	Diana DeGette: 73.8% (272,892);
	Raymon Anthony Doane: 3.1% (11,606)
* Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
	- Winning Summary:
	Winner: Diana DeGette;
	Winning Vote Count: 272,892;
	Winning Percentage: 73.8%

## 2. Election Audit Summary
### 
* Applying this script to any election audit is easy. The first thing we would need to do is import from whatever results file we would have. 
	- Add a variable to load a file from a path.
	  - ***Original Script***
	    - file_to_load = os.path.join("Resources", "election_results.csv")
	  - ***Modified Script***
	    - file_to_load = os.path.join("Any_election_results.csv)
* If this was a national election we could instead gather votes by state.
	- Create a list and votes dictionary
	  - ***Original Script***
	    - county_options = []
	    - county_votes = {}
	  - ***Modified Script***
	    - state_options = []
	    - state_votes = {}
