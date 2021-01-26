# Growth Curve Fitting

One of the most common experiments in microbiology is the growth curve. Typically, absorbance measurements (wavelength = 600 nm) are taken over time, which correspond to cell density in the liquid medium. As cells divide to reproduce, their overall growth reflects an exponential process, until they run out of food and stop growing. These growth curves are often used as *qualitative* data to show that cells grew more slowly or to a lower density in one condition compared to another. However, there are many ways that growth curves can be understood *quantitatively*. Microbiologists have long appreciated this fact, and generations of trainees have calculated parameters by finding the slope of a growth curve on a log scale. This project aims to modernize this tradition, by empowering users to rapidly quantify parameters and uncertainty from their data without having to code.

## One model to rule them all

The primary model (or curve) that this project uses to fit growth curves is called the Gompertz model. 

<a href="https://www.codecogs.com/eqnedit.php?latex=y&space;=&space;A&space;*&space;exp&space;\left(&space;-exp&space;\left(&space;\frac{\mu_{m}}{A}(\lambda&space;-&space;t)&space;&plus;&space;1&space;\right)&space;\right)&space;&plus;&space;C" target="_blank"><img src="https://latex.codecogs.com/gif.latex?y&space;=&space;A&space;*&space;exp&space;\left(&space;-exp&space;\left(&space;\frac{\mu_{m}}{A}(\lambda&space;-&space;t)&space;&plus;&space;1&space;\right)&space;\right)&space;&plus;&space;C" title="y = A * exp \left( -exp \left( \frac{\mu_{m}}{A}(\lambda - t) + 1 \right) \right) + C" /></a>

parameters

<img src="https://render.githubusercontent.com/render/math?math=\mu_m">
