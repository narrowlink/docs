The client allows you to easily set up port forwarding for RDP (Remote Desktop Protocol) connections, enabling you to connect to a remote machine using RDP even when behind a restricted NAT network.

Follow the steps below to configure port forwarding for RDP with Narrowlink client:

- [Install Narrowlink](/getting-started/installation/#cargo)

- Execute the following command, replacing the placeholder values with your actual values:

    `narrowlink forward -k <secret> -n <agent_name> -l <local_ip>:<local_port> <remote_ip>:<remote_port>` 

    -   `<secret>`: The passphrase for encryption. Choose a strong and secure passphrase.
    -   `<agent_name>`: The name of the agent. Choose a descriptive name for easy identification.
    -   `<local_ip>`: The local IP address you want to bind for forwarding. This is the IP address of your local machine.
    -   `<local_port>`: The local port number you want to use for forwarding. Choose an available port number.
    -   `<remote_ip>`: The IP address of the remote machine running a service.
    -   `<remote_port>`: The port number of the remote machine.

    For example, to forward RDP traffic from a remote machine's IP address 192.168.1.200 to your local machine with IP address 127.0.0.1, you would use the following command:

    `narrowlink forward -k mysecret -n office -l 127.0.0.1:3389 192.168.1.200:3389` 

-  You can now use your RDP client to connect to the local IP address and port number you specified in the command, which will forward the RDP traffic to the remote machine and establish the RDP connection.
   

That's it! You have successfully set up port forwarding for RDP using the Narrowlink client. Enjoy seamless remote desktop access to your remote machine even when behind a restricted NAT network!
