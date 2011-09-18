OneWire Agent
=============

An experiment in making a simple agent that is non-monolithic. The agent will read and control sensors and switches on a 1-Wire network. The components will run separately and collaborate via a message bus and database.

Status
------

Brand new! No files yet.

Architecture Choices
--------------------

Hmm. Interesting question. The whole point is to experiment with these very choices, so there are multiple approaches to be tried over the course of the experiment. All should be available in the code base with the 'active' choices selected from a config file at runtime.

- 1-Wire interface: owserver
- Message passing: 1) rabbitmq, 2) 0mq, 3) Resque
- Raw data capture: RRD
- Database: 1) MySQL, 2) Redis
