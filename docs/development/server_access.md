### Step 0: Pre-requisites

!!! warning
    
    The access to the College networks has been recently been streamlined. As a result, the documentation has been updated. 

You should install the following

- **[Cisco Secure Client (for University VPN)](https://help.it.ox.ac.uk/vpn)**, and
- [Visual Studio Code](https://code.visualstudio.com)

In the Visual Studio Code, please ensure that 

- you have installed the **Remote - SSH** extension, and
- you have login using your your Github account.

!!! tip
    
    You can also install the **Github Copilot** extension if you have access to the Github Copilot (which you should if you have an education account).


### Step 1: Request access to the College server
To request access to the College server, please send a request to the College IT Support (`it@univ.ox.ac.uk`). 

- Please send the request **using the WCR External Affairs Email** (`wcr.externalaffairs@univ.ox.ac.uk`), cc'ing yourselves.
- In the email, you should provide your name and the University sortcode (in the form of `univXXXX`).

Failure to follow the above instruction may result in delays for you having access to the College server. Please also follow any further instructions from the College IT officer.

At the end, you should receive account details for logging you into the College server.

!!! tip
    
    You may not have access to the External Affairs email at this point, for which case you may find it more convenient to ask the current/previous committee request both access to the WCR External Affairs email and the College server at the same time.


## Step 2: Logging in to the College server.

1. Access to the server is only available via University VPN (`vpn.ox.ac.uk`). Please refer to the [official University guidance](https://help.it.ox.ac.uk/vpn) for details on how to sign in.

1. In Visual Studio Code, navigate yourself to the **Remote Explorer** to establish a new connection. You should use the command
```
ssh <univXXXX>@wcr.univ.ox.ac.uk
```
The Visual Studio Code will open a new window, after which you will then be prompted to login to the server. The password should have been provided by the College IT Officer.

