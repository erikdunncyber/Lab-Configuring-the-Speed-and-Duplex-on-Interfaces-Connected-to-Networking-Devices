<h1>Packet Tracer - Configuring the Speed and Duplex on Interfaces Connected to Networking Devices</h1>

<p align="center">
This is the diagram od the network where I'll be configuring the speed and duplex on interfaces: <br/>
<img src="https://imgur.com/YrcSp1N" height="80%" width="80%"/>
<br />
<br />
I'll first start with router 1. I'll access its CLI and enter Configuration mode from Privileged Exec mode. I'll give the router the hostname of R1 and enter Interface Configuration Mode with the command "int g0/0". I'll configure the IP address to 172.16.255.254 and declare the subnet mask to be 255.255.0.0 since the prefix length for this network is /16. Now I'll configure the speed of the interface to 1000 Mbps and put it in full duplex. I'll also add a description noting that this interface is connected to switch 1. Lastly, I'll enable the interface by using the "no shutdown" command: <br/>
<img src="https://i.imgur.com/FzkFoxQ.png" height="80%" width="80%"/>
<br />
<br />
Now I'll exit back to Privileged Exec mode with the "end" command and save the running configuration to the startup configuration: <br/>
<img src="https://i.imgur.com/Vetadgh.png" height="80%" width="80%"/>
<br />
<br />
Now that I'm done configuring the interface for router 1, I'll configure the IP addresses and subnet mask for PC 1-4: <br/>
<img src="https://i.imgur.com/rk23Z9j.png" height="80%" width="80%"/>
<br />
<br />
I'll be moving on to configuring switch 1. I'll enter Configuration mode on the switches CLI and give it the hostname of SW1. I'll enter into the configuration mode for interface g0/1 and configure the interface's speed to 1000 Mbps and set its duplex to full. I'll add a description stating that this interface is connected to Router 1. I'll repeat these steps for the rest of the interfaces in use on switch 1 (f0/1, f0/2) as needed: <br/>
<img src="https://i.imgur.com/YlWVAc7.png" height="80%" width="80%"/>
<br />
<br />
Next, I'll add a description for unused interfaces as "## not in use ##" and enable all the changes on swtich 1: <br/>
<img src="https://i.imgur.com/4Rsk1Tt.png" height="80%" width="80%"/>
<br />
<br />
I can verify if all the changes in configurations I made on switch 1 has gone through successfully with the "show interface status" command. I manually set the duplex and speed of the interfaces but it appears that due to a bug Packet Tracer shows them as auto negotiated. Either way, it appears that the necessary configurations have been applied successfully: <br/>
<img src="https://i.imgur.com/qnb9BT5.png" height="80%" width="80%"/>
<br />
<br />
Finally, I'll save the running configuration to the startup configuration and use the "show startup configuration" command to make sure all the configurations have transferred over. It appears everything is in order: <br/>
<img src="https://i.imgur.com/dF1DXtm.png" height="80%" width="80%"/>
<br />
<br />
</p>

