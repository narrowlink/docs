
# Client

The Narrowlink client is a versatile and powerful tool that offers a wide range of features to access net network resource by connecting to the agent thorough of the gateway. From setting up sock proxy servers to connecting to share internet access of a computer behind of a net network to connect their services like RDP and SSH, It also offers end-to-end encryption based on Xchacha20 and SHA3 for enhanced security.

In this documentation, we will provide an overview of the Narrowlink client, its features, and practical examples of how it can be used in different scenarios. We will also cover installation instructions, configuration steps, and compliance considerations to ensure proper usage of Narrowlink in accordance with applicable laws and regulations.

Whether you are a network administrator, developer, or an open-source enthusiast, the Narrowlink client offers a flexible and powerful solution for managing your network configuration needs. Let's dive in and explore the capabilities of Narrowlink client for your networking requirements.

## Features of Narrowlink Client

-   Sharing internet access of computer behind NAT networks.
-   Connecting to private network services like RDP and SSH.
-   End-to-end encryption based on Xchacha20 and SHA3.
-   Remote address autnetication by using HMAC.

## Practical Examples

Here are some practical examples of how you can use Narrowlink client:

-  [Setting up a proxy server](/client/proxy/) to share internet access of another computer behind a restricted NAT network:

`narrowlink proxy -n office 192.168.1.100:8080` 

-  [Port forwarding](/client/port-forwarding/) to connect to a remote desktop service (RDP):

`narrowlink forward -n office -l 127.0.0.1:3389 127.0.0.1:3389` 

-  [Connecting to a SSH](/client/connect/) server:

```
#~/.ssh/config
Host <agent>
    ProxyCommand office connect -n <agent> %h:%p
    HostName 127.0.0.1
    Port 22
    User <username>
```
That's it! These are just a few examples of the many capabilities of Narrowlink client.

You can explore more features and options by exploring the documentation and experimenting with different command line options.
Happy networking with Narrowlink!
