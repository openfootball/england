# England (and Wales) - English Premier League

## What's `football.db`?

A free open public domain football database & schema
for use in any (programming) language (e.g. uses plain text data sets).
More [`football.db` Project Site »](http://openfootball.github.io)


## Intro

Free open public domain football data for England (and Wales).
National football club leagues include:

| Level |                               |           |
| ----: | ----------------------------- | --------- | 
|     I | English Premier League        | 20 Clubs  |


Example:

```
### English Premier League

chelsea,     Chelsea|Chelsea FC|FC Chelsea,             CHE
manunited,   Manchester United|Man Utd|Manchester U.,   MUN
...
```

```
### English Premier League

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
##########################
# Arsenal

1    Wojciech Szczęsny (POL)      GK  2007-
13   David Ospina (COL)           GK  2014-
26   Damián Martinez (ARG)        GK  2010-

2    Mathieu Debuchy (FRA)        DF  2014-
3    Kieran Gibbs                 DF  2007-
4 (vc) Per Mertesacker (GER)      DF  2011-
6    Laurent Koscielny (FRA)      DF  2010-
18   Nacho Monreal (ESP)          DF  2013-
21   Calum Chambers               DF  2014-

7    Tomáš Rosický (CZE)          MF  2006-
8 (c)  Mikel Arteta (ESP)         MF  2011-
10    Jack Wilshere               MF  2008-
11    Mesut Özil (GER)            MF  2013-
15    Alex Oxlade-Chamberlain     MF  2011-
16    Aaron Ramsey (WAL)          MF  2008-
19    Santi Cazorla (ESP)         MF  2012-
20    Mathieu Flamini (FRA)       MF  2013-
24    Abou Diaby (FRA)            MF  2006-
34    Francis Coquelin (FRA)      MF  2008-
35    Gedion Zelalem (GER)        MF  2013-

9     Lukas Podolski (GER)        FW   2012-
12    Olivier Giroud (FRA)        FW   2012-
14    Theo Walcott                FW   2006-
17    Alexis Sánchez (CHI)        FW   2014-
22    Yaya Sanogo (FRA)           FW   2013-
23    Danny Welbeck               FW   2014-
27    Serge Gnabry (GER)          FW   2012-
28    Joel Campbell (CRC)         FW   2011-
```



## Build Your Own `england.db` Copy

Use the `sportdb` command line tool to build your own `england.db` copy
from the plain text data sets. [More »](http://openfootball.github.io/build.html)


Note:  The English Premier League includes teams from Wales
(e.g. Swansea City or Cardiff City).


### Examples

Build the database for all English (incl. Welsh) clubs, leagues and seasons:

    $ sportdb new en

Build the database for the 2015/16 season:

    $ sportdb new en2015-16



## Questions? Comments?

Send them along to the
[Open Sports & Friends Forum/Mailing List](http://groups.google.com/group/opensport).
Thanks!
