../solc DEXgastracker.sol 
../tvm_linker compile DEXgastracker.code -o ./DEXgastracker.tvc --lib ../stdlib_sol.tvm
../tonos-cli genaddr DEXgastracker.tvc DEXgastracker.abi.json --genkey DEXgastracker.keys.json

Seed phrase: "scout hub royal better erupt brisk bicycle tone pretty silent cost cereal"

Raw address: 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db

../tonos-cli deploy --abi DEXgastracker.abi.json --sign DEXgastracker.keys.json ./DEXgastracker.tvc {}


setTongrams(uint128 msgGramPrice1, uint128 msgGramPrice2)
getTongrams()
getWalletAddr()
createNewEmptyWallet(bool selector)
setNewEmptyWallet(address value0)

Root
0:4afee5881a9c911df66064eab46b5c49f4efb7ccd7b19cbb0efef250836218d5
{
  "public": "35002b6f8489c74a2f16b0186f9775f8a1da1a1ad2bd74732f83fbc48555e3a4",
  "secret": "f76f890eae142168a36eed46a0aef5b28bee39e8701d91361944aa88a0a87c18"
}
0:aea887e196ecc21e8289dac5106a52d93ead0d97aa57a0ae27439f005839797b


    "name": "getWalletAddress",
    "inputs": [
    { "name":"workchain_id", "type":"int8" },
    { "name":"pubkey", "type":"uint256" },
    { "name":"owner_std_addr", "type":"uint256" }
    ]

../tonos-cli run 0:4afee5881a9c911df66064eab46b5c49f4efb7ccd7b19cbb0efef250836218d5 getWalletAddress '{"workchain_id":0,"pubkey":"0x35002b6f8489c74a2f16b0186f9775f8a1da1a1ad2bd74732f83fbc48555e3a4","owner_std_addr":0}' --abi ./RootTokenContract.abi

../tonos-cli run 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db getTongrams {} --abi ./DEXgastracker.abi.json

../tonos-cli run 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db getWalletAddr '{"root":"0:4afee5881a9c911df66064eab46b5c49f4efb7ccd7b19cbb0efef250836218d5"}' --abi ./DEXgastracker.abi.json

../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db getWalletAddr '{"root":"0:4afee5881a9c911df66064eab46b5c49f4efb7ccd7b19cbb0efef250836218d5"}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli run 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db createNewEmptyWallet '{"root":"0:4afee5881a9c911df66064eab46b5c49f4efb7ccd7b19cbb0efef250836218d5"}' --abi ./DEXgastracker.abi.json

../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db createNewEmptyWallet '{"root":"0:4afee5881a9c911df66064eab46b5c49f4efb7ccd7b19cbb0efef250836218d5"}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json




<!-- ../tonos-cli run 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setNewEmptyWallet '{"value0":true}' --abi ./DEXgastracker.abi.json -->




../tonos-cli run 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":400000000, "forRoot":600000000}'  --abi ./DEXgastracker.abi.json

../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":400000000, "forRoot":600000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":300000000, "forRoot":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":50000000, "forRoot":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":200000000, "forRoot":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json




../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":2000000, "forRoot":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json




../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":1000, "forRoot":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":10, "forRoot":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json


../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":1000000000, "forRoot":2000000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json



../tonos-cli call 0:876e279838d21f3cd5b01d15bab72c10e5fa1576ab9288668ce7870b398376db setTongrams '{"forNewWallet":5000000000, "forRoot":10000000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json


