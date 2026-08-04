# DoubleDeltas

The successor to DoNotDelta - a high performance take on Colinear Double Delta Kinematics. 


# 2026-08-02
**Time spent: 2.5 hours**

Motor module 2 electric boogaloo??

Ok so, a friend told me to make some motor modules out of sheet metal. This is a good idea! Unfortunately I think it is out of budget... but it is nice to have around!! 

Anywho.

<img width="1100" height="668" alt="image" src="https://github.com/user-attachments/assets/7d5abb2a-f580-4ef5-8127-8276540d2200" />

Start with the same layout as before. 

<img width="1231" height="852" alt="image" src="https://github.com/user-attachments/assets/6a5f4794-2305-41a4-b001-aeeec71f10b4" />

Create a motor side plate. This plate is not thick enough for the bearing on its own - it will need stacked with another. That makes these motor modules 3 plates each. 3 times 6 is 18 plates total. Youch, my wallet.

<img width="1558" height="1087" alt="image" src="https://github.com/user-attachments/assets/a36b0057-05f7-4792-bcd6-42410508d043" />

Extend it and create a matching idler side plate. This plate can be thick enough for the bearings on its own, so it won't need stacked. This is good for budget.

<img width="1318" height="1132" alt="image" src="https://github.com/user-attachments/assets/056432a9-78ec-439d-a0ab-6c5284f4b54d" />

There's that second stacked plate. Each thin plate is 0.1". The thick plate is, you guessed it, 0.2". 

<img width="1108" height="949" alt="image" src="https://github.com/user-attachments/assets/50644c87-bc7d-400d-a44d-aead2d4e3cd5" />

From there I made these simple printed part structural spacers. These are designed to be minimal at the top so I can still hopefully route belts. I think it will be difficult to route belts in this design no matter what I do, but this could help. 

<img width="1385" height="828" alt="image" src="https://github.com/user-attachments/assets/7492fc36-67f4-46de-bfb5-0c2dada79597" />

Last, I just add screws and nuts that go through the whole sandwich. This is the easiest and most rigid way I could think of assembling. And I think it turned out really nice! 

It's just... these would add $200-$250 to my budget... I think I would rather bulk up the printed part. So that's what I will do next entry - bulk up the printed version! It is such a small part that I think it is fine - end to end, this thing is like, 110mm. So it really shouldn't matter much. 

Actually, one last thing.

<img width="1248" height="749" alt="image" src="https://github.com/user-attachments/assets/a19fd783-a08d-466b-beea-5d1f84ac1e31" />

This cutout will help a ton with belt routing. 

Ok that's all for real this time. 


# 2026-08-1
**Time spent: 3.5 hours**

Motor assemblies!!

These motor assemblies are required to get horizontal belt pathing without moving the motors outside of the frame. 

<img width="1072" height="831" alt="image" src="https://github.com/user-attachments/assets/88b0f702-3ba1-4b5a-be48-b9728e1b8e1d" />

You can see my preliminary sketch here. I will be using bearings and live shaft idlers to offset the motors about 72mm. Now, moving the motors out of the frame would be a 45mm offset. So, the difference is about an inch. That's really not bad! I am willing to accept that.

Anywho, I take that preliminary sketch and use fusion's Derive tool, which I just discovered, to move this design into a seperate document. That way we can keep the timeline of this part and the overall printer a bit cleaner. A bit.

<img width="1141" height="825" alt="image" src="https://github.com/user-attachments/assets/6699e86b-cde5-45ea-940e-924aa2462e3c" />

I am using 605 bearings basically everywhere here since they are nice and beefy for high tension 9mm belts. You can see them on either end of the pulley on the right as well as standalone slightly to the upper left of that pulley as an idler on the back of the belt. 
This setup mimics having the motor aligned with the carriage path without it actually being, as otherwise the motor would hit the frame. 

<img width="1172" height="981" alt="image" src="https://github.com/user-attachments/assets/29261b8c-240b-42b8-b010-70183ebc9790" />

I always like to start with doubleshear on the motor. No particular reason, that's just where I start. 

<img width="1097" height="977" alt="image" src="https://github.com/user-attachments/assets/d9f4ccbc-dd23-4f2e-a6b5-513fdbac5b44" />

From there it just gets extended. 

<img width="1371" height="968" alt="image" src="https://github.com/user-attachments/assets/7f0954eb-cf29-4921-b263-a2859f8c737e" />

Then I add the 30mm shafts for the idlers and some countersinks for the motor screws! That way I don't need super long motor screws. 

<img width="1214" height="809" alt="image" src="https://github.com/user-attachments/assets/5910a73d-d80c-4f96-aabe-56d0b4f04c69" />

I actually then extended up one end. I figured I can use this part to help locate the linear rail! So this print extends to exactly the height the linear rail needs. Since there is one on both top and bottom, it will sandwich the rail and align it.

From here, I decided to challenge myself a bit. I wanted this part to be organic! Not as blocky. 

<img width="1450" height="821" alt="image" src="https://github.com/user-attachments/assets/99b177c4-20be-45e7-bc6f-a632e0cfe2c8" />

So, I made this nice spline! This curve is pretty nice looking and is just defined by some random points and the idler bores. 

<img width="1447" height="902" alt="image" src="https://github.com/user-attachments/assets/5f09525a-98ee-41e5-b39c-46350c4c40dc" />

With a few fillets, you get a pretty nice result. 

Slight issue, however, is that this part is centered on the pulleys being centered. Which is fine, except that the pulleys have hubs. 

<img width="1246" height="775" alt="image" src="https://github.com/user-attachments/assets/52bd6512-113c-4db3-9f7b-31e8bcef4959" />

You can see those hubs here. So the actual belt is currently not centeed. This is a relatively easy fix! 

The one big constraint is that the end of this part, where the belt is coming out and the highest point of the part, needs to be 30mm wide. This is because my vertical extrusion is only 30mm wide. So, if it is wider, it will hit the horizontal extrusions of the frame. 

<img width="1385" height="963" alt="image" src="https://github.com/user-attachments/assets/a5481afe-032e-4a55-a287-dfb6ed2b77ea" />

With a couple extrudes here and there, some press pulls, blah blah, we get this!! 

The part looks super organic with the recesses on the sides and whatnot. Those are mainly there to provide enough material for the bearing but still keep the part thin enough at the end to fit between the horizontal parts of the frame! 

<img width="1657" height="1064" alt="image" src="https://github.com/user-attachments/assets/e03b15da-2353-4d6b-ba38-4d0b0bb464e2" />

And here they are in place in the frame. Currently they are mounted by 3 screws bolting up through the bottom plate and no other mounting. I may change that a bit though... Like, I could bolt to the extrusions, or I could bolt to the top plate of the frame sandwich, all for higher rigidity! 

For now, I am done though. I am pretty happy with this part as is. 


# 2026-07-30
**Time spent: 3.5 hours**

Carriages! 

Okay, these had me stumped for a while. I spent hours (that I am not logging) staring at what others have done, staring at my own CAD, staring at previous designs I have worked with. And I came to a conclusion - I don't like belt paths where the belt is perpendicular to the carriages.

I just don't. It is so annoying to work with. 

<img width="1268" height="748" alt="image" src="https://github.com/user-attachments/assets/64f4ac65-3ba9-4fb7-8a5c-f76c77bcfa45" />

This is what I mean by perpendicular by the way, sketched over a basic flat carriage I had thrown together. This carriage is what I spent most of my time staring at. Because, somehow, I needed to add belt clamps to this. I hated it. There wasn't a way I could think of to do it CNC, and that was something I really wanted to do for this project (cnc parts). 

So, I wanted the belt parallel to the carriages (aka rotated 90 degrees). This would be way easier to clamp the belts and allow for much lighter carriages. 

<img width="1549" height="979" alt="image" src="https://github.com/user-attachments/assets/c0023a8b-1063-452e-8ec7-7e1eea0712ce" />

<img width="1122" height="923" alt="image" src="https://github.com/user-attachments/assets/b8f49e1d-0d0b-4ee9-adc8-7913e4ce382b" />

<img width="957" height="864" alt="image" src="https://github.com/user-attachments/assets/0bbb3917-1dde-4cfd-aefe-bfff3d05968d" />

This is what I came up with. CNC machined unibody with a flat lasercut plate as a belt clamp. The plate is sandwiched between the carriage and linear rail carriage. So, I just crank down on the 4 mounting screws and it grabs the belt. The belt tooth geometry is based off of Ruiqimao's Carveoff belt clamps, as those are proven working for 9mm tension. 

A friend - well actually three friends - then suggested one change, which makes the carriages look nicer and way stronger.

<img width="1518" height="838" alt="image" src="https://github.com/user-attachments/assets/86119c42-ff55-4f37-b2bf-696310b2bd55" />

Diamond carriages! I think this looks awesome. 

Now, I keep having people telling me to double shear the ball joints. I don't think this is necessary. But, they didn't believe me. So, I decided to try and run a fusion 360 static force sim!


First, I calculated the max load on the carriages using a [tool from my friend Deadlock](https://github.com/dead-lock-ed/DeltaCalcs/tree/main). This gave me:

<img width="653" height="578" alt="image" src="https://github.com/user-attachments/assets/89d658bb-5591-46f0-a5e0-0bb080f29312" />

A max of 30 ish newtons for 500k accel. Not bad. I will be simming with 50 newtons just to be special and over the top. 

<img width="2099" height="1165" alt="image" src="https://github.com/user-attachments/assets/276cc8ed-bf18-4636-b5ff-e2f63d895cdc" />

After messing with the sim for a while, I got this result. Setting this up was weird and I have no idea if it is correct, but basically I just defined the screw connections as bolts into threaded holes, assigned materials, and it... worked? Oh I also put the middle of the carriage as stationary/locked in place so it would flex properly. 

Anywho, to explain the image. The numbers represent factor of safety. The lowest one on the joint is 35. This means that the strength of the part at that point is 35 times higher than the point it would noticeably deflect/fail. Meaning, this part is PLENTY strong. Unlesss I did the sim wrong of course, but I don't think I did? the deflection is exaggerated just to show what mode of force it is testing. 

That's carriages. I really like how these turned out - and most importantly, they only weigh 35 grams each! 35 grams!! Practically nothing. 

# 2026-07-29
**Time spent: 7 hours**

Frame! 
So, when I left off, we just had extrusions and linear rails. First order of business: connecting those extrusions together!

<img width="880" height="491" alt="image" src="https://github.com/user-attachments/assets/641c375c-cecb-46b0-972a-0a6435ed5c32" />

I started with a very simple shape that extends over the horizontal for mounting, and interfaces with the vertical for mounting. 

<img width="1174" height="780" alt="image" src="https://github.com/user-attachments/assets/ac384dc8-d16d-4259-bab0-d4c9b2a45fa4" />

After that, I add mounting holes. I am using M5 screws for pretty much all the frame stuff as it consolidates parts and makes assembly easier - I just buy a big bag of M5x10 socket head screws and send it. 

<img width="954" height="589" alt="image" src="https://github.com/user-attachments/assets/20567d3d-5e92-42a4-844b-2e65e8c5059b" />

These corner brackets will be printed out of some sort of fiber filled high performance polymer, like abs-gf. I actually tried a simpler CNC version, but it would've been $600 (before tariffs) to get all 12 of the brackets made, so that was a no. Printed it is! I can compensate by sandwiching with lasercut steel. I will show that soon. 

<img width="851" height="1019" alt="image" src="https://github.com/user-attachments/assets/a2ba1565-3b1d-41a9-99b2-3e4f419ffe98" />

I then add the 11 remaining brackets via a circular pattern and some copy pasting. My one complaint about copy pasting components, or moving components between parent components, in fusion 360 is that it absolutely nukes your timeline. But I guess if I didn't use a hybrid design approach it wouldn't be an issue. Alas, I do hybrid rather than top down (components completely seperate). Meh.

Bam, add screws. 

<img width="885" height="1124" alt="image" src="https://github.com/user-attachments/assets/804a98d8-0395-4f19-9e7c-97879f78d78b" />

6 screws per bracket, 12 brackets... that's 72 bolts!! Wow. This is gonna be fun to build! 

<img width="1619" height="1036" alt="image" src="https://github.com/user-attachments/assets/f14fdbdd-04c2-44ce-8c0e-565af5120c82" />

Next was working on those aforementioned plate sandwiches. I started out with 1/4 inch steel but ultimately ended up reducing it to 0.12" (practically 1/8") steel due to pricing. Gotta save money! 

Anywho, the panels have holes for bolting to the horizontal extrusions with M5 screws as well as bolting into the ends of the vertical extrusions with M8 screws. 

<img width="893" height="811" alt="image" src="https://github.com/user-attachments/assets/9be5cf29-3c73-4783-9128-5ca3d14f7c12" />

I also added two more holes to each corner for bolting into the plastic. I am not super worried about this since I am bolting to the aluminum so rigidly, but it does need a bit. I orginally had 4, aka 2 per bracket, but I went down to 1 because of a feature I will be adding later (steel cable eyebolts). 

<img width="1252" height="775" alt="image" src="https://github.com/user-attachments/assets/5d91d2fe-ecee-4333-ab94-ad52ed5ca6fc" />

Screws!! Keep in mind the bottom is currently identical to this top, so double everything. 

<img width="986" height="1051" alt="image" src="https://github.com/user-attachments/assets/db300644-4fbb-40ef-b326-e0e0d745540c" />

See! 

Now let's do some screw counting again. 

30 screws per side, double for top and bottom, that's 60 more screws, 48 of which are M5. So the count now is 132 screws, 120 of which are M5x10. 

Surely it won't get much higher?


So, remember how I said this is a steel sandwich? Right now, we only have the outermost panel of the two sandwiches (top/bottom assemblies). 

We gotta add the second panel of each sandwich! 4 panels total, 2 per top/bottom assembly. The motor modules will be bolting to these panels, so they are pretty important. They also help a lot with rigidity and weight. Making weight go up that is. Heavier is better for frame. 

<img width="1584" height="952" alt="image" src="https://github.com/user-attachments/assets/35a1a24b-1c54-442c-a9b0-c55986a09897" />

These panels are quite similar to the outer panels so I am not gonna show the full process. Just know they have cutouts for the belts to pass through, cutouts for the vertical extrusions, and one big cutout in the middle. I am not totally sure if that middle cutout will be staying but for now it is useful to let me see where I am working. And honestly, the more open the better, as that means I can mess with motors and stuff without dissasembling the frame!

<img width="1459" height="933" alt="image" src="https://github.com/user-attachments/assets/2cbbca6b-3855-46e8-b4f2-37baecca9fa5" />

More screws!!! These ones are all M5x10. 24 per side, thats 48 total. Add that to the 132 and we now have 180 screws! 168 of which are M5x10. Phew. This is rough.

<img width="2052" height="131" alt="image" src="https://github.com/user-attachments/assets/48859b02-e45d-4f4e-b576-f3025d257ba9" />

This is what I mean by nuking timelines, ugh. All the copy and paste icons are from organizing the screws in my CAD. Sorting them with their components etc. Absolutely ruins timelines. 


Last, but certainly not least, I add the eyebolts.

<img width="1556" height="549" alt="image" src="https://github.com/user-attachments/assets/f084d8aa-f2d8-4cf1-9875-f640fa8192dc" />

These bad boys are for attaching tensioned steel cable diagonals to prevent frame twist. There are 4 of these per side, and this time I mean side of the triangle that is the frame, not top/bottom. So, there is 12 total. You can kinda see the nuts at the bottom - they bolt through the entire sandwich. Should be more rigid and means I don't have to deal with tapping the panels after they get powder coated, which is kinda a nightmare. 

<img width="707" height="887" alt="image" src="https://github.com/user-attachments/assets/05bcddae-2173-4980-b401-e160591d1e97" />

That brings us to the end of this entry, the frame entry. I think it looks really nice, and more importantly, it looks rigid. It weighs about 40 pounds as is, which is nuts. It may not be possible to fly this fella without an oversized baggage fee. But that's probably fine... Later me problem!

To recap, we did:
- Printed corner brackets
- Steel Sandwich Panels
- Steel Cable Eyebolts

This took a lot of planning and research as I looked at how other deltas did their frame and how I could adapt it to my design theory/preferences. My biggest inspirations are Colphaer for the steel cable diagonals and 84Dragon (both on discord) for the style of corner brackets and plate sandwiches, though I did take fairly different approaches to both. 

So, what's next? In no particular order:
Carriages, motor assemblies, bringing in the effectors and assembling the gantries, endstop mounts, idlers, tensioning, electronics, and a bunch of little touches all over! 

I have a lot to do, but thankfully, a lot of time to do it. I love summer break. 



# 2026-07-28
**Time spent: 7 hours**

Ok. I kinda did a lot, but I also kinda only achieved a little. 
First things first, I made the bed effector setup. This was quick and easy - I reused the CNC machined effector piece so I can save money by buying two of the same part, and then slapped a bed on it. Instead of through bolting this bed I will be attempting to bond mounting points onto the back, much like how LH Stinger does it. We will see if it works! I sure hope so, as it makes using the fiberglass/carbon fiber bed as a print surface way easier. 

<img width="1288" height="340" alt="image" src="https://github.com/user-attachments/assets/a8ef94b9-0f49-4181-bd44-4b7749411d15" />

<img width="1453" height="988" alt="image" src="https://github.com/user-attachments/assets/c1c20e05-a89c-4cc2-a803-5b0c0189e373" />

Fairly simple! I need to add a few more screws but I wanted to move on. 

<img width="1492" height="345" alt="image" src="https://github.com/user-attachments/assets/9a43c591-a54b-4c87-aa63-29b5715d64fa" />

Next was the arms! This is a super simple part, with a 0.5mm wall stainless steel tube and the 2 cups of the MPJet Joints. 

This is a 200mm arm length. I would later find out this is wrong...

Next was the frame! Boy was this a doozy. 
I got this wrong a few times. 

<img width="921" height="1095" alt="image" src="https://github.com/user-attachments/assets/434498c2-fb87-40be-993f-797ff19a6265" />

I started at this scale. 800mm verticals and 300mm horizontals, fully 3060 extrusion. 

I then realized I was 130mm short. How was I 130mm off? Well, lets do the math. 

200mm arms + 180mm z height = 380mm needed travel. Double that to 760mm since it's a double delta. Round up to 800 and that gives me space for idlers in the middle and whatnot. Easy peasy.

Except, I forgot to take into account the height of the horizontal extrusions - 60mm plus 60mm, or 120mm total. Add 10mm as a buffer/to get to a nice imperial number, since the seller I am buying frame extrusions from sells in imperial and 930mm is a yard and 5/8 of an inch, which is a nice and easy number.



Wait, I forgot to take into account linear rail carriages! That's 45mm each. So... over a meter now...
I somehow ended up at 1120mm. This was a weird number, but I was convinced it was right. 

<img width="604" height="1037" alt="image" src="https://github.com/user-attachments/assets/4a20bed1-b1d4-4ad0-b47a-7d54b2b91b9d" />

Oh right, 1120mm because that lets me use 1 meter rails instead of cutting to 930mm. Easy. 


It was at this point I realized something felt off. And I was right! I was waaay bigger than I needed to be. 

How did I manage to get so far off? 'Cause the final frame ended up at 620.725mm (24.438 inches, the closest imperial size they sold to 620mm).

Well. 

I was sizing for 180mm of travel PER SIDE. I only need 90 per side. So yeah, I was almost double what I needed to be. 


Catching this mistake let me cut down the arms to 100mm and the frame height to the aforementioned 620mm ish. Makes things sooo much nicer and way more rigid than the floppy meter long nonsense.

When I tell you this took me 2.5 hours of back and forth math, I am not exaggerating. I went through so many different sizes. I started accounting for rails around the meter mark too, so I had more to adjust than the extrusion length and bleh. Wanted to stick to standard sizes.

The final math ended up being: 100mm arm length plus 90 mm z travel plus 45mm carriage is 235mm. Doubled (double delta) is 470mm needed travel. Rounding to 500mm gives me space in the middle for idlers and some overtravel. Add 120 for the frame horizontal heights and you get 620mm. 

620mm lets me use 500mm rails! Which are signficantly easier to find and cheaper than meter long rails. 

<img width="771" height="812" alt="image" src="https://github.com/user-attachments/assets/2cdb4934-1ebf-4c85-ab62-1b650e1a665c" />

Anywho, that's the final frame, with linear rails added. Now I can finally get to work on the corner joints that actually join the horizontal extrusions to the vertical ones, which will hopefully incorporate some CNC machined parts! Unless it costs too much of course. 

# 2026-07-27
**Time spent: 6 hours**

Toolhead!
As stated previously, this is made out of CNC machined aluminum. 

<img width="1410" height="1031" alt="image" src="https://github.com/user-attachments/assets/d197ea5d-4b0c-45ae-9d2d-b9ab1f192fd3" />

I started with a simple sketch defining a triangle that is circumscribed around a 59mm circle. Why 59mm? That was the smallest number I could get that still left space for the arm joints to do full range of motion without colliding. Weirdly specific, I know. 
The center hole is for the hotend.

<img width="1188" height="906" alt="image" src="https://github.com/user-attachments/assets/ce928a0e-3a5f-4550-91be-eb6dc354446f" />

That gets extruded, sides get filleted, and the joints get added with tapped m3 holes for mounting. No double shear should be needed since I am mounting to metal. 

Next was duct. I started by making a rounded cutout in my effector that I want as the start (well, actually midpoint ish, you will see) of the duct and a square I want as the outlet. 

<img width="1229" height="1023" alt="image" src="https://github.com/user-attachments/assets/48466d1f-4353-40a3-9e7e-8a210f58b6b9" />

<img width="1065" height="812" alt="image" src="https://github.com/user-attachments/assets/7180de03-c9c0-497a-9faf-c566afba47f3" />

I moved this square to align with where I want the air to go. The sizing of these was somewhat arbitrary, with the main design constraint being matching a certain cross sectional area - a gentle taper down to 70% of the inlet. So if the inlet is a 17mm circle (19mm hose with a 1mm wall), tahts about 230mm^2 I get to play with. 70% of that is 161mm^2, which is about what my outlet is.

You may be thinking, shouldn't that outlet be a lot smaller to account for the air stream being split into multiple ducts??

No.
I will be running 2 ducts. Each duct has its own hose and blower. That's right, dual cpap. 

<img width="941" height="986" alt="image" src="https://github.com/user-attachments/assets/e7d97daf-959e-4a1a-9ebd-e1fa61d223fe" />

Next is a loft with a curved centerline. This gets me my duct! 

<img width="1016" height="943" alt="image" src="https://github.com/user-attachments/assets/367e947c-6f38-4c5d-a480-310c829860e0" />

Then it gets mirrored to the other side of course.


At this point my friend was like. You know, having 3 ducts would make it symmetrical/match the delta-esque shaping. Triangles and such.

But having 3 CPAP blowers would be silly!! Absurd even!!


I love silly. 

<img width="1123" height="918" alt="image" src="https://github.com/user-attachments/assets/6f482df6-05ca-433d-b71d-ce06c5ce0e59" />

Triple duct, triple cpap. I will NOT be limited by cooling.

<img width="1124" height="788" alt="image" src="https://github.com/user-attachments/assets/f4e2b602-48b2-48d6-8a5d-c97237545524" />

Next is a little top plate for mounting the hotend. 

<img width="1059" height="937" alt="image" src="https://github.com/user-attachments/assets/d14ccc81-3c4e-4a93-a7b0-3a3b420fadf7" />

This guy just takes 3x 30mm M3 standoffs, super simple. And it's all metal, so hopefully rigid af. 

<img width="1264" height="917" alt="image" src="https://github.com/user-attachments/assets/089fe80a-b45a-4cd6-95a0-d554d281ba74" />

<img width="1117" height="979" alt="image" src="https://github.com/user-attachments/assets/4decff19-1ace-4679-82c6-875cf06c8b51" />

Another sketch and extrude gets us an extension to the top plate. This is for holding the 3 cpap mounts. 

<img width="1110" height="1004" alt="image" src="https://github.com/user-attachments/assets/4150dd1b-1654-4a0e-809b-f1dcec349820" />

<img width="833" height="934" alt="image" src="https://github.com/user-attachments/assets/4a5137ec-e4aa-4359-9a15-daa697f857a5" />

One more loft, extrude, and circular pattern gets us the upper section of duct. 
This is connected in one ring. The whole thing is mounted purely by compression from the upper plate and the effector through the standoffs - no additional hardware. It makes things rather clean.

And that's it! Kinda. I need to figure out how berd air hotend cooling works since I don't want a fan on the toolhead. But I don't even know if that takes any additional cad? We will find out!

This thing is silly. It's crazy overkill. It's bonkers. I love it though. Really sets the tone for the rest of this printer. 


# 2026-07-27
**Time spent: 2.5 hours**

Alright. Officially kicking this bad boy off. Basically, DoNotDelta V2 for real. Here is my X tier funding pitch:

--

DDs: DoubleDeltas.
DoNotDelta goes big. 

All new design. Bigger, better, faster.
180mm bed instead of 65mm.

Designed to push the speed benefits I initially sought to explore with this kinematic concept.

CNC machined parts. Metal panels. Tensioned steel cable diagonal bracing.

I learned a LOT building donotdelta. A bit of what works, a whole lot of what doesn’t. All this learning will be carried on through DoubleDeltas.

Now that donotdelta works, I feel confident that this motion system is worth exploring further.
So, go big or go home.


Tech specs:

MGN12 linear rails. No more janky linear rods.

2504MAC stepper motors sponsored by LDO

High rigidity engineering filament for all parts, Sponsored by Sunlu

High performance Duet clone electronics, sponsored by Fysetc.

Carbon fiber or thin wall steel arms for high rigidity and low mass (haven't decided)

Custom composite heated bed (carbon fiber or fiberglass) for high rigidity and low mass

Dual drive Boombox extruder configured in an ultra short Kevlar-sheathed Bowden setup.

Undecided high flow hotend - potentially custom.

--

So, from that initial pitch, a couple things hav ebeen decided/added on. First of all, after a lot of research, I have decided to use a Mellow Heatcore UHF ALPS for the hotend, with an MZE (meltzone extender). This should grant me plenty of flow, have good rigidity, and importantly, have nozzle probing. That will hopefully make callibration a lot easier overall, something I am looking forward to. 

<img width="606" height="930" alt="image" src="https://github.com/user-attachments/assets/26a3700a-f713-41b9-995a-cdfd1e4363cb" />

That looks like this. 

I also decided that for the frame I will be using metric 3060 extrusions. This is because I found them for cheap and they are large so they are high rigidity. Paired with MGN12H rails, I should have a really solid foundation to work off of. From there we get stainlesss steel arms and unibody machined effectors 
(aluminum) for even further rigidity. I am really leaning into rigidity here because I am sick of wimpy printers that can't handle proper belt tension and have issues with parts flexing (donotdelta...). 

I actually started working on an effector using SeeMeCNC barbells instead of MPJet joints and lasercut plates sandwiching them, like this: 

<img width="1049" height="865" alt="image" src="https://github.com/user-attachments/assets/f0a4c557-1ce1-49c0-afb0-0c67dcf3f47f" />

But ultimately I have decided that I will be sticking with MPJet joints and doing a CNC machined effector instead of lasercut plates. I will also likely be doing CNC machined carriages for the vertical towers, but I haven't decided. Definitely some CNC frame bits. I have the budget (i think), since I already have electronics and motors, which are usually two of the biggest costs. Well, most of the electronics. I need PSUs still. 

Speaking of PSUs, I actually didn't mention this in the X tier pitch, but I think I'm gonna do 48v motors. Once again a speed thing. I want to push this bad boy HARD. 

So yeah. Let's have fun with this one! No burn out for months like with DoNotDelta. 
