World Cup SQL Project
This project is a SQL-based implementation for managing World Cup tournament data.

Overview
The World Cup SQL Project aims to organize and manage data related to the FIFA World Cup tournaments. It includes schema definitions, data insertion scripts, and SQL queries for interacting with tournament information.

Features
Database Schema: Defines tables for managing information about teams, games, and tournament details.

Data Insertion Scripts: Provides scripts for populating the database with teams, game results, and tournament information.

Query Examples: Includes SQL queries for retrieving tournament statistics, team performance, and match details.

Schema
The project includes the following tables:

Teams: Contains team information such as team_id and team name.

Games: Stores details about tournament games, including match results, participating teams, and game-specific details.

Usage
Setting Up the Database
Schema Creation: Execute the SQL script to create the necessary tables and define relationships.

Data Insertion: Utilize the provided scripts to insert teams' information and game results into the database.

Querying the Database
Execute SQL queries to retrieve information:

sql
Copy code
-- Retrieve the list of teams participating in the 2018 World Cup
SELECT name FROM teams WHERE team_id IN (
  SELECT winner_id FROM games WHERE year = 2018
);
Getting Started
To start using the World Cup SQL Project:

Clone the repository to your local machine.
Create a PostgreSQL database and execute the schema script to set up the tables.
Run the data insertion scripts to populate the database with tournament data.
Use SQL queries to interact with and retrieve information from the database.
Contributions
Contributions, suggestions, and feedback are welcome! If you have enhancements, bug fixes, or new ideas for queries, feel free to open issues or submit pull requests.
