# Labs, Websites and blogs

* [The Chair of Network Architectures and Services](https://www.net.in.tum.de) 
Technical University of Munich , 
In research and teaching we focus on components, methods and systems of digital telecommunication and networking. The general term for all these fields is telematics (the combination of telecommunication and informatics).

The chair is active in the following research areas:

* Network Security
* Blockchain Technology
* Information Privacy
* Traffic Measurement and Analysis
* Software Defined Networking
* Future Internet
* Peer-to-Peer and Overlay Networks
* Autonomic Networks / Self-Management
* Wireless Networks
* Resilience

# Packet Process

## DPDK
* [DPDK](http://dpdk.org/) DPDK is a set of libraries and drivers for fast packet processing.
* [DPDK Summit](https://dpdksummit.com/) DPDK Summit Userspace is a community event focused on software developers who contribute to or use DPDK.
* [Packetgraph ](https://github.com/outscale/packetgraph)  Packetgraph is a library aiming to give the user a tool to build networks graph easily, It's built upon the fast DPDK library.

## eXpress Data Path
* [XDP](https://www.iovisor.org/technology/xdp)  XDP or eXpress Data Path provides a high performance, programmable network data path in the Linux kernel as part of the IO Visor Project. XDP provides bare metal packet processing at the lowest point in the software stack which makes it ideal for speed without compromising programmability. Furthermore, new functions can be implemented dynamically with the integrated fast path without kernel modification

## Packet Generator

* [TRex](https://trex-tgn.cisco.com/)  TRex is an open source, low cost, stateful traffic generator fuelled by DPDK. It generates L4-7 traffic based on pre-processing and smart replay of real traffic templates. TRex amplifies both client and server side traffic and can scale to 200Gb/sec with one UCS.
* [pktgen-dpdk](http://dpdk.org/browse/apps/pktgen-dpdk)  Traffic generator powered by DPDK
* [MoonGen](https://github.com/emmericp/MoonGen) MoonGen is a fully scriptable high-speed packet generator built on DPDK and LuaJIT. It can saturate a 10 Gbit/s connection with 64 byte packets on a single CPU core while executing user-provided Lua scripts for each packet. Multi-core support allows for even higher rates. It also features precise and accurate timestamping and rate control.

## Wrappers
* [PcapPlusPlus](http://seladb.github.io/PcapPlusPlus-Doc/index.html)  PcapPlusPlus is a multiplatform C++ network sniffing and packet parsing and crafting framework. PcapPlusPlus is meant to be lightweight, efficient and easy to use. It's a C++ wrapper for popular engines like libpcap, WinPcap, DPDK and PF_RING
  * [Github](https://github.com/seladb/PcapPlusPlus)
* [dpdk adapter](https://github.com/PLVision/dpdkadapter)

## [ixy](https://github.com/emmericp/ixy)  a userspace network driver in 1000 lines of code

ixy is a simple userspace packet processing framework. It takes exclusive control of a network adapter and implements the whole driver in userspace. Its architecture is similar to DPDK and Snabb and completely different from (seemingly similar) frameworks such as netmap, pfq, pf_ring, or XDP (all of which rely on kernel components).

# Network Stack

* [F-Stack](http://www.f-stack.org/)  F-Stack is an user space network development kit with high performance based on DPDK, FreeBSD TCP/IP stack and coroutine API. 
  * [Github](https://github.com/F-Stack/f-stack)
* [mTCP](https://github.com/eunyoung14/mtcp)  A Highly Scalable User-level TCP Stack for Multicore Systems
* [libuinet](https://github.com/pkelsey/libuinet)  a library version of FreeBSD's TCP/IP stack plus extras
* [mirage-tcpip](https://github.com/mirage/mirage-tcpip)  TCP/IP networking stack in pure OCaml, using the Mirage platform libraries. Includes Ethernet, DHCP, ARP and TCP/IPv4 support. https://mirage.io
* [lwIP](http://savannah.nongnu.org/projects/lwip/)  lwIP is a small independent implementation of the TCP/IP protocol suite that has been initially developed by Adam Dunkels and is now continued here. 
* [net-next-nuse](https://github.com/libos-nuse/net-next-nuse)  Network Stack in Userspace
* [OpenOnload](http://www.openonload.org/) OpenOnload® is a high performance network stack from Solarflare that dramatically reduces latency and cpu utilisation, and increases message rate and bandwidth. OpenOnload runs on Linux and supports TCP/UDP/IP network protocols with the standard BSD sockets API, and requires no modifications to applications to use. It achieves performance improvements in part by performing network processing at user-level, bypassing the OS kernel entirely on the data path. Networking performance is improved without sacrificing the security and multiplexing functions that the OS kernel normally provides.
* [ustack](https://github.com/jiakai1000/ustack)  user space TCP/IP stack based on DPDK
* [dpdk-ans](https://github.com/ansyun/dpdk-ans)  ANS(Accelerated Network Stack) on DPDK, DPDK native TCP/IP stack.
  * [dpdk-nginx](https://github.com/ansyun/dpdk-nginx)  Fork from official nginx-1.9.5, and run on the dpdk user space TCP/IP stack(ANS"accelerated network stack").
  * [dpdk-redis](https://github.com/ansyun/dpdk-redis)  Fork from official redis-3.0.5, and run on the dpdk user space TCP/IP stack(ANS).
  * [dpdk-iperf](https://github.com/ansyun/dpdk-iperf) Fork from official iperf-3.1.3, and run on the dpdk user space TCP/IP stack(ANS).


# Complex

* [Seastar](http://www.seastar-project.org/)  Seastar is an advanced, open-source C++ framework for high-performance server applications on modern hardware. Seastar is used in ScyllaDB, a high-performance NoSQL database compatible with Apache Cassandra. Applications using Seastar can run on Linux or OSv.
  * [Github](https://github.com/scylladb/seastar)
* [Vector Packet Processing (VPP)](https://fd.io)  What is VPP? Is it a software router? A virtual switch? A virtual network function? Or,something else? In fact it is all of the above and a whole lot more. It is a modularizedand extensiblesoftware framework for building bespoke network data plane applications. And equally importantly, VPP code is written for modern CPU compute platforms (x86_64, ARMv8, PowerPC,to name a few), with a great deal of care and focus given to optimizing the software-hardware interface for real-time,network I/O operations and packet processing.
* [lagopus](https://github.com/lagopus/lagopus)  Lagopus software switch is a yet another OpenFlow 1.3 software switch implementation. Lagopus software switch is designed to leverage multi-core CPUs for high-performance packet processing and fowarding with DPDK. Many network protocol formats are supported, such as Ethernet, VLAN, QinQ, MAC-in-MAC, MPLS and PBB. In addition, tunnel protocol processing is supported for overlay-type networking with GRE, VxLAN and GTP.
* [Open vSwitch](https://github.com/openvswitch/ovs)  Open vSwitch is a multilayer software switch licensed under the open source Apache 2 license. Our goal is to implement a production quality switch platform that supports standard management interfaces and opens the forwarding functions to programmatic extension and control.
* [Snabb](https://github.com/snabbco/snabb)  Snabb (formerly "Snabb Switch") is a simple and fast packet networking toolkit.
* [xDPd](https://github.com/bisdn/xdpd)  "The OpenFlow eXtensible DataPath daemon (xDPd) is a multi-platform, multi OF version, open-source datapath built focusing on performance and extensibility."  xDPd can also be considered a framework for building OpenFlow datapath elements, as it is designed to be easily extended with the support of new forwarding devices.
* [butterfly](https://github.com/outscale/butterfly)  Butterfly connects Virtual Machines and control their traffic flow
* [ostinato](http://ostinato.org/)  Network Traffic Generator and Analyzer

# Application

* [Rspamd](https://rspamd.com/)  Rspamd is an advanced spam filtering system that allows evaluation of messages by a number of rules including regular expressions, statistical analysis and custom services such as URL black lists. Each message is analysed by Rspamd and given a spam score.
  * [Github](https://github.com/vstakhov/rspamd)





