---
type: PostLayout
title: DWCs
date: '2024-09-03'
excerpt: >-
  Nunc rutrum felis dui, ut consequat sapien scelerisque vel. Integer
  condimentum dignissim justo vel faucibus.
addTitleSuffix: true
colors: colors-a
backgroundImage:
  type: BackgroundImage
  url: /images/bg2.jpg
  backgroundSize: cover
  backgroundPosition: center
  backgroundRepeat: no-repeat
  opacity: 100
---
DWCs are gas-filled rectangular chambers that help you track a particle - or at least get their position at the moment they pass the detector. They work like this: a particle passes the gas-filled chamber. If the particle is charged, then it will ionize the gas inside. In the chamber there are multiple layers of parallel wires, each layer acting as an electrode. The ions and electrons will start to move towards their respective electrodes (electrons towards anode and positive ions towards cathodes). They're not only moving towards the electrodes, they are also accelerating due to the Coulomb force. Electrons are even accelerated to such a high velocity, that they start to ionize the gas even further, creating an avalanche (more specifically a Townsend avalanche). Eventually all of the electrons that got kicked out, reach an anode and cause a great current in it. This current in the anode will go on to create an image current in the cathode. This step is important, because it's not the anode current that we are measuring, it's instead the image current in the cathode. Also, the current will be produced in 2-3 cathode wire, closest to the anode wire where avalanche took place. 

Neighbouring cathode wires are connected to each other with little delay lines. The two edgemost wires are connected to a sensor. The current that passes the sensor has a characteristic mountain shape in time.

Each step is the contribution from a single wire. They add up at various times thanks to the delay lines, but this is not really the important part. The delay lines are actually there so that the little current mountain would reach the two detectors at opposite sides of the cathode at different times. The moment when the signal is detected is not at the peak of the mountain, it is at the rising edge. 

The time interval between signal arrivals is all that is needed to find where the particle passed through.

