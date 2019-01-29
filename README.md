<h1><a id="Unusual_Pyramid_0"></a>JS-Unusual Pyramid</h1>
<p>A mirrored “pyramid” made with a JS for loop.</p>
<p>You can check the live preview on: <a href="https://negrut112.github.io/JS-unusual-piramyd/">https://negrut112.github.io/JS-unusual-piramyd/</a><br>
<img src="https://i.imgur.com/2rgp8cQ.jpg">

<b>HTML</b>
<p>I have used the HTML to define the area where I’m working defining the height, width and the border style:</p>
<p>&lt;canvas id=“myCanvas” height=“310” width=“500” style=“border: 1px solid black”&gt;&lt;/canvas&gt;</p>

<b>JavaScript</b>
<p>This for loop is drawing lines from top and bottom to middle of canvas.<br>
For the “upper” pyramid the begining point is found on top-middle from where we draw ex. 450 lines to the middle at distance of 3 between them.<br>
The lower “pyramid” is doing the oposit way - 450 lines from bottom to middle, at distance of 3 between them, but the first line is starting with an extra unit.</p>
<p>context.strokeStyle=‘red’;<br>
context.beginPath();<br>
for(i=0;i&lt;=450;i+=3){<br>
context.moveTo(225,0);<br>
context.lineTo(i+0,150);<br>
}for(i=0;i&lt;=450;i+=3){<br>
context.moveTo(225,300);<br>
context.lineTo(i+1,150);<br>
}context.stroke();</p>
