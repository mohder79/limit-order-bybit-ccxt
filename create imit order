import ccxt
from pprint import pprint
import api_config as ac


exchange = ccxt.bybit({
    'options': {
        'adjustForTimeDifference': True,
    },
    'apiKey': ac.API_KEY,
    'secret': ac.SECRET_KEY,
    'password': ac.PASSWORD,
})


markets = exchange.load_markets()
print(exchange)


symbol = 'BTC/USDT:USDT'
amount = 0.001
price = 25000
type = 'limit'



order = exchange.create_limit_buy_order(
    symbol, amount, price)
pprint(order)
