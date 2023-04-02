# Installation

Narrowlink can be installed in the following three ways:

 - Installing via Cargo (Recommended)
 - Downloading the precompiled binary from the website
 - Installing from the source code

Each component of Narrowlink has an individual binary and package name with specific functionalities:

 - `narrowlink` represents the [Client] component
 - `narrowlink-agent` represents the [Agent] component
 - `narrowlink-gateway` represents the [Gateway] component.


##Cargo
Cargo is a package manager for the Rust programming language. It simplifies the process of managing Rust packages and their dependencies.
###Prerequisite
To install Narrowlink using Cargo, you must first install Cargo. On macOS, Linux, or another Unix-like system, you can run the following command in your terminal:

```curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh```

If you're using Windows, please refer to the "[Other Installation Methods]" section on the Rust website.

### Client
```cargo install narrowlink```
### Agent
```cargo install narrowlink-agent```
### Gateway
```cargo install narrowlink-gateway```

##Precompiled Binary
If you prefer to use precompiled binaries, they are available on the GitHub release page. Currently, we provide binaries for Linux, macOS, and Windows platforms for both ARM and x86 architectures. However, it's worth noting that Narrowlink is not limited to these platforms - you can build for other targets using alternative installation methods.
### Client
```https://github.com/narrowlink/client/releases```
### Agent
```https://github.com/narrowlink/agent/releases```
### Gateway
```https://github.com/narrowlink/gateway/releases```

##Source Code
If you prefer to obtain pre-release versions of Narrowlink or modify the code before building, you can download the source code from [Narrowlink's GitHub repository] and build and install it yourself. This installation method requires the Git and Cargo commands to be installed on your system.



[Client]: /client/introduction/
[Agent]: /agent/introduction/
[Gateway]: /gateway/introduction/
[Other Installation Methods]: https://forge.rust-lang.org/infra/other-installation-methods.html
[Narrowlink's GitHub repository]: https://github.com/narrowlink/