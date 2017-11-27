# NozzleDesign

This git contains a series of MATLAB scripts that serve as the basis to generate the axisymmetric supersonic nozzles and has a couple of limitations which include, but are not limited to those listed below. The code may not always have 

  No attempt has yet been made to model anything upstream of the initial value line generated by the code; i.e.: where the velocity in the y direction is sufficiently close to zero and the magnitude of the Mach number is greater than 1.

  The initial value line is currently only defined for axisymmetric nozzles using the relations of Kliegl and Levine (1969).

  The code itself uses the irrotational and adiabatic, 2-D method of characteristics to solve for the inviscid flowfield in the diverging section of a theoretical supersonic nozzle. These equations came from Gas Dynamics Volumes I and II by Zucrow and Hoffman.

  The chemistry is assumed to be frozen, so no changes in gas composition are calculated. Properties such as gamma are allowed to change as a function of temperature and composition though, so the code may be extended in the future to include chemical reactions.

  The thermodynamic properties are calculated from the NASA 9-coefficient polynomial format, but are limited to species that contain C, H, N, O, Ar, and/or Xe.

To execute the code: load thermInfo.mat, open testingNozzle, and change desired parameters.
