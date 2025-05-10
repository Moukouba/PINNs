# 🧠 Physics-Informed Neural Networks (PINNs) for ODEs and PDEs

This repository contains a collection of experiments using **Physics-Informed Neural Networks (PINNs)** to solve **Ordinary Differential Equations (ODEs)** and **Partial Differential Equations (PDEs)**.

PINNs integrate physical laws (e.g., differential equations) directly into the loss function of a neural network. This approach enables the network to learn not only from data, but also from the governing equations of the system, allowing for interpretable and physically consistent predictions.

---

## 📘 Featured Example: Salt Mixing in a Tank (ODE)

We consider a classic **first-order ODE** problem:

> A tank initially contains 10 kg of salt in 100 liters of water. Pure water flows in at 3 L/min and the well-mixed solution flows out at 2 L/min. What is the quantity of salt in the tank after 60 minutes?

This problem leads to the differential equation:

\[
\frac{dx}{dt} = -\frac{2x(t)}{100 + t}
\]

with initial condition:

\[
x(0) = 10
\]

The **analytical solution** is:

\[
x(t) = \frac{100000}{(100 + t)^2}
\]

A **PINN model implemented with TensorFlow** accurately approximates this solution and is compared against the analytical form.

---

## 📂 Repository Structure
