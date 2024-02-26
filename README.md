# TDD_SlotConfiguration
In 5G NR, slot configuration can be done in a static, semi-static or fully dynamic fashion. The Static and  semi-static slot configuration is done using RRC while dynamic slot configuration is done using PDCCH  DCI. 
The rapid evolution of wireless communication technologies has led to the advent of 5G NR, promising unparalleled data rates, lower latency, and enhanced network efficiency. This study delves into slot configuration in 5G NR, studying its impact on system performance, resource utilization, and overall network capabilities. In 5G NR, slot configuration can be done in a static, semi-static or fully dynamic fashion. The Static and 
 semi-static slot configuration is done using RRC while dynamic slot configuration is done using PDCCH DCI.

## Slot Formats
A slot can be classified as downlink (all symbols are dedicated for downlink) or uplink (all symbols are 
dedicated for uplink) or mixed uplink and downlink transmissions. In the case of FDD, all symbols within a 
slot for a downlink carrier are used for downlink transmissions and all symbols within a slot for an uplink 
carrier are used for uplink transmissions. 
5G TDD uses flexible slot configuration. OFDM symbols in a slot can be classified as 'downlink', 'flexible', 
or 'uplink'. Flexible symbol can be configured either for uplink or for downlink transmissions. Like LTE TDD 
system, a guard period is necessary for transceiver switching from downlink to uplink and to allow timing 
advance in the uplink. 
In LTE TDD, UL/DL configuration provided via SIB1 informs UEs that a subframe is used for uplink, downlink 
or as a special subframe. The configuration of special subframe is also provided via SIB1. In 5G, the 
configuration of slot format can be done in static, semi-static or fully dynamic fashion. Static and semistatic slot configuration is done using RRC while dynamic slot configuration is done using PDCCH DCI.
This is discussed in the upcoming sections. 
Now we will go through a deep study for 5G slot configuration.

# Slot Configuration
As we mentioned above A slot format includes downlink symbols, uplink symbols, and flexible symbols.
NR supports the slot configuration in static, semi-static or fully dynamic fashion. In TDD, for small/isolated 
cells, dynamic TDD is suitable to adapt to traffic variations, while for large cells, semi-static TDD may be 
more suitable for handling interference issues than fully dynamic TDD. 
Slot configuration via RRC (static and semi static) consists of two parts. First part is configured by the tddUL-DL-ConfigurationCommon, and second part is configured by the tdd-UL-DL-ConfigurationDeticated.
