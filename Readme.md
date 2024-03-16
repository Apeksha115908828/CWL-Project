Formal Verification of PBFT

This project is to write the PBFT protocol in distalgo and perform the formal verification of the safety and liveness properties of the PBFT protocol.

Setup:
Install python 3.78
then install distalgo using pip

\$ pip3 install pyDistAlgo

create virtual environment
go to cd . and activate the venv created:

\$ source bin/activate

to execute, go to the folder pbft

\$ cd pbft

\$ python -m da orig.da

PBFT:
The Practical Byzantine Fault Tolerance (PBFT) algorithm is a state machine replication protocol designed to tolerate Byzantine faults in distributed systems. It ensures both liveness and safety as long as fewer than one-third of the replicas are faulty. PBFT operates in asynchronous systems, incorporating optimizations to achieve efficient performance and providing a practical solution for Byzantine fault tolerance in real-world applications.

![PBFT](//assets/pbft.png?raw=true "PBFT")

File: pbft/orig.da has implementation for pbft using distalgo, the current is checking for basic properties such as for f faulty nodes, each server should receive 2 * f + 1 requests before it can move to the next stage. The current implementation is not complete, I will continue working on this file to move to the next stage.

DistAlgo is a language that lets you write and run distributed algorithms easily and quickly. We are using distalgo language for our implementation with reference to the work defined in [4].



References:

[1]Miguel Castro and Barbara Liskov, Practical Byzantine Fault Tolerance https://www.pmg.csail.mit.edu/papers/osdi99.pdf (February 1999)

[2]Distalgo implementation: https://github.com/DistAlgo/distalgo

[3]Paxos with distalgo: https://github.com/DistAlgo/distalgo/blob/master/da/examples/lapaxos/orig.da

[4]Distalgo tutorial: https://drive.google.com/file/d/1nyG_XOAEtiOd7DboI2HSkWa90jDfIY6O/view

[5]ACM PODC 2019 Tutorial: https://drive.google.com/file/d/1uzxBVK2AQjnnx1E1fo5X4wZtSdXfNYKT/view

[6]Saksham Chand, Yanhong A. Liu & Scott D. Stoller, Formal Verification of Multi-Paxos for Distributed Consensus https://link.springer.com/chapter/10.1007/978-3-319-48989-6_8 (11 Nov 2019)