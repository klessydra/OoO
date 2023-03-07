 <img src="/pics/Klessydra_Logo.png" width="400"> 

 # KLESSYDRA-OoO "BETA VERSION!!!!!" Out-of-Order Execution Processor

This is a non-functioning beta version that can only run a helloworld atm. Updates will follow shortly along with diagrams and a manual explaining the functionality of the core

Intro: The Klessydra processing core family is a set of processors featuring full compliance with RISC-V, and pin-to-pin compatible with the PULPino Riscy cores. Klessydra-OoO is a bare-metal 32-bit Out-of-Order Executing processor fully supporting the RV32IM from the RISC-V ISA, and one instruction from the Atomic "A" extension. 'OoO' further extends the instruction set with a set of custom vector instructions. 

Architecture: Klessydra-OoO is a six pipeline stage processor Fetch-Decode, Rename, Issue, Registerfile, Execute/Ld-Str, Writeback. The Renamed register file has a parametrizable number of registers. The registerfile can support up-to twelve read ports and three write ports. A commit counter handles the out-of-order commit of the registers, and an ROB handles the recovery in case of traps or branch misses.

 The OoO furhter supports the vector accelerator present in the Morph, T13, and S1.
