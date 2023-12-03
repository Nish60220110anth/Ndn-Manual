# What is ndnSIM?

## Module Description

In this module, we will learn about the ndnSIM simulator. What are main some of the features provided by the ndnSIM simulator that 
makes it a good choice for NDN research.

## Procedure

1. ndnSIM is a module that adds NDN to the NS-3 simulator to simulate NDN networks. We can use other types of networks as well but what makes ndnSIM a good choice for NDN research is the fact that it is a discrete-event network simulator, which means that it is a simulator that operates on discrete events.

2. ndnSIM is written in C++ and provides a Python binding. This makes it easy to use and extend.

3. ndnSIM also provides a lot of models for different types of networks and protocols.

4. The main ideology behind ndnSIM is to provide flexibility to the user. I can technically use any type of network topology, any type of routing protocol, any type of forwarding strategy, any type of application, and any type of traffic generator.

Even i can simulate a network in my local system using NFD daemon and then use that network to simulate my application.

In further modules, we will learn how ndnSIM sits of top of NS-3, what are main components in ns-3 which is important to understand to use ndnSIM, and how to use ndnSIM to simulate NDN networks.