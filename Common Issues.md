

# Common Issues
## Player(s) can't connect
### Error is "Unable to establish connection to the Game Server"
1. Pull the connect string straight for dathost. 
	 * Hover over the hostname (Globe/Internet Icon). 
	 * Under the Console Connect Command hit the clipboard button. 
	 * Paste that into Discord. Match support, DM, or wherever
	 * Add a code block around it by putting ``` before and after the command. (This can help reduce copy paste errors)
	 * `connect robert.dathost.net:26563;password SecureCSCPassword`
2. Get the IP address of the server and try to connect that way
	* Go into the dathost console for the relevant server
	* Type `status` and hit enter
	* Look for the IP address. The line should look like this 
	```
	 ----- Status -----
	:  @ Current  :  game
	:  source   : console
	:  hostname : Drip Pug
	:  spawn    : 1
	:  version  : 1.39.9.2/13992 9961 secure  public
	:  steamid  : [G:1:10505667] (85568392930545091)
	:  udp/ip   : 169.150.232.39:26314
	:  os/type  : Linux dedicated
	:  sourcetv[0] : 169.150.232.39:26315 delay 0.0s
	:  players  : 0 humans, 1 bots (0 max) (not hibernating) (unreserved) 
	```
	* We're looking for the line udp/ip
	* Modify the connect link using the IP address instead of the hostname
	* `connect 169.150.232.39:26314; password SecureCSCPassword`
### Error is "Kicked by Game Server"
Fix whitelisting

