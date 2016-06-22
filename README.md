<h1>Security Camera HTML</h1>
<h3>Bootstrap, Fancybox (lightbox alternative)</h3>

I have created a self contained webpage in order to show the current feed from the cameras.

It currently loads and image from each camera every .3 seconds and when you click on a particular image it will load the fill video feed in an iframe so that it will drop the connection when the modal is closed.

This is used mainly to watch the cameras, it does not record or edit snapshots.

Tested and working IP Cameras:

- Foscam
  - Get Available Resolutions
    - http://CAMERA-IP/param.cgi?cmd=getvideoattr
  - Image
    - http://CAMERA-IP/CGIProxy.fcgi?cmd=snapPicture2&t=
  - Video
    - http://CAMERA-IP/CGIStream.cgi?cmd=GetMJStream
- Axis
  - Get Available Resolutions
    - http://CAMERA-IP/axis-cgi/param.cgi?action=list&group=Properties.Image.Resolution
  - Image
    - http://CAMERA-IP/axis-cgi/jpg/image.cgi?resolution=480x270&t=
  - Video
    - http://CAMERA-IP/axis-cgi/mjpg/video.cgi?resolution=1280x720
