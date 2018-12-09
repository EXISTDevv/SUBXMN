# SUBX source
subx SUBX development tree

subx is a PoW PoS-based cryptocurrency.

Development process
Developers work in their own trees, then submit pull requests when they think their feature or bug fix is ready.

The patch will be accepted if there is broad consensus that it is a good thing. Developers should expect to rework and resubmit patches if they don't match the project's coding conventions (see coding.txt) or are controversial.

The master branch is regularly built and tested, but is not guaranteed to be completely stable. Tags are regularly created to indicate new stable release versions of subx.

Feature branches are created when there are major new features being worked on by several people.

From time to time a pull request will become outdated. If this occurs, and the pull is no longer automatically mergeable; a comment on the pull will be used to issue a warning of closure. The pull will be closed 15 days after the warning if action is not taken by the author. Pull requests closed in this manner will have their corresponding issue labeled 'stagnant'.

Issues with no commits will be given a similar warning, and closed after 15 days from their last activity. Issues closed in this manner will be labeled 'stale'.

<table>
  <th colspan=2>Official links:</th>

<tr><td>Website:</td><td> http://www.subexcoin.com/</td></tr>
<tr><td>Explorer:</td><td> http://144.202.18.54:3001/</td></tr>
<tr><td>White Paper:</td><td> https://github.com/EXISTDevv/SUBX-WHITEPAPER</td></tr>
<tr><td>Discord:</td><td> https://discord.gg/73PwrnK</td></tr>
<tr><td>Twitter:</td><td> https://twitter.com/SUBX15</td></tr>
<tr><td>Telegram:</td><td> https://t.me/joinchat/F6rHEA4DNsjF5AoPbmq71w</td></tr>
<tr><td>Bitcointalk ANN:</td><td> https://bitcointalk.org/index.php?topic=5038669</td></tr>
<tr><td>Github:</td><td> https://github.com/EXISTDevv/SUBXMN</td></tr>
<tr><td>CoinMarketCap</td><td>https://coinmarketcap.com/currencies/sub-invest/</td></tr>
</table>

<table>
  <th colspan=2>Exchanges</th>
<tr><td>Crex24:</td><td>https://crex24.com/nl/exchange/SUBX-BTC</td></tr>
</table>

### Coin Specs
<table>
<tr><td>Algo</td><td>Scrypte</td></tr>
  <tr><td>Masternode Collateral</td><td>1000,000,000 SUBX</td></tr>
<tr><td>Difficulty Retargeting</td><td>Every Block</td></tr>
<tr><td>Max Coin Supply</td><td>3 Trillion</td></tr>
<tr><td>Premine in block 1</td><td>600 Billion*</td></tr>
<tr><td>Full Premine</td><td>to handle snapshot*</td></tr>
  <tr><td>Block Time</td><td>180 seconds</td></tr>
  <tr><td>Block Minting</td><td>4 confirmations</td></tr>
  <tr><td>Block Transactions</td><td>5 confirmations</td></tr>
  <tr><td>Minimum Stake Age</td><td>3 days</td></tr>
</table>
*for swap and additional coins in premine not for snapshot distributed to promote the project (not to be retained by developers)

### Reward Distribution

<table>
<th colspan=4>PoW Phase</th>
<tr><th>Block Height</th><th>Reward Amount</th><th>Notes</th></tr>
<tr><td>1-300</td><td>2000,000,000 SUBX</td><td>Initial Premine to Former Chain</td></tr>
<tr><td>301-50,000</td><td>100 SUBX</td><td>Closed Mining</td></tr>
<tr><th colspan=4>PoS Phase</th></tr>
<tr><th>Block Height</th><th colspan=1>Reward Amount</th></tr>
<tr><td>5001-*</td><td>Variable reward (Triangle wave, 20 blocks)</td></tr>
  <tr><td>Max reward</td><td>1000,000 SUBX</td></tr>
  <tr><td>Min reward</td><td>1000 CSTL</td></tr>
  <tr><td>Masternode Reward 85%</td><td>15 % Stake</td></tr>
</table>

Install on linux
----------------

### Prepare needed library to compile your daemon
`apt-get install git automake build-essential libtool autotools-dev autoconf pkg-config libssl-dev libboost-all-dev software-properties-common libgmp-dev unzip -y`

### Adding bitcoin apt repository
`sudo add-apt-repository ppa:bitcoin/bitcoin && sudo apt-get update`

### installing libdb and miniupnp from bitcoin repository
`apt-get install libdb4.8-dev libdb4.8++-dev libminiupnpc-dev`

### clone source code
`git clone https://github.com/EXISTDevv/SUBXMN.git`

### build
`cd SUBXMN/src && make -f makefile.unix`
