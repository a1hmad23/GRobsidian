### 5.1 On The Relation Of Gravitation To Curvature

- SR does not include forces.
- The postulates of SR lead existence of inertial frames that fill all of spacetime: all of spacetime can be described by a single frame, all of whose coordinates are at rest with respect to the origin, and all of whose clocks run at the same rate. [see section 1.2]
- The fundamental postulates lead to the idea of the interval $\Delta s$, which gives an invariant geometrical meaning to certain physical statements:
	- When $\Delta s >0$, the interval is timelike. In that case $v<c$, (divide the interval by $t$), so since the interval is invariant, it can be considered to be that of a travelling particle. Moreover, let $\Delta s=k$ for any positive number $k$. Then, a rest frame can found such that $\Delta t=k$. In this case, the events are only separated temporally, so the interval corresponds to a reading of a clock in the rest frame between the two events. Notice that this argument holds because in the interval, the temporal term is positive.
	- When $\Delta s<0$, the interval is spacelike. Analogous to the above argument, $\Delta r=-k$ can be found in which case $\Delta t=0$ and the events in that frame are simultaneous. Hence, the interval can be considered to be the (Euclidean) length of a rod.
- The mathematical function that calculates the interval is the metric, and so the metric of SR is defined by physically lengths of rods and readings of clocks. This is the reason for the usefulness of $\eta_{\alpha \beta}$ ( we could have chosen other metrics).
- This makes the theory falsifiable.
- So is it possible to construct a frame in which the clocks all run at the same rate? (if not, inertial frames do not exist and SRs)

*The Gravitational Redshift Experiment*
- Drop a particle from some height. At the bottom, convert all the mass into a photon with the same energy (permitted by the mass energy relation I guess). The photon must be redshifted, since upon reaching the top it can be converted back to a mass and the mass can then again gain kinetic energy without bound. 
- So, in gravitational fields, light is redshifted.

*Nonexistence Of A Lorentz Frame At Rest On Earth* 
- Consider light in a uniform gravitational field. Observe two light crests emitted. In Minkowskian geometry (flat geometry) whatever the effect of gravity on light maybe, it must be the same for both the crests, since the gravitational field is constant in time. However, we know that light gets redshifted at the top, so the frequency of the light at the top is difference, and hence its period, which means the time interval between the crests at the top is different that that at the bottom, contradicting the predictions of Minkowskian geometry.

*The Principle Of Equivalence*
- In an inertial frame, a particle at rest remains at rest if no forces act on it. However, on earth this fact cannot be used since to be experimentally useful, we need a particle that is not effected by gravity but there is no such particle.
- However, the frame that falls freely with the gravitational field is such a frame where particles remain at constant velocity, since the falling of the frame is equal to the falling of the particles. This frame is a candidate for an inertial frame.
- The above arguments are obviously only valid locally, since gravitational fields are not uniform, so a frame that matches the acceleration of one test particle would not match the acceleration of some other test particle far away and so that particle will be soon to be accelerating without the presence of any forces.
- The equivalence of gravitational effects and acceleration due to any other cause is called the principle of equivalence.

*The Redshift Experiment Again*
- By doppler shift (I guess), in a freely falling frame, light is not seen to be redshifted which gives a sound basis for the postulate that freely falling frames are (locally) inertial.

*Local Inertial Frames*
- Due to non uniformities of the gravitational field, it is impossible to construct a global inertial frame, but constructing a local inertial frame is possible.
- However, any gravitational field can be regarded as uniform or a vanishingly small region of space and time, which is the reason for the possibilities of constructing local inertial frames. Analogous to MCRFs for each fluid element.
- Hence, the mathematical notion that any theory of gravity must admit local inertial frames: frames that a point admit SR, is emphasized.

*Tidal Forces*
- Non uniformities in the gravitational field are called tidal forces. Since these forces prevent the construction of global inertial frames, it is these forces that are regarded as the fundamental manifestation of gravity in GR.

*The Role Of Curvature*
- In SR, test particles obey the parallelism axiom of Euclid, which gives it a flat, albeit non Euclidean geometry (difference metric).
- In GR, particles that start parallel might not necessarily remain so, and so the parallelism axiom is not dropped. When this is the case in Euclidean geometry, the space is called a curve space.
- Sufficiently close to a point, the space can be considered flat so lines can be locally straight. However, such as in a sphere, these locally straight lines can intersect (the shortest lines (geodesics) between two points is called a straight line, on a sphere these are segments of great circles-circles which pass through the center of the sphere, since these have the minimum curvature, equal to that of the sphere and nothing more- they stick to the surface)
- The sphere is thus locally flat. All Riemannian spaces are locally flat, but the geodesics might not remain parallel.
- Einstein's genius was to see the similarity between Riemannian spaces and gravitational physics. He identified the trajectories of freely falling particles with the geodesics of a curved geometry: they are locally straight since spacetime admits local inertial frames in which those trajectories are straight lines, but globally they do not remain parallel.
- We look for a theory of gravity which uses a curved spacetime to represent the effects of gravity. To do this we study curvature, which is easier when one has first studied curvilinear coordinates in flat geometry.

### 5.2 Tensor Algebra In Polar Coordinates

- Let $(x,y)$ be coordinates in the Euclidean plane. Let $(\zeta, \eta)$ be new coordinates. Then, $(\zeta (x,y),\eta (x,y))$. Then, a displacement $(\Delta x,\Delta y)$ can be represented in the new coordinates as $(\Delta \zeta,\Delta \eta)$, where $\Delta \zeta=\frac{\partial \zeta}{\partial x} \Delta x +\frac{\partial \zeta}{\partial y}\Delta y$ and analogously for $\Delta \eta$. Since you can associate with the displacement an arrow, a geometrical object in space, it will be the same regardless of whichever coordinate system it is viewed in.

*Vectors And One-Forms*
- Vectors are geometrical objects whose components transform in the same manner as the displacement. Hence, displacement is defined to be a vector and anything that transforms in the same manner as it does is a vector.
- Thus, we can write down a transformation matrix (Jacobian) for vector components:
- The modern way is to associate with the gradient of a scalar function a geometrical object called the One-Form $\tilde{d}\phi$, whose components in any frame are just the partial derivatives of $\phi$ with respect to the coordinates of that frame.
- These lead to a transformation rule for one-forms naturally, and so all one forms are defines. Vectors are then defines as functions of one forms that return a scalar, and hence must transform in the opposite way to a one-form.
- The two transformation matrices are inverses of each other.

*Curves And Vectors*
- A path is a connected series of points in the plane. A curve is a parametrized path.
- The derivative of a scalar field along a curve is $\frac{d\phi}{ds}$ which is equal to the contraction between the gradient one-form $\tilde{d}\phi$ and the tangent vector $\vec{V}$. Hence  $\frac{d\phi}{ds}=\langle \tilde{d}\phi,\vec{V} \rangle$.
- A curve has a unique tangent, since both the path and parametrization are given.

*Polar Coordinate Basis One-Forms*
- $\vec{e}_{\alpha'}=\Lambda^{\beta}_{\alpha'}\vec{e}_{\beta} \rightarrow \vec{e}_{r}=\Lambda^{\beta}_{r}\vec{e}_{\beta}=\Lambda^{x}_{r}\vec{e}_{x} +\Lambda^{y}_{r}\vec{e}_{y}$   and analogously for theta.
- $\tilde{\omega}^{\alpha'}=\Lambda^{\alpha'}_{\beta}\omega^{\beta}\rightarrow \tilde{d}r=\Lambda^{r}_{\beta}\omega^{\beta}=\Lambda^{r}_{x}\tilde{d}x+\Lambda^{r}_{y}\tilde{d}y$ 
- The basis vectors are not constant. Both their magnitudes and directions change. The theta basis vector has a component of 1 for theta displacement. It must be longer to do this at larger radii.

*Metric Tensor*
- Dot products are calculates by knowing the metric tensor components in that frame.
- In Cartesian Coordinates **g**$(\vec{e}_{\alpha},\vec{e}_{\beta})=\delta_{\alpha \beta}$ 
- In Polar coordinates $g_{\alpha' \beta'}=\vec{e}_{\alpha'}\cdot \vec{e}_{\beta'}$  
- A convenient way to present both information about the metric tensor and the coordinates is the infinitesimal line element $d \vec{l}$ calculated as follows: $(d \vec{l} \cdot d \vec{l})^\frac{1}{2}=$|$dr \vec{e}_{r}+d \theta \vec{e}_{\theta}$|$=dr^{2}+r^{2}d \theta^{2}$ 
- Any 2nd rank tensor can be written as a linear combination of basis one forms:
- ![[Pasted image 20231125210354.png]]
- When this is fed the vector line element, it produces the above equation.
- The inverse metric has components $g^{\alpha \beta}$  and can be used as a mapping between one form components and vector components:
	- Let $\phi$ be a scalar field. The gradient one-form has components $(\tilde{d}\phi)_{\beta}=\phi_{,\beta}= \frac{\partial \phi}{\partial x^{\beta}}$. The vector gradient has components $(\vec{d \phi})^{\alpha}=g^{\alpha \beta}\phi_{,\beta}\rightarrow (\vec{d}\phi)^{r}=g^{r \beta}\phi_{,\beta}=g^{rr}\phi_{,r}+g^{r\theta}\phi_{\theta}$


### 5.3 Tensor Calculus In Polar Coordinates

- Consider the vector $\vec{e}_{x}$ For different values of $x$, this is a constant vector field. Now consider its components in polar coordinates: $(\vec{e}_{x})^{\alpha'}=\Lambda^{\alpha'}_{\beta}(\vec{e}_{x})^{\beta}\rightarrow (\vec{e}_{x})^{r}=\Lambda^{r}_{x}(\vec{e}_{x})^{x}\rightarrow \vec{e}_{x}\rightarrow_{polar}(\Lambda^{r}_{x},\Lambda^{\theta}_{x})=(cos\theta,\frac{-1}{r}sin \theta)$
- These are not constant, even though the vector is. Their derivatives are also not 0. These point to the fact that we have to differentiate the basis vectors too.

*Derivatives Of Basis Vectors*

*Derivatives Of General Vectors*
-  A general vector $\vec{V}$ has components on the polar basis of $(V^{r},V^{\theta})$. Its derivative with respect to $r$ is then: $\frac{\partial \vec{V}}{\partial r}=\frac{\partial V^{\alpha}}{\partial r}\vec{e}_{\alpha}+V^{\alpha}\frac{\partial \vec{e}_{\alpha}}{\partial r}$. More generally, in any coordinate basis, we have $$\frac{\partial \vec{V}}{\partial x^\beta}=\frac{\partial V^{\alpha}}{\partial x^{\beta}}\vec{e}_{\alpha}+V^{\alpha}\frac{\partial \vec{e}_{\alpha}}{\partial x^{\beta}}$$
*The Christoffel Symbols*
- The term $\frac{\partial \vec{e}_{\alpha}}{\partial x^{\beta}}$ is just a limit of a difference of a vector, so is itself a vector and hence can be expressed as $\frac{\partial \vec{e}_{\alpha}}{\partial x^{\beta}}= \Gamma^{\mu}_{\alpha \beta}\vec{e}_\mu$ 
- The Christoffel symbols are just the coefficient of the derivatives of basis vectors. To calculate them in polar coordinates, one can express the polar vector basis in terms of the cartesian basis, take derivatives with respect to polar coordinates, convert the result in terms of polar basis vectors. The cartesian basis is only used for the ease of taking derivatives (they are constant vectors). The coefficients one gets are then the Christoffel symbols.

*The Covariant Derivative*
- The derivative of a vector can now be written as $\frac{\partial \vec{V}}{\partial x^\beta}=\frac{\partial V^{\alpha}}{\partial x^{\beta}}\vec{e}_{\alpha}+V^{\alpha}\frac{\partial \vec{e}_{\alpha}}{\partial x^{\beta}}$ 
- 