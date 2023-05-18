## HTML Multimedia
* Multimedia on the web is sound, music, videos, movies, and animations.

## What is Multimedia?
* Multimedia comes in many different formats. It can be almost anything you can hear or see, like images, music, sound, videos, records, films, animations, and more.

* Web pages often contain multimedia elements of different types and formats.

**Browser Support**
* The first web browsers had support for text only, limited to a single font in a single color.

* Later came browsers with support for colors, fonts, images, and multimedia!

## Multimedia Formats
* Multimedia elements (like audio or video) are stored in media files.

* The most common way to discover the type of a file, is to look at the file extension.

* Multimedia files have formats and different extensions like: .wav, .mp3, .mp4, .mpg, .wmv, and .avi.

## Common Video Formats
**Videoformats**	There are many video formats out there.

* The MP4, WebM, and Ogg formats are supported by HTML.

* The MP4 format is recommended by YouTube.

|Format|	File  |	Description|
|------|----------|------------|
|MPEG	|.mpg,.mpeg|	MPEG. Developed by the Moving Pictures Expert Group. The first popular video format on the web. Not supported anymore in HTML.|
|AVI|	.avi	|AVI (Audio Video Interleave). Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers.|
|WMV	|.wmv|	WMV (Windows Media Video). Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers.|
|QuickTime|	.mov|	QuickTime. Developed by Apple. Commonly used in video cameras and TV hardware. Plays well on Apple computers, but not in web browsers.|
|RealVideo|	.rm ,.ram|	RealVideo. Developed by Real Media to allow video streaming with low bandwidths. Does not play in web browsers.|
|Flash|	.swf,.flv|	Flash. Developed by Macromedia. Often requires an extra component (plug-in) to play in web browsers.
Ogg	.ogg	Theora Ogg. Developed by the Xiph.Org Foundation. Supported by HTML.|
|WebM|	.webm|	WebM. Developed by Mozilla, Opera, Adobe, and Google. Supported by HTML.|
|MPEG-4 or MP4|	.mp4|	MP4. Developed by the Moving Pictures Expert Group. Commonly used in video cameras and TV hardware. Supported by all browsers and  recommended by YouTube. |
* **Note:** Only MP4, WebM, and Ogg video are supported by the HTML standard.


## Common Audio Formats
* MP3 is the best format for compressed recorded music. The term * MP3 has become synonymous with digital music.

* If your website is about recorded music, MP3 is the choice.

|Format	|File	|Description|
|-------|-------|-----------|
|MIDI	|.mid, .midi|	MIDI (Musical Instrument Digital Interface). Main format for all electronic music devices like synthesizers and PC sound cards. MIDI files do not contain sound, but digital notes that can be played by electronics. Plays well on all computers and music hardware, but not in web browsers.|
|RealAudio|	.rm,.ram|	RealAudio. Developed by Real Media to allow streaming of audio with low bandwidths. Does not play in web browsers.|
|WMA|	.wma|	WMA (Windows Media Audio). Developed by Microsoft. Plays well on Windows computers, but not in web browsers.|
|AAC|	.aac|	AAC (Advanced Audio Coding). Developed by Apple as the default format for iTunes. Plays well on Apple computers, but not in web browsers.|
|WAV|	.wav|	WAV. Developed by IBM and Microsoft. Plays well on Windows, Macintosh, and Linux operating systems. Supported by HTML.|
|Ogg|	.ogg|	Ogg. Developed by the Xiph.Org Foundation. Supported by HTML.|
|MP3|	.mp3|	MP3 files are actually the sound part of MPEG files. MP3 is the most popular format for music players. Combines good compression (small files) with high quality. Supported by all browsers.|
|MP4	|.mp4|	MP4 is a video format, but can also be used for audio. Supported by all browsers.|
* **Note:** Only MP3, WAV, and Ogg audio are supported by the HTML standard.

## The HTML `<video>` Element
* To show a video in HTML, use the `<video>` element:

```
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
```
### How it Works
* The controls attribute adds video controls, like play, pause, and volume.

* It is a good idea to always include width and height attributes. If height and width are not set, the page might flicker while the video loads.

* The `<source>` element allows you to specify alternative video files which the browser may choose from. The browser will use the first recognized format.

* The text between the `<video>` and `</video>` tags will only be displayed in browsers that do not support the `<video>` element.

## HTML `<video>` Autoplay
* To start a video automatically, use the autoplay attribute:
```
<video width="320" height="240" autoplay>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
```
**Note:** Chromium browsers do not allow autoplay in most cases. However, muted autoplay is always allowed.

* Add muted after autoplay to let your video start playing automatically (but muted):

```
<video width="320" height="240" autoplay muted>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
```
### Browser Support
* The numbers in the table specify the first browser version that fully supports the `<video>` element.

## HTML Video Formats
* here are three supported video formats: MP4, WebM, and Ogg. The browser support for the different formats is:

|Browser|	MP4|	WebM  |Ogg|
|-------|------|---------|---|
|Edge|	YES|	YES|	YES|
|Chrome|	YES|	YES|	YES|
|Firefox|	YES|	YES|	YES|
|Safari|	YES|	YES|	NO|
|Opera|	YES|	YES|	YES|

## HTML Video - Media Types
|File Format|	Media Type|
|-----------|-------------|
|MP4	|video **/** mp4|
|WebM	|video **/** webm|
|Ogg	|video **/** ogg|

## HTML Video - Methods, Properties, and Events
* The HTML DOM defines methods, properties, and events for the `<video>` element.

* This allows you to load, play, and pause videos, as well as setting duration and volume.

## HTML Audio
* The HTML `<audio>` element is used to play an audio file on a web page.

## The HTML <audio> Element
* To play an audio file in HTML, use the `<audio>` element:
```
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
```
## HTML Audio - How It Works
* The controls attribute adds audio controls, like play, pause, and volume.

* The `<source>` element allows you to specify alternative audio files which the browser may choose from. The browser will use the first recognized format.

* The text between the `<audio>` and `</audio>` tags will only be displayed in browsers that do not support the `<audio>` element.

* HTML `<audio>` Autoplay
* To start an audio file automatically, use the autoplay attribute:
```
<audio controls autoplay>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
```
* **Note:** Chromium browsers do not allow autoplay in most cases. However, muted autoplay is always allowed.

* Add muted after autoplay to let your audio file start playing automatically (but muted):
```
<audio controls autoplay muted>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
```
## Browser Support
* The numbers in the table specify the first browser version that fully supports the `<audio>` element.

## HTML Audio Formats
* There are three supported audio formats: MP3, WAV, and OGG. The browser support for the different formats is: 

|Browser|	MP3|	WAV|	OGG|
|-------|------|-------|-------|
|Edge/IE|  YES|	YES* |	YES* |
|Chrome	|YES|	YES	|YES|
|Firefox	|YES|	YES	|YES|
|Safari	|YES|	YES	|NO|
|Opera	|YES|	YES	|YES|

***From Edge 79**


## HTML Audio - Media Types
|File Format|	Media Type|
|-----------|-------------|
|MP3        |	audio/mpeg|
|OGG        |	audio/ogg|
|WAV        |	audio/wav|

## HTML Audio - Methods, Properties, and Events
* The HTML DOM defines methods, properties, and events for the `<audio>` element.

* This allows you to load, play, and pause audios, as well as set duration and volume.


## HTML Plug-ins
* Plug-ins are computer programs that extend the standard functionality of the browser.

### Plug-ins
* Plug-ins were designed to be used for many different purposes:

* To run Java applets
* To run Microsoft ActiveX controls
* To display Flash movies
* To display maps
* To scan for viruses
* To verify a bank id

***Warning !***
* Most browsers no longer support Java Applets and Plug-ins.
* ActiveX controls are no longer supported in any browsers.
* The support for Shockwave Flash has also been turned off in modern browsers.

## The `<object>` Element
* The `<object>` element is supported by all browsers.

* The `<object>` element defines an embedded object within an HTML document.

* It was designed to embed plug-ins (like Java applets, PDF readers, and Flash Players) in web pages, but can also be used to include HTML in HTML:

`<object width="100%" height="500px" data="snippet.html"></object>`

Or images if you like:

`<object data="audi.jpeg"></object>`

* The `<embed>` Element
* The `<embed>` element is supported in all major browsers.

* The `<embed>` element also defines an embedded object within an HTML document.

* Web browsers have supported the `<embed>` element for a long time. However, it has not been a part of the HTML specification before HTML5.

`<embed src="audi.jpeg">`
* **Note** that the `<embed>` element does not have a closing tag. It can not contain alternative text.

* The `<embed>` element can also be used to include HTML in HTML:

```
<embed width="100%" height="500px" src="snippet.html">
```

## HTML YouTube Videos
* The easiest way to play videos in HTML, is to use YouTube.

## Struggling with Video Formats?
* Converting videos to different formats can be difficult and time-consuming.

* An easier solution is to let YouTube play the videos in your web page.

## YouTube Video Id
* YouTube will display an id (like tgbNymZ7vqY), when you save (or play) a video.

* You can use this id, and refer to your video in the HTML code.

* Playing a YouTube Video in HTML
* To play your video on a web page, do the following:

* Upload the video to YouTube
* Take a note of the video id
* Define an `<iframe>` element in your web page
* Let the src attribute point to the video URL
* Use the width and height attributes to specify the dimension of the player
* Add any other parameters to the URL (see below)
```
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY">
</iframe>
```

## YouTube Autoplay + Mute
You can let your video start playing automatically when a user visits the page, by adding autoplay=1 to the YouTube URL. However, automatically starting a video is annoying for your visitors!

* **Note:** Chromium browsers do not allow autoplay in most cases. However, muted autoplay is always allowed.

* Add **mute=1** after **autoplay=1** to let your video start playing automatically (but muted).

## YouTube - Autoplay + Muted
```
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?autoplay=1&mute=1">
</iframe>
```

## YouTube Playlist
* A comma separated list of videos to play (in addition to the original URL).

## YouTube Loop
* Add **loop=1** to let your video loop forever.

**Value 0 (default):** The video will play only once.
**Value 1:** The video will loop (forever).

## YouTube - Loop
```
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
</iframe>
```

## YouTube Controls
* Add controls=0 to not display controls in the video player.

**Value 0:** Player controls does not display.

**Value 1 (default):** Player controls display.

## YouTube - Controls
```
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?controls=0">
</iframe>
```

|Tag	| Description|
|-------|------------|
|`<!--...-->`	|Defines a comment|
|`<!DOCTYPE>`|Defines the document type|
|`<a`>      |Defines a hyperlink|
|`<abbr>`|	Defines an abbreviation or an acronym|
|`<acronym>`|	Not supported in HTML5. Use `<abbr>` instead. Defines an acronym|
|`<address>`|	Defines contact information for the author/owner of a document|
|`<applet>`|	Not supported in HTML5. Use `<embed>` or `<object>` instead. Defines an embedded applet|
|`<area>`|	Defines an area inside an image map|
|`<article>`|	Defines an article|
|`<aside>`|	Defines content aside from the page content|
|`<audio>`|	Defines embedded sound content|
|`<b>`|	Defines bold text|
|`<base>`|	Specifies the base URL/target for all relative URLs in a document|
|`<basefont>`|	Not supported in HTML5. Use CSS instead. Specifies a default color, size, and font for |all text in a document
|`<bdi>`|	Isolates a part of text that might be formatted in a different direction from other text outside |it
|`<bdo>`|	Overrides the current text direction|
|`<big>`|	Not supported in HTML5. Use CSS instead. Defines big text|
|`<blockquote>`|	Defines a section that is quoted from another source|
|`<body>`|	Defines the document's body|
|`<br>`|	Defines a single line break|
|`<button>`|	Defines a clickable button|
|`<canvas>`|	Used to draw graphics, on the fly, via scripting (usually JavaScript)|
|`<caption>`|	Defines a table caption|
|`<center>`|	Not supported in HTML5. Use CSS instead. Defines centered text|
|`<cite>`|	Defines the title of a work|
|`<code>`|	Defines a piece of computer code|
|`<col>`|	Specifies column properties for each column within a `<colgroup>` element |
|`<colgroup>`|	Specifies a group of one or more columns in a table for formatting|
|`<data>`|	Adds a machine-readable translation of a given content|
|`<datalist>`|	Specifies a list of pre-defined options for input controls|
|`<dd>`|	Defines a description/value of a term in a description list|
|`<del>`|	Defines text that has been deleted from a document|
|`<details>`|	Defines additional details that the user can view or hide|
|`<dfn>`|	Specifies a term that is going to be defined within the content|
|`<dialog>`|	Defines a dialog box or window|
|`<dir>`|	Not supported in HTML5. Use `<ul>` instead. Defines a directory list|
|`<div>`|	Defines a section in a document|
|`<dl>`|	Defines a description list|
|`<dt>`|	Defines a term/name in a description list|
|`<em>`|	Defines emphasized text |
|`<embed>`|	Defines a container for an external application|
|`<fieldset>`|	Groups related elements in a form|
|`<figcaption>`|	Defines a caption for a `<figure>` element|
|`<figure>`|	Specifies self-contained content|
|`<font>`|	Not supported in HTML5. Use CSS instead. Defines font, color, and size for text|
|`<footer>`|	Defines a footer for a document or section|
|`<form>`|	Defines an HTML form for user input|
|`<frame>`|	Not supported in HTML5. Defines a window (a frame) in a frameset|
|`<frameset>`|	Not supported in HTML5. Defines a set of frames|
|`<h1>`| to `<h6>`	Defines HTML headings|
|`<head>`|	Contains metadata/information for the document|
|`<header>`|	Defines a header for a document or section|
|`<hr>`|	Defines a thematic change in the content|
|`<html>`|	Defines the root of an HTML document|
|`<i>`|	Defines a part of text in an alternate voice or mood|
|`<iframe>`|	Defines an inline frame|
|`<img>`|	Defines an image|
|`<input>`|	Defines an input control|
|`<ins>`|	Defines a text that has been inserted into a document|
|`<kbd>`|	Defines keyboard input|
|`<label>`|	Defines a label for an `<input>` element|
|`<legend>`|	Defines a caption for a `<fieldset>` element|
|`<li>`|	Defines a list item|
|`<link>`|	Defines the relationship between a document and an external resource (most used to link to |stylesheets)
|`<main>`|	Specifies the main content of a document|
|`<map>`|	Defines an image map|
|`<mark>`|	Defines marked/highlighted text|
|`<meta>`|	Defines metadata about an HTML document|
|`<meter>`|	Defines a scalar measurement within a known range (a gauge)|
|`<nav>`|	Defines navigation links|
|`<noframes>`|	Not supported in HTML5.Defines an alternate content for users that do not support frames|
|`<noscript>`|	Defines an alternate content for users that do not support client-side scripts|
|`<object>`|	Defines a container for an external application|
|`<ol>`|	Defines an ordered list|
|`<optgroup>`|	Defines a group of related options in a drop-down list|
|`<option>`|	Defines an option in a drop-down list|
|`<output>`|	Defines the result of a calculation|
|`<p>`|	Defines a paragraph|
|`<param>`|	Defines a parameter for an object|
|`<picture>`|	Defines a container for multiple image resources|
|`<pre>`|	Defines preformatted text|
|`<progress>`|	Represents the progress of a task|
|`<q>`|	Defines a short quotation|
|`<rp>`|	Defines what to show in browsers that do not support ruby annotations|
|`<rt>`|	Defines an explanation/pronunciation of characters (for East Asian typography)|
|`<ruby>`|	Defines a ruby annotation (for East Asian typography)|
|`<s>`|	Defines text that is no longer correct|
|`<samp>`|	Defines sample output from a computer program|
|`<script>`|	Defines a client-side script|
|`<section>`|	Defines a section in a document|
|`<select>`|	Defines a drop-down list|
|`<small>`|	Defines smaller text|
|`<source>`|	Defines multiple media resources for media elements (`<video>` and `<audio>`)|
|`<span>`|	Defines a section in a document|
|`<strike>`|	Not supported in HTML5. Use `<del>` or `<s>` instead.Defines strikethrough text|
|`<strong>`|	Defines important text|
|`<style>`|	Defines style information for a document|
|`<sub>`|	Defines subscripted text|
|`<summary>`|	Defines a visible heading for a `<details>` element|
|`<sup>`|	Defines superscripted text|
|`<svg>`|	Defines a container for SVG graphics|
|`<table>`|	Defines a table|
|`<tbody>`|	Groups the body content in a table|
|`<td>`|	Defines a cell in a table|
|`<template>`|	Defines a container for content that should be hidden when the page loads|
|`<textarea>`|	Defines a multiline input control (text area)|
|`<tfoot>`|	Groups the footer content in a table|
|`<th>`|	Defines a header cell in a table|
|`<thead>`|	Groups the header content in a table|
|`<time>`|	Defines a specific time (or datetime)|
|`<title>`|	Defines a title for the document|
|`<tr>`|	Defines a row in a table|
|`<track>`|	Defines text tracks for media elements (`<video>` and `<audio>`)|
|`<tt>`|	Not supported in HTML5. Use CSS instead.Defines teletype text|
|`<u>`|	Defines some text that is unarticulated and styled differently from normal text|
|`<ul>`|	Defines an unordered list|
|`<var>`|	Defines a variable|
|`<video>`|	Defines embedded video content|
|`<wbr>`|	Defines a possible line-break|