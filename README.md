# 🚀 audion-receiver-3

New audion receiver modell, with tuned amplifier. This is the third model of this old radio version, ❤️ it's fun and works very well. ❤️ **Try it yourself.**

**I will make a video about it soon and post the link here.**

# ⭐ The circuit

This circuit is similar as first and second version, but there is **tuned preamplifier** in this version. Why?

![image](https://github.com/user-attachments/assets/08c44f44-f1ee-4207-9c09-9d120852517b)

## 📐 How it works?

▶️ **Channel selector:** 

This section is a tuned bandwidth filter. 

😡 What does it mean that selectivity is weak if there is only one resonant circuit in the radio? 😡 The strongest radio station can be heard in the full band. 

▶️ **Input** stage:

  - receives the antenna signal
  - make impedance transformation

▶️ **Tuned RF preamplifier** stage:

Second bandwidth filter in collector section.

  - tunnable f0 of bandwidth
  - tunnable gain of amplifier

▶️ **Audion with filter** stage:

  - make signal demodulation
  - filter for smoothing the carrier signal

▶️ **Output** stage:

  - separation stage between headphones and audion
  - make impedance transformation for headphone

## ⭐ Simulation (frequency transfer)

Parameters of simulaton:

Parallel LC:
- L = 330uH
- C = 400pF

Input voltage generator:
- Vp = 1V
- R_gen = 200ohm
- 
**Channel selector:**

This parallel LC circuit performs very weak filtering. The "Channel selector" name comes from super-heterodyne technology where the IF frequency and the frequency of the actual band is far apart. In that case this function is more effective as in a non frequency-transformer circuit.

You can see here the Bode-chart

![image](https://github.com/user-attachments/assets/ea0b8126-370e-4f37-97fd-293203dc166e)

**Input** stage:

This circuit make an impedance transformation between the antenna and the preamplifier. The Bode diagram showing the current in capacitor C2, which controls the bipolar transistor of the preamplifier.

![image](https://github.com/user-attachments/assets/0265fce7-7fef-4710-bd2e-a97db8ab18cc)

**Tuned RF preamplifier** stage:

Here you can control the gain of the preamplifier with a potentiometer. The second parallel LC circuit is located here in the collector section. Look at the transfer function if the preamplifier potentiometer remains at 10%. ❤️ Selectivity is better!

![image](https://github.com/user-attachments/assets/4ef140b7-c7a6-45d8-b486-a833fe05acce)

**Audion with filter** stage:

This stage provides the AM demodulation and reduces the frequency of carrier. This diagram showing the voltage after C7 which goes to Gate of FET in output stage.

![image](https://github.com/user-attachments/assets/487e15c2-eefa-47d4-b79a-c2e1bde7445a)

## 🔀 Variable capacitor

You can find a simple variable capacitor from an old radio. You can see it here:

![image](https://github.com/user-attachments/assets/5c950bc2-e86f-4a89-848e-30a9ef93c83f)

This capacitor have two parts on a shaft. One part for "channel selector" (bevor input stage), the other for oscillator section.

Luckily, you can find such a model, where the two parts have equal capacity. (In many case, the part of capacitor for oscillator have smaller capacity.) **If you find a model like that, you can use it in this circuit.**

## ♊ Tow parts of capacitor

Where should the two parts of the capacitance be connected?

**First part** is the channel selector. (red circle) 

![image](https://github.com/user-attachments/assets/237be0cf-63e5-4bec-8b60-c240e6e7c56b)

**Second part** is the resonant LC circuit for RF preamplifier in collector section.

The selectivity of this radio is increased by the LC circuit. (orange circuit)

![image](https://github.com/user-attachments/assets/cffae2a8-1ed9-4a8d-ade1-bf8c14fc95b3)


## Contact

Varga Laszlo - https://vargalaszlo.com - mail@vargalaszlo.com

Project Link: https://github.com/vargalaszlo87/audion-receiver-3

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](http://vargalaszlo.com)
