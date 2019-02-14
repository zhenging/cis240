### Chapter 3 Memory Types

#### Program Memory vs Data Memory

#### Registers

#### MOV Instruction and Copying Data From One Location to Another
1\. **Register move** - From on register to another
```
MOV AX,BX       ;copy the contents of BX to AX
                ;if BX contains 1234 before execution, AX will also equal 1234
                ;after the instruction is executed by the CPU
```

2\. **Immediate data move** - From Program Memory to an internal register
```
MOV AX,1234     ;copy 1234 stored in program memory to the register AX
```

3\. **Direct or Indirect memory moves** - From data memory to an internal register **OR** from an internal register to data memory
_Indirect Move_
```
MOV AX,[BX]     ;this is a indirect move and copies the memory contents
                ;pointed to by BX into AX
```
_Direct Move_
```
MOV AX,[1234]   ;this is a direct move and copies the memory contents
                ;pointed to by data memory address 1234 into AX
```

#### Address and Data Paths

#### Types of CPU Buses

#### MOV Instructions vs. IN and OUT Instruction

#### Accessing Program Memory and Assembling Programs

#### The Difference Between Program and Data Memory in PC Memory Devices

#### Physical Memory Locations

##### Protected and Long Mode Registers Sets
