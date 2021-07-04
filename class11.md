# Read: 11 - Assorted Topics
## Flash, VidEo & Audio
The most popular way of adding **Flash** into a web page is using *JavaScript*.
```
 <script type="text/javascript">
 swfobject.embedSWF("flash/bird.swf",
 "bird", "400", "300", "8.0.0");</script>
 ```
 You can obtain a copy of it for free
from Google, and you can see how we use it on the next page.

The easiest way to add a **video** to your site is to upload the video to a site like YouTube or
Vimeo and use the features provided on their
site to embed the video in your page.



There are three steps you need to follow to add
a Flash Video to your web page:
Preparing a Flash
Video for Your Site
1. Convert Your Video into FLV Format

2. FinD an FLV Player to Play the Video.

3. Include the Player & Video in Your Page.

Despite the HTML5 ```<video> ```element being a
very recent addition, it is enjoying widespread
use. 

To specify the location of the file to be played, you can use the ```<source>``` element inside the video element. (This should replace the ***src*** attribute on the opening ```<video>```tag.)


HTML5 introduced the ```<audio>``` element to include audio files in your pages.

It is possible to specify more than one audio file using the ```<source>``` .
![attributes](https://csharpcorner-mindcrackerinc.netdna-ssl.com/UploadFile/2072a9/html5-media-elements/Images/Attributes%20Video.jpg)