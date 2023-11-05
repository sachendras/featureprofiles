# GNMI-2: gnmi_subscriptionlist_test

## Summary
This is to test for subscription to multiple paths with different Subscription modes in a single request using Subscriptionlist. Goal here is to ensure that the NOS supports "Subscriptionlist" and also supports the desired subscriptionmodes per path.

## Procedure
  * Send a single Subscription request to the DUT with a **SubcriptionList** and **SubscriptionMode** matching the "Telemetry Parameter Coverage section below
  * Ensure that the implementation successfully allows subscription to all the paths mentioned below.


## Telemetry Parameter Coverage

  * SubscriptionMode: ON_CHANGE
    * /interfaces/interface/state/admin-status
    * /lacp/interfaces/interface/members/member/interface
    * /interfaces/interface/ethernet/state/macaddress
    * /interfaces/interface/state/hardware-port
    * /interfaces/interface/state/id
    * /interfaces/interface/state/oper-status
    * /interfaces/interface/ethernet/state/port-speed
    * /components/component/integrated-circuit/state/node-id
    * /components/component/state/parent
    * /components/component/state/oper-status
    * /interfaces/interface/state/forwarding-viable
  * SubscriptionMode: TARGET_DEFINED
    * /interfaces/interface/state/counters/in-unicast-pkts
    * /interfaces/interface/state/counters/in-broadcast-pkts
    * /interfaces/interface/state/counters/in-multicast-pkts
    * /interfaces/interface/state/counters/out-unicast-pkts
    * /interfaces/interface/state/counters/out-broadcast-pkts
    * /interfaces/interface/state/counters/out-multicast-pkts
    * /interfaces/interface/state/counters/in-octets
    * /interfaces/interface/state/counters/out-octets
    * /interfaces/interface/state/counters/in-discards
    * /interfaces/interface/state/counters/out-discards
    * /interfaces/interface/state/counters/in-errors
    * /interfaces/interface/state/counters/out-errors
    * /interfaces/interface/state/counters/in-fcs-errors
    * /qos/interfaces/interface/output/queues/queue/state/transmit-pkts
    * /qos/interfaces/interface/output/queues/queue/state/transmit-octets
    * /qos/interfaces/interface/output/queues/queue/state/dropped-pkts
    * /components/component/integrated-circuit/backplane-facing-capacity/state/available-pct
    * /components/component/integrated-circuit/backplane-facing-capacity/state/consumed-capacity
    * /components/component/integrated-circuit/backplane-facing-capacity/state/total”
    * /components/component/integrated-circuit/backplane-facing-capacity/state/total-operational-ca
pacity
