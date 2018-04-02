---


---

<h1 id="from-makecode-to-python-while-loop-and-if-statement">From Makecode to Python: while loop and if statement</h1>
<p><a href="https://youtu.be/x1b70lIpeT8">Screencast on while vs. if in Makecode</a><br>
<a href="http://youtu.be/VGLsfKFcIFw?hd=1">Screencast on translation</a></p>
<h2 id="while-vs.-if">While vs. If</h2>
<p>While Program<br>
<img src="https://gracehanningxu.files.wordpress.com/2018/03/screen-shot-2018-03-15-at-1-58-24-pm.png?w=294&amp;h=254" alt="enter image description here"><br>
<img src="https://gracehanningxu.files.wordpress.com/2018/04/screen-shot-2018-04-01-at-3-51-19-pm.png?w=337" alt="enter image description here"><br>
If Program<br>
<img src="https://gracehanningxu.files.wordpress.com/2018/03/screen-shot-2018-03-15-at-1-42-19-pm2.png?w=302&amp;h=221" alt="enter image description here"><br>
<img src="https://gracehanningxu.files.wordpress.com/2018/04/screen-shot-2018-04-01-at-3-52-47-pm.png?w=305" alt="enter image description here"></p>
<p>In Makecode, the blue <em>if</em> statement cannot run on it self, so I put it into a “on start” block so that the code would run. Similarly, the <strong>while</strong> loop also needs to be inside the “on start” block. As you can see, the two programs are completely identical other than the <strong>while</strong> loop between the two blocks in the second program. Similarly, to change the <strong>while</strong> program into an <em>if</em> program, I simply took out the “While True” line and deleted the spaces before the if and else conditions.<br>
After trying out these two sets of programs on the CPx, I came to the understanding that without the <strong>while</strong> loop enclosing the <em>if</em> statement, the program would only run through the <em>if</em> statement once. On the other hand, if we add in the <strong>while</strong> loop surrounding it, the program would run for as long as the condition of the <strong>while</strong> loop remains true. My screencast (linked above) shows the differences using animation on the CPx simulator provided by the Adafruit website.</p>
<h2 id="program-translation">Program Translation</h2>
<h3 id="makecode">Makecode</h3>
<p><img src="https://gracehanningxu.files.wordpress.com/2018/04/screen-shot-2018-04-01-at-3-32-05-pm.png" alt="Screen Shot 2018-04-01 at 3.32.05 PM.png"></p>
<h3 id="python">Python</h3>
<p><img src="https://gracehanningxu.files.wordpress.com/2018/04/screen-shot-2018-04-01-at-3-27-28-pm.png" alt="Screen Shot 2018-04-01 at 3.27.28 PM.png"><br>
In the translation of Makecode to Python (or Python to Makecode, for that matter), it is important to pay attention to the slight stylistic differences, although most functional lines are similar between the platforms. In the above example, for example, it is quite easy to identify the “set all pixels to___” blocks, the <strong>while</strong> loops, and the <em>if</em> statement conditions in both platforms.<br>
In Makecode, all commands must be put into a general block, usually the “forever” block that I used on the outermost. This block makes sure that the contents inside this block runs again and again. It is most commonly used in conjunction with the <strong>while</strong> loop. There is also the “on start” block, which only runs through all the code enclosed in it once.<br>
In Mu, it was imperative that I imported certain functions from datasets so that functions would run. I also had to set the initial sensor setting to 0, and attribute a variable name to the light sensor.<br>
Essentially, this program told the CPx to shine white light if light level &lt;= 100, shine red light if 100 &lt; light level &lt; 200, and shine green light if light level &gt;= 200. Because all these commands are in a <strong>while</strong> loop, which means that it runs through the commands multiple times, as I change the light level, the CPx would change colors accordingly.</p>

