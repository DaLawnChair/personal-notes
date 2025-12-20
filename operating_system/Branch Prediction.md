Many times we can note performing if statements on ordered values where there are partitions that are lead to one outcome and another the other, run faster.


The compiler/interpreter is doing work with the machine code. This ordering reduces jump commands as the compiler knows that these can be skipped and be done more efficiently. 

Instruction pipelines allow for the set of instructions to be performed in the same order without deviation, and thus we spend less time moving/processing new steps, and instead spend that time performing the same steps.

If we have conditional statements, then the CPU will predict what will happen next based on its heuristics on the compiled code.

It will assume a prediction and precalculate the next steps in the pipeline for it. Later on it will check if the condition passes. If it does then it proceeds. If it doesn't then it flushes the intermediate steps and starts from its position after the condition.



Reference:
https://www.youtube.com/watch?v=Q5YJLRyudK4
* Very basics of branch prediciton
* Ordered values lead to less jumps required when compiled/interpreted