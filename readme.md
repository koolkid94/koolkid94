![title.png](title.png) </center>


<center> A total "overhaul" of TacZ 1.1.7 with new features 

![Jdk-17.0.6.10-hotspot 2025.12.19 - 14.23.32.01.gif](Jdk-17.0.6.10-hotspot%202025.12.19%20-%2014.23.32.01.gif) </center>


<center> Modular Attachment System </center> 
<center> Magazines and Animated Firearm Manipulations 

Rough Project Scope & Outline [here](https://docs.google.com/document/d/17dVBlS1kNZ8BBDibv30S84Fb3FFpDjXTLl2TkmrA0iU/edit?tab=t.0)

Check out the New Branch  [here](https://github.com/koolkid94/tacz_mags/tree/intellij-project) 


![img_2.png](img_2.png)

Currently, a private build, as assets are taken from pre-existing works. No release is planned. Overall design direction is trying to give the mod a more open-ended / "sandboxy" feel and to move away from the arcady feel of the base mod. Guns are no longer just stat tweaks of each-other, but each a unique item with its own intricacies and balancing issues implemented through ammunition choices and attachment accessibility. Attachment mounting system loosely models a variety of mounting solutions. 

![Jdk-17.0.6.10-hotspot_2025.12.24_-_10.49.44.02.gif](Jdk-17.0.6.10-hotspot_2025.12.24_-_10.49.44.02.gif)
</center>Animations Needed:

mag_unload<br>
--> removing magazine<br>
mag_load<br>
--> inserting magazine<br>
mag_load_bolt<br>
--> inserting magazine on open bolt<br>
mag_load_empty<br>
--> inserting magazine on empty chamber<br>
breach_load<br>
--> single shot reloading<br>
prime<br>
--> manipulating charging handle to expel chamber<br>
prime_empty<br>
--> manipulating charging handle<br>
unjam (do later)<br> (low priority)
--> unjamming a stovepipe<br>
fold<br>
--> folding stock <br>
unfold<br>
--> unfolding stock <br>
low_ready <br>
--> place gun in low ready (safety on) <br>

![img_4.png](img_4.png)

![Jdk-17.0.6.10-hotspot 2025.12.31 - 00.22.22.06.gif](Jdk-17.0.6.10-hotspot%202025.12.31%20-%2000.22.22.06.gif)

![img_6.png](img_6.png)

![img_5.png](img_5.png)

and much much more...!

toggle (do later) (priority 1)
--> toggling magnifier<br>

elcan_swap_in(do later) (low priority)
--> move elcan lever in<br>
elcan_swap_out(do later)
--> move elcan lever out<br>
lpvo_dial_in(do later)
--> zoom lpvo in<br>
lpvo_dial_out(do later)
--> zoom lpvo out<br>
tactical (do later)
--> turn on/off laser/light/switch<br>
remove sight (do later)
--> remove equipped optic<br>
remove silencer (do later)
--> remove silencer<br>
remove grip (do later)
--> remove grip<br>

change batteries (do later) (low priority)
--> change batteries on optic<br> <center>

![Jdk-17.0.6.10-hotspot 2025.12.24 - 11.07.32.03.gif](Jdk-17.0.6.10-hotspot%202025.12.24%20-%2011.07.32.03.gif) 

![Jdk-17.0.6.10-hotspot 2025.12.19 - 00.23.21.01.gif](Jdk-17.0.6.10-hotspot%202025.12.19%20-%2000.23.21.01.gif) </center>

--JAVA--<br>
ModAnimationConstant --> constant, to be passed into lua machine<br>
LocalPlayerANIMATIONNAME --> client side handling of triggering of animation<br>
ModClientPlayerGunOperator --> interface holding the undefined function for the logic (be sure to sync with server thru messages)<br>
ANIMATIONNAMEKey --> handles keybind<br>
--LUA-- (in tacz default pack)<br>
DefaultStateMachineLua<br>
runANIMATIONNAME<br>
-(input getter function)<br>

![img.png](img.png)

![img_1.png](img_1.png)

![2025-12-26_14.41.40.png](2025-12-26_14.41.40.png)