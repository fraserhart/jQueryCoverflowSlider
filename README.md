jQueryCoverflowSlider
=====================

Coverflow inspired jQuery slider

<h2>Installation</h2>
1. Include the CSS in the head of your document:

<link rel="stylesheet" type="text/css" href="jquery.coverflow.slider.css" />

2. Specify the cover images in an unordered list (ul) wrapped in a div:
<div id="contentSlider">
	<ul>
		<li><img src="cover1.jpg"></li>
		<li><img src="cover2.jpg"></li>
		<li><img src="cover3.jpg"></li>
		<li><img src="cover4.jpg"></li>
		<li><img src="cover5.jpg"></li>
		<li><img src="cover6.jpg"></li>
		<li><img src="cover7.jpg"></li>
		<li><img src="cover8.jpg"></li>
	</ul>
</div>

3. Include jQuery and jquery.coverflow.slider.js before the closing body tag of your document.

<script src="http://code.jquery.com/jquery-1.10.1.min.js"></script>
<script src="jquery.coverflow.slider.js"></script>

4. Initialise the plugin below the inclusion of the coverflow js file
$('#contentSlider').coverFlow()

5 (optional). Options:
$('#contentSlider').coverFlow({
	'initialFocus' : 0, //the index of the slide you want to be focused on load
	'speed' : 200, // the speed of the animation
	'addClasses' : "", //classes to add to the slider
	afterChange: function(index){
		console.log('Slide in focus: ' + index);
	} //executes after the slide has changed
});