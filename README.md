# Easy-Camera-Circuit-Bend

An easy way to circuit bend a toy camera with a CMOS chip to take glitchy pictures, with only basic skills needed in soldering.

<img src="Readme ressources/preview.png">

:warning: **Big disclaimer here:** I did not invented this hack, I discovered it with [this cool video](https://www.youtube.com/watch?v=hnv6Nud2QAo) by [overwhelminglyneutral (cool person)](https://www.youtube.com/@oneutral101) and I wanted to add more to it while making it more practical to use, by being able to switch between different effects.

The modifications we will be doing to the camera are reversible and not directly soldered to the board, making it easy to swap if you need to get back to a normal toy camera.

## *What is circuit bending*

Wikipedia says circuit bending is the creative customization of the circuits within electronic devices such as children's toys and digital synthesizer to create new musical or visual instruments and sound generators. Circuit bending is manipulating a circuit to get an output that was not intended by the manufacturer.
It is a really interesting and creative topic, but sometimes I find that it can get quite esoteric and difficult to understand, especially if you have no knowledge in electronics to begin with. I wanted this project to be achievable by people with very little skills with soldering (like me) so everyone can try this little hack and take cool pictures. I will try my best to include a lot of details.

## *How this circuit bend works ?*

Within this camera, there is a camera module, sending information to the motherboard inside the main body. This camera basically tells what it sees throught electric signals throught 24 tiny cables and the motherboard is processing this signal to display it on the screen, save it on the SD card, add filters etc.

What we want to do is mix thoses signals together by shorting some pins together and mess with the signals being sent to the motherboard.

<img src="Readme ressources/goal of the bend.png">

To achieve this, you are supposed to solder tiny enameled copper wire to the 0.5mm ribbon cable connector pins on the main board, but it was way too difficult for me so I found an other way using adaptor cards and a spare ribbon cable. The result looks like this without a case to hold everything together :

<img src="Readme ressources/no case.png">

## *Tools and materials you will need*

### [The toy camera](https://www.amazon.fr/Faburo-Appareil-Num%C3%A9rique-Mpixels-Gar%C3%A7ons/dp/B07W45FTG8)
The Toy camera I used was [this Faburo Toy Camera](https://www.amazon.fr/Faburo-Appareil-Num%C3%A9rique-Mpixels-Gar%C3%A7ons/dp/B07W45FTG8). It is available on amazon and is pretty cheap, around 16 euros. There are also the same cameras available on aliexpress for a little cheaper if you are willing to wait a little bit more. Also, it is a good idea to check on the seconde hand market first, I found several there.

This circuit bend probably also work on many other cheap toy camera such as theses ones:

_______________________________________________________________________________

### Two [24 pin Ribbon cable to pins converter boards](https://fr.aliexpress.com/item/1005005485116729.html?spm=a2g0o.detail.pcDetailTopMoreOtherSeller.6.f003nvO5nvO55p&gps-id=pcDetailTopMoreOtherSeller&scm=1007.40050.354490.0&scm_id=1007.40050.354490.0&scm-url=1007.40050.354490.0&pvid=dd1d1b7d-951f-4a07-9ccf-86fbf27bccbe&_t=gps-id:pcDetailTopMoreOtherSeller,scm-url:1007.40050.354490.0,pvid:dd1d1b7d-951f-4a07-9ccf-86fbf27bccbe,tpp_buckets:668%232846%238113%231998&pdp_npi=4%40dis%21EUR%212.00%210.99%21%21%2114.70%217.27%21%40211b61a417367906687343405e3798%2112000033269437110%21rec%21FR%21%21ABX&utparam-url=scene%3ApcDetailTopMoreOtherSeller%7Cquery_from%3A)
I ordered them from aliexpress because it was the easiest way for me to souce these parts. The most important thing to know is that we need a **24pin adaptor with 0.5mm of paths thickness**. So make sure to tick the same boxes like in the picture when you order. **We will need 2 of these.**

<img src="Readme ressources/IMG_20250215_151707.jpg">

_______________________________________________________________________________

### Two rows 24 pins headers

I used a longer one that I trimmed to size, but you can find 24pins ones if you want. This will be used to connect the two adapter boards together. Alternatively, you can connect the big pins from the adapter boards directly to other stuff you want to use to short the pins, but I find this much easier and will be handy later.

<img src="Readme ressources/IMG_20250215_151742.jpg">

_______________________________________________________________________________

### Longer [24pin ribbon cable](https://fr.aliexpress.com/item/1005005982573926.html?spm=a2g0o.order_list.order_list_main.22.15f35e5bKARcTH&gatewayAdapt=glo2fra)
In order to connect the adaptor boards back to the main board of the camera, we will need another ribbon cable like this one :
<img src="Readme ressources/IMG_20250215_151718.jpg">

:warning: Make sure it is a **24pin ribbon cable with a thickness of 0.5mm**. I chose a length of 10cm, since it will more than enough for my case.

_______________________________________________________________________________

### Jumper wire
Or any wire that fits into our 24 pins header just to trigger the bends once we are finished.

_______________________________________________________________________________

### A soldering Iron

Any soldering iron will do, we are not going to do complex stuff with it, just make sure its tip is clean. If you don't know of to solder, i found [this video that cover all the steps we will need](https://www.youtube.com/watch?v=Qps9woUGkvI).

_______________________________________________________________________________

### Solder
Try using lead free solder, but again any solder will do the trick here.

_______________________________________________________________________________

### A small phillips screwdriver
We will be using it to disassemble the camera



## *Step by step guide*

I made a video tutorial on Youtube that covers all the steps to assemble the module, i find it easier to understand this way:

[![](https://img.youtube.com/vi/pKovYRPuqpo/0.jpg)](https://www.youtube.com/watch?v=pKovYRPuqpo)

Also you can find the complete pinout of the bends I found with [this link](https://docs.google.com/spreadsheets/d/120eRuoZbcSEhcIwTfrmM8TAaZlizbV74gkXWp9CGXoM/edit?usp=sharing), or in PDF format in the folder Pinout] of this repo. As mentionned in the video, **I strongly advise you to test out the bends on your particular camera**, since those are very cheap and vary a lot on one another, even with the same models.

After completing the module and plugging it into the camera, you will need a way to hold everything together nicely. To do so, I 3D modeled a new case for the camera, with more space to fit everything into it. If you have access to a 3D printer, you can print this with the flat side facing down with no support.

Then you just have to screw the camera module inside it, stick the connector pins throught the hole and plug the ribbon cable back into the camera. The current case holds together with duct tape but maybe later I will 3D model a new cas uses the screws used the hold the camera together originally.

<img src="Case 3D model/3D model.jpg">

:warning: **Make sure to test if the module works before putting it into its new case or it will be annoying to take it appart**

The 3D model can be found in this repo into the **Case 3D model folder**.

## *Future of this project*

I plan on doing "presets" for this camera. Using the exposed connector, i can plug a specific short that creates a glitch effect I like and have multiple of those presets modules into my pocket and switch between them idk.

Also I would like to do some "shields" that plung onto the connectors and able manual control with switch and potentiometers over the more interestings bends such as the pin 1 6 and 20. I have drawn some ideas and I could be a cool project to learn about PCB making.

<img src="Readme ressources/shields ideas.jpeg">

## *Here are some picture I took with it*

The timestamp can be removed in the parameters of the camera, and the image quality (mostly the size of the image on your SD card) can be changed as well. I am using 2 jumper cables for most of my pictures.

<img src="Some picture I took/PICT0035.jpg">
<img src="Some picture I took/PICT0048.jpg">
<img src="Some picture I took/PICT0053.jpg">
<img src="Some picture I took/PICT0093.jpg">
<img src="Some picture I took/PICT0104.jpg">
<img src="Some picture I took/PICT0114.jpg">
<img src="Some picture I took/PICT0125.jpg">
<img src="Some picture I took/PICT0133.jpg">
<img src="Some picture I took/PICT0165.jpg">










This work is licensed under CC BY-NC 4.0
