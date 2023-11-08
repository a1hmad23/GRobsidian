### 2.1 Definition Of A Vector

- A vector is something whose components transform like the coordinates under a coordinate transformation. A typical vector is the displacement vector, which points from one event to another and has components equal to the coordinate differences: $\Delta x \rightarrow_{O}(\Delta t, \Delta x, \Delta y, \Delta x)$. The Vector is an arrow between two events while the components are a set of 4 coordinate dependent numbers.
- A vector is a geometrical object: something which can be defined without reference to a coordinate system.
- The Lorentz transformations (between coordinate systems) are linear: $$\Delta x^{\alpha'}= \Lambda^{\alpha'}_{\beta} \Delta x^{\beta}$$
- The Lorentz transformations are for coordinates, and hence for vectors.

### 2.2 Vector Algebra

**Basis Vectors**
- In SR, for any frame $O$ there exist four basis vectors defined by giving their components. Basis vectors are defined with respect to a coordinate system. For example, $e_{0}\rightarrow_{O}(1,0,0,0)$ is different than $e_{0'}\rightarrow_{O'}(1,0,0,0)$.
- Basis vectors are equivalently defined as: $(e^{\alpha})^{\beta} =\delta_\alpha^\beta$ 
- Any vector can be expressed in terms of basis vectors(through contraction in a frame $O$)

**Transformations of basis vectors**
- In different frames, although the basis vectors and components of a vector are different, their contractions denote the same geometrical invariant vector objects (the components are just different representations of the same vector), Hence, we can write $$A^{\alpha}e_{\alpha}= A^{\alpha'}e_{\alpha'}$$
- Since we know how the components transform (like the coordinates, which transform by the Lorentz transformations), we can deduce the transformation rule for basis vectors by the idea that vectors (in different representations) are invariant:
$$A^{\alpha}e_{\alpha} = \Lambda^{\alpha'}_{\beta}A^{\beta}e_{\alpha'}$$
- On the right there's a double sum. Since $\Lambda^{\alpha'}_{\beta}$and $A^{\beta}$ are just numbers (under the summation), their order can be interchanged $A^{\beta}\Lambda^{\alpha'}_{\beta}e_{\alpha'} = A^{\alpha}e_{\alpha}$ , and renaming the dummy indices: $A^{\alpha}e_{\alpha} = A^{\alpha}\Lambda^{\beta'}_{\alpha}e_{\beta'}\rightarrow$   
- $$
e_{\alpha} = \Lambda^{\beta'}_{\alpha}e_{\beta'}$$
- This gives each element of one set of basis vectors as a linear combination of another set of basis vectors.

**Inverse Transformations**
- The Lorentz matrix $\Lambda ^{\beta'}_{\alpha}= \Lambda ^{\beta'}_{\alpha}(v)$ depends only on the relative velocity of the two frames- namely the relative velocity of the upper index frame ($O'$ in this case) with respect to the lower one ($O$). Let that be $v$ Hence, the inverse transformation (of some quantity in the $O$ to the same quantity expressed in the $O'$ frame) must be carried out by using the relative velocity of $O$ with respect to $O'$- name $-v$. Hence: $e_{\mu'} = \Lambda^{\nu}_{\mu'}(-v)e_{\nu}$ plugging this into the equation $e_{\alpha} = \Lambda^{\beta'}_{\alpha}e_{\beta'}$, we get $e_{\alpha} = \Lambda^{\beta'}_{\alpha}(v)\Lambda^{\nu}_{\beta'}(-v)e_{\nu}$. If we expand the sum over $\beta$ first, we find that the coefficient of each $e_\nu$ on RHS is $\Sigma_{\beta} \Lambda^{\beta'}_{\alpha}(v)\Lambda^{\nu}_{\beta'}(-v)$ for each value of $\alpha$. But since only the coefficient for $e_{\alpha}$ on RHS must be non zero and equal to 1, and all the others must vanish, (simply put, the expression must equal $e_{\alpha}= \delta^{\nu}_{\alpha}e_{\nu}$ ,which is an identity) we find that $$\Lambda^{\beta'}_{\alpha}(v)\Lambda^{\nu}_{\beta'}(-v) = \delta^{\nu}_{\alpha}$$
- Moreover, if we regard the components of $\Lambda$ as elements of a matrix, the above sum of products can be regarded as matrix multiplication, and so for all values of $\alpha$ and $\nu$, $\delta^{\nu}_{\alpha}$ can be regarded as an identity matrix and the Lorentz transformation matrices as inverses of each other.
- An expression for components of a vector in frame O can be found by applying the inverse Lorentz transformation to the components in O' frame.

### 2.3 The Four Velocity

- Defined as a tangent to a particles world line, of length such that it stretches one unit of time in the particles rest frame. Since in the particles own frame, its movement through spacetime is only through its proper time, its velocity is only in the time direction, the unit basis vector $e_0$ in the time direction.
- Although an accelerating particle has no inertial frame in which it is always at rest, its 4- velocity can be defined in a 'momentarily comoving reference frame' MCRF

### 2.4 The Four Momentum

- $P = mU$, where m is the rest mass of the particle as measured in its own rest frame.
- In some frame $O$, it has components conventionally denoted by $P \rightarrow_{O} (E,p^{1},p^{2},p^{3})$, where $p^0$ is called the energy and the other components are its spatial momentum.
- *Example* A particle with rest mass m moves with speed $v$ in the $x$ direction of some frame $O$, what are the components of its four-velocity and four-momentum (in the frame $O$)?
	- In the particles own rest frame, which is a frame with relative velocity $v$ to $O$, its four-velocity is the time basis vector $e_{0'}$ .This vector could be transformed to the frame $O$ with a Lorentz transformation, and its components in the frame $O$ would be: $U^{\alpha}=\Lambda^{\alpha}_{\beta'}(e_{0})^{\beta'}$.
	- For small $v$, the spatial components of the four-velocity are $(v,0,0)$,and for the momentum are $(mv,0,0)$, and the $p^0$ (energy) is $m + \frac{1}{2}mv^2$ (rest mass energy plus Galilean kinetic energy).

**Conservation of four-momentum**
-  Since the components of $P$ (four-momentum) reduce to 3-momentum in the nonrelativistic limit, in which it conserved, it is postulated that in spacetime 4-momentum is conserved. It is a postulate because other quantities are also conserved in the non relativistic limit. However, its predictions are verified by experiment.
- Since 4-momentum is conserved after every collision, it does not matter if there is a system in which two collisions take place that spacelike separated, such that there exists observers for whom all combinations of which collisions have taken place at t,t',t'' = 0. Total 4 momentum is an invariant, even though the individual 4 momentum vectors vary by the frame.

**Centre of momentum frame** CM frame
- Inertial frame where the total momentum has no spatial components, that is, $$\Sigma_{i}P_{i}\rightarrow_{CM}(E_{total},0,0,0)$$
- As with MCRFs, any frame at rest relative to a CM frame is also a CM frame.


### 2.5 Scalar Product

**Magnitude of a vector**  $A^{2}= -(A^{0})^{2}+ (A^{1})^{2}+ (A^2)^{2}+(A^3)^{2}$ .
- It is defined to have the same form as the spacetime interval, which makes it invariant across frames since the components transform in the same way as coordinates.
- Also like the spacetime interval, the magnitude of a 4-vector could be spacelike, lightlike, or timelike. The null vector is different from the $0$ vector, which has all of its components equal to 0.

**Scalar product of two vectors** Again has the same form as the spacetime interval, but since each term is not a square but a product of two different components, we have to verify if its invariant: Since for any two vectors $A,B$, $A+B$ is also a vector, so without any loss of generality, we consider the magnitude of $A+B$: $$(A+B)^{2}= A^{2}+B^{2}+2A\cdot B$$
Since we know that in any different frame $O'$, the LHS and the first two terms on the RHS are the same, it must be the case that the scalar product is also invariant.
- 2 vectors are orthogonal if $A \cdot B =0$. However, because of the special time component (negative sign), the two vectors might not appear to be at right angles in a space time diagram.
- A null vector is orthogonal to itself. Such a phenomenon doesn't occur in spaces where the scalar product is positive-definite.
- *Example* By the scalar product defined above, the basis of any frame make an orthonormal tetrad. However since the scalar product of the time basis vectors equal $-1$, a new symbol is defined for the scalar product of basis vectors: $$e_{\alpha}\cdot e_{\beta}=\eta_{\alpha \beta}$$
- In spacetime diagrams, orthogonal vectors make the same angle with a light ray.
- *Example* Since in an MCRF, the particles rest frame, the four-velocity is just a time basis vector, whose scalar product with itself, and thus its magnitude is 1. Since the scalar product is invariant, this is the case in all frames: $$U\cdot U =-1 \ \ \ \ in\ all\ frames$$

### 2.6 Applications

**Four-velocity and acceleration as derivatives**
- Suppose a particle makes an infinitesimal displacement $dx$ in spacetime, (independent of any coordinate system), whose coordinates in a frame $O$ are: $dx \rightarrow_{O}(dt,dx,dy,dz)$ and whose magnitude in frame $O$ and thus in all frames (of the displacement (vector)) is $-dt^{2}+dx^{2}+dy^{2}+dz^{2}$, which is just the spacetime interval $ds^{2}= dx\cdot dx$ (of the starting and ending events of the displacement).
- Since worldlines are timelike, this is negative. Considering the particles own rest frame: $d \tau ^{2}=-dx\cdot dx=-ds^{2}$.
- Now, the vector $\frac{dx}{d\tau}$ is just a scalar multiple of $dx$ (the scalar being $\frac{1}{d \tau}$), it is tangent to $dx$, and hence the particle's worldline. It's magnitude is $\frac{dx}{ d \tau}\cdot \frac{dx}{ d \tau} = \frac{dx\cdot dx}{d \tau^{2}} = -1$
- Hence, it is a timelike vector of unit magnitude ($-1$), and so if we transform to the particles rest frame(MCRF), it is a vector whose magnitude is $-1$, which makes it the time basis vector of a MCRF. In an MCRF, $dx \rightarrow_{MCRF}(dt,0,0,0)$, and so $$\frac{dx}{d \tau} \rightarrow_{MCRF}(1,0,0,0)$$
Or, $\frac{dx}{ d \tau} = (e_{0})_{MCRF}$  . These are just the definition for four-velocity, and so we have $$U=\frac{dx}{d \tau}$$
- To examine four-acceleration $\frac{dU}{d ta} = \frac{d^{2}x}{d \tau}$, we could take the derivative of $U\cdot U$: $\frac{d}{d \tau} (U\cdot U) = 2U \cdot (\frac{dU}{d \tau})$ . But since $U\cdot U = -1$, a constant, its derivative is $0$, and so $$U \cdot \left(\frac{dU}{d \tau}\right)= 0$$
- In an MCRF, $U$ has only a time component, so this implies that $\frac{dU}{d \tau} \rightarrow_{MCRF}(0,a^{1},a^{2},a^{3})$
This defines the acceleration.

**Energy and Momentum**
- Consider a particle whose momentum is $P$. Then, $P\cdot P = m^{2}U\cdot U = -m^{2}$. But $P\cdot P = -E^{2}+ (p^1)^{2}+(p^{2})^{2}+(p^{3})^{2}$
Hence, $$E^{2}= m^{2}+ p^2,$$
is an expression for the total energy of the particle, where $p^{2}= \Sigma_{i=1}^{3}p_{i}$ is the magnitude of the spatial momentum of the particle.

- In the frame $O$, let a particle move with momentum $p$ and let another observer move with four-velocity $O'$. Then, $p\cdot U_{obs} = p\cdot e_{0'}$ , where $e_{0'}$ is the observers four-velocity in its own frame. In the observers $O'$ frame, the four-momentum of the particle has components $p\rightarrow_{O'}(E,P^{1},p^{2},p^{3})$. Choosing to find (evaluate) the invariant scalar product in the observers frame (the result will hold for all frames), we find: $$-p\cdot U_{obs} = E$$
- This gives the energy of a particle relative to some specific observer. Hence, the energy of a particle relative to some observer can be calculated by anyone by taking the scalar product of the momentum of the particle that they measure with the 4-velocity of the observer that they measure. It is a frame invariant expression for a particle's energy relative to some observer.


### 2.7 Photons

**No Four Velocity**
- Photons move on null lines, so $ds^{2}=0 \rightarrow d \tau^{2}=0$ so 4-velocity cannot be defined. Since no proper time can be defined, it implies there exists no inertial rest frame for photons. This also follows from the second postulate: In all inertial frames, the speed of light is $c$. Thus no $e_0$ will be tangent to a photon's worldline in any frame. This doesn't exclude general vectors, for e.g., $dx$ is one, but they are just not of unit magnitude- all of them have vanishing magnitude, since any vector tangent to a photons worldline is a 45 degree vector, whose magnitude would be $0$ (for such vectors, $A^{2}= ds^{2}= 0$)

**Four Momentum**
- Not a unit vector.
- In some frame, the 4-momentum of a photon will have components $(E,p^1,p^2,p^3)$. Let it move in the $x$ direction only, so that $p^{2}=p^{3}=0$. Since the 4-momentum must be parallel to it's worldline, in the photons case it must be oriented at 45 degrees, which means it's magnitude (calculated in the same manner as the spacetime interval) must be $0$. Hence, we must have $p^{x}=E$. More generally, the magnitude of the spatial momentum of the particle must equal its energy, so that $P^{2}= -E^{2}+E^{2}=0$.
- From Quantum Mechanics, a photon has energy $E=h \nu$. This formula and Lorentz transformation (since 4-momentum is a 4-vector), gives the formula for Doppler shift:
	- Suppose in a frame $O$, the photon has energy $E$ and frequency $\nu$, and that in this frame the photon moves only in the $x$ direction. Since the energy is a component of the 4-momentum, the Lorentz transformation can be used to find its energy in some other frame $O'$. Suppose $O'$ has velocity $v$ in the $x$ direction relative to $O$. Then, using the Lorentz transformations and putting $h \nu$ and $h \nu'$ for the energy in the two frames, we can find how the two frequencies are related.

**Zero Rest-Mass Particles** 
- The rest-mass of a photon must be $0$ since, $p\cdot p = m^2$. More generally, any particle with a null 4-momentum must have $0$ rest-mass, and vice versa.



