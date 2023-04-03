#Architecture 

Narrowlink is composed of three primary components that facilitate NAT traversal, as illustrated in the accompanying diagram and described below.
<figure markdown>
![Narrowlink System Architecture](/assets/Diagram.svg) <figcaption>System Architecture</figcaption>
</figure>

##[Client]
The client component of Narrowlink is responsible for sending and receiving packets to or from end users and forwarding them to the Narrowlink network infrastructure. This component is typically installed on the end user's device or server, and it communicates with the Agent component to facilitate NAT traversal.

##[Agent]
The agent component acts as a proxy that sends and receives packets on behalf of the client to or from the targeted hosts that can be on the same machine or network. This component is responsible for managing the NAT traversal process and ensuring that packets are correctly forwarded between the client component. The agent component can be installed on a server or a virtual machine in the cloud, depending on the use case.

##[Gateway]
The gateway component of Narrowlink is responsible for routing packets between the agents and clients and enforcing access control policies. This component is usually deployed on a public-facing server in the cloud and acts as the entry point into the Narrowlink network. The gateway component provides load balancing and redundancy features to ensure high availability and fault tolerance. Additionally, it can receive HTTP/S requests directly without client intervention and forward them to the appropriate agent to publish a web service behind the NAT network.

[Client]: /client/introduction/
[Agent]: /agent/introduction/
[Gateway]: /gateway/introduction/