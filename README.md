# Benchtop Waggle Driver (BWD)

#### Lead: Sean Shahkarami
### Overview:
When a physical Waggle node is “hosted”, it is attached to a Linux system that can test and operate the node.  Waggle nodes that are part of Chameleon or a nightly test harness are managed by the BWD.  The BWD provides a remotely controllable interface to a physical Waggle node.

### Requirements:
The BWD should control as many physical attributes of the Waggle node as possible, including the serial console.  Ideally, almost everything that can be done physically, while a node sits on a desk, can be done remotely via the BWD.  Separation of privileged and user modes might be helpful for protecting the node from destruction or actions that cannot be recovered without physical access.

### Use Cases:

#### Waggle node shipped to developer:
* Node is “unboxed” and plugged in on a developers desk.
* Following the instructions and using the tools of the BWD, the developer logs in and begins testing and developing new code

#### Waggle node is hosted on Chameleon:
* Developer receives 10 Waggle nodes.
* The nodes are attached via Ethernet and serial cables to Chameleon modes.
* Users may then request a “job” be run on the Linux nodes hosting a Waggle.
* Users may then directly interact with the node.

###  Milestones:
* Publish design document
* 8 Waggle nodes deployed into Chameleon and available for reservations and use
* Release BWD V1.0 with support for desktop kits
