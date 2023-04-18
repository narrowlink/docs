The Narrowlink client can acts like `netcat` command to connect to the services that are running on the agent network machine. It is useful for various porpurses such as connecting to a ssh server behind a restricted NAT network by using official ssh client.

Follow the steps below to connect to a ssh server by using narrowlink and official ssh client:


- [Install Narrowlink](/getting-started/installation/#cargo)

- Add the bellow setting to your ssh client configuration which is normally at `~/.ssh/config` to use narrowlink to conenct to your machines:

```
Host <agent>
    ProxyCommand narrowlink connect -n <agent> %h:%p
    HostName 127.0.0.1
    Port 22
    User <username>
    #StrictHostKeyChecking no #optional to ignore host key checking
    #UserKnownHostsFile=/dev/null #optional to ignore host key checking
```

Replace `<agent>` with the name of the machine you want to connect to, `<username>` with your actual username.

-  You can now use `ssh office` command to connect to the office machine.
   

That's it!