<p>This plugin allows you to add a retro style high score name text field to your game. The player uses his / her keyboard to switch each character to the desired letter of the alphabet to make up his / her name.</p>

<p><strong>Usage is really simple:</strong></p>

<p>Include the entity in your module requires: 'game.entities.retrohighscorenamefield'</p>

<p>In your games init function spawn an instance of the entity by passing in two different fonts and the number of characters you need and then save the object returned so that you can ask it for the name later.</p>

<pre><code style="overflow: hidden; white-space: pre-wrap; max-height: none;" class="highlight prettyprint lang-null theme-balupton prettyprint-has"><span class="kwd">this</span><span class="pun">.</span><span class="pln">retroNameField </span><span class="pun">=</span><span class="pln"> ig</span><span class="pun">.</span><span class="pln">game</span><span class="pun">.</span><span class="pln">spawnEntity</span><span class="pun">(</span><span class="typ">EntityRetroHighsSoreNameField</span><span class="pun">,</span><span class="pln"> x</span><span class="pun">,</span><span class="pln"> y</span><span class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>fontNormal</span><span class="pun">:</span><span class="pln"> </span><span class="kwd">this</span><span class="pun">.</span><span class="pln">fontNormal</span><span class="pun">,</span><span class="pln"><br>fontHighlighted</span><span class="pun">:</span><span class="pln"> </span><span class="kwd">this</span><span class="pun">.</span><span class="pln">fontHighlighted</span><span class="pun">,</span><span class="pln"><br>numberOfChars</span><span class="pun">:</span><span class="pln"> </span><span class="lit">3</span><span class="pun">,</span><span class="pln"> </span><span class="com">// Optional, defaults to 3</span><span class="pln"><br>letterSpacing</span><span class="pun">:</span><span class="pln"> </span><span class="lit">20</span><span class="pln"> </span><span class="com">// Optional, defaults to 20</span><span class="pln"><br></span><span class="pun">});</span></code></pre>

<p>To get the name after saying the Enter key was pressed simply call getName()</p>

<pre><code style="overflow: hidden; white-space: pre-wrap; max-height: none;" class="highlight prettyprint lang-null theme-balupton prettyprint-has"><span class="kwd">this</span><span class="pun">.</span><span class="pln">retroNameField</span><span class="pun">.</span><span class="pln">getName</span><span class="pun">()</span></code></pre>