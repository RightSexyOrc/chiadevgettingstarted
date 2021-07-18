# Developers Getting Started with the Chia Protocol and ChiaLisp

Welcome. We'd like to help you have a smoother journey getting started with developing for the chia protocol and blockchain, and developing with Chialisp.

We'll start off with helping you get a development environment and testing setup. Then we'll start getting into Chialisp.


## Getting your development environment setup

You'll want to install chia, and also the CLVM, Chialisp virtual machine, which includes the run and brun compilers.

Which IDE should you use to develop in Chialisp?
Try Atom, https://atom.io

Why? Helps save you from unclosed parentheses!

# Blockchain Testing Environment

There are 3 ways to experiment with Chia besides on its mainnet:

1) connect to one of the live Chia testnets

2) use its built-in simulator

3) rolling your own local testnet!


## Using a Live Chia Testnet

To run the Chia GUI with testnet in 3 steps:

Note: We'll use testnet7, because the configuration values are already available in the default install, and there's
a "faucet" website we can use to get some free testnet chia easily.

1) edit ~/.chia/mainnet/config and change the selected_network line to "selected_network: testnet7" 

2) at the command line, type: "chia configure -t true"

#chia #chiablockchain #LearnChia #ChiaFAQ 


3) start the chia-blockchain-gui within its directory: "npm run electron &"

If you have problems, check the logs in ~/.chia/mainnet/log/debug.log

Sync-ing up the testnet may take a huge amount of time, like many hours, for the first block of the testnet. Have patience.

If you want to make sure something is really going on, you can change the debug logging level and restart.

first draft of these instructions, may contain orc turds

4) Now you can get yourself some TestChia, head to http://chia-faucet.com/


Note: To run the Chia GUI for both mainnet and testnet at the same time, you may wish to run them in separate docker containers, so they don't see the other instance and quit.


## Using the Chia Simulator

To experiment with #chiablockchain, you can run the simulator on your local Linux or MacOS machine. 

Assuming you've already installed chia, you need to install timelord and then run the simulator. 

Follow these steps: 

To install the timelord, go to the main chia directory, then activate venv, set the install file to executable, and run the install file with these commands:

. ./activate
chmod +x ./install-timelord.sh
sh http://install-timelord.sh

If the install script runs without errors, you can now start the simulator. Note that the command in the documentation is wrong, should be:

chia start simulator
(simulator, not sim)

Oh, and 1 more thing, when you upgrade your chia version, run the install_timelord.sh script again! Hope this helps.


Reference:
https://github.com/Chia-Network/chia-blockchain/wiki/Quick-Start-Guide


## Rolling Your Own Testnet

Follow these steps for a full local testnet of your own:
https://github.com/Chia-Network/chia-blockchain/wiki/Create-a-local-testnet-for-fast,-private-testing


# Getting Started with Chialisp

Resources:

How to Secure a Coin With a Custom Puzzle and Spend It
https://docs.google.com/document/d/1x2PHn1qnMESc9RhPiBflDHWKoch2K0ds50brfSc7LPc/edit


# Author Orcs

RightSexyOrc, https://twitter.com/RightSexyOrc
(you?)
