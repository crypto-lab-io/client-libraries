# Libraries for CryptoLab
Website: https://www.crypto-lab.io  
Documentation: https://www.crypto-lab.io/documentation  
Swagger: https://www.crypto-lab.io/swagger

Libraries for:
* Python3
* .NET (soon)
* PHP (soon)


## Python
Install library from Pypi ```pip install cryptolab```

Sample to use it to replay data 
```python
import cryptolab

# Init lib with api key
cl = cryptolab.CryptoLab('{YOUR_API_KEY}', on_error)

# Init the raplayer with the parameters
cl.init_replayer(event, '{EXCHANGE}', '{MARKET}', '{START_DATE}', '{END_DATE}')

# On event - callback
def event(trade):
    print(trade)
    # add you algorithm here to backtest your strategy

# On event error
def on_error(message):
    print(message) # ex: quota reached, data not avaible, plan inactive, etc.
```

## .NET
soon


## PHP
soon

![Logo](https://1.gravatar.com/avatar/5121577298f39a1661507198f8615319a7d7a14fad36f9ec52d20ae0d446bf69?size=128)