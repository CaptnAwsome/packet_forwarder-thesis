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
