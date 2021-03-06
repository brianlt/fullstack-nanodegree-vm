# Tournament Results
This repository uses postgresql to manage a Swiss tournament style tracking.

## Installation

Clone this repository using:

`git clone https://github.com/Seananigans/fullstack-nanodegree-vm.git`


## Usage

1. First change into the tournament directory:

	`~/fullstack-nanodegree-vm/vagrant/tournament`

2. Second create the database by starting up posgresql and executing the following command:

	`CREATE DATABASE tournament;`

3. Set up the tables in the database and tables by running:

	`psql -f tournament.sql`

4. Then test the program using:

	`python tournament_test.py`

5. The test program should verify that the below functions are working properly.

	* deleteMatches()
		- Clear all scores from a tournament to restart the tournament with the same players.

	* deletePlayers()
		- Clear the tournament to start with new players.

	* registerPlayer(player_name)
		- Register a player in the tournament.

	* countPlayers()
		- Count the number of players in the tournament.

	* playerStandings()
		- Get the player standings.

	* reportMatch(id_of_winner, id_of_loser)
		- Update the tournament results by reporting the winner and loser of a match.

	* swissPairings()
		- Get the pairings for the next matches.