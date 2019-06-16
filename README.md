# [CanSat](https://www.esa.int/Education/CanSat) 2018

### What is CanSat?

CanSats in Europe is an initiative of the [European Space Agency (ESA)](https://www.esa.int/ESA).

A CanSat is a simulation of a real satellite, integrated within the volume and shape of a soft drink can. The challenge for the students is to fit all the major subsystems found in a satellite, such as power, sensors and a communication system, into this minimal volume. The CanSat is then launched to an altitude of a few hundred metres by a rocket or dropped from a platform or captive balloon and its mission begins: to carry out a scientific experiment and achieve a safe landing.

CanSats offer a unique opportunity for students to have a first practical experience of a real space project. They are responsible for all aspects: designing the CanSat, selecting its mission, integrating the components, testing, preparing for launch and then analysing the data.

### Sizing a Parachute

For the CanSat edition of 2018, I wrote a Python script based on J.R. Brohm's "The Mathematics of Flat Parachutes" which calculates how big the CanSat parachute should be.

It takes as input:

- **Height**(m) : height from which the CanSat is thrown
- **Mass**(g) : CanSat's mass
- **Terminal Velocity**(m/s) : desired terminal velocity
- **Type of parachute**:
  - N-sided-polygon
    - Without hole
    - With hole
  - Cross
  - **Number of Sides**(>=5) : optional! only if type N-sided-polygon
  - **Hole Diameter**(cm) : optional! only if type N-sided-polygon with hole
  
  And outputs:
  
  - **Time of flight without parachute**(s)
  - **Impact velocity without parachute**(m/s)
  - **Parachute area**(m^2 and cm^2)
  - **Pretty Graph** : optional!
