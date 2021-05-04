# ATAK geo bot
This script is a client to a TAK server which forwards messages to web services like What3Words.
It has been tested with https://github.com/tkuester/taky but should work with other TAK servers which support geochat / CoT.

## Setup

 1.     Install the following dependancies if they are not already.
 	
	- pip3 install geocoder
	- pip3 install OSGridConverter

 2.	Edit the settings in the script for your server and API keys
 
|Parameter  | Default | Description |
|--|--|--|
| TAK_SERVER_ADDRESS | 127.0.0.1 | TAK Server IP address |
| TAK_SERVER_PORT | 8087 | TAK Server TCP port |

3.	In a terminal, run your TAK server

	    taky -l debug
    
4.	In a new terminal, run the chatbot script

	    python3 geobot.py
	    
5.	Expect to see a message on your TAK client in "All Chat Rooms"
	"GEO-BOT online"
	
6.	Start chatting to the bot directly, not in the "All Chat Rooms"

## BOT commands
BOT commands are ... TBC
Presently just type anything and the location in your geochat message will be extracted and forwarded, anon, to W3W.
The W3W response will be sent back to you via geochat.


 

