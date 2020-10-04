# blabla
Implementation of the BlaBla version of the ChaCha stream cipher in Hardware.

BlaBla is a version of ChaCha develped by JP Aumasson. The big difference is that the Blake2b permutation is being used.
The reference implementation by Aumasson is here: https://github.com/veorq/blabla

The big benefit compared to ChaCha is the doubled block size and thus that the number of bytes/cycles increeases.
This is of course a HW implementation which means that the number of registers will increase, the logic will increase and the clock frequency will
be decreased. How much? Too early to say.

Basically we take the ChaCha core and change what is needed. This includes the Python model.

Here we go...
