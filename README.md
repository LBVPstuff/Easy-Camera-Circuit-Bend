# Easy-Camera-Circuit-Bend

An easy way to circuit bend a toy camera with a CMOS chip to take glitchy pictures, withonly basic skills needed in soldering. I wanted this project to be achievable by people with very little skills with soldering (like me) so everyone can try this little hack and take cool pictures. I will try my best to include a lot of details.

Big disclaimer here: I did not invented this hack, I discovered it with [this cool video](https://www.youtube.com/watch?v=hnv6Nud2QAo) by [overwhelminglyneutral (cool person)](https://www.youtube.com/@oneutral101) and I wanted to add more to it while making it more practical to use, by being able to switch between different effects.

The modifications we will be doing to the camera are reversible dans not directly soldered to the board, making it easy to swap if you need to get back to a normal toy camera.

## *What is circuit bending

Wikipedia says circuit bending is the creative customization of the circuits within electronic devices such as children's toys and digital synthesizer to create new musical or visual instruments and sound generators. Circuit bending is manipulating a circuit to get an output that was not intended by the manufacturer.
It is a really interesting and creative topic, but sometimes I find that it can get quite esoteric and difficult to understand, especially if you have no knowledge in electronics to begin with.

## *How this circuit bend works ?

Within this camera, there is a camera module, sending information to the motherboard inside the main body. This camera basically tells what it sees throught electric signals in 24 tiny cables and the motherboard is processing this signal to display it on the screen and save it on the SD card. 

What we want to do is mix thoses signals together by shorting some pins together and mess with the signals being sent to the motherboard.

To achieve this, you are supposed to solder tiny enameled copper wire to the 0.5mm connector pins on the main board, but it was way too difficult for me so I found an other way using adaptor cards and a spare ribbon cable.

## *Tools and materials you will need

### [The toy camera](https://www.amazon.fr/Faburo-Appareil-Num%C3%A9rique-Mpixels-Gar%C3%A7ons/dp/B07W45FTG8)
The Toy camera I used was [this Faburo Toy Camera](https://www.amazon.fr/Faburo-Appareil-Num%C3%A9rique-Mpixels-Gar%C3%A7ons/dp/B07W45FTG8). It is available on amazon and is pretty cheap, around 16 euros. There are also the same cameras available on aliexpress for a little cheaper if you are willing to wait a little bit more. Also, it is a good idea to check on the seconde hand market first, I found several there.

This circuit bend probably also work on many other cheap toy camera such as theses ones:
![[Pasted image 20250206162326.png]]

### [ 24 pin Ribbon cable to pins converter boards](https://fr.aliexpress.com/item/1005005485116729.html?spm=a2g0o.detail.pcDetailTopMoreOtherSeller.6.f003nvO5nvO55p&gps-id=pcDetailTopMoreOtherSeller&scm=1007.40050.354490.0&scm_id=1007.40050.354490.0&scm-url=1007.40050.354490.0&pvid=dd1d1b7d-951f-4a07-9ccf-86fbf27bccbe&_t=gps-id:pcDetailTopMoreOtherSeller,scm-url:1007.40050.354490.0,pvid:dd1d1b7d-951f-4a07-9ccf-86fbf27bccbe,tpp_buckets:668%232846%238113%231998&pdp_npi=4%40dis%21EUR%212.00%210.99%21%21%2114.70%217.27%21%40211b61a417367906687343405e3798%2112000033269437110%21rec%21FR%21%21ABX&utparam-url=scene%3ApcDetailTopMoreOtherSeller%7Cquery_from%3A)
I ordered them from aliexpress because it was the easiest way for me to souce these parts. The most important thing to know is that we need a **24pin adaptor with 0.5mm of paths thickness**. So make sure to tick the same boxes like in the picture when you order. **We will need 2 of these.**
![[Pasted image 20250206162057.png]]
