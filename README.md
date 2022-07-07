# Playnite extensions features
An overview of features for Playnite extensions

## General features

|                     | Uninstalled games | Official metadata | Play time import | Installation | 
| ------------------- | ----------------- | ----------------- | ---------------- | ------------ | 
| Amazon              | •                 |                   |                  | •            | 
| Battle.net          | •                 | •                 |                  | •            |
| Battlestate Games   | ?                 | ?                 | ?                | ?            |
| Epic                | •                 | •                 | •                | •            |
| Fanatical           | ?                 | ?                 |                  | ?            |
| GamersGate          | •[^d]             |                   |                  | •[^c]        |
| GOG                 | •                 | •                 | •                | •            |
| Groupees            | •[^d]             |                   |                  | •[^c]        |
| Humble              | •                 |                   |                  | •            |
| Humble Keys         | ?                 | ?                 |                  | ?            |
| Indiegala           | ?                 | ?                 |                  | ?            |
| itch.io             | •                 | •                 |                  | •            |
| JAST USA            | ?                 | ?                 |                  | ?            |
| Legacy Games        | •[^a]             |                   |                  |              |
| Microsoft XCloud    | ?                 | ?                 | ?                | ?            |
| MultiMC             | ?                 | ?                 | ?                | ?            |
| Nintendo            | ?                 | ?                 |                  | ?            |
| NVIDIA GeForce Now  | ?                 | ?                 | ?                | ?            |
| Oculus              | •[^a][^b]         | •                 |                  |              |
| Origin              | •[^e]             | •[^e]             | •[^e]            | •[^e]        |
| Playstation         | •                 | •                 |                  |              |
| Riot Games          | ?                 | ?                 | ?                | ?            |
| Rockstar Games      | ?                 | ?                 | ?                | ?            |
| Space Station 13    | ?                 | ?                 | ?                | ?            |
| Steam               | •                 | •                 | •                | •            | 
| Uplay               | •                 | •                 |                  | •            | 
| Xbox                | •                 |                   | •                | •            |

* Import of installed games is always supported
* Play time is always tracked when launched through Playnite

[^a]: Reads local client files. Requires you to start up the client to add new games.
[^b]: Only Oculus Rift titles. This excludes native Oculus Quest (2) or Oculus Go titles.
[^c]: Manual installation only: you are pointed to a download URL and can link the game to an installation folder once you've installed it.
[^d]: Only the ones downloadable from the website (so excluding keys for Steam or other services)
[^e]: No support for the EA Desktop client (also known simply as EA).

## Library metadata support

|             | Icon  | Background image | Description | User ratings | 
| ----------- | ----  | ---------------- | ----------- | ------------ |
| Battle.net  | •     | •                |             |              | 
| Epic        | •[^1] | •                | •           |              | 
| GOG         | •     | •                | •           | •            | 
| Humble      | •[^3] |                  |             |              | 
| itch.io     |       | •                | •           | •            | 
| Oculus      | •[^4] | •                | •           | •            |
| Origin      | •[^1] | •                | •           |              |
| Playstation | ?     | ?                | ?           | ?            |
| Steam       | •     | •                | •           | •            | 
| Uplay       | •[^2] | •[^2]            |             |              | 
| Xbox        | •[^1] |                  |             |              | 

[^1]: Only if game is installed
[^2]: Only if import of uninstalled games is enabled
[^3]: Trove games won't have icon assigned
[^4]: Only on initial import
