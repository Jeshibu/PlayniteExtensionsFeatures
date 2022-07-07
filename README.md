# Playnite extensions features
An overview of features for Playnite library extensions. Library extensions allow you to import games from other services/websites/clients/consoles.

* You will still need the original game clients like Steam or Ubisoft Connect or Origin.
* Playnite does not make any games available for free, nor does it support piracy.
* The console library extensions (Nintendo, Playstation) do not enable you to play their games on PC. These are here solely for organization and management. The exception is Xbox, which while it does not enable you to play Xbox-console only games, does have many games available for PC.

## Contributing
This list is currently not yet complete, and fields marked with a question mark (?) I have not yet had the time to research or confirm. Feel free to contribute by filling those in, or adding columns or rows to the tables, or fixing typos in a pull request.

## General features

|                    | Not installed games | Official metadata | Play time import | Installation |
| ------------------ | ------------------- | ----------------- | ---------------- | ------------ |
| Amazon             | •                   |                   |                  | •            |
| Battle.net         | •                   | •                 |                  | •            |
| Battlestate Games  | ?                   | ?                 | ?                | ?            |
| Epic               | •                   | •                 | •                | •            |
| Fanatical          | ?                   | ?                 |                  |              |
| GamersGate         | •[^d]               |                   |                  | •[^c]        |
| GOG                | •                   | •                 | •                | •            |
| Groupees           | •[^d]               |                   |                  | •[^c]        |
| Humble             | •                   |                   |                  | •            |
| Humble Keys        | ?                   | ?                 |                  |              |
| Indiegala          | ?                   | •                 |                  | ?            |
| itch.io            | •                   | •                 |                  | •            |
| JAST USA           | ?                   | ?                 |                  | ?            |
| Legacy Games       | •[^a]               |                   |                  |              |
| Microsoft XCloud   | •                   | ?                 | ?                | ?            |
| MultiMC            | ?                   | ?                 | ?                | ?            |
| Nintendo           | •[^f]               |                   |                  |              |
| NVIDIA GeForce Now | ?                   | ?                 | ?                | ?            |
| Oculus             | •[^a][^b]           | •                 |                  |              |
| Origin             | •[^e]               | •[^e]             | •[^e]            | •[^e]        |
| Playstation        | •                   | •                 |                  |              |
| Riot Games         | ?                   | ?                 | ?                | ?            |
| Rockstar Games     | ?                   | ?                 | ?                | ?            |
| Space Station 13   | ?                   | ?                 | ?                | ?            |
| Steam              | •                   | •                 | •                | •            |
| Ubisoft Connect    | •                   | •                 |                  | •            |
| Xbox               | •                   |                   | •                | •            |

* Import of installed games is always supported
* Play time is always tracked when launched through Playnite

[^a]: Reads local client files. Requires you to start up the client to add new games.
[^b]: Only Oculus Rift titles. This excludes native Oculus Quest (2) or Oculus Go titles.
[^c]: Manual installation only: you are pointed to a download URL and can link the game to an installation folder once you've installed it.
[^d]: Only the games downloadable from the website (so excluding keys for Steam or other services)
[^e]: No support for the EA Desktop client (also known simply as EA).
[^f]: Only games purchased in the last 2 years, via https://ec.nintendo.com/my/transactions/1

## Library metadata support
The library extensions that have "Official metadata" in the table above can download metadata for the games from its own library. This is visible as a metadata provider named "Official Store" when applicable, in the mass metadata import window (ctrl+D) as well as at the bottom left of the game edit window.

|                 | Icon  | Cover      | Background image | Description | User ratings |
| --------------- | ----- | ---------- | ---------------- | ----------- | ------------ |
| Battle.net      | •     | vert       | •                |             |              |
| Epic            | •[^1] | vert       | •                | •           |              |
| GOG             | •     | vert       | •                | •           | •            |
| Humble          | •[^3] |            |                  |             |              |
| IndieGala       |       | hor        | •                | •           |              |
| itch.io         |       | hor        | •                | •           | •            |
| Oculus          | •[^4] | square[^4] | •                | •           | •            |
| Origin          | •[^1] | vert       | •                | •           |              |
| Playstation[^5] | ?     | square     | ?                | ?           | ?            |
| Steam[^5]       | •     | hor,vert   | •                | •           | •            |
| Ubisoft Connect | •[^2] | vert[^6]   | •[^2]            |             |              |
| Xbox            | •[^1] |            |                  |             |              |

[^1]: Only if game is installed
[^2]: Only if import of uninstalled games is enabled
[^3]: Trove games won't have icon assigned
[^4]: Only on initial import
[^5]: Also available as a separate metadata source extension (for games that weren't imported by these library extensions)
[^6]: 240x280, which is barely vertical and almost square