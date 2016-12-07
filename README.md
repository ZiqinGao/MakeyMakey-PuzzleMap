# MakeyMakey-PuzzleMap
Read the clues and find your way through a Makey-Makey connected map

<img src="build images/0 - 0 how it works.png" alt="how it works" width="800">
<p>(The images in build images are numbered to match their respective tutorial step)</p>

<h3>You Need:</h3>
<ul>
<li>a computer with a browser, a USB port, and speakers</li>
<li>a Makey Makey board</li>
<li>electrical wire (insulated)</li>
<li>alligator clips (I used 8)</li>
<li>decorative (but conductive) wire, such as beading wire</li>
<li>a stretched canvas</li>
<li>paint (I used acrylic)</li>
<li>paper</li>
<li>black tea (I used an orange pekoe teabag)</li>
</ul>

<h3>Step One - Puzzle Design</h3>
<ol>
<li>Design symbols</li>
<li>Pick a six symbol answer</li>
<li>Design map (be careful to avoid getting too close to the edges of the map)</li>
<li>Paint/print puzzle</li>
<li>Create aged paper for the puzzle hints or story by rubbing a used teabag on some paper and tearing the edges</li> 
<li>Since mosts pens are water soluble I recommend writing the hints after the paper finishes drying</li>
</ol>

<img src="build images/1 - 1 2 3 design symbols.jpg" alt="design symbols" width="200">
<img src="build images/1 - 4 paint canvas in progress.jpg" alt="in progress" width="200">
<img src="build images/1 - 4 paint canvas.jpg" alt="paint setup" width="200">
<img src="build images/1 - 4 paint canvas finished.jpg" alt="finished canvas" width="200">
<img src="build images/1 - 5 aged paper.jpg" alt="aged paper" width="200">
<img src="build images/1 - 6 write puzzle easy.jpg" alt="write puzzle" width="200">
<img src="build images/1 - 6 write puzzle full.jpg" alt="write puzzle" width="200">

<h3>Step Two - The Wiring</h3>
<ol>
<li>Use beading wire to recreate the symbols on the map, poking the wires through to the other side of the canvas.
(Some of my designs fell over the wooden frame of the canvas and were more difficult to poke through, so please take that into consideration).
I broke the symbols down into small straight segments and added them in like staples.
You will have to add wire to both the correct and red herring symbols, otherwise the answer would be pretty obvious.</li>
<li>Flip over the canvas and use the insulated electrical wire to attach all of the symbols that are not part of your final solution together.
Make sure to strip the wire so the metal of the wire is touching the metal of the beading wire.
Note: while you could normally solder the wires together, solder and acrylic paint can probably release unhealthy fumes, and canvas can catch fire, so I used tape.</li>
<li>Use an alligator clip to attach the dummy symbols to the space bar part of the Makey-Makey board.</li>
<li>Add six male to male wire connectors to the W A S D F G ports on the back of the Makey-Makey board. </li>
<li>Use alligator clips to attach the back of each remaining symbol to the other end of its respective wire connector to the Makey-Makey board. The first key to W, the second to A, and so on.</li>
<li>Use a last alligator clip and attach it to a ground on the Makey-Makey board and a conductive object that the user will hold while solving the puzzle.</li>
<li>Plug in the Makey-Makey board to the computer via USB.</li>
</ol>

<h3>Step Three - The Browser (webpage)</h3>
<ol>
<li>In between the head tags of the document use the audio tag to preload any sound you want to play when the puzzle is solved. </li>
<li>Write a JavaScript script that listens for “key downs” from the keyboard, stores the entries and checks them against an expected password.
In my code the end goal is "W,A,S,D,F,G" and every time a new key is pressed on the map, the value is pushed onto the end of the 6 value password array and the oldest entry is shifted off. The function that pushes and shifts the array does not accept the same key twice in a row to allow for the player accidentally pressing the same key multiple times.</li>
<li>If the password is correct the browser plays the selected sound.</li>
<li>Please see index.html for more detailed comments on how the JavaScript works.</li>
</ol>

<h3>Step Four – Solve the Puzzle</h3>
<ol>
<li>Load the html page onto a browser</li>
<li>I used a desk easel to display my puzzle</li>
<li>While holding the ground to the Makey-Makey board in one hand, use the other hand to solve the puzzle.</li>
</ol>
