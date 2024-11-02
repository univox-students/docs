### Step 0: Pre-requisites
You should install the following

- [FortiClient](https://www.fortinet.com/support/product-downloads), and
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
- Please also ask them to provide instruction on how to connect to the College VPN, including the **custom port** needed.

Failure to follow the above instruction may result in delays for you having access to the College server, as the College IT officer will have to take extra steps to verify your identity. Please also follow any further instructions from the College IT officer.

At the end, you should receive account details for logging you into the College server.

!!! tip
    
    You may not have access to the External Affairs email at this point, for which case you may find it more convenient to ask the current/previous committee request both access to the WCR External Affairs email and the College server at the same time.


## Step 2: Logging in to the College server.

1. Access to the server is only available via VPN provided by the FortiClient. You can add a new connection with the following details.

    - **Remote gateway:** `vpn.univ.ox.ac.uk`
    - **Port:** (to be emailed from the College IT office)

1. Login to FortiClient using the following credential

    - **Username:** University sortcode `univXXXX`
    - **Password:** University WiFi password. If you forget the password, you can reset it by [visiting the University self-registration website](https://register.it.ox.ac.uk/self/index).

1. In Visual Studio Code, navigate yourself to the **Remote Explorer** to establish a new connection. You should use the command
```
ssh wcr.univ.ox.ac.uk
```
The Visual Studio Code will open a new window, after which you will then be prompted to login to the server. Please use the following credentails:

    - **Username:** University sortcode `univXXXX`
    - **Password:** Password provided by the College IT Officer.

4. You should now have access to the College server.

