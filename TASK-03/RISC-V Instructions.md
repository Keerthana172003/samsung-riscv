
![Disassembly machine code](https://github.com/user-attachments/assets/c3649aac-33a0-42e8-a45d-82702c5688f7)

### Here are 15 unique RISC-V instructions from the disassembly, with their 32-bit machine codes, types, and brief explanations:

1) addi sp, sp, -32
Machine code: 0xfe010113
Type: I-type
Explanation: Adjusts the stack pointer by subtracting 32 for stack space allocation.

2) sd ra, 24(sp)
Machine code: 0x00113c23
Type: S-type
Explanation: Stores the return address register (ra) at offset 24 from sp.

3) sd s0, 16(sp)
Machine code: 0x00813823
Type: S-type
Explanation: Stores the frame pointer (s0) at offset 16 from sp.

4) li a5, 10
Machine code: 0x00a00793
Type: I-type
Explanation: Loads the immediate value 10 into register a5.

5) sw a5, 28(s0)
Machine code: 0xfea42623
Type: S-type
Explanation: Stores the value of a5 at offset 28 from s0.

6) sw zero, 20(s0)
Machine code: 0x00010223
Type: S-type
Explanation: Stores zero at offset 20 from s0.

7) lw a4, 24(s0)
Machine code: 0xfea42283
Type: I-type
Explanation: Loads a word from offset 24 of s0 into a4.

8) addw a3, a5, a4
Machine code: 0x00f787bb
Type: R-type
Explanation: Adds a5 and a4 and stores the result in a3.

9) bge a4, a5, main+0x28
Machine code: 0x04a10863
Type: B-type
Explanation: Branches if a4 is greater than or equal to a5 to the address main+0x28.

10) addi a5, a5, -1
Machine code: 0xfff78793
Type: I-type
Explanation: Decrements a5 by 1.

11) jal a0, printf
Machine code: 0x1e78151b
Type: J-type
Explanation: Jumps to the address of the printf function and stores return address in a0.

12) ld ra, 24(sp)
Machine code: 0x00c12083
Type: I-type
Explanation: Loads the value at offset 24 from sp into ra.

13) ld s0, 16(sp)
Machine code: 0x00812403
Type: I-type
Explanation: Loads the value at offset 16 from sp into s0.

14) add sp, sp, 32
Machine code: 0x02010113
Type: I-type
Explanation: Restores the stack pointer by adding 32, undoing the stack allocation.

15)ret
Machine code: 0x00008067
Type: R-type (special encoding for return)
Explanation: Returns control to the calling function.

