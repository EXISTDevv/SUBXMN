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
