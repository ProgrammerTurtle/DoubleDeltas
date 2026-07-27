# DoubleDeltas

The successor to DoNotDelta - a high performance take on Colinear Double Delta Kinematics. 

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
