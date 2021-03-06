# Oddlab
Oddlab (Odds labels) is a deployable traffic engineering approach for ensuring the quality of service (QoS) of multi-rooted data center (DC) traffic in both symmetric and asymmetric modes. We used  Openflow switches statistics, such as residual bandwidth and the number of mounted flows, to create a heuristic model based on concepts for avoiding bottleneck links and rerouting trapped elephant flows. Our preliminary findings show that Oddlab reduce Flow Completion Time (FCT), increase bisection bandwidth, increase network utilization, and reliably identify broken ties, all of which boost the DC's productivity.

# Implementation
Oddlab is a python program that runs on the Ryu controller and builds a multi-rooted K-4 fat-tree DCN using mininet as a real-time network emulator and the OpenFlow protocol 1.3. The testbed has 16 hosts connected to twenty-four-port OpenFlow switches, each of which comprises four pods with four core switches. To maintain connection precision in the mininet's real-time environment, the link capacity through the DCN is set to 10 Mbps.

* The work has been published as a paper in the Annals of Telecommunications journal (Springer Nature).

Alawadi, A.H., Molnár, S. Oddlab: fault-tolerant aware load-balancing framework for data center networks. Ann. Telecommun. (2021). https://doi.org/10.1007/s12243-021-00898-0
