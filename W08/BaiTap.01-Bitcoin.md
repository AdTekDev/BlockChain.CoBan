
#Bitcoin Clients and APIs 


- Cài đặt Bitcoin Core
https://bitcoin.org/en/download

- Cài từ Source
https://github.com/bitcoin/bitcoin


- Chạy thử
https://developer.bitcoin.org/examples/testing.html 


Opts:
- Cài đặt thư viện LibBitcoin
https://libbitcoin.dyne.org


Xem thông tin Ví, địa chỉ, giao dịch, ...
-  https://www.bitaddress.org/
- https://www.blockchain.com/explorer 
- https://live.blockcypher.com/ 


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


File cấu hình tham khảo:
- https://github.com/bitcoin/bitcoin/blob/master/share/examples/bitcoin.conf

Các mạng Test - Faucets:
- https://en.bitcoin.it/wiki/Testnet#Faucets 

Các câu lệnh chạy thử: (sách - Chapter 8: Bitcoin Clients and APIs)
mẫu - bitcoin-cli --testnet <command>

bitcoind --testnet -daemon
bitcoin-qt –testnet
bitcoind --testnet -daemon
bitcoin-cli --testnet getmininginfo
bitcoin-cli --testnet help
bitcoin-cli --testnet stop
bitcoind -regtest -daemon
bitcoin-cli -regtest getbalance
bitcoin-cli -regtest generatetoaddress 200 $(bitcoin-cli -regtest getnewaddress)
bitcoin-cli -regtest getbalance
bitcoin-cli -regtest getmininginfo
bitcoin-cli -regtest getblockchaininfo
bitcoin-cli -regtest stop


bitcoin-cli -regtest getnewaddress
2NC31WFFRwRkwd3S4TpyjN5GGDY7E63GSVd

bitcoin-cli -regtest sendtoaddress \
2NC31WFFRwRkwd3S4TpyjN5GGDY7E63GSVd 20.00

bitcoin-cli -regtest generatetoaddress 7 $(bitcoin-cli -regtest  getnewaddress)

bitcoin-cli -regtest gettransaction ... 

bitcoin-cli getblock \
"000000007bc154e0fa7ea32218a72fe2c1bb9f86cf8c9ebf9a715ed27fdb229a"

