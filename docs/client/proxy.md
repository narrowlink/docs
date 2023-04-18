The Narrowlink client provides a simple way to set up a SOCKS proxy, allowing you to access the internet through a designated machine, even when both machines are behind a restricted NAT network.

The client allows you to easily set up a SOCKS proxy to access the internet through a designated machine even when both machines are behind a restricted NAT network.

Follow the steps below to configure a SOCKS proxy with the Narrowlink client:


- [Install Narrowlink](/getting-started/installation/#cargo)

- Execute the following command, replacing the placeholder values with your actual values:

    `narrowlink proxy -k <secret> -n <agent_name> <local_ip>:<local_port>` 

    -   `<secret>`: The passphrase for encryption. Choose a strong and secure passphrase.
    -   `<agent_name>`: The name of the agent. Choose a descriptive name for easy identification.
    -   `<local_ip>`: The local IP address you want to bind socks proxy server for forwarding network traffic.
    -   `<local_port>`: The local port number you want to bind socks proxy server for forwarding network traffic.
    
    For example, to forward your network traffic to your remote machine with the name of `office`, you would use the following command:

    `narrowlink p -n office -l 127.0.0.1:1080` 

-  You can now use your RDP client to connect to the local IP address and port number you specified in the command, which will forward the RDP traffic to the remote machine and establish the RDP connection.
   

That's it! You have successfully set up a proxy server that can forward your network connections to your remote machine even when behind a restricted NAT network!
