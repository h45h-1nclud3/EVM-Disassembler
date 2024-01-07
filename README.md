# EVM-Disassembler
Python script to convert hex EVM opcodes to equivalent EVM instructions
# Run
Execute the script with the hex opcodes string as an argument
## Example: 
`python3
./Disassemble_EVM.py 60806040526004361061013d5763ffffffff7c010000000000000000000000000000000000000000000000000000000060003504166305d2035b811461014257806306fdde031461016b578063095ea7b3146101f557806317ffc320146102195
`

0x0: --> PUSH1 ---> 0x80

0x2: --> PUSH1 ---> 0x40

0x4: --> MSTORE

0x5: --> PUSH1 ---> 0x04

0x7: --> CALLDATASIZE

0x8: --> LT

0x9: --> PUSH2 ---> 0x013d

0xc: --> JUMPI

0xd: --> PUSH4 ---> 0xffffffff

0x12: --> PUSH29 ---> 0x0100000000000000000000000000000000000000000000000000000000

0x30: --> PUSH1 ---> 0x00

0x32: --> CALLDATALOAD

0x33: --> DIV

0x34: --> AND

0x35: --> PUSH4 ---> 0x05d2035b

0x3a: --> DUP2

0x3b: --> EQ

0x3c: --> PUSH2 ---> 0x0142

0x3f: --> JUMPI

0x40: --> DUP1

0x41: --> PUSH4 ---> 0x06fdde03

0x46: --> EQ

0x47: --> PUSH2 ---> 0x016b

0x4a: --> JUMPI

0x4b: --> DUP1

0x4c: --> PUSH4 ---> 0x095ea7b3

0x51: --> EQ

0x52: --> PUSH2 ---> 0x01f5

0x55: --> JUMPI

0x56: --> DUP1

0x57: --> PUSH4 ---> 0x17ffc320

0x5c: --> EQ

0x5d: --> PUSH2 ---> 0x0219

