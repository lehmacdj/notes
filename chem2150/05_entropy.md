#Entropy
##Per bond enthalpy
+ add together the energy of all of the bonds
+ written like H(C-H) = 104 kJ/mol
+ positive but has a negative enthalpy
+ bond energies are not always exactly the same
    + therefore not very accurate
    + at most ±5% accurate
    + therefore shouldn't be trusted hightly

##Some basic thinking
+ it is easy to think that only exothermic reactions will react
+ howerver that is not always true
+ sometimes endothermic reactions are spontaneous

##Definition
+ It is a state function

```
   final
∆S = ∫ dqrev / T
  initial
} dqrev = dq reversible
```

+ has units of J/K

###Cases
####Isothermal
```
      1  final
∆S = --- ∫ dqrev = qrev / T
      T  init
qrev = -w
∆S -= nRln(V2/V1)
constant temperature
volume increases
∴ entropy increases
```

####Adiabadic
```
qrev = 0
∴ ∆S = 0
```

####Constant pressure or volume
```
c = 1/n ∂q/∂T
dqrev = n C dT
} C: molar heat capacity
    final         final         T2
∆S = ∫ dqrev / T = ∫ nCdT/T = nC ∫ dT/T
    initial       init          T1
positive
∆S = nC ln(T2/T1)
with constant P or V
temperature increases
∴ entropy increases
```

####Reversable vs Irreversable
+ qrev > qirrev
+ wirrev > wrev

###Thermodynamics 
+ we partition the environment into teh surroundings and the system
+ ∆S = ∫dq/T for the system
+ ∆S = q/T for the surroundings (rev, or irrev) since T remains approximately equal

####The laws of thermodynamics
1. ∆Usys = ∆Usurr = 0
    + } ∆Usurr = -(q + w)
2. ∆Ssys + ∆Ssurr ≥ 0
3. S -> 0 as T -> 0 ∴ S = ∫(0, T) dqrev/T

###Measuring entropy
+ dqrev = nCpdT
+ ∆T/∆Q = 1/(nCp)
+ the entropy is the area under the Cp/T to T curve

###Entropy properties
+ The more parts the more entropy
+ The more gasseous the more entropy
+ complexity => more entropy
+ floppyness => more entropy
+ different molecules

