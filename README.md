<h2 align="center">
   <strong>Basic Debian HoneyPot Server</strong>
   </br></br>
</h2>

This is a VMWare template for a Debian linux server that is a basic honeypot server.
Logging is to a basic .log file, and it is possible to edit the script to make exclusions for specific IPs/Ports/Networks/Protocols.

## Deployment instructions
Login to your ESX host or vCenter, and use the OVF Import facility to import the VM.
Ensure the network card is attached to a network with DHCP, or manually configure a static IP address afterwards.
The initial credentials are visible before logon.

## Examine the honeypot.log file
Tail the honeypot.log file to check it records things, e.g. ping it and it should record items.

## Exclusions
Based on the results of the honeypot testing, add any exclusions to the runhoneypot.sh file using nano.
Some examples are provided in the script


## Next steps
(Note that these are out of scope)

Install SSH for remote access (add to exclusions?)

Build a script to email changes to the log file.
