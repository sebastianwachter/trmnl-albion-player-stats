# TRMNL Plugin: Albion Player Stats

Display an Albion Online player's stats on your TRMNL.

## How to find a player's ID

Open the following URL (select the you need based on your server's region) in your browser - replace `<name>` with the wanted player's ingame name:

```
https://gameinfo.albiononline.com/api/gameinfo/search?q=<name>      # Americas
https://gameinfo-ams.albiononline.com/api/gameinfo/search?q=<name>  # Asia
https://gameinfo-sgp.albiononline.com/api/gameinfo/search?q=<name>  # Europe
```

This URL will respond with a JSON document based on your request. In the `players` array find the player you were looking for. The object should have a field `Id`: copy its value and paste it into the TRMNL plugin's settings screen.

## Caveats

This plugin polls its data from the `gameinfo` API that the Albion Online website uses for its data as well. I don't know when this data is getting updated. The update cycles seem very random with some of my test users getting updated daily while some others did not receive an update since january. Therefore the data displayed may be outdated.
