---
title: Signals
permalink: /docs/signals/
---

CutSMS [Signal]() is an abstract vector that keeps values with defined units, according to the selected [Time grid]().

There are following signals types:

{: .note .info} 
Source<br>
signal captured directly from origin
[Sources]() must be first defined in the capture module where you set [unit]() for it. 

{: .note .info} 
Sync<br>
original signal without gaps or errors synchronized with selected [Time grid]() signal.
Has the same unit as correspond [Source]() signal


{: .note .info} 
Indicator<br>
new calculated signal from minimum two [Sync]() signals (simple recursion and aggregation of information)

{: .note .info} 
Model<br>
complex calculated signal from other [Sync](), [Indicator](), [Model]() (complex recursion and aggregation of information)

{: .note .info} 
Weight<br>
technical signal kipping values from range [(-1;1)]() without defined unit synchronized to selected [Time grid]()  

{: .note .info} 
Time grid<br>
signal kipping values of time interval

See [Requirements]({{ '/docs/registration/#requirements' | relative_url }}) for guides and details.

