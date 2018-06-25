================ INTRODUCING ================
ProfitTrailer Default Settings by @CryptoCoyn
    Version 2.0.13 19th June, 2018
    Copyright (c) 2018, ProfitTrailer.com
=============================================

Please Note:

All investment carries risk and you must take ownership of your day
trading investments. Trading in cryptocurrency carries a high level
of risk, and is not suitable for all investors.  The possibility 
exists that you could lose some or all of your investment capital and
therefore you should not invest money that you cannot afford to lose.

No representation is being made that any trading methodology will or
is likely to achieve profits similar to those described here. Also
past performance of any trading methodology is not necessarily
indicative or a guarantee of future results.

These settings do not constitute financial advice. We do not and
will not provide financial advice. Any information presented is
strictly for educational purposes only and should not be construed
as investment advice or an offer to buy or sell securities.

You should be aware of all risks associated with investing / trading
in cryptocurrency and should seek professional financial advice from
an independent,competent, licensed accountant or financial advisor.

Description:

These settings will work for all versions of ProfitTrailer 2.x 

Usage instructions:

Within the settings you will find the following sections:
    Setting sections are marked       -----------------------------
    Market Sentiment is marked        #### BEAR MARKET SETTING ####
    Exchange settings are marked         ****Exchange Name****
    Trading Market settings are marked    ----Market Name----
    Strategy section is marked        *****************************

Strategies Available:
    All Markets  - El Dorado - The Market Maker
    All Markets  - El Toro - Run With The Bulls
    All Markets  - Old Faithful - The Gift That Keeps On Giving
    Bear Market  - FrankenStrategy - Its Alive, Its Alive!!!
    Bear Market  - Double Cross - Trade the trend
    Bull Market  - Jobbing The Market - Intraday Trading

You can always see the latest strategy in action here:
    https://demo.profittrailer.com


Bug Fixes:
*   El Toro strategy Trailing Buy and Trailing Profit values fixed;
*   Comments in application.properties updated to reflect Version 2.x changes;
*   Use of EMASPREAD and EMACROSS removed only EMACROSS required as they both return spread value;
*   In DCA DEFAULT_DCA_buy_min_change_percentage and DEFAULT_DCA_buy_max_change_percentage setting
    names corrected.

    Note: Thank you to the ProfitTrailer community for assisting in debugging these settings

New Features:
* Added new "El Dorado" Strategy for use in all market conditions;
* El Dorado Strategy backtested in TradingView;
* Tested these settings against ProfitTrailer versions: 2.0.9, 2.0.10, 2.0.11, 2.0.12 and 2.0.13;
* Also tested these settings against the 2.1.x Beta versions currently in development; and
* Both live and paper trading bots were used to test the settings.

Notes:
* Settings support all markets that ProfitTrailer supports, ETH, USDT, etc. Just comment out 
the BTC settings provided and uncomment the ETH settings see usage directions at top of each 
file or above;
* DCA settings will purchase the same number of coins per DCA level as the first purchase does;
* DCA triggers at -10 and has a limit of 5 buys;
* A DCA calculator has been configured for these settings and is provided in the #pt-default-settings 
channel to assist you get your maximum number of trading pairs and initial cost settings correct; and
* We recommend having a 50/50 split of your trading budget so 50% for normal day to day trading 
(buying pairs, normal DCA) and a 50% reserve for DCA when Bitcoin price drops significantly as it
has done in the recent past. The DCA calculator is configured to do this 50/50 split for you by balancing
out your max trading pairs and initial cost settings to allow for it.

To Install these settings:

    Before you start download and install the following text editor:
    https://code.visualstudio.com/

    The instructions provided below assume you will be using this text editor.

    NOTE: Do note try and use Word, Wordpad or Notepad on Windows they will insert incorrect 
    characters into your files and corrupt them. Notepad++ that is also suitable for
    editing these files and is available from here: https://notepad-plus-plus.org/
    
    1. Ensure you have installed ProfitTrailer and have it working first, to do this:
        a. Download the latest version of ProfitTrailer here: 
            https://github.com/taniman/profit-trailer/releases

        b. Note your use of ProfitTrailer is subject to and indicates your acceptance of the 
        terms of service provided here: https://profittrailer.com/tos/

        c. Install profit trailer and get it running with the settings that come with it as per 
        these instructions: https://wiki.profittrailer.com/doku.php?id=instructions or if you are
        an existing version 1 customer and looking to upgrade to ProfitTrailer 2.x then follow 
        these instructions: https://wiki.profittrailer.com/doku.php?id=upgrade_instructions2

        Open your web browser and enter the following URL to make sure the Profit Trailer is working:
        http://localhost:8081/

        Note: If you have trouble here make sure port 8081 is free and not blocked by your firewall.
        If you do have trouble try changing the port number in the applications.properties file and
        try again replacing the port number in the URL.

        If not contact the support team via the #support channel on the ProfitTrailer community discord.

    2.  Now stop ProfitTrailer and do a backup of your ProfitTrailer folder by copying and pasting it to
        another folder. 

        Note: You will need this backup copy in one of the steps below so do not skip doing the 
        backup;

    3.  Unzip the ProfitTrailer Default Settings into a separate folder on your PC;

    4.  Copy the new application.properties file supplied with these settings to your ProfitTrailer
        folder overwriting the old file.

    5.  Open up your ProfitTrailer directory using the text editor by selecting the File menu, Open option.
        Now open the ProfitTrailer directory by clicking on it. 
    
        You should see the following files:
        - initialization/DCA.Properties;
        - initialization/INDICATORS.Properties;
        - initialization/PAIRS.Properties;
        - applications.properties *;

        The file marked with an * above is the one you need to edit.

        Now open the application.properties file by click on it from the list of files on the left. 
        
        Note: the initialization files are only used on the very first time that ProfitTrailer is installed
        and executed. We are assuming you have already done that as per Step 1.

    6.  Using another instance of the text editor open up the ProfitTrailer Backup directory you created. 
        You can do this by selecting the File menu, New Window option. Now open the ProfitTrailer Backup 
        directory by clicking on it. 
    
        Now open the application.properties file by clicking on it from the list of files on the left. 

        At this point you should now have both the new Application.properties file and the backup 
        application.properties files open side by side for comparison.
    
    7.  Copy and paste from your existing application.properties file:
        
        - your ProfitTrailer License Key;
        - your exchange API Keys;
        - your API Key secrets;
        - your notifications settings;

        And put these into the new application.properties file supplied with these settings. 
    
    8.  Now save the new application.properties file and close both text editors.
    
    9.  Use the DCA calculator provided on the ProfitTrailer discord in the #pt-default-settings channel 
        to obtain max trading pairs and initial cost settings suitable for your trading budget.

    10. Start ProfitTrailer and use the web based GUI to access the Indicators configuration screen.

    11. Copy and Paste the contents of the Indicators.properties file supplied with these settings into 
        the Indicators configuration screen replacing its contents and save it

    12. Copy and Paste the contents of the DCA.properties file supplied into the DCA configuration screen
        replacing its contents and save it

    13. Copy and Paste the contents of your edited Pairs.properties file into the Pairs configuration screen 
        replacing its contents but DO NOT SAVE it yet.

        Now using the web based GUI Pairs configuration screen:
        a. uncomment the Exchange, Market and Strategy settings you wish to use;
        b. Set your starting balance as per the current balance shown in your Exchange account;
        c. Set your max trading pairs and initial cost settings as per the DCA calculator recommendations;
        d. Make sure your min buy volume is suitable for the exchange and market you are trading in; and
        e. Save it and close the configuration screen and open the main ProfitTrailer monitor screen.

        Note: We recommend using the max cost percentage as this will allow your trades to grow as your 
        trading budget grows. If however you have a small trading budget of $2000 or less than we recommend
        you use a fixed initial cost until your budget grows larger. See inside the pairs.properties 
        settings supplied for suggested minimum values. If you cant decide on suitable values 3 pairs at 
        0.0025 are safe numbers to start with. We always recommend starting ProfitTrailer in Test Mode 
        which will enable Paper Trading where the bot will trade just like the live bot but wont make 
        live trades on the exchange. This enables you to get your settings configured correctly first and 
        then go live once you are satisfied the bot is working correctly. By default ProfitTrailer will 
        be set to Test Mode.

    14. You have now completed the install of the new default settings. Happy Trading :-)

Any further updates to the settings will be posted in the pt-default-settings channel on the ProfitTrailer
community discord. 

All other instructions are in the settings file itself as to how to configure settings. 

You uncomment / comment out the ones you want to change to suit the market conditions, 
your trading style, etc. 

From there go to  https://wiki.profittrailer.com/  for an in-depth explanation of all the various 
ProfitTrailer settings.

Copyright © 2018, ProfitTrailer.com  All rights reserved worldwide.