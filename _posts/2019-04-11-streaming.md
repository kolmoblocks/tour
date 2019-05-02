---
layout: post
permalink: /streaming/
---

# How KolmoLD can benefit streaming media

KolmoLD can also be applied to streaming media. 
Suppose we are streaming a video at 480p off of a site that uses adaptive bitrate streaming.
Our buffer will hold a few 480p frames to prevent stalling. Once the video player detects that our network could support 720p, our 480p frames in buffer will be discarded. 

With the help of KolmoLD, we can avoid having to discard the buffered frames. 
Data expressions provide many ways for us to formulate our desired higher resolution frame. 

![Streaming Diagram](/images/streaming_diagram.png)

In this example, we would like to upgrade our 480p BMP to 720p BMP.
Two data expressions are provided to formulate the 720p BMP:
1. Directly downloading the 720p image 
2. Using a web assembly module that takes in both resolutions and uses the difference of them to build the higher resolution BMP from the lower resolution BMP






