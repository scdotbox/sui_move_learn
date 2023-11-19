
## sui 钱包1
```bash
curl --location --request POST 'https://faucet.devnet.sui.io/gas' \
--header 'Content-Type: application/json' \
--data-raw '{
    "FixedAmountRequest": {
        "recipient": "0xa17d0a6bc7ddcdd2cd445e5999023f9867326bc27d9538b62d3b9b6b500730a6"
    }
}'
```


## sui 钱包2
```bash
curl --location --request POST 'https://faucet.devnet.sui.io/gas' \
--header 'Content-Type: application/json' \
--data-raw '{
    "FixedAmountRequest":{
        "recipient":"0xf7aef823a3b9b6e0c7ef2223cb3c2ea13b1b5b14fcb25c3cecea8d47c96e8b43"
    }
}'
```


#sui 的钱包地址
0xf7aef823a3b9b6e0c7ef2223cb3c2ea13b1b5b14fcb25c3cecea8d47c96e8b43

sui keytool import


sui client new-env --alias mainnet --rpc https://sui-mainnet.nodeinfra.com:443
sui client new-env --alias localnet --rpc https://127.0.0.1:9000

sui client new-env --alias localnet --rpc http://127.0.0.1:5173

sui client new-env --alias localnet --rpc http://127.0.0.1:9000

sui = { git = "https://github.com/MystenLabs/sui.git", subdir = "crates/sui-framework/packages/sui-framework", rev = "framework/devnet" }
Sui = { git = "https://github.com/MystenLabs/sui.git", subdir = "crates/sui-framework/packages/sui-framework", rev = "devnet-v1.1.0"}

Sui = { git = "https://github.com/MystenLabs/sui.git", subdir = "crates/sui-framework/packages/sui-framework", rev = "framework/devnet" }

Sui = { git = "https://github.com/MystenLabs/sui.git", subdir = "crates/sui-framework/packages/sui-framework", rev = "framework/localnet" }

cargo rustc -- -C link-args="-e __start"

RUST_LOG="off,sui_node=info" cargo run --bin sui-test-validator -- -C link-args="-e __start"



curl --location --request POST 'http://127.0.0.1:9123/gas' \
--header 'Content-Type: application/json' \
--data-raw '{
    "FixedAmountRequest": {
        "recipient": "0xf7aef823a3b9b6e0c7ef2223cb3c2ea13b1b5b14fcb25c3cecea8d47c96e8b43"
    }
}'