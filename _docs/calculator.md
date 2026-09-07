---
title:  Vector Calculator
permalink: /docs/calculator/
---

[Vector Calculator]() is the module where you define how to  calculate [Indicators]() and [Models]()

{: .note .info} 
[Sync]() definition<br>
Set how to correct gaps and wrong value of the originally captured [Source]() signal.
It is incremental process - that means only new values are checked.
Finally you assign the [Time grid]() signal. This step simulate the sampling rate for the [Sync]() signal.

{: .note .info} 
[Indicator]() definition<br>
Set the formula to calculate or shift the new [Indicator]() from two or more [Sync]() signals.
Each [Sync]() signal must have the same [Time grid]() for the calculation and the new [Indicator]()
will have also the same [Time grid]().

{: .note .info} 
[Model]() definition<br>
Model is a set of signals with same [Time grid] and can contain [Sync](), [Indicator][], [Model]() in the list with the same [Time grid]().
Additionally it can have formula to calculate new member of the set from signals in the set.
Mathematically a [Model]() is a matrix. 

