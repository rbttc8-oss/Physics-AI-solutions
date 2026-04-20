### **Problem Statement**

Consider a spherically symmetric, non-rotating star modeled as a polytrope of index ( n = 1 ), with equation of state:

[
P = K \rho^{1 + \frac{1}{n}}
]

Given:

* Total mass: ( M = 2 \times 10^{30} , \text{kg} )
* Radius: ( R = 7 \times 10^8 , \text{m} )

Using the Lane-Emden solution for ( n = 1 ), compute the **central pressure ( P_c )**.

---

### **Assumptions & Model Setup**

* Hydrostatic equilibrium
* Newtonian gravity
* Polytropic index ( n = 1 )
* Known analytical solution:
  [
  \theta(\xi) = \frac{\sin \xi}{\xi}
  ]
* First zero: ( \xi_1 = \pi )

---

### **Analytical Solution**

For polytropes:

[
P_c = \frac{\pi}{2} \frac{G M^2}{R^4}
]

Substitute values:

[
P_c = \frac{\pi}{2} \cdot \frac{(6.674 \times 10^{-11})(2 \times 10^{30})^2}{(7 \times 10^8)^4}
]

---

### **Computational Verification (Python)**

```python
import numpy as np

G = 6.674e-11
M = 2e30
R = 7e8

Pc = (np.pi / 2) * (G * M**2) / (R**4)

print("Central Pressure (Pa):", Pc)
```

---

### **Final Answer**

[
P_c \approx 1.74 \times 10^{16} , \text{Pa}
]
