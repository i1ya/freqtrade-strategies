# My freqtrade-strategies

Hi there!
This is repo for my freqtrade-strategies. My name is Ilya Zelenchuk, I'm a lecturer at the SPbU university (https://english.spbu.ru/). These strategiest is my hobbie and I'm not a trader or financial analytics and my strategies are not a financial advise. 

# FAQ

 **Q**: What is the difference between strategies?  
 **A**: CombinedBinHClucAndMADV using optimized stratic pairlist. BigZ using dynamic (based on volume) pairlist

 **Q**: I run strategy for one day. But did not trade. Is bot running Ok?  
 **A**: Every strategy has buy signals. Depending on market there is a day or maybe two when no buy signals is trggered. So, it's ok. Also, checkout the docs - https://www.freqtrade.io/en/latest/faq/#i-have-waited-5-minutes-why-hasnt-the-bot-made-any-trades-yet  
 
 **Q**: CombinedBinHClucAndMADV5 has "order_types = {'buy': 'limit', 'sell': 'limit', 'stoploss': 'market', 'stoploss_on_exchange': False}" but CombinedBinHClucAndMADV9 and BigZ* has "order_types = {'buy': 'market', 'sell': 'market', 'stoploss': 'market', 'stoploss_on_exchange': False}". What is the difference between "'buy': 'market'" and "'buy': 'limit'"?  
 **A**: If your strategy using "'buy': 'market'" than you have to change in your config file "bid_strategy" section to "price_side": "ask" and "ask_strategy" section to "price_side": "bid". For more info checkout the docs - https://www.freqtrade.io/en/stable/configuration/#prices-used-for-orders
 
 
