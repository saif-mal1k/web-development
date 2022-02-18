image element:
<figure>
	<img src="bird.jpg" , alt="photo of bird" />
<figcaption>  fig:1.21  <figcaption>
</figure>	
note: image element can have two attributes width and height its recommended to adjust only one of two. more important always specify width or height to stop layout breaking due to image not loading.
other attributes:  hspace,  vspace,  border,  align. 

video element:
<video src="videosrc.mp4" autoplay>		<!- - autoplay 	     no controls - ->
<video src="videosrc.mp4" controls>			<!- - no autoplay video  available controls - ->
<video src="videosrc.mp4" poster=”posterlink.jpg”  controls>            <!- -poster is thumbnail- ->
other attribute :
autoplay	auto play video when page loads.
muted 	video will start muted.
loop 		video will restart automatically every time it ends.
controls 	provides controls for video.
