# 🚀 audion-receiver-3

New audion receiver modell, with tuned amplifier. This is the third model of this old radio version, it's fun and works very well. **Try it yourself.**

**I will make a video about it soon and post the link here.**

# ⭐ The circuit

This circuit is similar as first and second version, but there is **tuned preamplifier** in this version. Why?

![image](https://github.com/user-attachments/assets/08c44f44-f1ee-4207-9c09-9d120852517b)

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


