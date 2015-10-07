#Spontaneaity
+ If the ∆S of the universe is < 0 Won't happen Heat flow cold -> Hot
+ If the ∆S of the universe = 0 the reaction is at equilibrium
+ If the ∆S of the universe > 0 the reaction will proceed spontaneously

##Gibbs free energy
+ ∆Ssurr = ∆Hsurr/T = -∆Hsys/T
+ ∆Suniv = ∆Ssys = ∆Ssurr > 0 = ∆Ssys - ∆Hsys/T ≥ 0
+ ∆G ≣ ∆H - T∆S ≤ 0
    + this is equivalent to the second law of thermodynamics
+ **make sure when calculating ∆G that the units for entropy and enthalpoy are the same units**

###Conclusions from the gibbs free energy
+ ∆G > 0 Won't Happen
+ ∆G = 0 Equilibrium
+ ∆G < 0 Spontaneous

###The amount of ∆G matters
+ The system adjusts until the ∆G for the system is equal to zero

###Alternate representation of the ∆G
+ using the reaction 2A <=> B
```
G(P,T,n) = H - TS = U + PV - TS
∂G/∂P | T,n = V -> dG = dP @ const T,n
dG = nRT * 1/P * dP
more proof...
G(P) - G˚ = nRT(lnP - lnP˚)
```
+ This leads to the conclusion that G(P) - G˚ = nRT ln(P/P˚) 
+ per mole this is equal to G / n written as Ḡ

##The Equilibrium Constant
+ the equilibrum constant follows from the lg part of the gibbs free energy reaction

```
PBeq * P˚
-------  = e^(-∆G˚/RT) = Keq(T)
PAeq^2
```
+ P˚ is the pressure that ∆G˚ was measured at

###Interpreting the equilibrium constant

####The reaction quotient
+ Q = P˚Pb/Pa^2
    + basically K not at equilibrium
+ compare with K: which is the amount at equilibreum constant at equilibrium

Q and K | ∆G     | Reaction direction
--------|--------|------------------------------
Q > K   | ∆G > 0 | Right -> left, more reactants
Q = K   | ∆G = 0 | Equilibrium
Q < K   | ∆G < 0 | Left -> Right, more products

### LeChâtliers principle
+ equilibrium resists change in
    + amount
    + volume / pressure
    + temperature
+ qualitative reasoning
    + exothermic case
        + heat is like a product
        + increasing temperature is like adding heat
        + reaction is pushed to the left
    + endothermic case
        + heat is a reactant
        + increasing temperature is increasing heat
        + reaction is pushed to the right
+ quantitative reasoning
    + when temperature increases delta T increases
    + ∂K = dK/dT * ∂T
    + calculus...
    + ∂K = ∆H˚/RT * ∂T/T * K
    + conclusion: K is dependent on ∆H
        + endo ∆H > 0 -> ∂T > 0 -> ∂K > 0 => more product
        + exo -> ∆H < 0 -> dT > 0 -> ∂K < 0 => more reactants

###Equilibrium in solutions
+ we write Kc which has units, whereas K does not have units
+ Kp for gasses
+ ∆G˚f for things in reference state = 0

[Supplementary notes](supplementary/oct2.ppt)

### Solving difficult equations
+ drop x from the denominator if the reaction is centered around reactants, and x << the amount of products
+ repeat the process several times until the answer is quite stable
