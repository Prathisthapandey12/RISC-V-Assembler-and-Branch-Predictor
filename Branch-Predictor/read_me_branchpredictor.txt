Question1: How to give input ?

Answer: The format of input should be as defined below:
core   0: 0x8000c81c (0x00150513) addi    a0, a0, 1
core   0: 0x8000c820 (0xfff5c703) lbu     a4, -1(a1)
core   0: 0x8000c824 (0x00078863) beqz    a5, pc + 16
core   0: 0x8000c828 (0xfee786e3) beq     a5, a4, pc - 20
core   0: 0x8000c814 (0x00054783) lbu     a5, 0(a0)
core   0: 0x8000c818 (0x00158593) addi    a1, a1, 1
core   0: 0x8000c81c (0x00150513) addi    a0, a0, 1
core   0: 0x8000c820 (0xfff5c703) lbu     a4, -1(a1)
core   0: 0x8000c824 (0x00078863) beqz    a5, pc + 16
core   0: 0x8000c828 (0xfee786e3) beq     a5, a4, pc - 20
.........................................................
.........................................................
We have given the input using an input file "input.txt" . We have opened this file using file handling and have read it line by line. We have
then sliced the string into tokens, so as to access the address of each instruction and the offset in case of a branch instruction. We have 
created a vector of strings and have stored each token in it. Proper whitespaces in the input lines are required since lack of them will lead to 
incorrect output, for eg pc+16, pc +16 , 0:0x8000c81c are incorrect input format for this particular program.




Question2: What do we get as output?

Answer: .We have printed the accuracy of four branch predictors: 
Always_taken branch predictor
Always_not-taken branch predictor
One-bit branch predictor
Two-bit branch predictor
We then ask the user to print the branch target buffer table for each prediction methods
Each table is of the format:
Branch Address Target Address