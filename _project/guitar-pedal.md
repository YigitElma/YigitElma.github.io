---
title: "Compressor, Overdrive and Delay Eﬀect Pedals for Electric Guitar"
img: pedals.webp
collection: project
date: 2022-04-12
---
<div align="justify" style="margin-bottom:10px;">
When I was 10, as a birthday present, I asked for <i>"Guitar Hero"</i>, a popular game at the time. My mom said, "I can buy you an actual guitar instead!". A bit cliche -for my generation- but this is how I started playing electro guitar. I may not be a virtuoso today, but I have a talent that most guitar players don't. I am an engineer! :smile:
</div>

<center>
<img src="/images/pedals.webp" alt="First Pedal" style="width: 90.0%;border-radius:3px;margin-top:8px;margin-bottom:8px;"/>
</center>

<div align="justify" style="margin-bottom:10px;">
As you know, sound is transported in waveform. For electro guitar, this is the alternating electrical signal induced by the vibration of strings on the guitar's electromagnetic coils, aka. Pick-ups. Usually, these are sinusoidal waves; however, one can change the shape to get different tones. Although the actual notes itself does not change, the distinct features of the sound may be highly different.
</div>

<center>
<img src="/images/screamerCircuit.jpeg" alt="TubeScreamer Clone" style="height:300px;border-radius:3px;margin-right:30px;margin-top:8px;margin-bottom:8px;"/>
<img src="/images/screamerPots.jpeg" alt="TubeScreamer Inside" style="height:300px;border-radius:3px;margin-top:8px;margin-bottom:8px;"/>
</center>

<div align="justify" style="margin-bottom:10px;">
You may be familiar with the terms capacitor, transistor, and op-amp from your physics or circuit courses. Arranging those components can result in an intended effect on the sound, such as compression, distortion, overdrive, etc. There are sound engineers explicitly working on the design of these circuits. However, this project was to test my handcrafting skills, create valuable products for my hobby, and learn about electronics during the process. Now, I am much more confident in electronics. For example, in courses, you only see the symbol of a capacitor or an op-amp, but by physically working with them, I saw different types of them, why they are different, and how can their unique properties benefit other applications.
</div>

<center>
<img src="/images/signal-change.png" alt="How clipping works" style="width: 70.0%;border-radius:3px;margin-top:8px;margin-bottom:8px;"/>
</center>

<div align="justify" style="margin-bottom:10px;">
The above figure shows the effect of op-amp and diodes. In <b>A</b>, the original signal is amplified by a gain circuit whic uses op-amp. In <b>B</b>, you can see that the top portion of the sinus wave is trimmed. This is due to the diode connected to the ground. When the current is above what the diode can block in reverse direction, excess current goes to ground. If you use two reverse diodes in parallel to the ground, you achieve a signal shown in <b>C</b>. This is the basic principle behind the distortion pedals used extensively in Rock and Metal songs.
</div>
<div align="justify" style="margin-bottom:10px;">
In our daily lives, we may sometimes miss-use or not understand electricity. For instance, one shocking example of this is the voltage supply of an adapter. You may think a charger should give constant voltage since nearly all electronic devices use DC. However, most adaptors do not convert AC to perfect DC. A small amount of noise always remains if you are not using an isolated power supply, such as a Li-Po battery. If your guitar pedal does not filter these, your amplifier will increase its amplitude and cause an actual noise. In fact, when you plug in an adaptor, you collect all the dumped signals of your electronic devices in your house from the ground. For many applications, it's not worth caring about it, but in my project, I had to. That is why I built custom adaptors to filter the fluctuations in the voltage by using various capacitors, diodes, resistors, and voltage regulators.
</div>

<center>
<img src="/images/painting.jpeg" alt="Painting Process" style="width: 35.0%;border-radius:3px;margin-top:8px;margin-bottom:8px;"/>
</center>