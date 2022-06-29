# Thermochemistry

Simple code to reproduce  Gaussian 09 results for CO2 with B3LYP/6-31G(d).
Gaussian does not print hessian matrix in output, but it can be extracted from formatted checkpoint  ("Cartesian Force Constants").
The thermochemistry implementation is based on the equations from "G98thermo.pdf"  document.

 Needed info:
    coordinates   :    for rotational contribution (inertia moments)
    Hessian       :    for vibrational contribution
    symmetry      :    "sigma" Rotational symmetry number  
    E_electronic  :     DFT energy for electronic contribution

 Files descritption:
    CO2.fchk                     # g09  formatted checkpoint (with Hessian_
    CO2.out                      # g98  opt+frequency  output file  for co2
    G98thermo.pdf                # g09 white paper on thermochemistry 
    octave-Hessian-fch.inp       #  code
    octave-Hessian-fch.out       #
