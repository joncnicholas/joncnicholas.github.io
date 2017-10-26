---
author: joncn89
comments: true
date: 2016-01-06 13:00:34+00:00
layout: post
link: https://joncnicholas.wordpress.com/2016/01/06/a-flying-invention/
slug: a-flying-invention
title: A Flying Invention
wordpress_id: 375
icon: wordpress
image: envelope.jpg
category: flying
tags:
- Flight and Interview Resources
---

After a number of navigation trips since passing my PPL, I started looking for efficiency savings in time when it came to flying. I found the biggest use of time is navigation planning in the days before and the morning before the trip. As such, my day job has led me to produce some complex numerical models primarily in Excel and thought I’d try and produce a tool that will automate some of the navigation planning given a set of inputs. All in an effort to let me wake up later on the day!

Navigation planning is exceptionally important and the proper time should be spent on ensuring you have all aspects covered because being unprepared can lead to bad decisions, ultimately making a fun trip, hazardous.

I have created an Excel “Pre-Flight Calculator” (attached below) which effectively takes a set of variables and calculates: weight and balance (including fuel calculations), centre of gravity (CoG -including aircraft envelopes), and all necessary performance calculations. You cannot automate everything in navigation planning, but after a number of flights using various iterations of this calculator, I have been able to save circa 30-40 minutes on the morning If all pre-flight planning was complete prior.  The model does require input on a number of elements like landing & take-off ground roll and assessment of conditions to establish what performance conditions are pertinent on the day. However, once these are known the results process is automated and near instant.

{% include image.html
            img="/post-img/flying/Performance_tools/pfpm_front.png"
		max-width="1000px"
            title="Performance_Planning"
            caption="Performance Calculator front page" %}

<a href="/post-img/flying/Performance_tools/Pre Flight Calculator v1.9 - Master.xlsx">**Pre Flight Calculator v1.9 - Master**.</a>

I have created the model based upon Stapleford Flight Centre aircraft and out of the box it is compatible with the following general aviation aircraft types: Cessna 152 &172, Piper Warrior (PA28) and Arrow (PA28R). However, I have designed this model to be easily adaptable to any aircraft type with foundational excel knowledge given that the user knows the correct information to input i.e. aircraft schedule information, fuel limitations and aircraft envelope details. These can all be seen in ‘Aircraft Schedule info’ tab. What I have mentioned here is aimed at providing accurate weight, fuel and CoG representation. The last part of the model provides automated representation of the performance calculations. This section takes user input variables on airfield and performance conditions and uses model information in the ‘Airfields and Performance’ tab to accurately display required take-off and landing distances.

Audience and Considerations of use:

	
  1. I produced the model to streamline my planning. However, I envisage 3 further users for the tool: GA pilots wanting a free and easy to use tool (majority), GA pilots wanting to adapt it (minority) and possibly commercial pilots flying smaller aviation aircraft wanting to adapt it (few).

	
  2. If you want to use for general aviation purposes, then you can use this model out of the box with foundational excel knowledge. However, if you want to use it for new aircraft a basic understanding of excel formulae and logic is required to amend correctly.

	
  3. The model only supports aircraft using AVGAS 100LL fuel with a Specific Gravity of 0.72. It is not compatible with AVTUR because of my current uses. However, the fuel calculations are actually derived using weights and conversions which can be seen in Appendix A tab (AVGAS based). <span style="color: red">*Functionality added in **v1.7** - See comment #2*</span>

	
  4. If you want to use the model with new aircraft types ensure you change the third and fourth yellow tabs (described above) and ensure you sanity check the variables sheet as larger aircraft will require more boxes for more passenger weights and therefore, a small change to the weight and balance tab to reflect the aircraft.

	
  5. Units in this model are consistent throughout: Pounds [lbs] for weight and Litres [L] for volume. However, conversions to USG and Kilograms [kg] are present in relevant places. <span style="color: red">*As of **v1.9**, the introduction of meteorological units (hPa and degrees Centigrade) to ascertain pressure and density altitude in feet have been added - see comment #4.</span>


I’d relish feedback on the attached model so please use it, adjust it and disperse it to your heart’s content. Likewise, please feel free to comment.

I enjoyed producing this tool as it has given me a better understanding of the aircraft I fly, allowed me to become more efficient in my navigation planning and ultimately I hope it leads me to become a safer pilot.

<h1> Change Control </h1>

**1. Minor update to the calculator (v1.5 –>1.6 – January 08, 2016):**<br>
	Implemented automated update of distinct types in input Tabs 3 & 4 with array formulas – This allows aircraft types and new airfields to be automatically generated (limiting manual changes by user).<br>
**2. Minor update to the calculator (v1.6 –>1.7 – February 05, 2016):**<br>
	Implemented fuel variables (AVGAS & AVTUR) with Specific Gravity 0.72 and 0.8 respectively. Appendix 2 added for conversion table.<br>
**3. Minor update to the calculator (v1.7 -> 1.8 – July 05, 2016):**<br>
	Implemented the Piper Arrow II & III (PA28-200 & PA28-201) including envelopes and tested for any errors which came up clean.<br>
**4. Functionality update to the calculator (v1.8 -> 1.9 – July 07, 2017):**<br>
	Implementation of meteorological units (hPa and degrees Centigrade) and airfield elevation (ft) to ascertain pressure and density altitude in feet. Density altitude formula taken from <a href="https://www.aopa.org/training-and-safety/active-pilots/safety-and-technique/weather/density-altitude">**AOPA**.</a><br>
