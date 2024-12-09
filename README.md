testing.cct : a file that testing the computer without Register array , instruction decoder and Instruuction cache


Component testing.cct : file that testing the component individually 

List of component:
mem_ctrl: a controller for your memory module, for when it is connected to the
main data bus.
db_ctrl: a controller for bidirectional data bus, using which you can control the direction in which information traverses.
16bit buffer: same as other buffer, when 
Pad: output the 8bit value of IMM
Branching:
Register Array: an array with 8 register that save the output from instruction decoder and ouput Rn_data,Rm_data,Rx_data,PC_data to different component
instruction decoder: Receive instruction input from Instruction cache, and decode the output the value of RM,Rn,Rx,Rd,Reg_EN to the register array 
MEM_ADD: Calculates an address from PC (R7), apply immediate offset and save it in target register
Branching: Depends on the condition , input Imm to PC to get new PC 
CMP: compare Rn_data and Rm_data depends on the condition
Pad: output Imm 8bit value
MEM_CE: depends on the Instruction , control the input of CE for Main Memory

main.cct: main computer file

