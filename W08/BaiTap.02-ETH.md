
Cài đặt dApp Node
- https://docs.dappnode.io/
- https://docs.dappnode.io/get-started/intro 

dApp node - Code / Install / ISO img
- https://github.com/dappnode/DAppNode/releases/

ethNode
- https://github.com/vrde/ethnode 


Thông tin node:
- https://ethereum.org/en/run-a-node/
- https://ethereum.org/en/developers/docs/nodes-and-clients/ 
- https://docs.ethhub.io/using-ethereum/running-an-ethereum-node/


**Lệnh tham khảo:
**

npm install geth  parity 

geth  --help
geth --syncmode light
parity --light
parity --light --no-hardcoded-sync

geth --syncmode full
parity --no-warp
geth --syncmode full --gcmode archive
parity --no-warp --pruning archive

geth --http

*** https://geth.ethereum.org/docs/interface/command-line-options

