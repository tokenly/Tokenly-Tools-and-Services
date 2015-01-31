# Tokenly
##Tools & Services

An outline of all available tools, components and services in the Tokenly ecosystem

#Software & Services

###Tokenly CMS

* General purpose content management system
* Multi-blogging platform
* Forum and community platform
* Address proof of ownership and Counterparty token tracking
* Token Controlled Access
* Token distribution integration and asset dropper
* Token redemption system
* User participation reports (combine with distributor to create a rewards program)
* Easily extendable web API
* Integration with other Tokenly systems

**Status:** In production (and active development)

**Repositories**

[Tokenly CMS](https://github.com/tokenly/tokenly-cms)

###XChain

Address and Token Balances  
Incoming/Outgoing Payment Notifications  
Platform Wallet Services

**Status:** In production (and active development)

**Repositories**

[XChain](https://github.com/tokenly/xchain)  
[XChain-Client](https://github.com/tokenly/xchain-client)  
[xcaller](https://github.com/tokenly/xcaller) - calls webhooks from a queue and returns results  
[xstalker](https://github.com/tokenly/xstalker) - reads insight transactions and loads a queue for processing by XChain

###SwapBot

* Standalone system acts as a token "vending machine"
* Accepts either BTC or Counterparty tokens to a "vending address", and spits out (after X confirmations) a different type of token based on defined exchange rate.
* Can accept multiple types of tokens at different variable rates
* Dynamic prices which can be fixed, based on an API request or Counterparty broadcast, or based on a custom function.
* Other extra features such as automatic income forwarding, automatic new token issuances, automatic broadcasts and more.
* Support for running multiple swapbot-machines
* Separate front-end "swapbot directory" system for public listings of available swapbot/vendng machines.

**Repositories**

**Status:** In development

[SwapBot-Machine](https://github.com/tokenly/swapbot)  
SwapBot-Directory (coming soon!)  
[Functional prototype script](https://github.com/tokenly/xcp-gateway)

###BitSplit

* Token distribution and payment splitting system
* For distributions, accepts a list of addresses and amounts, adds up the total amount creates a single deposit address. User sends in total amount plus sufficient BTC for fees to the deposit address, and BitSplit handles the sending to each address provided.
* Useful for sending large group payments, or scheduled distributions (e.g LTBCOIN)
* Able to do persistant distrubutions aka "splitting"; instead of supplying a total amount, any payments (BTC or counterparty tokens) sent to the "split address" are automatically split up between each of the defined output addresses

**Status:** In development

**Repositories**

[BitSplit](https://github.com/tokenly/BitSplit)

###Auction Machine

BTC bidding -> TOKEN out  
TOKEN bidding -> TOKEN out

**Repositories**

[Auction Machine](https://github.com/tokenly/auction-machine)

###Tokenly Accounts

Platform-Wide Preferences (email, name, etc)  
Verified Counterparty Addresses  
oAuth

**Status:** In development

**Repositories**

[Accounts](https://github.com/tokenly/accounts)

###Examples and Tutorials

* [Toy Vending Machine](https://github.com/tokenly/toy-vending-machine) demonstrating how to use XChain

#Tools & Components

####Generic Components:

* [XChain-Client](https://github.com/tokenly/xchain-client) - Interact with XChain
* [token-controlled-access](https://github.com/tokenly/token-controlled-access) - Check for the presence of tokens
* [bitcoin-payer](https://github.com/tokenly/bitcoin-payer) - compose and send BTC transactions
* [counterparty-sender](https://github.com/tokenly/counterparty-sender) - compose and send Counterparty transactions
* [counterparty-transaction-parser](https://github.com/tokenly/counterparty-transaction-parser) - parse a BTC tx and extract Counterparty data
* [counterparty-asset-info-cache](https://github.com/tokenly/counterparty-asset-info-cache) - load and cache Counterparty asset information (e.g. divisible)
* [insight-client](https://github.com/tokenly/insight-client) - A client for the insight API
* [xcpd-client](https://github.com/tokenly/xcpd-client) - A client for counterpartyd
* [bitcoin-address-lib](https://github.com/tokenly/bitcoin-address-lib) - a BIP32 address and private key library
* [bitcoin-currency-lib](https://github.com/tokenly/bitcoin-currency-lib) - Convert value to/from satoshis
* [hmac-auth](https://github.com/tokenly/hmac-auth) - sign and validate API calls with a token, secret key and nonce
* [token-generator](https://github.com/tokenly/token-generator) - generate random tokens (as in passwords, not Counterparty tokens)

####Other Services:
* [pusher](https://github.com/tokenly/pusher) - push public client-side notifications to javascript clients



