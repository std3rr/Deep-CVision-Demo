# Deep-CVision-Demo
Preservation of a fullstack demo of deep learning through mobile computer vision, processed in the cloud.<br><br>
I made this in the summer of 2017 as a live demonstration for a deep learning presentation.<br>
The stack consisted of a **darknet/yolo v2** backend that streamed video through **ffmpeg**.<br>
A **nginx** webfront served **javascript** and **html** and a **websocket service** written in **go** that coordinated the streaming.<br>
The input came from a **live video streaming** service called **bambuser**.<br>
Bambuser shut down their service in januari 2018.<br><br>
The service where also capable of multiplexing audio sent to **google speech** for text caption analyzed in the front.<br>
With this you could tell it to draw some colored objects and move them around through voice.<br>
It also had a feature to play the minions banana song when a banana showed up in the live stream.<br>
*( My kids loved that feature :smile: )*<br><br>
All this where set up on a p2xlarge **EC2** GPU instance in the **AWS** cloud.
<br><br>
![some snapshot from 2017](cvdemo.png)
<br>
The darknet files included are those I identified where changed. <br>
Changes I made to make it take raw piped image input and output json data including captions, bounding boxes for predictions and image data.
