---
layout: project
type: project
image: images/peec-poster.png
title: Indigenous Knowledge in Engineering
permalink: projects/ike-peec
# All dates must be YYYY-MM-DD format!
date: 2020-07-02
labels:
  - Arduino
  - Engineering
  - Sustainability
summary: Created Arduino coding project in sustainability, “Using LEDs for Visible Spectrum Color Therapy Along a Temporal Axis.
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/micromouse-robot.png">
  <img class="ui image" src="../images/micromouse-robot-2.jpg">
  <img class="ui image" src="../images/micromouse.jpg">
  <img class="ui image" src="../images/micromouse-circuit.png">
</div>

Traditionally, Hawaiians believe that the rainbow is a pathway between the two worlds of the physical and the spiritual. Spiritually, the origin story of rainbows designate them as sad omens by Kahalaopuna, and also signify the presence of aura of ali’i. Rainbows were also used as communal weather forecasts, such as the kuhonu, the “male” upside-down rainbow, predicting flash floods, and six consecutive east facing rainbows predicting the 1931 Halema’uma’u crater eruption. Rainbows are created by water droplets refracting light, and it is this scientific explanation that gave initial inspiration to this project. Influenced by this Hawaiian culture focus, the personal project that is engineering related and also has a sustainability aspect is an LED panel that outputs various colors following Hawaiian mysticism according to time of day. This project was inspired by how mood rings are affected by a temperature variable and translates itself into different visual color. This color idea was expanded to visual representations on a RGB LED depending on the variable of time. Other variables such as the temperature and luminosity sensor were not appropriate due to Hawaii’s relatively temperate climate and potential light interference respectively. From further research into chromotherapy and Hawaiian mysticism, specifically targeting colors at different intervals were chosen depending on the scheduled activity. Each individual color has a unique therapeutic benefit and Hawaiian mystic effect on the human body, mind, and soul. By creating and using this LED code, a daily schedule would eventually become optimized for the user.

Here is some code that illustrates how we read values from the line sensors:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [Symposium Website](https://sites.google.com/hawaii.edu/2020peeciisymposium/kapcc/kelly-hwang?authuser=0)



