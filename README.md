<h2 align="center">
   <strong>Basic Debian HoneyPot Server</strong>
   </br></br>
</h2>

This is a VMWare template for a Debian linux server that is a basic honeypot server.
Logging is to a basic .log file, and it is possible to edit the script to make exclusions for specific IPs/Ports/Networks/Protocols.

## Deployment instructions
<p>Login to your ESX host or vCenter, and use the OVF Import facility to import the VM.<br>
Ensure the network card is attached to a network with DHCP, or manually configure a static IP address afterwards.<br>
The initial credentials are visible before logon.</p>

## Examine the honeypot.log file
Tail the honeypot.log file to check it records things, e.g. ping it and it should record items.

## Exclusions
<p>Based on the results of the honeypot testing, add any exclusions to the runhoneypot.sh file using nano.<br>
Some examples are provided in the script.</p>


## Next steps
<p>(Note that these are out of scope)<br>
<br>
Install SSH for remote access (add to exclusions?)<br>
Build a script to email changes to the log file.</p>
