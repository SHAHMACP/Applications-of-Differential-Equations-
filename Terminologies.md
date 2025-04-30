## 📝 Notes

- **Jacobian matrix and eigenvalues:**  
  The stability of typical equilibria of smooth ordinary differential equations is determined by the **eigenvalues of the Jacobian matrix**. These eigenvalues are often referred to as the *eigenvalues of the equilibrium*.  
  The Jacobian matrix of a system of smooth ODEs is the matrix of partial derivatives of the right-hand side with respect to state variables:
![image](https://github.com/user-attachments/assets/0d54a5b7-bf2d-4bbf-90a6-24e9380aae33)



  All derivatives are evaluated at the equilibrium point $x = x_0$.  
  Its eigenvalues determine **linear stability properties** of the equilibrium.

- **Isocline:**  
  A line on a diagram or map connecting points of equal gradient or inclination.

- **Trajectories:**  
  The parametric curves traced by the solutions are sometimes called their **trajectories**.


- **Phase plane:**  
  The Cartesian plane where the phase portrait resides is called the *phase plane*.

- **Phase portrait:**  
  A phase portrait is a geometric representation of the trajectories of a dynamical system in the phase plane.  
  Each set of initial conditions is represented by a differential curve or point.  
  A phase portrait is a graphical tool to visualize how the solutions of a given system of differential equations would behave in the long run.

Here we list the type and stability of the equilibrium solutions of linear systems by the shape and behavior of its phase plane.


### 🔵 NODE: Two distinct eigenvalues with the same sign  
- **Unstable** if both eigenvalues are positive  
- **Asymptotically stable** if both eigenvalues are negative

![image](https://github.com/user-attachments/assets/d9ef04c0-6256-4593-a0ce-5660cad5103a) ![image](https://github.com/user-attachments/assets/005228c3-47ce-4bc3-9f5b-f5977e75dda8)

### 🔵 SADDLE POINT: 2 distinct real eigen values, opposite sign, always unstable
![image](https://github.com/user-attachments/assets/9b91e1e6-21e0-46fb-8a3b-fa079ed24aab)

### 🔵 SPIRAL POINT: complex eigen values, non-zero real part, unstable if real part is positive, stable if real part is negative. 
![image](https://github.com/user-attachments/assets/000ea6d5-0043-4778-b302-0416283c7934)

### 🔵 PROPER NODE: repeated real eigen value, 2 eigen vectors, unstable if positive, asymptotically stable if negative.
![image](https://github.com/user-attachments/assets/459140d7-b8ef-46df-a51d-80ddd27eee1f)

### 🔵 CENTER: complex eigen value, purely imaginary, stable or neutrally stable, not asymptotically stable.
![image](https://github.com/user-attachments/assets/e7320ea8-57a7-4401-a364-fcef06464bea)

### 🔵 IMPROPER NODE: repeated real eigen value, one eigen vector only, unstable if positive, asymptotically stable if negative.
![image](https://github.com/user-attachments/assets/28e51597-7cbc-4bf3-a01c-1145612920a3)  ![image](https://github.com/user-attachments/assets/06a6b937-0bcd-4dac-8e65-e163fa736a73)
----





