# Profit-Trailer - DCA Dilition methode

Source: [YouTube Channel: Patrick Bier](https://www.youtube.com/watch?v=AUP4CsvZpgo)

1) Fill out spreadsheet
2) create sell order for the "expensive" price (D7 and E7)
3) put coin in watchmode 
    * COIN_trading_enabled = false
4) put the buy order on the exchange awaiting fill (B20 and chosen buy price from exchange, hopefully a "dip"!)
5) adjust spreadsheet "new buy price/coin" A23 to actual number from buy order
6) Hotconfig "new coin ave cost" number D23 from spreadsheet as
    * COIN_reset_stored_average = true
    * COIN_bought_price = ###
7) change again to enable trading:
    * COIN_trading_enabled = true
8) After PT sells the newly created bag with shard then set from spreadsheet "Price/Coin" B3 into PT by another Hotconfig 
    * COIN_reset_stored_average = true
    * COIN_bought_price = ###
9) Start again for another round at #1 above…
