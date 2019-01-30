---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: page
title: i-PI v2 has been released!
header:
  image_fullwidth: wpig6_blue.jpg

#callforaction:
#  url: https://tinyletter.com/feeling-responsive
#  text: Inform me about new updates and features ›
#  style: alert
#
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---


**The second release of i-PI is ready for download. Several new features including replica exchange molecular dynamics, instanton calculations, perturbed path integrals and open path integrals have been implemented and merged to the master branch in the [official i-PI repo](https://github.com/i-pi/i-pi), which has also been stripped of the (rather intricate) git history.
The release is accompanied by the publication of a [reference paper on Computer Physics Communications](https://doi.org/10.1016/j.cpc.2018.09.020), that constitutes the new default reference to acknowledge use of this release.
Further development of i-PI will happen on the official repository. You are invited to fork and contribute back by means of pull requests.**


i-PI is a universal force engine interface
written in Python, designed to be used together with an ab-initio (or 
force-field based) evaluation of the interactions between the atoms. 
The main goal is to
decouple the problem of evolving the ionic positions to sample the
appropriate thermodynamic ensemble and the problem of computing the
inter-atomic forces.

<p align="center">
  <img src="{{ site.urlimg }}ipi-logo-alpha.png" alt="iPi-logo" />
</p>

The implementation is based on a client-server paradigm, where i-PI
acts as the server and deals with the propagation of the nuclear
motion, whereas the calculation of the potential energy, forces and
the potential energy part of the pressure virial is delegated to one
or more instances of an external code, acting as clients.

i-PI is free software, distributed under a dual MIT/GPLv3 licence. You
are welcome to dowload, use, modify and redistribute it. If you find it
useful for your research, a citation would be appreciated to

[Kapil et al., Comp. Phys. Comm. 236, 214--223 (2018)](https://doi.org/10.1016/j.cpc.2018.09.020)


As of today, the following codes provide out-of-the-box an i-PI interface: 
[CP2K](https://www.cp2k.org/),
[DFTB+](http://www.dftb-plus.info/),
[Lammps](http://lammps.sandia.gov/),
[Quantum ESPRESSO](http://quantum-espresso.org),
[Siesta](http://departments.icmab.es/leem/siesta/),
[FHI-aims](https://aimsclub.fhi-berlin.mpg.de/),
[Yaff](http://molmod.github.io/yaff/),
[deMonNano](http://demon-nano.ups-tlse.fr/),
[TBE](https://www.questaal.org/).
If you are interested in interfacing your code to i-PI please get in touch,
we are always glad to help!

If you have questions about running i-PI calculations, or including new features
into the code, you can get help on the [user forum](https://groups.google.com/forum/#!forum/ipi-users), 
or on the [github pages](https://github.com/i-pi/i-pi).
