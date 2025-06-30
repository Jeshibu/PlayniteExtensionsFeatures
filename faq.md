# Frequently Asked Questions

# Does Playnite replace clients like Steam/Epic/EA/Ubisoft Connect?
No. Playnite only allows you to have a centralized list of games that you can organize and start from one place. Replacing clients has never been part of the aims of the project. You'll still need Steam to download and install Steam games, and the same goes for every other client. The only exception is Indiegala, which allows you to download and install their DRM free games from within Playnite.

# What's the point of the Playstation and Nintendo library plugins? Can I play those games on PC with them?
No, you cannot play those games on PC via those plugins. They are meant for game library management, for example to track which games you already own.

# How do I import playtime?
For library plugins that support it, you can let them dictate the total playtime for your games in Playnite.
Check the `Play time import` column in the table linked below to see which libraries support this.

[***CLICK HERE TO SEE A COMPARISON TABLE FOR WHAT LIBRARY PLUGINS CAN PROVIDE WHAT DATA***](./libraries.md)

1. Go to `main menu > Settings > General` and set `Import playtime of games in library` to `Always`
2. Click `main menu > Update Game Library > Update All` to import your games again so they'll get updated with the correct playtimes

## Steam specific playtime troubleshooting
Make sure your Steam profile is public:
1. Go to your [Steam profile page](https://steamcommunity.com/my/profile)
2. Click `Edit Profile`
3. Click `Privacy Settings`
4. Make sure `My profile` and `Game details` are both set to `Public`
5. Make sure `Always keep my total playtime private even if users can see my game details` is not checked
6. In Playnite, click `main menu > Update Game Library > Update All` to import your games again

Alternatively, set a Steam API key:
1. Go to `main menu > Add-ons > Extension settings > Steam`
2. Check the `Private account` checkbox
3. Click `Get API Key`
4. Once you've gotten your API key, enter it in the `API Key` textbox
5. Click `Save`
6. Click `main menu > Update Game Library > Update All` to import your games again

# I've uninstalled a library plugin, why are my games still there?
Playnite never removes your games automatically (except some extensions under very specific circumstances). You can delete them from your library this way:

1. Select all relevant games as you would in Windows Explorer with ctrl- or shift-clicking, or by pressing ctrl+A to select every game
2. Press `DEL` on your keyboard or right-click and select `Remove`

# My games are not importing
1. Check that your library plugin is configured and authenticated correctly via `main menu > Add-ons > Extension settings > Libraries` - make sure especially that uninstalled games are set to import if that setting is available
2. Make sure that you're logged into the right account with the library plugin
3. Check if the game is present in `main menu > Settings > Import exclusion list`

# My games are gone
1. **Filtered**: Does it say "Filter enabled" in the top bar? If so, right click that text, or enable the filter panel with `ctrl+G` and click `Clear filters` at the top
2. **Hidden**: In the filter panel, check the `Hidden` checkbox

# Can I change my games' Library field value?
No. The library field is what Playnite uses to connect games to their library plugin. Editing it manually would lead to technical issues.
There is an alternative: use the Source field. You can create and edit this arbitrarily, and it's normally filled by library plugins too.

# Can I sort games manually by dragging and dropping?
No. You can instead edit the games' `sorting name` field: `right click the game > Edit`.

# My games are missing covers or other data! (or: What is metadata?)
Metadata is all the data Playnite has on a game. Things like cover image, description, developers, release date, etc.
To get metadata for games automatically, there are several metadata provider plugins available in Playnite. The steps below will lead you through installing, configuring, and using them.

## Installing metadata provider plugins
To decide which metadata providers you want to use, you can reference the table linked below to see what data you can expect from each plugin.

[***CLICK HERE TO SEE A COMPARISON TABLE FOR WHAT METADATA PLUGINS CAN PROVIDE WHAT DATA***](./metadata.md)

1. Go to `main menu > Add-ons > Browse > Metadata Sources`
2. For each of the plugins you want, select them and click `Install` on the right
3. Click `Save`
4. Click `Yes` to restart Playnite

## Configuring individual metadata provider plugins
Now that you've installed your metadata provider plugins, you'll want to make sure that they're configured correctly. Some, like SteamGridDB or Giant Bomb, will not work without an API key for example.

1. Go to `main menu > Add-ons > Extension settings > Metadata Sources`
2. Go through each of the plugins listed there to make sure any required API keys are entered, and optionally that other settings are to your liking
3. Click `Save`

## Configuring metadata provider plugin use and priority
When games get imported, they'll automatically get data from metadata providers (unless you uncheck `Settings > General > Download metadata after importing games`). You can configure what metadata providers provide what data, and in what order of preference.

1. Go to `main menu > Settings > Metadata`
2. For each of the dropdowns, enable and reorder the metadata providers to your liking

The order here matters, because the first metadata provider in the list to find data will supply it to that field.
There is currently no automated merging possible. If you want merged collection fields, you'll have to do it manually per game.

## Starting automatic metadata collection manually
If you want to collect metadata for one or many games automatically, press `ctrl+D` or `main menu > Library > Download metadata` and follow the on-screen instructions.

## Manually getting metadata from a single provider for a single game
If you want to correct some metadata by pulling from a specific provider:

1. Right click your game
2. Click `Edit`
3. At the bottom left of your "Edit Game Details" window, there will be a button that says `Download Metadata` - click it
4. Click the metadata provider you want data from
5. You'll likely get a search window that lets you pick the right game - double click the right game
6. You might get one or more windows to let you pick which image to use for an icon/cover/background
7. If data was found for fields that already have data, you'll get a comparison window that lets you pick which metadata to use
8. Click `Select` in the data comparison window
9. All the new data will be marked with an exclamation mark in the "Edit Game Details" window
10. If you decide any of that new data is bad, you can decide not to save the changes to that field by clicking the checkbox to the left of it
11. Click `Save` in the "Edit Game Details" window
