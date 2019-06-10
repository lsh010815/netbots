# Classes System Introduction


## Classes

### default
<img src="images/default.png" width="60%">

### heavy
<img src="images/heavy.png" width="60%">

### light
<img src="images/light.png" width="60%">

### machineGun
<img src="images/machineGun.png" width="60%">

### sniper
<img src="images/sniper.png" width="60%">

### turtle
<img src="images/turtle.png" width="60%">

## How to make classes system work
In rundemo.bat, add `-allowclasses` in the start server line.
```
start "NetBot-Server" cmd /K py -3 src/netbots_server.py -p 20000 -allowclasses
```
Then in your robot join request line, add a class message with the class name
```
joinReply = botSocket.sendRecvMessage({'type': 'joinRequest', 'name': robotName, 'class': "heavy"}, retries=300, delay=1, delayMultiplier=1)
```

