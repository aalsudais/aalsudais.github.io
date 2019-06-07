---
layout: inner
title: Research
permalink: /research
---




#### Current Projects

- <span style="color:teal; font-size:11pt;">**Homing Geo-distributed Network Services**</span> -- Network service providers (NSPs) typically run geo-distributed network infrastructures to
better serve their clients' needs.
Network services offered by NSPs consist of virtual network functions (VNFs) and policies of how such network functions should be deployed.
In addition to the geo-distributed nature of the infrastructure, the ever evolving requirements impose an additional challenge.
Thus, we need an extensible framework that can (and should) accommodate new requirements on the fly. We design such framework that can flexibly
serve complex homing requests and formulate the homing problem using binary quadratic programming (BQP) and implement an incremental solution to the problem.

#### Previous Projects

- <span style="color:teal; font-size:11pt;">**Scalable Search Service for Geo-distributed Systems**</span> -- Finding nodes which match certain criteria, based on potentially highly dynamic information, is a critical need
in many distributed systems, ranging from cloud management, to network service deployments, to emerging IoT applications.
With the increasing scale, dynamicity, and richness of data, existing systems, which typically implement a custom solution
based around message queues where nodes push status to a central database, are ill-suited for this purpose. To this end,
we present FOCUS, a general and scalable service which easily integrates into existing and emerging systems to provide this
fundamental capability. FOCUS utilizes a gossip-based protocol for nodes to organize into groups based on attributes and
current value. With this approach, nodes need not synchronize with a central database, and instead the FOCUS service only
needs to query the sub-set of nodes which have the potential to positively match a given query. We show FOCUS’s flexibility
through an operational example of complex querying for Virtual Network Functions instantiation over cloud sites, and illustrate
its ease of integration by replacing the push-based approach in OpenStack’s placement service. Our evaluation demonstrates a
5-15x reduction in bandwidth consumption and an ability to scale much better than existing approaches.
<br />
**Publications**: [FOCUS (IEEE ICDCS'19)](files/papers/focus.pdf) and [NodeFinder (Usenix HotCloud'18)](files/papers/nodefinder_hotcloud18.pdf)
<br />&nbsp;
- <span style="color:teal; font-size:11pt;">**Automated Network Management using Natural Language**</span> -- In this work, we introduce Natural Language Processing to network management by leveraging the capabilities of
Natural Language Processing tools, such as speech recognition and text parsing, to extract useful information to build network
tasks. We propose an intermediate network-agnostic layer that acts as the medium between natural language input (spoken
or written) and different network implementations. We have leveraged the programmability that Software Defined Networks
(SDN) offers to build a prototype tool that takes natural language text as an input and uses it to build abstract tasks. Such tasks
are then passed to a network controller to be performed in real time. To our knowledge, this is the first work that provides such
interface between network users (in the form of natural language) and different network systems. This work is along the lines of the now trending theme of "intent-based networking" (IBN).
<br />
**Publications**: [HeyNet: (IEEE INFOCOM WORKSHOPS'17)](files/papers/HeyNet.pdf)
<br />&nbsp;
- <span style="color:teal; font-size:11pt;">**Sateless Network Functions**</span> -- In this work, we propose Stateless Network Functions, a new architecture for network functions virtualization,
where we decouple the existing design of network functions into a stateless processing component along with
a data store layer. In breaking the tight coupling, we enable a more elastic and resilient network function infrastructure. Our StatelessNF processing instances are
architected around efficient pipelines utilizing DPDK for high performance network I/O, packaged as Docker
containers for easy deployment, and a data store interface optimized based on the expected request patterns to efficiently access a RAMCloud-based data store.
A network-wide orchestrator monitors the instances for load and failure, manages instances to scale and provide
resilience, and leverages an OpenFlow-based network to direct traffic to instances. We implemented three example network functions (network address translator, firewall, and load balancer). Our evaluation shows (i) we are able to reach a throughput of 10Gbit/sec, with an added
latency overhead of between 100µs and 500µs, (ii) we are able to have a failover which does not disrupt ongoing traffic, and (iii) when scaling out and scaling in we
are able to match the ideal performance.
<br />
**Publications**: [StatelessNF: (Usenix NSDI'17)](files/papers/stateless.pdf)
