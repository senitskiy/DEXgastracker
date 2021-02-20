../solc DEXgastracker.sol 
../tvm_linker compile DEXgastracker.code -o ./DEXgastracker.tvc --lib ../stdlib_sol.tvm
../tonos-cli genaddr DEXgastracker.tvc DEXgastracker.abi.json --genkey DEXgastracker.keys.json

Seed phrase: "chase chair oil stool duck thing shoulder excite smooth stand country glare"

Raw address: 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497

../tonos-cli deploy --abi DEXgastracker.abi.json --sign DEXgastracker.keys.json ./DEXgastracker.tvc {}


setTongrams(uint128 msgGramPrice1, uint128 msgGramPrice2)
getTongrams()
getWalletAddr()
createNewEmptyWallet(bool selector)
setNewEmptyWallet(address value0)


../tonos-cli run 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 getTongrams {} --abi ./DEXgastracker.abi.json

../tonos-cli run 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 getWalletAddr {} --abi ./DEXgastracker.abi.json


../tonos-cli run 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 createNewEmptyWallet '{"selector":true}' --abi ./DEXgastracker.abi.json

../tonos-cli run 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 createNewEmptyWallet '{"selector":false}' --abi ./DEXgastracker.abi.json

../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 createNewEmptyWallet '{"selector":true}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 createNewEmptyWallet '{"selector":false}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json



../tonos-cli run 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setNewEmptyWallet '{"value0":true}' --abi ./DEXgastracker.abi.json




../tonos-cli run 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":400000000, "msgGramPrice2":600000000}'  --abi ./DEXgastracker.abi.json

../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":400000000, "msgGramPrice2":600000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":300000000, "msgGramPrice2":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":50000000, "msgGramPrice2":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":200000000, "msgGramPrice2":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json




../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":2000000, "msgGramPrice2":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json




../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":1000, "msgGramPrice2":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json

../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":10, "msgGramPrice2":500000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json


../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":1000000000, "msgGramPrice2":2000000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json



../tonos-cli call 0:f25a9123cf2d022f7c918cca23dc1aa96317d35e0d4c0acc1612d4c73f4d0497 setTongrams '{"msgGramPrice1":5000000000, "msgGramPrice2":10000000000}' --sign ./DEXgastracker.keys.json --abi ./DEXgastracker.abi.json
