# MultiVLM

The Full Multi-wake Vortex Lattice Method (FMVLM)

Visual Studio project including a code (Fortran; development version) to obtain the potential non-linear aerodynamic characteristics of flat plates plantforms for steady detached flow condition.

Notes: 
Post-stall detached vorticity model is under development/testing (do not use yet).
For v2, circulation distributions are numerically symmetrical (for non-sideslip condition) but due to transparency level in post-processor cannot be adjusted manually, these look slight asymmetrical.

BUG detected in v2: 
In subrutine vind_vxlat, change:
if (a_v>=eps) then 

instead of:
if (a_v>=core_rad) then
