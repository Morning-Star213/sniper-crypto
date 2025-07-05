<div align="center">
    <img src="https://i.imgur.com/mF3T0jn.png">
    <h3 align="center">Eryx - Crypto Sniper</h3>
</div>

## Description
![Alt Text](https://i.imgur.com/8M3XqVQ.gif)

A fast and efficient bot written in NodeJS to automatically buy and sell tokens on the blockchain as soon as liquidity is added and trade is enabled.
<br><br>
The bot is extremely fast as long as you use a **good** node and not a public one. With a node from Quicknode you can expect a buy/sell transaction in less than 5 seconds.
<br><br>
The bot uploaded on github is the **lite** version of the real bot. 
You do **not** get all of the features from the premium version.

### Features

Current features supported by the **FREE** version:

- [x] Buying (BNB & ETH pairs only)
- [x] Gas estimation system
- [x] Regular liquidity sniper

Additional features supported by the **premium** version:
- [x] Buying (ALL pairs)
- [x] Multi blockchain support.
- [x] Bytecode checker / blocker.
- [x] MethodID waiter.
- [x] Multi-buy mode (all transactions are in the same block). 
- [x] Wrapped mode for any ETH-like token (BNB, MATIC, etc..). 
- [x] Tax checker (all pairs are supported)
- [x] Pinksale / dxsale support.
- [x] Sell using a delay
- [x] Sell using the space key
- [x] Auto / manual selling
- [x] Mempool sniping mode.
- [x] Block-offset system
- [x] Auto updates (updates are done automatically without the need of a re-download)
- [x] Trailing auto-sell.
- [x] Support

You can view the latest feature list here: https://eryx.io/docs/#features


### Supported chains
- Binance Smart Chain
- Arbitrum
- Avalanche
- Ethereum
- Polygon
- Cronos
- Milkomeda
- Metis
- Fantom
- Dogechain

If you wish to change the blockchain the bot will operate on, just change the WSS_NODE endpoint in config.ini to the right endpoint.

### Installation

1. Download and install NodeJS from <a href="https://nodejs.org/en/download/">here</a>.
2. Download and install Git from <a href="https://git-scm.com/downloads">here</a>.
3. Open a command prompt / terminal and clone the repository.
	```sh
	git clone ...
	```
4. In the same command prompt, install the NPM packages.
	```sh
	npm install
	```
5. That's it! Time for configuration. 🎉

### Configuration

```ini
[WALLET]
; This is your BSC wallet's private key.
SECRET_KEY=private_wallet_key

; The uptime of this node is pretty bad, you should consider using a private node.
WSS_NODE=wss://bsc-ws-node.nariox.org:443


[CONTRACTS]
; These variables support some pre-defined contracts (BNB, ETH, BUSD). 
; For other contracts you'll have to specify the contract address yourself.
INPUT=BNB
OUTPUT=BUSD


[TRANSACTION]

GAS_LIMIT=500000
GAS_PRICE=5

; This variable is the amount of crypto you wish to use with the input contract.
; If for example you use WBNB as input, you will have to use WBNB's format.
AMOUNT_IN=0.0033

BUY_SLIPPAGE=10
```

### Usage
To launch the bot use the command ```node index.js```


