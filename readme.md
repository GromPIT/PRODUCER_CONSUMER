## ** PRODUCER - CONSUMER CONCURRENT PROBLEM IN ADA WITH USE OF MONITORED SHARED RESOURCE **

### Written on 13th of May 2023 by Piotr M. Garczyński

Producers generate random Integer numbers and put them to monitored protected 
shared resource (queue or stack) while consumers read them from it. 

To use FIFO (queue) put procedure call queueBuffer.write in the producer body
and queueBuffer.read in the consumer body (in main.adb)

To use LIFO (stack) put procedure call stackBuffer.write in the producer body
and stackBuffer.read in the consumer body. 

Size of buffer is defined as queueSize constant in queuePackage.ads for queue
and in stackPackage.ads as stackSize constant for stack. 

Simulation will last for time defined in begin/end block of main procedure.
