IRCCC
=====

IRC client for ComputerCraft

This is a ComputerCraft IRC client, or more specifically a client for the qwebirc backend server.
Unfortunately the HTTP API in ComputerCraft doesn't allow for a true IRC client (even though the
HTTP protocol can in theory be used to communicate with an IRC server[1]). This client provides
a work-around by interfacing with the qwebirc backend. qwebirc is a popular webchat interface and
is relatively straightforward to work with. In addition, several IRC servers already host a webchat
server, so there's no need to set up your own, although that remains a possibility if you can't
find a webchat for your favourite server to connect to.

How to use:

	* Download with: pastebin get gaSL8HZC irc
	* Check that the baseUrl and dynamicUrl parameters are correct. Examples are provided for espernet
	  and quakenet. By default the client connects to espernet.
	* Start the client with:
		irc

You can also supply an optional nick argument to set your nickname, or you can change your nick within the client with the standard /nick command.
Currently supported commands are:

/window N			- switch to window N
/join CHANNEL		- join CHANNEL
/part				- part the current channel or private chat
/quit 				- disconnect and quit
/nick NICK			- change nickname to NICK
/query USER 		- start a private chat with user USER
/help 				- list available commands


1. https://www.youtube.com/watch?v=2ctRfWnisSk#t=343

TODO:
		- color support
		- better handling of the IRC protocol
		- use window API where available

This program is released under the MIT license.
