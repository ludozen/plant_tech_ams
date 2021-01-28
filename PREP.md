# Preparing for the Make Event

Makers that are well prepared get the most out of their experience. Before you attend your Make Day, there are a couple of activities to complete. Please walk through the steps below and make sure to have a working system before the actual Make session starts. It should only take about 15 minutes!

## Step 1 - Arduino IDE

Download and install the [Arduino IDE](https://www.arduino.cc/en/main/software). Alternatively you can use [Micropython](https://github.com/OfferZen-Make/plant_tech_ams#micropython-submitted-by-michiel-erasmus)

## Step 2 - Test your water pump

Sometimes the pumps have a few issues and can take a while to get working, so it's a good idea to test if yours is working before the evening.

For these steps you don't need to program anything, just connect the motor to the power on the board and the board to your laptop.

1. Strip the black and red wires of the pump (rather strip them more than too little.
2. Now connect the + (red wire) of the pump to 3V pin on the ESP, and the - (black wire) to the ground pin (G).
Note: You can do this by manually touching the stripped ends to the pins on the board, or you can use the white connector block to connect dupont cables to the stripped wires.
4. Connect your board to your laptop.

Now power should be flowing to the pump, and you will hear a soft humming noise. If it doesn't work see [troubleshooting](https://github.com/OfferZen-Make/plant_tech_ams#my-pump-isnt-working).

## Step 3 - Set up your system

We will begin by installing the ESP8266 (that thingy in your box with the micro-USB port) support for the Arduino IDE:

- Open the Arduino IDE
- Go to Files (for Windows) or Arduino (for Mac) > Preferences
- Copy this: http://arduino.esp8266.com/stable/package_esp8266com_index.json
- Paste it in the 'Additional Boards Managers URLs' field
- Click OK and close the preferences window
- Go to Tools > Board > Boards Manager...
- Navigate to esp8266 by esp8266 community and install the software for Arduino.

## Step 4 - Connect your ESP8266

Now it's time to plug the ESP8266 board in your computer, and see how to blink an LED (the Hello World in the electronics):

- Navigate to Tools > ESP8266 Boards (2.7.4) > NodeMCU 1.0 (ESP-12E Module)
- Select the right USB port from Tools > Port
- Clone (or download, or simply copy-paste to your Arduino IDE window) the [BlinkESP](https://github.com/OfferZen-Make/plant_tech_ams/blob/master/BlinkESP.ino) code and run it in Arduino IDE by clicking 'Upload'.
- After compiling and uploading, the LED on your ESP8266 board should start flashing. You did it!

### Big Sur compatability issue:

If you're getting this issue `pyserial or esptool directories not found next to this upload.py tool` when uploading your sketch on Big Sur, [click here](https://forum.arduino.cc/index.php?topic=702144.0#msg4793318) for the work around.

<img src="https://media.giphy.com/media/3ohryhNgUwwZyxgktq/giphy.gif" alt="seven" width="300"/>

### Troubleshooting

All project troubleshooting is here https://github.com/OfferZen-Make/plant_tech_ams/wiki

## Step 5 - Take a photo of your setup and share it!

Please help us spread the word about Make events so that we can grow the community and keep helping devs learn new tech 🚀 💦 🌱.

### Share photo on Twitter

1. Take a photo of your set up
2. Click here to [📸  -> Share on Twitter](https://twitter.com/intent/tweet?url=&text=I'm%20setup%20and%20ready%20to%20go%20for%20my%20%23offerzenmake%20event%20with%20%40offerzen!) with a message

### && / || Share photo on LinkedIn

If you don't have Twitter you can share it on LinkedIn. Steps:
* Copy this message: `I'm setup and ready to go for my #offerzenmake event with @offerzen! `.
* Upload a photo of your setup and the message above to [LinkedIn](https://www.linkedin.com/).

### Fabulous example

Here's a fabulous example from @hendrikdelarey

[<img src="https://i.imgur.com/seoUZT8.png"/>](https://twitter.com/hendrikdelarey/status/1336696671556825091?s=20)

### If you don't do social media...

And if you abhor all social medias and don't do any of that then please share it on the #project-arduino-plant channel in Slack 😂 Thank you, it really helps to keep the lights on 💡. See you soon <3

## Step 6 - Chart a course for self-watering plant mastery

Read through the [Plant Tech readme](https://github.com/OfferZen-Make/plant_tech_ams/blob/master/README.md) including [project extensions](https://github.com/OfferZen-Make/plant_tech_ams/blob/master/README.md#project-extensions), [community contributions](https://github.com/OfferZen-Make/plant_tech_ams/blob/master/README.md#community-contributions) and [useful resources](https://github.com/OfferZen-Make/plant_tech_ams/blob/master/README.md#useful-resources) to get an idea for where you want to take your self-watering plant project on the evening of the event.

Please edit or add to the docs as you go!
