Download Link: https://assignmentchef.com/product/solved-cs6313-mini-project-1
<br>
<ol>

 <li> Consider Exercise 4.11 from the textbook. In this exercise, let <em>X<sub>A </sub></em>be the lifetime of block A, <em>X<sub>B </sub></em>be the lifetime of block <em>B</em>, and <em>T </em>be the lifetime of the satellite. The lifetimes are in years. It is given that <em>X<sub>A </sub></em>and <em>X<sub>B </sub></em>follow independent exponential distributions with mean 10 years. One can follow the solution of Exercise 4.6 to show that the probability density function of <em>T </em>is</li>

</ol>

(

0<em>.</em>2exp(−0<em>.</em>1<em>t</em>) − 0<em>.</em>2exp(−0<em>.</em>2<em>t</em>)<em>, </em>0 ≤ <em>t &lt; </em>∞<em>, f<sub>T</sub></em>(<em>t</em>) =

0<em>,                                                                    </em>otherwise<em>,</em>

and <em>E</em>(<em>T</em>) = 15 years.

1

<ul>

 <li>Use the above density function to analytically compute the probability that thelifetime of the satellite exceeds 15 years.</li>

 <li>Use the following steps to take a Monte Carlo approach to compute <em>E</em>(<em>T</em>) and <em>P</em>(<em>T &gt; </em>15).

  <ol>

   <li>Simulate one draw of the block lifetimes <em>X<sub>A </sub></em>and <em>X<sub>B</sub></em>. Use these draws to simulate one draw of the satellite lifetime <em>T</em>.</li>

   <li>Repeat the previous step 10,000 times. This will give you 10,000 drawsfrom the distribution of <em>T</em>. Try to avoid ‘for’ loop. Use ‘replicate’ function instead. Save these draws for reuse in later steps. [<strong>Bonus</strong>: 1 bonus point for not taking more than 1 line of code for steps (i) and (ii).]</li>

  </ol></li>

</ul>

<ul>

 <li>Make a histogram of the draws of <em>T </em>using ‘hist’ function. Superimpose the density function given above. Try using ‘curve’ function for drawing the density. Note what you see.</li>

</ul>

<ol>

 <li>Use the saved draws to estimate <em>E</em>(<em>T</em>). Compare your answer with the exact answer given above.</li>

 <li>Use the saved draws to estimate the probability that the satellite lasts morethan 15 years. Compare with the exact answer computed in part (a).</li>

 <li>Repeat the above process of obtaining an estimate of <em>E</em>(<em>T</em>) and an estimate of the probability four more times. Note what you see.</li>

</ol>

<ul>

 <li>Repeat part (vi) five times using 1,000 and 100,000 Monte Carlo replicationsinstead of 10,000. Make a table of results. Comment on what you see and provide an explanation</li>

</ul>

<ol start="2">

 <li>Use a Monte Carlo approach estimate the value of <em>π </em>based on 10<em>,</em>000 replications. [<strong>Ignorable hint</strong>: First, get a relation between <em>π </em>and the probability that a randomly selected point in a unit square with coordinates — (0<em>,</em>0), (0<em>,</em>1), (1<em>,</em>0), and (1<em>,</em>1) — falls in a circle with center (0<em>.</em>5<em>,</em>0<em>.</em>5) inscribed in the square. Then, estimate this probability, and go from there.]</li>

</ol>