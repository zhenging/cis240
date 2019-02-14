```
/*
    Zhongyuan Zheng / zhongyuan_zheng@my.cuesta.edu
    CIS 240
    Chapter 3 Homework
*/
```
1\. What is the difference between data memory and register memory?
>Solution
While the program is running, the CPU is performing computations and needs to store results in temporary storage outside the CPU, this is called **Data memory**. The CPU, however, also has internal storage for both program and data memory, this is called **Register Memory**.

2\. What part of the CPU directs the accessing of program memory?
>Solution
The program counter.

3\. What does the IP register point to?
>Solution
IP register points to program memory, in particular it points to the **next instruction** to be executed.

4\. Write out the register combination needed to access the following types of memory?
>Solution

|        | Segment Register | Pointer Register/s |
|--------|-------------------|-----------------|
| Program  | CS | IP |
| Data     | DS | BP |
| Stack    | SS | SP |

5\. What are the following types of move?
Register to register: **Register Move**
Program memory to register: **Immediate Data Move**
Data memory to register (or register to memory): **Direct of Indirect Move**

6\. Write an example of each of the four types?
>Solution
Register Move: `MOV AX,BX`
Immediate Data Move: `MOV AX,1234`
Direct Move: `MOV AX,[1234]`
Indirect Move: `MOV AX,[BX]`

7\. Write an example of a memory write and a memory read using _direct_ memory access at address 0104h, from and to **AX** data register
>Solution
Read: `MOV AX,[0104]`
Write: `MOV [0104],AX`

8\. Write an example of a memory write and a memory read using _indirect_ memory access using **BP** address register from and to the **AX** data register
>Solution
Read: `MOV AX,[BP]`
Write: `MOV [BP],AX`

9\. What prevents system bus conflicts?
>Solution
Todo

10\. What is the difference between the **MOV** and **IN/OUT** instructions?
>Solution
1\. `MOV` is bi-directional, meaning it can perform both write and read operation. `IN/OUT` are unidirectional. `IN` can only perform a device read, and `OUT` can only perform a device write.
2\. `MOV` is normally used to access memory devices such as the main memory (RAM), or battery backed RAM (CMOS). `IN/OUT` are usually used to access hardware devices such as harddisks, floppy drivers, keyboards, serial port items such as modems and mouse, and parallel port items such as printers or scanners.

11\. What is the difference between the debug command and a CPU instruction:
>Solution
Todo


12\. What seperate program, data, and stack that are all located in **DRAM** memoery?
>Solution
Todo


13\. When acessing memory what is the function of a segement register and a pointer register?
>Solution
The memory can be addressed at the location of segment * 10 + offset (pointer register).

14\. List all the registers that are associated with offsets?
>Solution
`BX, DI, SI, BP, IP, SP`

15\. What is the maximum amount of memory that a 16bit segement and offset register can address?
>Solution
From `xxxx0 + 0000` to `xxxx0 + ffff`, that is $2^{16}$ bytes, or $64$ kilobytes.

16\. Calculate the physical address of the data to be accessed if **DS=2300** and **BX=0456**
>Solution
`2300 * 10 + 0456 = 23456`
