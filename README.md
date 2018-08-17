# Profit-Trailer-Settings

Collection of different strategies for Profit Trailer 2.0.3.
Each time we will try to put the results obtained as well as the test period


## Configs list in pt_community_config folder

Timeframe | Autor Name | PTM Ready | Source | Explication |
:------------ | :------------- | :------------- | :------------- | :------------- |
| 5min | ASH | yes (v2.2) | [Discord PT FR](https://discordapp.com/channels/400170732648398849/400664557099679756) | Good on bull market
| 5min | Bit4boy | Yes Ash adaptation | [Discord PT FR](https://discordapp.com/channels/400170732648398849/400664557099679756) | Adding PTM settings to the ASH config
| 5min | Nomandog | - | Fork ASH | 
| 5min | Znuf | - | USA/ASIA | 
| 5min | nAffies | - | USA/ASIA | 
| 5min | PT-Officiel | - | [PT Discord](https://discord.gg/K9a37Vh) | Go pt-dedefault-settings channel
| 30min | Crypto Zen | Yes (stable) | [Youtube](https://www.youtube.com/watch?v=2GXXXZzIx0c) |
| 60min | Crypto Zen | No (testing) | [Youtube](https://www.youtube.com/watch?v=2GXXXZzIx0c) |
| 60min | Team (very serious) | Think for | [github](https://github.com/stevenshizzleh/the-north-star) | Search for entry points according to the situation of each pair 

## PT Profit Type Compartif
[Google Sheets PT_profit_type_default_grow_shrink](https://drive.google.com/open?id=1M-iD7QbuNuhVM1cDgBiJF5G81TH3YEIyLdivE1wa7Ns)

## PT Remember 

Reset data test:
- http://localhost:8081/settings/test/reset

Disable SOM - SOMO
- /settings/overrideSellOnlyMode?enabled=false  (to disable and maintain disabled SOM)
- /settings/overrideSellOnlyMode?enabled=true (to activate and maintain activated SOM)
- /settings/overrideSellOnlyMode  normal - the btc_rise, btc_drop parameters then work again.)
- /settings/overrideSellOnlyMode?type=&enabled=false  disable SOM