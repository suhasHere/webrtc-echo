Project - Echo Server'ish WebRTC server component
================================================
In order to test this , do the following

1. Install the node app under the sever/
2. Start the server : node app.js
3. Apply the patch under the patch/
4. Start the native application under the <obj-dir>/dist/bin/RTCApp
5. Start the firefox bin and point it to
       URL: http://localhost:8000/
   5a. enter a name and login
6. Click Start Call in the following webpage.

Now,
Listen to some random tones for 10 seconds and yes that's the test for now

 Few Points to note
===================
* Currently the test-case works only on a single machine due to 
  ICE processes failing - Yet to Debug
* The code is of version 1 now and please do expect things to fail. 
* The call should always be initiated from the Browser App. This can
  be easily extended.
* We support only on Native Client as part of the APP. Extending it to
  number of peer-connections supported by underlying system, is pretty easy
* Ajax Requests are supported Sync only. Not a big deal to make it non-sync.
  

NOTE: This project is a version of the code we used at WebRTC Expo for
Plantronics demo.
