# England (and Wales) - English Premier League

## What's `football.db`?

A free open public domain football database & schema
for use in any (programming) language (e.g. uses datasets in plain text).
More [`football.db` Project Site »](http://openfootball.github.io)


## Intro

Free open public domain football data for England (and Wales).
National football club leagues include:

| Level |                               |           |
| ----: | ----------------------------- | --------- |
|     I | English Premier League        | 20 Clubs  |
|    II | English Championship          | 24 Clubs  |
|   III | English League One            | 24 Clubs  |
|    IV | English League Two            | 24 Clubs  |


Notes:

- Starting with the 2004/05 season the Football League's Division 1, Division 2 and Division 3 changed to Championship, League One and League Two.



Example:

```
= English Premier League

Matchday 1

[Sat Aug/16]
  Manchester United    1-2  Swansea City
  Leicester City       2-2  Everton FC
  Queens Park Rangers  0-1  Hull City
  Stoke City           0-1  Aston Villa
  West Bromwich Albion 2-2  Sunderland AFC
  West Ham United      0-1  Tottenham Hotspur
  Arsenal FC           2-1  Crystal Palace
[Sun Aug/17]
  Liverpool FC         2-1  Southampton FC
  Newcastle United     0-2  Manchester City
[Mon Aug/18]
  Burnley FC           1-3  Chelsea FC

...
```

```
= Arsenal

 1  Wojciech Szczęsny (POL)      GK  2007-
13  David Ospina (COL)           GK  2014-
26  Damián Martinez (ARG)        GK  2010-

 2  Mathieu Debuchy (FRA)        DF  2014-
 3  Kieran Gibbs                 DF  2007-
 4 (vc) Per Mertesacker (GER)    DF  2011-
 6  Laurent Koscielny (FRA)      DF  2010-
18  Nacho Monreal (ESP)          DF  2013-
21  Calum Chambers               DF  2014-

 7  Tomáš Rosický (CZE)          MF  2006-
 8 (c) Mikel Arteta (ESP)        MF  2011-
10  Jack Wilshere                MF  2008-
11  Mesut Özil (GER)             MF  2013-
15  Alex Oxlade-Chamberlain      MF  2011-
16  Aaron Ramsey (WAL)           MF  2008-
19  Santi Cazorla (ESP)          MF  2012-
20  Mathieu Flamini (FRA)        MF  2013-
24  Abou Diaby (FRA)             MF  2006-
34  Francis Coquelin (FRA)       MF  2008-
35  Gedion Zelalem (GER)         MF  2013-

 9  Lukas Podolski (GER)         FW   2012-
12  Olivier Giroud (FRA)         FW   2012-
14  Theo Walcott                 FW   2006-
17  Alexis Sánchez (CHI)         FW   2014-
22  Yaya Sanogo (FRA)            FW   2013-
23  Danny Welbeck                FW   2014-
27  Serge Gnabry (GER)           FW   2012-
28  Joel Campbell (CRC)          FW   2011-
```


## Build Your Own `england.db` Copy

Use the `sportdb` command line tool to build your own `england.db` copy
from the datasets in plain text. 

Note:  The English Premier League includes teams from Wales
(e.g. Swansea City or Cardiff City).


### Alternative I - Use the Quick Starter Templates

Use the quick starter datafile templates to start from scratch. Examples:

Build the database for all English (incl. Welsh) clubs, leagues and seasons:

    $ sportdb new eng

Build the database for the 2020/21 season:

    $ sportdb new eng2020-21

[More »](https://github.com/openfootball/quick-starter)



### Alternative II - Do-It-Yourself (DIY) - Downlad and Unpack Zip Archive or Git Clone

Download and unpack the zip archive with the datasets or if you have git installed use the `git clone` command to
get a local copy.

Try in your working folder (that is, `/england`):

```
$ sportdb build
$ sportdb --verbose build     # or for more (verbose) details incl. debug info
```

This will

- setup a new single-file SQLite database e.g. `./sport.db` and
- read in all datasets in plain text (`.txt`)

That's it.


### Alternative III  - Read / Load Match files with `football-to-sqlite` / `football-to-psql`

Run the `football-to-sqlite` tool against match files in the Football.TXT format like so:

```
$ football-to-sqlite england.db 2020-21/1-premierleague.txt
```

or pass in more than one match file (e.g. different leagues or more seasons):

```
$ football-to-sqlite england.db 2020-21/1-premierleague.txt \
                                2020-21/2-championship.txt  \
                                2020-21/3-league1.txt       \
                                2020-21/4-league2.txt       \
                                2020-21/5-nationalleague.txt

# -or-

$ football-to-sqlite premier.db 2020-21/1-premierleague.txt  \
                                2019-20/1-premierleague.txt  \
                                2018-19/1-premierleague.txt  \
                                2017-18/1-premierleague.txt  \
                                2016-17/1-premierleague.txt
```

Note: If the single-file SQLite database (and its tables, views & indices) do not (yet) exist, 
they get auto-created on the first run.

[More »](https://github.com/sportdb/football.db/tree/master/football-to-sqlite)




## License

![](https://publicdomainworks.github.io/buttons/zero88x31.png)

The football.db schema, data and scripts are dedicated to the public domain. Use it as you please with no restrictions whatsoever.


## Questions? Comments?

Send them along to the
[Open Sports & Friends Forum/Mailing List](http://groups.google.com/group/opensport).
Thanks!
