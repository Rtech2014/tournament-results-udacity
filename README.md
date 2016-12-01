
# Tournament Results
udacity Full Stack Web Developer Nanodegree Project - Tournament Results

##Files
* tournament.py -- Methods definitions (Swiss-system tournament)
* tournament.sql -- table definitions for the tournament project.
* tournament_test.py -- Test cases for tournament.py

## Instructions
* Open terminal type vagrant up
* Type vagrant ssh to access vagrant VM

##Usage
```bash
vagrant@vagrant-ubuntu-trusty-32:/vagrant/tournament$ psql

vagrant=> CREATE DATABASE tournament;
CREATE DATABASE
vagrant=> \q
```
Run SQL schema
```bash
vagrant@vagrant-ubuntu-trusty-32:/vagrant/tournament$ psql tournament < tournament.sql
```
run test python file
```bash
vagrant@vagrant-ubuntu-trusty-32:/vagrant/tournament$ python tournament_test.py
1. countPlayers() returns 0 after initial deletePlayers() execution.
2. countPlayers() returns 1 after one player is registered.
3. countPlayers() returns 2 after two players are registered.
4. countPlayers() returns zero after registered players are deleted.
5. Player records successfully deleted.
6. Newly registered players appear in the standings with no matches.
7. After a match, players have updated standings.
8. After match deletion, player standings are properly reset.
9. Matches are properly deleted.
10. After one match, players with one win are properly paired.
Success!  All tests pass!
```
