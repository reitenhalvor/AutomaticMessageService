# MessagingBot
Will automatically send messages via iMessage to anyone of your choosing that has iMessage. You prewrite all your messages in a JSON-file (including constraints on when it can be sent), then, given a frequency of "sending messages" that you've set, a random message will be sent to the recipient every now and then. When the message is sent, you will receive an email notification. 

### Procedure:
1. Prewrite all your messages in ```messages.json```, including date limitations ("this message can be sent between 05.08.2017 and 25/08/2017") and what category the messages belongs to (morning, midday, evening or night).
2. In ```MessageProgram.java```, edit the details concerning who's sending and receiving the messages, as well as the paths so that they correspond correctly. 
3. This is the tricky part. You must, on your own, set up a procedure on your system that will run the program with a given frequency. I highly recommend using LaunchControl. So everytime you run the program, a new valid message (if there are any left) will be sent, and LaunchControl will make sure it happens on a given frequency (say every 4th day or something).
4. Once you've set up LaunchControl, the program is ready to roll. You should receive email notifications once you send a new message, so you'll know when stuff is sent on your behalf. 

Notice: It can be risky to use, but it actually does work (tested). 
