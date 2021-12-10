---
layout: post
title: Einstein's Equations
joomla_id: 38
joomla_url: einsteins-equations
date: 2013-04-15 06:43:05.000000000 +00:00
---
<h3>Describing How Mass Warps Spacetime</h3>
<aside>
<ul>
<li><a href="index.php?Itemid=177">Review the meaning of warped space and time</a></li>
<li><a href="index.php?Itemid=179">See <span class="no-tooltip">Einstein's Equations</span> in action</a></li>
</ul>
</aside>
<p>One of the central challenges of physics is — and has always been — to predict how things move. The earliest astronomers were really nothing more than astrologers, trying to discern when stars would appear on the horizon, or where the Sun would be found at a certain date. Eventually, this turned into true, scientific astronomy, and physicists used their laws to predict how all sorts of bodies moved through the heavens. Newton showed us that the same laws that described how planets move could also be used to predict more earth-bound things, such as how an apple falls from a tree. Modern physicists are concerned with the motions of the tiniest particles in the atoms around us, and the motions of the heaviest objects in the heavens above.</p>
<p>We've mentioned that geometry gives us tools to understand the motion of particles when spacetime is curved. But it doesn't say anything about <em>why</em> spacetime should be curved. Einstein took the tools of differential geometry, and showed us how and why spacetime curves. In doing this, he gave us very powerful tools to predict the motion of particles. To understand how these tools work will only require a little review of how to keep track of points in geometry, and the Pythagorean Theorem.</p>
<h4>Coordinates</h4>
<p>Suppose you want to keep track of an astronaut who is somewhere along a single line, like in our examples from the section on <a href="index.php?Itemid=116" title="Relativity">Relativity</a>. You could choose a particular point — which we will call the origin — and measure how far the astronaut is from that point. If the astronaut is, for example, ten meters to the right of the origin, you might say that she is at the coordinate <i>x</i>=10. Ten meters to the left, and you could call it <i>x</i>=-10. She could even be at a fractional coordinate like <i>x</i>=6.78.</p>
<p><img class="caption" title="An astronaut at the coordinate x=10. Note the big blue dot representing the origin, at the coordinate x=0. " alt="astronaut 1D" src="images/einsteins_equation/astronaut_1D.jpg" /></p>
<p>Of course, coordinates are just numbers that we place at each point to label that point, and to keep track of what happens at each point. We can lay those numbers down in any way we want. We might, for example, only put in one coordinate tick for every <em>two</em> meters. Then, if the astronaut is at a coordinate of <i>x</i>=5, she would still be 10 meters to the right of the origin. We say that there is a factor of proportionality which is the real distance between coordinate ticks — two, in this case. Then, if we want the actual distance, we just multiply the coordinate <i>x</i> by the factor of proportionality:</p>
<p>$$\text{distance in meters} = x \text{ coordinate} \times \text{meters per coordinate tick}$$</p>
<p>It's very important to remember that the real physical situation doesn't change, even if we change how we label the physical points.</p>
<p>Now this astronaut may want to keep track of another astronaut, but he's strayed off the coordinate axis she is on. So, she decides to create a new set of coordinates, using two dimensions to keep track of him. She takes herself as the origin and constructs two axes — one in each of the two dimensions she needs. Then, to figure out what coordinates her fellow astronaut is at, she sees how far along one axis she would need to go, then how far parallel to the other axis she would need to go. For example, our second astronaut might be six meters to the right, and eight meters up. His coordinates would be <i>x</i>=6 and <i>y</i>=8. If he were eight feet down, his coordinates would be <i>x</i>=6, and <i>y</i>=-8. We can see this in the figure below.</p>
<p><img class="caption" title="A second astronaut in the new coordinate system, at coordinates x=6 and y=8." alt="A second astronaut in the new coordinate system, at coordinates x=6 and y=8." src="images/einsteins_equation/astronaut_2D.jpg" /></p>
<p>But now, if our first astronaut wants to get to the second, she wouldn't want to go six meters over and eight meters up; she'd want to go straight. To know how far she has to go, we need the help of an old theorem from high-school geometry.</p>
<h4>Pythagoras's Theorem</h4>
<p><img class="tnr caption" title="The Pythagorean Theorem" alt="The Pythagorean Theorem" src="images/einsteins_equation/pythagoras.jpg" />The Pythagorean theorem tells us the length of one side of a triangle, given the lengths of the other two sides. This is a very basic, and straightforward theorem that applies to any triangle with one right angle — that is, one angle of 90 degrees. The theorem is not very difficult to use. Suppose we have a triangle with a shortest side of 6 meters, and a second-shortest side of 8 meters. We take these numbers and square them (multiply them by themselves), giving 36 and 64 square meters. We add these together, and get 200 square meters. Now, whatever the longest side is, its square must be 100. The correct length, then, is 10 meters, since 10 squared is 100.</p>
<p>Using this knowledge, it's pretty easy to figure out how far apart our two astronauts are. One leg of the triangle is just the <i>x</i> coordinate; the other leg is the <i>y</i> coordinate. So, the distance between the two is given by</p>
<p>$$(\text{distance in meters})^2 = (x \text{ coordinate})^2 + (y \text{ coordinate})^2$$</p>
<p>If the coordinates measure meters, then he is 6 meters to the right and 8 meters up, so the Pythagorean Theorem tells us that he is 10 meters from the origin.</p>
<p>More generally, there could be a factor of proportionality to take into account, or even two — one factor for each dimension. In this case, we just have to incorporate those factors first to find the real distance in each direction, then use the Pythagorean Theorem to get the real distance from the origin. The formula in this case is just a combination of the last two formulas we've seen:</p>
<p>$$\begin{align}(\text{distance in meters})^2 = &amp;((x \text{ coordinate}) \times (\text{meters per } x \text{ coordinate tick}))^2 + \\&amp;((y \text{ coordinate}) \times (\text{meters per } y \text{ coordinate tick}))^2\end{align}$$</p>
<p>Basically, we've just dealt with any stretching that might happen to our grid. Of course, there's one more slight complication we'll need to deal with before we can understand Einstein's equations; some times, coordinates can be skewed, as well as stretched.</p>
<h4>Skewed Grids and The Law of Cosines</h4>
<p>We have already seen that curved spaces can make things complicated. For example, it's not always clear how to make a perfect square grid, like the one we assumed gave us our 2-D coordinates above. Some times, there's just no getting away from the fact coordinates might be skewed. Specifically, we might have a coordinate system where the <i>y</i> axis isn't perpendicular to the <i>x</i> axis. Instead, it might be tilted over at some angle.</p>
<p>We can look at this example with our two astronauts. Say the <i>y</i> axis is tilted over, as we see below. In this case, we would have to go farther to the right to be “under” the astronaut because when we go “up”, we have to go in the same direction as the skewed <i>y</i> axis. And, as a result, we would have to go farther “up” to get to him. To put some numbers to all this, say our axis is tilted by 15 degrees. Then, we'd actually have to go 8.14 meters to the right, and up 8.28 meters.</p>
<p><img class="caption" title="The two astronauts at the same positions as before, on a skewed coordinate grid. Note that the two astronauts have not moved — only the coordinates we use to keep track of them have changed." alt="The two astronauts at the same positions as before, on a skewed coordinate grid. Note that the two astronauts have not moved — only the coordinates we use to keep track of them have changed." src="images/einsteins_equation/astronaut_2Dskewed.jpg" /></p>
<p>As before, we want to know how far apart the two astronauts — we want to know how long that dashed green line is. We'd like to use the Pythagorean Theorem, but that only works for <em>right</em> triangles — triangles with one angle of 90 degrees. Fortunately, there's a more general version that will work even in this case. All it takes is one extra term in the formula. We know the length of two sides of the triangle, and the angle between them. If we call that angle α, then the “Law of Cosines” is just like the Pythagorean theorem, except that we subtract an additional term.</p>
<p><img class="caption" title="The Law of Cosines" alt="The Law of Cosines" src="images/einsteins_equation/cosine_law.jpg" /></p>
<p>Specifically, we take the normal Pythagorean Theorem, and subtract two times the length of one leg, times the length of the other leg, times the cosine of the angle between them. You might remember the cosine function here from high-school math class, written as “cos”. It takes the angle, and gives back another number, as shown below:</p>
<p><img class="caption" title="A plot of the cosine function. Notice that it is zero for 90°." alt="A plot of the cosine function. Notice that it is zero for 90°." src="images/einsteins_equation/cosine.jpg" /></p>
<p>When α is 90 degrees, the cosine is 0, so the extra term in the Law of Cosines drops away, and it reduces to the same thing as the Pythagorean Theorem. When α is less than 90 degrees, we see that the extra term makes the side with length <i>C</i> smaller, which we would expect. Similarly, if α is greater than 90 degrees, the extra term makes <i>C</i> larger.</p>
<p>Now, we can apply this formula for finding the distance between the two astronauts when the coordinates are skewed by the angle α:</p>
<p>$$(\text{distance})^2 =&nbsp;(x \text{ coordinate})^2 + (y \text{ coordinate})^2 - 2 \times&nbsp;(x \text{ coordinate}) \times (y \text{ coordinate}) \times cos(\alpha)$$</p>
<p>In this case, we've already measured the two sides of the triangle to be 8.14 and 8.28 meters, and we know that the angle between them is 90 - 15 = 75 degrees. If we plug these numbers into the formula, we find that the distance squared is 100 — so the distance is 10 meters, exactly as before.</p>
<p>This is an important point to make: the coordinates we used to measure everything changed, but the physical situation remained the same. In particular, the distance between the two astronauts didn't change just because we skewed the coordinate grid. We could also change the coordinates in other way — by moving the origin, say, or rotating the coordinates, or any combination. But still, the physical situation (distances, for example) wouldn't change.</p>
<h4>The Metric</h4>
<p>When laying down a grid for coordinates, we could also combine the stretch with the skew. In general, then, we would need a formula relating distance to coordinates like</p>
<p>$$\begin{align}(\text{distance in meters})^2 = &amp;[(x \text{ coordinate}) \times (\text{meters per } x \text{ coordinate tick})]^2 \\&amp;+ [(y \text{ coordinate}) \times (\text{meters per } y \text{ coordinate tick})]^2&nbsp;\\&amp;- 2 \times [(x \text{ coordinate}) \times (\text{meters per } x \text{ coordinate tick})] \\&amp;\times [(y \text{ coordinate}) \times (\text{meters per } y \text{ coordinate tick})] \times cos(\alpha)\end{align}$$</p>
<p>Obviously, this is starting to get complicated — and tiring to write out. We can save time and effort by grouping some of the terms together and writing this same formula as</p>
<p>$$(\text{distance in meters})^2 = g_{xx} \times (x \text{ coordinate})^2 + g_{yy} \times (y \text{ coordinate})^2 + 2 \times g_{xy} \times (x \text{ coordinate}) \times (y \text{ coordinate})$$</p>
<p>That is, we group those big terms together, giving them new names. Specifically, we define</p>
<p>$$g_{xx} = (\text{meters per }x \text{ coordinate tick})^2$$</p>
<p>$$g_{yy} = (\text{meters per }y \text{ coordinate tick})^2$$</p>
<p>$$g_{xy} = - (\text{meters per }x \text{ coordinate tick}) \times (\text{meters per }y \text{ coordinate tick}) \times cos(\alpha)$$</p>
<p>These three numbers we've defined — \(g_{xx}\) , \(g_{yy}\) , and \(g_{xy}\) — are very important in physics. Together, they form the metric, which relates physical distances to whatever coordinates we decide to use.</p>
<p>In general, the metric is just a little more complicated than the one we have shown here. First, we could be dealing with more than two dimensions. In three dimensions, we would add a <i>z</i> coordinate, and we would need \(g_{zz}\) , \(g_{xz}\) , and \(g_{yz}\) for the metric. We could even be working with time by adding a <i>t</i> coordinate. With all four dimensions, the metric involves the numbers&nbsp;</p>
<p style="text-align: center;">\(g_{xx}\) , \(g_{xy}\) , \(g_{xz}\) , \(g_{xt}\) , \(g_{yy}\) , \(g_{yz}\) , \(g_{yt}\) , \(g_{zz}\) , \(g_{zt}\) , and \(g_{tt}\) .</p>
<p>More importantly, the metric could change from place to place. If our coordinates were warped, we might have a grid that looks like our straight grid in one place, but is bent over like the second grid in another place.</p>
<p>It is possible to draw warped grids on a flat piece of paper (or on a flat screen, like we showed above). In this sense, we would get a warped metric in a space that is actually flat. On the other hand, it is impossible to draw a nice, straight grid in a space that is really curved. By very carefully examining exactly how the metric changes from point to point, we can tell if we've just drawn curvy coordinates in a flat space, or if we've drawn our coordinates in a truly curvy space.</p>
<p>Now we are getting very close to Einstein's Equations. Einstein had these warped pieces of spacetime that he needed to describe in some quantifiable way. He saw that a careful examination of the metric — and how it changes from point to point — could describe the true geometry of any spacetime, whether curved or flat, so he used it for his theory. Einstein combined certain numbers describing the metric's changes from place to place into what is now called the Einstein tensor. Just like the metric, the Einstein tensor is a set of numbers. For four-dimensional spacetime, we have</p>
<p style="text-align: center;">\(G_{xx}\) , \(G_{xy}\) , \(G_{xz}\) , \(G_{xt}\) , \(G_{yy}\) , \(G_{yz}\) , \(G_{yt}\) , \(G_{zz}\) , \(G_{zt}\) , and \(G_{tt}\) .</p>
<p>These numbers describe what is physically interesting about the geometry of spacetime. Understanding the geometry of spacetime allows us to see how particles will move, bringing us one step closer to the ultimate goal of physics. There is just one more ingredient left.</p>
<h4>Energy, Matter, and the Curvature of Spacetime</h4>
<p>We've gotten a sneak preview of Einstein's equations before: \(G = 8πT\). The \(G\) on the left stands for the different numbers in the Einstein tensor. But, the Einstein tensor represents the geometry of spacetime, so this is what the left side really represents. We also know that the curvature of spacetime is caused by matter, so the \(T\) on the right must represent matter.</p>
<p>Just like \(G\), the symbol \(T\) stands for a set of numbers:</p>
<p style="text-align: center;">\(T_{xx}\) , \(T_{xy}\) , \(T_{xz}\) , \(T_{xt}\) , \(T_{yy}\) , \(T_{yz}\) , \(T_{yt}\) , \(T_{zz}\) , \(T_{zt}\) , and \(T_{tt}\) .</p>
<p>These numbers measure different things about matter. Together, they make up the Stress-Energy Tensor. Each component of this tensor has a slightly different physical interpretation:</p>
<table class="data">
<thead>
<tr><th colspan="2">Pieces of the Stress-Energy Tensor</th></tr>
</thead>
<tbody>
<tr>
<td>\(T_{tt}\)</td>
<td>Measures how much mass there is at a point — how much density</td>
</tr>
<tr>
<td>\(T_{xt}\)&nbsp;,&nbsp;\(T_{yt}\) and \(T_{zt}\)</td>
<td>Measures how fast the matter is moving — its momentum</td>
</tr>
<tr>
<td>\(T_{xx}\)&nbsp;,&nbsp;\(T_{yy}\) and \(T_{zz}\)</td>
<td>Measures the pressure in each of the three directions</td>
</tr>
<tr>
<td>\(T_{xy}\)&nbsp;,&nbsp;\(T_{xz}\) and \(T_{yz}\)</td>
<td>Measures the stresses in the matter</td>
</tr>
</tbody>
</table>
<p>As we see from the table, things like stress, pressure, and momentum come into Einstein's equations. That is, stress, pressure, and momentum all have some effect on the warping of spacetime. This is related to Einstein's most famous equation, \(E=mc^2\), which says that energy has mass.</p>
<p>Warped spacetime affects how matter moves by changing its geodesics. On the other hand, Einstein's equations show us how matter — and its movement and pressures — affect the shape of spacetime. Thus, Einstein solved the fundamental problem in Physics — in principle. Of course, solving something in principle is very different from solving in practice. Finding real solutions has proven to be very difficult. Often, it is a job best left to computers.</p>
