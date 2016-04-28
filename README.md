# Sample WebRTC App

This app uses a turn serever setup my me on aws.
* Server:  52.39.109.47:3478
* username: gorst
* credential: hero

### Dependencies
* node-static
* socket.io
to install node-static
```
$ npm install node-static
```
to install socket.io
```
$ npm install socket.io
```
### Run

to run the application, run the server.js in webRTC-Demo/ folder
```
$ cd webRTC-Demo
$ node server.js
```
Open up a browse at *localhost:2013* to use the application. 

you have to choose a tuen server you would like to connect either Google's server or a custom server setup by me.

You are then prompted to choose a room to connect. If the chosen room is already connected then you join the room and start conversing with the other person in the room.

If a room doesnot exist. The application will create the required room.

## Application Specification

* This application uses standard WebRTC library.
* It works perfectly on chrome
* It uses JSEP for Signalling
* The application has a hang up Button to hangup the call whenever a user wants.
* If someone hangs up the call the User is notified in the form of a pop up.
* You can also enable of disable Auto Echo Cancellation and Auto Gain Control. The application contains buttons that alows the same. By default AGC and AEC is set to True.
* By Default the Audio Codec is set to OPUS. If you would like to use a different audio codec. *localhost:2013/pcmu.html* uses PCMU as the default audio codec for transmission. 

