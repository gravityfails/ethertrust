Basic Concepts

guide to how to create an ethereum DApp
Will not restate what ios in existing tutorials, will only give reference to the tutorials used
this guide provides the learnoing path and steps to create a DApp, and the considerations both technical and economical in creating the DApp

things to do
platform target for the app
--DApp store
--html site with metamask integration
--myst browser
--toshi app
--android/ios - geth light client?

things to do
--ethereum name service

things to consider
--swarm vs. ipfs
--how to handle variations in contract behavior - god contract composition vs multiple contracts - inheritance?


things to consider long term
--redeploying the contract
--update the contract


Tutorials to get the basic concepts of the underlying technologies
--blockchain (what a bad name)
--ethereum
--solidity
--javascript - codeacademy
--node.js
--npm


the basics of getting setup
setting up an ethereum node
  usefule commands
    //-- know the rpc and net endpoints
    geth --testnet --syncmode "fast" --cache=1024 --rpc --rpcapi eth,net,web3,personal

    //-- node
    eth.syncing
    admin.nodeInfo
    web3.eth.blockNumber

    //-- minind
    miner.setEtherbase(eth.accounts[1])
    miner.start(1) - single thread to not use up all cpu
    miner.stop()
    web3.eth.mining


    //-- accounts
    eth.accounts
    personal.newAccount('some pass phrase')
    personal.unlockAccount('0x1aa1ff3396d744a72613cc3efc7546afa58d3e62', 'some pass phrase', 2*60*60)
    web3.eth.getBalance("0x9deb5d5eeb6ee6e3f21ceab901db6a91313bbacb")

