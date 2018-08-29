The following are required prerequisites:

* The Kvaser CANLIB API (https://www.kvaser.com/downloads/)
    * For Ubuntu 14.04/16.04 - Latest version (tested with at least v5.20.814)
    * For Linux kernel 4.13 or higher, version 5.21 of CANLIB is required (click the Tux on the right of the downloads page)
* `can_msgs`


**TOPICS**

*can_tx* [can_msgs::Frame]

This topic is published by the node. It expects to have other nodes subscribe to it to receive data which are *sent by the CAN device*.

*can_rx* [can_msgs::Frame]

This topic is subscribed to by the node. It expects to have data published to it which are intended to be *received by the CAN device*.

**PARAMETERS**

*~can_hardware_id*

This is the Kvaser Hardware ID (serial number) of the connected device.

*~can_circuit_id*

This is the 0-based index of the channel number *on the specific hardware device* designated by the *~can_hardware_id*.

*~can_bit_rate*

This is the communication rate to be used on the CAN channel in bits per second.
# Kvaser_reader
