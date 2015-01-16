# Tokenly-Tools-and-Services
An outline of all available tools, components and services in the Tokenly ecosystem

#Software & Services

###Tokenly CMS

Community publishing platform
forum
rewards system

###XChain

Address and Token Balances
Incoming/Outgoing Payment Notifications
Platform Wallet Services

###Counterparty Gateway

BTC in -> TOKEN out
TOKEN in -> BTC out
Valuations on BTC/USD quotes

###BitSplit

Token in -> Tokens Out to Many Recipients
BTC in -> BTC Out to Many Recipients

###Auction Machine

BTC bidding -> TOKEN out
TOKEN bidding -> TOKEN out

###Tokenly Accounts

Platform-Wide Preferences (email, name, etc)
Verified Counterparty Addresses
oAuth

###Examples and Tutorials

* Toy Vending Machine demonstrating how to use XChain

#Tools & Components

####Generic Components:

* XChain-Client - Interact with XChain
* token-controlled-access - Check for the presence of tokens
* bitcoin-payer - compose and send BTC transactions
* counterparty-sender - compose and send Counterparty transactions
* counterparty-transaction-parser - parse a BTC tx and extract Counterparty data
* counterparty-asset-info-cache - load and cache Counterparty asset information (e.g. divisible)
* insight-client - A client for the insight API
* xcpd-client - A client for counterpartyd
* bitcoin-address-lib - a BIP32 address and private key library
* bitcoin-currency-lib - Convert value to/from satoshis
* hmac-auth - sign and validate API calls with a token, secret key and nonce
* token-generator - generate random tokens (as in passwords, not Counterparty tokens)

####Other Services:
* pusher - push public client-side notifications to javascript clients

####XChain Specific Services:

* xcaller - calls webhooks from a queue and returns results
* xstalker - reads insight transactions and loads a queue for processing by XChain

