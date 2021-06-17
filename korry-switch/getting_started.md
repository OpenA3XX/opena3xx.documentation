---
description: Everything you need to know to build your own OpenA3XX Korry switch!
---

# Getting Started

![3D Visualization](../.gitbook/assets/5%20%282%29%20%282%29%20%282%29%20%282%29%20%281%29.png)

We have designed this Korry switch to be a very effective and efficient unit. It is a great part of the project to start with for those who may be unsure of their soldering abilities or want to test the waters with something a bit smaller first.  
For those who are experienced, this unit will be a hassle free and simple addition to your existing projects.  
We are aware that the fact this unit uses a PCB may be a bit off putting to some people, but we assure you it is very accessible, cheap and easy to use. We believe this design makes it much easier to use, and easy to connect to other hardware.  
Please read through these pages carefully, as everything is explained in detail. If you have questions, please don't hesitate to contact us.

## What You Need:

### **Parts & Components**

1x 3D printed outer shell  
1x 3D printed inner shell  
1x Acrylic inlay _\(see_ [_below_](getting_started.md#acrylic-inlays) _for more detail\)_  
1x PCB _\(see_ [_below_](getting_started.md#pcb) _for more details\)_  
2x Square LED _\(2mm x 3mm x 4mm\)_ in appropriate colours  
1x Push switch \(5.8mm x 5.8mm\)  
_\(in either self-locking or no-locking depending on type required\)_  
2x 270 ohm SMD resistors _\(1206 footprint\)_  
1x Pin header _\(1 row of 5\)_ 2.54mm

### **Tools**

Soldering iron  
Flux  
Solder  
Solder pump  
Helping hand  
Multimeter _\(Electrical/continuity circuit tester or some kind\)_  
Calipers

## 3D Printed Parts

The 3D printed parts consist of an inner and outer shell.

![](../.gitbook/assets/4%20%282%29%20%281%29%20%281%29.png)

The smaller part sits inside the larger part, and they are held together by friction. The top of the switch is joined into the hole of the inner part, and it moves with the switch. This is the same for both the locking and non-locking switches.

{% hint style="warning" %}
When you print these, please double check their sizes with calipers!

The outer shell should be 20mm x 20mm \(**not** including the lip\).  
The inner shell should be 16.8mm x 16.8mm.
{% endhint %}

When you're ready to print them, please goto the GitHub and download these 2 files:  
[**KS-3D-IN1.stl**](https://github.com/OpenA3XX/opena3xx.3D-CNC_Parts/blob/main/Korry%20Switch/3D%20Print%20Parts/KS-3D-IN1.stl)  
****[**KS-3D-OUT1.stl**](https://github.com/OpenA3XX/opena3xx.3D-CNC_Parts/blob/main/Korry%20Switch/3D%20Print%20Parts/KS-3D-OUT1.stl)\*\*\*\*

{% hint style="danger" %}
Print them in the orientation they are currently in. You will only need to add a support to the bridge on the inner part. No support is needed anywhere else as the lip on the outer part prints fine without support.
{% endhint %}

## **Acrylic Inlays**

The acrylic inlays are the surface of the actual button. The bit that your finger presses.  
It is a small peice of acrylic that is 2mm thick and is 14mm x 14mm.  
The acrylic is painted black on one side, and then the text is engraved through that paint, **MIRRORED!**   
It must be mirrored because the painted/engraved side will be the back, leaving the front to be smooth and clear for surface to push.

![Painted &amp; engraved \(mirrored\) side becomes the back.](../.gitbook/assets/img_5352.jpg)

![This side then becomes the front, the part that is actually pressed.](../.gitbook/assets/img_5351.jpg)

You can find out how to make these \(or order them to be made\) on the [Acrylic Inlay page](acrylic_inlays.md).

## PCB

The PCB is something that may be worrying or concerning to you. You may be thinking you can't make these yourself, or that it's too complicated.  
Please be assured that it is a really easy solution, and all of the hard work is already done for you.

In short, you only need to download the relevant files and send them off to a PCB manufacturer. There is even the option of having them install the small components to the board for you if you wish.  
The cost of having these boards made is actually a lot cheaper than you think!  
You can find out more about this on the [PCB page](pcb.md).

![3D render of PCB.](../.gitbook/assets/korry_pcb2%20%282%29.png)

