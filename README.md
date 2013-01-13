Project - Echo Server'ish WebRTC server component
================================================
In order to test this , do the following

1. Install the node app under the sever/
2. Start the server : node app.js
3. Apply the patch under the patch/
4. Build Firefox and copy the binary under bin to <obj-dir>/dist/bin
4. Start  the application : ./RTCApp from the above bin diretory
5. Start the firefox binary and point it to your server port 8000 as
       URL: http://localhost:8000/
   5a. enter a name and login
6. Click Start Call in the following webpage.

Now,
Listen to some random tones for 10 seconds and yes that's the test for now

 Few Points to note
===================
* The code is been active worked on at present in terms of design and
  development. So please use binary found under bin/ for quick testing.
* The code is of version 1 now and please do expect things to fail. 
* The call should always be initiated from the Browser App. This can
  be easily extended.
* We support only on Native Client as part of the APP. Extending it to
  number of peer-connections supported by underlying system, is pretty easy
* Ajax Requests are supported Sync only. Not a big deal to make it non-sync.
  

NOTE: The server piece of the code is restructured WebRTC Expo code
