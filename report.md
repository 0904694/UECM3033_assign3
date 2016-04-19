UECM3033 Assignment #3 Report
========================================================

- Prepared by: Alex Yong Wei Chun
- Tutorial Group: T3

--------------------------------------------------------

## Task 1 --  Gauss-Legendre formula

The reports, codes and supporting documents are to be uploaded to Github at: 

https://github.com/0904694/UECM3033_assign3/blob/master/task1.py

By using the Legendre function, the nodes and weights with any n from 1 to 100 is obtained. Nodes is represented by ‘x’ while weights is represented by ‘w’. Then, the x value is transformed into the integral from the interval [-1, 1] to [a, b]. The answer is calculated out by using the Gauss-Legendre Quadrature formula with np.polynomial.legendre.leggauss. The Jacobian of the transformation is calculated by using formula (b-a)/2.

My result of findings: I = -139/6 + 34*log(2), I = 0.400338097411



---------------------------------------------------------

## Task 2 -- Predator-prey model

The given value is stored into a, b and y.

We use linspace function is used to plot a line graph from year 0 to year 5. 
Then, Implementation of codes: t = np.linspace(0, 5, 100)

the nonlinear ODE system is solved using function odeint from the module scipy.integrate. 
Implementation of codes: sol = spIn.odeint(ode_system,y_initial,t,args=(a,b))

Graph of Predator y1 against Prey y0 is plotted. The initial condition is y0 = 0.11, y1 = 1.0. Inverse relationship between y0 and y1 is observed.

Is the system of ODE sensitive to initial condition? Explain. When the initial value change from 0.1 to 0.11, there is no significance changes can be seen from the graph, only small changes. Thus, this system of ODE is not sensitive to the initial conditio

-----------------------------------

<sup>last modified: change your date here</sup>
