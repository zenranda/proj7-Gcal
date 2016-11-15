# README #

###CS322 Project 7: Google Calendar; Busy Times###
###Author: Marc Leppold###

##Project Notes

The seventh project in CS322. A program that finds all the blocks of time that are busy in the user's Google Calendars. When the user first connects, they authorize the program to read their Google Calendar information. Once they give consent, they select a date rate, an hour range and which calendars they want to check. Once all the information has been entered and the user presses "Submit", this program retrieves the busy blocks of time that fit the criteria and returns them in sorted order.

Requires internet access in order to transact with Google. Requires the user to have a valid Google account and calendar data on Google Calendars with busy appointments on them. Attempting to use this program with a Google account that has no calendars will result in nothing being returned.

Usage note: Hour ranges are from 0...23. Entering an hour that doesn't fit this range or that isn't an integer will cause a crash.

Requires client credentials as well as an API key from Google; neither are included in this repository and are only supplied in certain distributions of this program. The user must supply their own otherwise.

### USAGE ###

Execute the following commands
```
git clone https://github.com/zenranda/proj7-Gcal InstallDirectory
cd InstallDirectory
. configure
make run
```
where InstallDirectory is the directory you cloned the files to.

Then while it's running, enter
```
HOST:PORT
```
into an internet browser, where HOST is the host IP of the computer the program is running on and PORT is the port it's configured to (default 5000).
Please note that this program requires a constant internet connection in order to recieve and send calendar info and authorization. If you wish to use your own API key from Google, make sure to include HOST and HOST/oauth2callback in its URI specifications.