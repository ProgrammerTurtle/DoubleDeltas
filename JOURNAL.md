# DoubleDeltas

The successor to DoNotDelta - a high performance take on Colinear Double Delta Kinematics. 


# 2026-07-28
**Time spent: 4 hours**

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

620mm lets me use 500mm rails! Which are signficantly easier to find and cheaper than meter long rails. 

<img width="771" height="812" alt="image" src="https://github.com/user-attachments/assets/2cdb4934-1ebf-4c85-ab62-1b650e1a665c" />

Anywho, that's the final frame, with linear rails added. Now I can finally get to work on the corner joints that actually join the horizontal extrusions to the vertical ones, which will hopefully incorporate some CNC machined parts! Unless it costs too much of course. 

# 2026-07-27
**Time spent: 3 hours**

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
**Time spent: 1.5 hours**

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
