TwitchChatPipe (C#)
==============

Pipes the Twitch Chat to a VirtualBox Virtual Machine

Note: This was thrown together quickly and not refactored/optimized. It's bare bones to get you started, it should be easy to add to it.

Screenshot: http://imgur.com/o5nkUmP

==============
Setup
==============

1) You will need to have VirtualBox installed with a Virtual Machine running.  

2) You will need to reference the VBoxC.dll in your "Program Files/Oracle/VirtualBox" folder for the c# code to compile.




==============
Usage
==============

1) You will need to generate a IRC password to access Twitch's Chat Servers here: http://twitchapps.com/tmi/

2) Setup your username and password (the password contains "oauth:" inside it.)

3) Edit the IRC data, you can have multiple servers seperated by a comma (no spaces).

4) Hit "Connect", wait about 5 seconds.

5) Hit "Join Channel", your Twitch Chat Channel is your username, for instance, "#myusername".

6) Verify the Virtual Machine Name matches your VirtualBox VM name.

7) Hit "Lock", to begin sending chat commands to virtual box.

Note: You do not have to be streaming for it to work, just go to your channel and start chatting.

==============
Custom Key Config
==============

The program is setup to use SNESKeys as it's default key command configuration.  
There is also an example for Final Fantasy 7 from Steam.
You can create a new enum in ButtonMaster.cs to map your desired keys to the key inputs of the program/emulator you use in virtualbox.
After you create the enum, pass it in the Form1 Constructor that creates the ButtonMaster object.