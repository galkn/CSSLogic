# CSSLogic v0.1.0

CSSLogic is a JavaScript plugin that lets you use variables in your CSS files, without having to compile anything or go through any server-side process.

## Your CSS will look like this

	/* style.css */
	
	pageWidth = 1000px;
	headerFont = "comic sans", arial, sans-serif;
	
	body {
		width: [pageWidth];
	}
	
	#header {
		height: 150px;
		width: [pageWidth];
	}
	
	h1 {
		color: red;
		font-family: [headerFont];
	}

Then just let CSSLogic will handle all the replacements.

## Usage

Require jQuery and CSSLogic (preferably instead your `header` tag) like so:

	<script type="text/javascript" src="jquery.min.js"></script>
	<script type="text/javascript" src="csslogic.js?css=style.css" id="csslogicscript"></script>

Pass the URL to your CSS file as `css` parameter, and remove its `<link ...>` tag from the DOM. Don't change the `id` attribute or it won't work.

## Copyright

Copyright (c) 2011 Gal Koren.

