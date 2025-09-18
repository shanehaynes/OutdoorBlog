---
layout: post
title: "Physics of Climbing: Anchor Angles and Force Magnification"
date: 2025-09-18
category: musings
featured_image: "assets/images/AnchorAngles/generic.jpeg"
---

The construction of a solid anchor is an important component of a climber's toolkit, especially when engaged in the more esoteric pursuits of trad or ice climbing. While well placed bolts are rated upwards of 20 kilonewtons, which is a force unlikely to ever be reached climbing, removable anchor pieces placed by climbers (like cams or ice screws) on route can be rated much lower: such as 6 kilonewtons for example. Climbers interested in esoteric vertical pursuits should learn the science behind anchor making in order to construct safer anchors.

The art of building a beautiful anchor is complex and there are plenty of articles explaining _what_ one should do. If you are unfamiliar with anchor building, I recommend you first learn what to do. Here, we will dive into the science behind *why* some anchors are much better than others - specifically how the interior angle between pieces relates to load on those pieces. This will be much more relevant if you know anchor building basics already.

*If you are only looking for takeaways and want to skip the science portion, go to the examples and look at how different angles produce widely different loads. At some angles, traditional anchors **will not hold**.*
# The Science
We are modeling short, quasi-static snapshots of an anchor under load, using:
- **Vector resolution**
- **Static equilibrium** 

Vector resolution means our forces can be identified as either a vertical or horizontal component and static equilibrium means our vertical and horizontal forces must balance.

We will not be modeling the full dynamics of a fall (rope stretch, belayer slip, device friction transients). Inclusion of those variables would change the magnitude of force applied to the master-point but not the geometric distribution of it.

Some scientific assumptions throughout are: 
- A frictionless master point
- Slings/cordelette are massless and inelastic

Although important to admit for transparency, the inclusion or omission of the above do not change the overall meaning of our conclusions here. 

## Two Piece Anchor Equation

$T_1 = \frac{Fsin(\alpha)}{sin(\alpha + \beta)}$

$T_2 = \frac{Fsin(\alpha)}{sin(\alpha + \beta)}$

where 

$T_1 =$ force exerted on anchor piece 1

$T_2$ = force exerted on anchor piece 2

$F =$ load put on masterpoint

$\alpha =$ interior angle from masterpoint to anchor piece 1 

$\beta =$ interior angle from masterpoint to anchor piece 2


<div class="image-annotated">
  <img src="{{ '/assets/images/AnchorAngles/generic.jpeg' | relative_url }}" alt="Blank Anchor Example" />
  <div class="image-annotation"></div>
</div>

## Examples
For the following examples, a climber will take a factor 2 whip right onto an *equalized* anchor. This will typically generate between 6-10 kilonewtons of force, so we will take the middle of that: 8. 

#### Shallow Anchor Angle

We arrive at anchor station and build an anchor like so: 

<div class="image-annotated">
  <img src="{{ '/assets/images/AnchorAngles/shallow.jpeg' | relative_url }}" alt="Shallow Anchor Example" />
  <div class="image-annotation"></div>
</div>

This anchor has a very shallow interior angle of 30 degrees. Given an 8kn load at the equalized masterpoint, we can deduce that each anchor piece is experiencing 4.14kn. 

$T_1 = \frac{8sin(15\degree)}{sin(30\degree)} = 4.14$

Since $T_1 = T_2$ (this is true because the masterpoint is equalized), $T_2$ also equals 4.14. 

**At a 30 degree angle, each anchor piece will experience 4.14kn.**

#### Medium Anchor Angle 

Now assume we arrive at the anchor station and build this: 
<div class="image-annotated">
  <img src="{{ '/assets/images/AnchorAngles/normal.jpeg' | relative_url }}" alt="Normal Anchor Example" />
  <div class="image-annotation"></div>
</div>

This anchor has an interior angle of 90 degrees. Given an 8kn load at the equalized masterpoint, we can deduce that each anchor piece is experiencing 5.66kn of force. 

$T_1 = \frac{8sin(45\degree)}{sin(90\degree)} = 5.66$

Since $T_1 = T_2$ (this is true because the masterpoint is equalized), $T_2$ also equals 5.66. 

**At a 90 degree angle, each anchor piece will experience 5.66kn.**

#### Wide Anchor Angle

Now we get to the anchor station and faultily build this anchor: 
<div class="image-annotated">
  <img src="{{ '/assets/images/AnchorAngles/wide.jpeg' | relative_url }}" alt="Wide Anchor Example" />
  <div class="image-annotation"></div>
</div>

This anchor has a wide interior angle of 150 degrees. Given an 8kn load at the equalized masterpoint, we can deduce that each anchor piece is experiencing **15.45kn of force**. 

$T_1 = \frac{8sin(75\degree)}{sin(150\degree)} = 15.45$

Since $T_1 = T_2$ (this is true because the masterpoint is equalized), $T_2$ also equals 15.45. 

**At a 150 degree angle, each anchor piece will experience 15.45kn.** This is more force than a typical cam, nut, hex, sling, and other standard climbing gear can withstand. An anchor built at such a wide angle can experience anchor failure from the magnification of force.

#### Angles to Forces Table

To drive this home, see how forces dramatically increase at really wide angles. 

| Angle (deg)          | ~0  | 15   | 30   | 45   | 60   | 75   | 90   | 105  | 120 | 135   | 150   | 165   | 180 |
| -------------------- | --- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | --- | ----- | ----- | ----- | --- |
| Force per piece (kN) | ~4  | 4.03 | 4.14 | 4.33 | 4.62 | 5.04 | 5.66 | 6.57 | 8   | 10.45 | 15.45 | 30.65 | ∞   |

That is not a typo - it would actually take an infinite amount of energy to get the angle between the masterpoint and its anchor pieces to 180 degrees. Of course this will never happen but this theoretical limit highlights why the anchor absorbs an increasing amount of force with wider interior angles.

Also worth highlighting is how quickly the forces skyrocket when at the higher end of anchor angles. Small angle differences like that between 120 and 135 is the difference between 8 and 10.5 kilonewtons -  which could very well be the difference between an anchor withstanding and failing in real world climbing scenario.

On the other hand, if you have marginal anchor pieces that are causing worry, take advantage of anchor angles to increase the safety of your setup! If you shallow your anchor angles from 120 to 60, you can cut an 8kn force into a 4.5kn load for each anchor piece. That is a significant improvement! 

## Three Piece Anchors
With three piece anchors, the same fundamentals apply. 
<div class="image-annotated">
  <img src="{{ '/assets/images/AnchorAngles/threePeice.jpeg' | relative_url }}" alt="Three Piece Anchor Example" />
  <div class="image-annotation"></div>
</div>
We now measure angles by the sections between pieces. There are two sections in the depiction above. The total angle of the pieces placed may be 120 degrees but each section would only be about 60 degrees. This is the noteworthy change to three peice anchors. 

Three piece anchors do reduce the force experienced by each anchor piece, by virtue of there being more pieces, but not by as much may be anticipated. For example, with a 60 degree interior angle with a two piece anchor and an 8kn load, each anchor piece experienced 4.62kn. With three pieces, that reduces to 4kn. While force reduction may not be a compelling argument for including more pieces, evaluating the strength of your placements can be tricky so more pieces do allow for a greater margin of error in human judgement. 

#### 3 Piece Anchor Equation and Table

We used the below formula to calculate forces for the table above.

$T = \frac{F}{1 + 2 cos(\theta)}$ 

| Angle (deg)           | 0    | 15   | 30   | 45   | 60  | 75   | 90  |
| --------------------- | ---- | ---- | ---- | ---- | --- | ---- | --- |
| Force per piece  (kN) | 2.67 | 2.73 | 2.93 | 3.13 | 4   | 5.27 | 8   |

Illustrated clearly is a similar pattern to the table for two piece anchors. The higher the angle, the higher the forces. This relationship is not linear and at the higher end of angles, forces can jump a drastic amount. For example, at 75 degrees, our pieces experience approximately 5kn but at 90 degrees, they experience 8kn. 

This table does not go past 90 degrees for a reason: to build a 3 piece anchor in which the interior angles between pieces is greater than 90 degrees, you would have to put the masterpoint above the side pieces. This is an obviously flawed and pretty unrealistic anchor set up. 



$T = \frac{F}{1 + 2 cos(\theta)}$ 

# Take Aways 

Do not build anchors with wide angles between pieces, no matter how many pieces exist in the anchor. Forces can become greater than your pieces are capable of handling and anchor explosion due to load magnification is possible. 

How can you prevent this? The simple and easy way to prevent wide interior anchor angles is have the masterpoint a significant distance below the pieces of your anchor. The lower your masterpoint, the lower the angles between pieces and the lower the forces your pieces will experience. 

<div class="image-annotated">
  <img src="{{ '/assets/images/AnchorAngles/multiple.jpeg' | relative_url }}" alt="Multiple Anchor Example" />
  <div class="image-annotation"></div>
</div>

<span style="font-size:25px; text-align:center; display:block; font-style:italic;"> Therefore, create your masterpoint a good distance below your lowest placed anchor piece to reduce interior anchor angles. </span>


