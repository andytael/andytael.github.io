---
title: "Classless Networks"
summary: Read about Classless Networks
date: March 20, 2024
aliases: ["/classless_networks"]
tags: ["Classless", "Network"]
author: ["Andy Tael"]
---
## CIDR Available Hosts

The formula to calculate the number of assignable IP address to CIDR networks is to subtract the number of network bits from 32. Raise 2 to that power and subtract 2 for the network and broadcast addresses. For example, a /24 network has 232-24 – 2 addresses available (28 – 2 = 254) for host assignment.

As the table indicates, two /29 networks equals a /28 network. Two /28 networks equals a /27 network. Two /27 networks equals a /26 network. And so on, and so on. The notion of combining two smaller networks into a larger one is another benefit of classless networks named supernetting. In order to create a supernet the smaller networks must be contiguous. For example, 192.0.2.240/29 and 192.0.2.248/29 can form a supernet 192.0.2.240/28, but 192.0.2.240/29 and 192.0.2.8/29 could not.

## CIDR Available Networks (subnets)

How many /24 networks fits into a /18 network? The shortcut to calculate this is easy: 

24 – 18 = 6 
26 = 64 
As the example shows, 64 /24 networks fits into a /28 network. 

How many /29 networks fits into a /24 network?

29 – 24 = 5 
25 = 32
/24 network can be divided into 32 /29 networks

