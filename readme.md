# Intro

This is receiving the following json from the server: { image: [image data converted to base64 binary to text encoding], imageId: [whatever identifier you'll need to recognize what image you're sending button presses for], jsonData: [whatever data you need displayed in the JSON display on the left side] }

upon button press, it is sending the following json data in string format: { imageId: [the identifier you sent from the server to verify what you're getting back matches which image], button: [hardcoded value you're sending back, I just picked 0, 1, 2 as defaults] }

## Setup

on line 17, change the websocket server to your desired server

## Expansion

Currently there are 3 buttons below the image(keep, reject, and retry). To make a new button, first copy/paste a prior button code(example, javascript, starting with `const keep` on lines 33-36), and rename to whatever the button you are creating shall be named, modify any json in the code as you see fit. Then duplicate the existing button(example, html, starting with `<button onClick="keep()">` on line 8), rename the button's onClick and inner html accordingly.
