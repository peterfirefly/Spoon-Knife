### Moscow ML -- The Zinc Oxide Experiment

[Moscow ML](https://en.wikipedia.org/wiki/Moscow_ML) is getting old.  Can we modernize it?  Can we make it faster?

Maybe we can.  The Zinc Oxide Experiment is an attempt to do just that.
It consists of a new VM, called [ZnO](znovm/), that is morally compatible with Moscow ML bytecode.
The new VM uses a smaller and slightly simpler instruction set in order to make the code
cleaner and smaller.  There are automatic translators from the bytecode used in many
versions of Moscow ML.

The new VM starts out as a dead simple VM so we can measure how much of a performance
loss it is to use the simpler instructions.  My guess is, not a lot.

After it is up and running with a profiler and a debugger, I expect to turn it into
a tracing JIT to see how much faster it can get while keeping the code small and sweet.

Blablabla
