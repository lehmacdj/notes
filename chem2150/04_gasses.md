# Gasses

## Kinetic Gas Model
+ **u** is the velocity vector of the gas
+ collisions are perfectly elastic
    + all velocity components are mirrored by surface that they collide with
+ force on the wall

```
F-x = change of momentum / collision * collisions / time
F-x = 2m * ux * 1/2 ux * A * N / V = m * ux^2 * A * N / V
F-x/A * V = N m * ux^2
} F-x/A = P
} n * NA * kB * T = N kg * T
P * V = nRT
```

##Ideal gas law
+ PV = nRT

##Energy of molecules
+ U = 3/2nRT
+ ∆U = 3/2nR∆T <=> ∆U = qv = n Cv ∆T
    + for Ideal gasses:
        + Compare: Cv = 3/2R
        + Cp = Cv + R = 5/2R:w

##Isothermal -- constant volume
```
∆H = ∆U + ∆PV
   = ∆U + nR∆T = 0
∆U = q + w => q = -w
Reversible isthermal expansion
     V1               V1
w = -∫ P(V) dV = -nRT ∫ 1/V dV
     V2               V2
w = -nRT * ln(V2/V1)
```
##Adiabatic -- no heat in
q = 0
∆U = w
dU = n * Cv dT
dw = -PdV = -nRT dV/V
set equal divide by n & T
Cv dT/T = -R * dV/V
Cv * ln(T1/T2) = -Rln(V2/V1) = Rln(V1/V2)
exponentiating
(T2/T1)^Cv = (V1/V2)^R 
