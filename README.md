# England

## What's `football.db`?

A free open public domain football (soccer) database & schema
for use in any (programming) language
(e.g. uses plain text fixtures/data sets).
More [`football.db` Project Site »](http://openfootball.github.io)

## Intro

Free open public domain football data for England / Europe. Events include:

| Level |                                |            |
| ----- | ------------------------------ | ---------- |
| I     |  Premier League                |  20 Clubs  |


Example:

~~~
### Premier League

chelsea,     Chelsea|Chelsea FC|FC Chelsea,             CHE, city:london
manunited,   Manchester United|Man Utd|Manchester U.,   MUN, city:manchester
...
~~~

~~~
### Premier League 2013/14

Matchday 1

Sa, 17.08.2013   Chelsea FC       Hull City
Sa, 17.08.2013   Manchester City  Newcastle United
...
~~~


## Build Your Own `football.db` Copy

To build your own `football.db` copy from the plain text fixtures
use the sportdb command line tool. Example:

Step 1:  Get a copy of the `world.db` fixtures

    $ git clone git://github.com/geraldb/world.db.git

Step 2:  Get a copy the `en-england` fixtures

    $ git clone git://github.com/openfootball/en-england.git

Step 3:  Let's build the `football.db`

    $ sportdb setup --include ./en-england --worldinclude ./world.db

That's it. For more
see the [`sportdb` command line tool project](https://github.com/geraldb/sport.db.ruby).


## Links


### Web Admin App

Try the `football.db` Web Admin app running on Heroku
[`footballdb.herokuapp.com/en`](http://footballdb.herokuapp.com/en).


### Premier League

Official Site - [`www.premierleague.com`](http://www.premierleague.com)

- 20 Teams
- 380 Matches

#### Wikipedia

- [Premier_League](http://en.wikipedia.org/wiki/Premier_League)
- [2013–14_Premier_League](http://en.wikipedia.org/wiki/2013–14_Premier_League)
- [2012–13_Premier_League](http://en.wikipedia.org/wiki/2012–13_Premier_League)



## Questions? Comments?

Send them along to the
[Open Sports & Friends Forum/Mailing List](http://groups.google.com/group/opensport).
Thanks!
