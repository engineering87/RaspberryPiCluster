# Install Go language environment

Download the archive from https://golang.org/doc/install and extract it into /usr/local, creating a Go tree in /usr/local/go.

```tar -C /usr/local -xzf go1.15.5.linux-amd64.tar.gz```

Add /usr/local/go/bin to the PATH environment variable.
You can do this by adding the following line to your $HOME/.profile or /etc/profile (for a system-wide installation):

```export PATH=$PATH:/usr/local/go/bin```

Note: Changes made to a profile file may not apply until the next time you log into your computer. To apply the changes immediately, just run the shell commands directly or execute them from the profile using a command such as source $HOME/.profile. Verify that you've installed Go by opening a command prompt and typing the following command:

```$ go version```

Confirm that the command prints the installed version of Go.

# Install Ethereum

```$ git clone https://github.com/ethereum/go-ethereum.git```

# Running an Ethereum Light Node 

```$ geth –cache=218 –syncmode “light”```
