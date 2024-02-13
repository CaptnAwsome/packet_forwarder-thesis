This repository is part of a Project used in a thesis about LoRaWAN.

It runs on the basis of Semtech's packet forwarder https://github.com/Lora-net/packet_forwarder and in addition allows to delay LoRaWAN uplink communication or to block LoRaWAN downlink communication.

Options:
While the program is running, the following commands can be entered:

U  /  u       :  to enable the uplink delay for the next packet (all others are dropped)

D  /  d       :  to enable the downlink blocking -> no downlinks are propagated

B  /  b       :  to activate both

Anything else : deactivate both

Example:
If both the delaying and the blocking are active and you type D, only the downlink communication blocking will stay active.

Remarks - 13.02.2024:
Although the commit "cd7f202" makes it seem like I wrote a lot of logic in the function "delayed_uplink", most of it is the basic "uplink" function but copied into a new method with added logic/constraints for sending packets. Correspondingly, the same holds for commit 80f399c and the function "blocked_downlink", a modified form of the basic "downlink" function.
