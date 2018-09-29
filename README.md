# Profit-Trailer-Settings

Version 5.2 is the most stable.
In comments, different adjustments are mentioned even if the default configuration does the job well
Currently, I use this configuration with PTDefender to sell my different bags

## Infos
This config has been changed from a 5min to 15min timeframe

15min is short, so you have to be ready to sell quickly.

If the bot bought a little too high and the price goes down a little, you have to be able to buy back a little lower to be sure to have a little margin to sell later.

**Indicateur:**
- La configuration officiel de PT "Mont et Carlo"

**Change Indicator file**
- Timeframe swtich 5 to 15min

**Change (in pairs and DCA file):** (After backtesting)
- Remove price_*  trigger on main currency
- Remove min and max change percentage
- Update DEFAULT_trailing_buy 0.01 to 0.7
- Update DEFAULT_DCA_trailing_buy 0.01 to 0.7
- Update DEFAULT_trailing_profit 0.25 to 0.1
- Update DEFAULT_A_sell_value (GAIN) 1.25% to 0.15
- In Bull market, Add DEFAULT_B_sell_strategy = STOCHRSICROSS
- In Bull market, Add DEFAULT_B_sell_value = -0.03

**In DCA**
- All Trigger
- Add DCA_max_trading_pairs
- Update Sell strategy


## Community Configs list

[Move to a dedicated git repository](https://github.com/But4ler/Profit-Trailer-Community-Settings)

## PT Remember 

Reset data test:
- http://localhost:8081/settings/test/reset

Disable SOM - SOMO
- /settings/overrideSellOnlyMode?enabled=false  (to disable and maintain disabled SOM)
- /settings/overrideSellOnlyMode?enabled=true (to activate and maintain activated SOM)
- /settings/overrideSellOnlyMode  normal - the btc_rise, btc_drop parameters then work again.)
- /settings/overrideSellOnlyMode?type=&enabled=false  disable SOM