### Bird routing daemon

## What is it ?

On UNIX-like operating systems the term "daemon" refers to a long running program that performs some service. Generally started by the systems startup scripts and stopped by it's shutdown scripts.

A routing daemon is a daemon that implements a routing protocol. It sends and receives routes from other routers and uses them to update the routing table in the kernel

## BGP

BGP is, quite literally, the protocol that makes the internet work. BGP is short for Border Gateway Protocol and it is the routing protocol used to route traffic across the internet. Routing Protocols (such as BGP, OSPF, RIP, EIGRP, etc...) are designed to help routers advertise adjacent networks and since the internet is a network of networks, BGP helps to propagate these networks to all BGP Routers across the world.

## BGP Peering

Two routers that have established connection for exchanging BGP information, are referred to as BGP peers. Such BGP peers exchange routing information between them via BGP sessions that run over TCP, which is a reliable, connection oriented & error free protocol. Bird helps to establish such networks.

## Configuration file

 Path : ```/etc/bird/bird.conf```
 
## Commands

Find status of running daemon

```service bird status```

Start/Stop/Restart bird daemon

```service bird start/stop/restart```

Show routing table in real-time

```birdc show route```
