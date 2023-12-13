### 5.1 On The Relation Of Gravitation To Curvature

- SR does not include forces.
- The postulates of SR lead to existence of inertial frames that fill all of spacetime: all of spacetime can be described by a single frame, all of whose coordinates are at rest with respect to the origin, and all of whose clocks run at the same rate. [see section 1.2]
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
- These lead to a transformation rule for one-forms naturally, and so all one forms are defined (as gradients of some scalar functions). Vectors are then defined as functions of one forms that return a scalar, and hence must transform in the opposite way to a one-form.
- The two transformation matrices are inverses of each other.

*Curves And Vectors*
- A path is a connected series of points in the plane. A curve is a parametrized path.
- The derivative of a scalar field along a curve is $\frac{d\phi}{ds}$ which is equal to the contraction between the gradient one-form $\tilde{d}\phi$ and the tangent vector $\vec{V}$. Hence  $\frac{d\phi}{ds}=\langle \tilde{d}\phi,\vec{V} \rangle$.
- A curve has a unique tangent, since both the path and the parametrization are given.

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
- The Christoffel symbols are just the coefficients of the derivatives of basis vectors. To calculate them in polar coordinates, one can express the polar vector basis in terms of the cartesian basis, take derivatives with respect to polar coordinates, and then convert back the result in terms of polar basis vectors. The cartesian basis is only used for the ease of taking derivatives (they are constant vectors). The coefficients one gets are then the Christoffel symbols.

*The Covariant Derivative*
- The derivative of a vector can now be written as $\frac{\partial \vec{V}}{\partial x^\beta}=\frac{\partial V^{\alpha}}{\partial x^{\beta}}\vec{e}_{\alpha}+V^{\alpha}\Gamma^{\mu}_{\alpha \beta}\vec{e}_\mu$ 
- Relabeling the indices and then taking common: $\frac{\partial \vec{V}}{\partial x^\beta}=(\frac{\partial V^{\alpha}}{\partial x^{\beta}}+V^{\mu}\Gamma^{\alpha}_{\mu \beta})\vec{e}_\alpha$     
- Hence, the vector field $\frac{\partial \vec{V}}{\partial x^\beta}$ has components $V^{\alpha}_{;\beta}=V^{\alpha}_{,\beta}+V^{\mu}\Gamma^{\alpha}_{\mu \beta}$ 
- Note that we interchange between considering $\vec{V}$ as a single vector and as a general vector in some vector field, in which case it could be any vector of some vector field, and so is a representation of that vector field. Then, any operations applied to it could be considered as applying those operations to all the vectors in that vector field which is equivalent to applying those operations to the vector field itself.
- Hence, we have the derivative of a vector field $\vec{V}$: $$\frac{\partial \vec{V}}{\partial x^\beta}=V^{\alpha}_{;\beta}\vec{e}_{\alpha}$$
Show that $\nabla \vec{V}$ is a $\begin{pmatrix}1\\ 1\end{pmatrix}$ tensor, as defined: $(\nabla \vec{V})^{\alpha}_{\beta}=V^{\alpha}_{;\beta}$  where $V^{\alpha}_{;\beta}=V^{\alpha}_{,\beta}+V^{\mu}\Gamma^{\alpha}_{\mu \beta}$ 
Answer: We let $\nabla \vec{V}$ be a function of vectors and one-forms (assumption 1), and we define its action on its inputs of vectors and one-forms to be such that $\nabla \vec{V} (\vec{X};\tilde{\omega})=V^{\alpha}_{;\beta}X^{\beta}\omega_{\alpha}$ (assumption 2)
Then, if we are able to show that the result is a scalar, and that the function is linear in both of its arguments, the proof will be done.
- 
- 
- Since the operation of taking a derivative amounts a limit of a difference, the derivative of a vector gives another vector. This way, if we take derivatives of all vectors in a vector field- of a vector field, we get another vector field.
- $A^{\beta}$ 
- Here, for a fixed $\beta$, we get a vector field where each vector has two components. However, since $\beta$ can take on two values, for a fixed vector, we get four components, and from a single vector field, we get two vector fields (one where the vectors are lets say the x-derivatives and the other where they are the -y derivatives of the original vectors). Hence, for each vector, we get 4 components, with two corresponding to each value $\beta$ can take.
- The above comments suggest that this situation is in line with where a tensor can be useful, so let us define a $\begin{pmatrix}1\\ 1\end{pmatrix}$ tensor $\nabla \vec{V}=V^{\alpha}_{;\beta}\vec{e}_{\alpha}\tilde{\omega}^{\beta}$ 
- This has components $(\nabla \vec{V})^{\alpha}_{\beta}=V^{\alpha}_{;\beta}$  (For a 2D space, these are 4 components)
- A $\begin{pmatrix}1\\ 1\end{pmatrix}$ tensor provides a mapping between vectors..
- $\nabla \vec{V}$ with a basis vector $\vec{e}_{\beta}$: $$\langle \nabla \vec{V}, \vec{e}_{\beta} \rangle= V^{\alpha}_{;\beta}\vec{e}_{\alpha} \langle \tilde{\omega}^{\beta}, \vec{e}_{\beta} \rangle=V^{\alpha}_{;\beta}\vec{e}_{\alpha}=\frac{\partial \vec{V}}{\partial x^\beta}$$
- Hence, to specify the value of $\beta$, we need to contract it with $\vec{e}_{\beta}$ This is why for a fixed $\beta$ we get a single vector field, but for two values of $\beta$ we get a tensor field: one vector field corresponding to each $\beta$, to choose the value of $\beta$/vector field/components we want to pick, we have to feed in a vector, and then we get in the domain of a single vector field out of the two.
- Hence, the derivative of a vector can be thought of as a result of the contraction between a one higher rank tensor with a specific basis vector. The Covariant derivative is the higher rank tensor. 
- The components of the covariant derivative $(\nabla \vec{V})^{\alpha}_{\beta}=V^{\alpha}_{;\beta}$ can be obtained in two ways. One is to calculate $V^{\alpha}_{;\beta}=V^{\alpha}_{,\beta}+V^{\mu}\Gamma^{\alpha}_{\mu \beta}$  in whatever coordinate system one is in by knowledge of the Christoffel symbols. The other is to make use of the fact that they are tensor components and so can be obtained by transformation: transform them from cartesian coordinates (where there form is simple because of the vanishing of the Christoffel symbols) by use of transformation matrices.

*Divergence And Laplacian*
- The divergence of a vector $\vec{V}$ is the scalar obtained by contracting $\nabla \vec{V}$ with basis one forms and basis vectors, that is, contracting $(\nabla \vec{V})^{\alpha}_{\beta}$ on its two indices: $(\nabla \vec{V})^{\alpha}_{\alpha}$ 
- In Cartesian $(\nabla \vec{V})^{\alpha}_{\alpha}=V^{\alpha}_{,\alpha}$ 
- More generally, $(\nabla \vec{V})^{\alpha}_{\alpha}=V^{\alpha}_{;\alpha}= V^{\alpha}_{,\alpha}+V^{\mu}\Gamma^{\alpha}_{\mu \alpha}$  
- Notice the sum on Christoffel symbols.
- Notice that theres a contraction, so for a specific covariant derivative, we get the same value for the expression coordinated in any system, and so the simple expression in cartesian will be equivalent to the general expression. Obviously, this had to be the case since it denotes a geometrical quantity: divergence.
- Laplacian is the divergence of the gradient. But there is no divergence of one-forms so we convert the gradient one form to a vector gradient and take its divergence (simply input that vector into the formula obtained for the divergence of a general vector).

*Derivatives Of One-Forms And Tensors Of Higher Types*
- Since a scalar field $\phi$ depends on no basis vectors, its derivative the gradient one form $\tilde{d}\phi$ is equivalent to its covariant derivative $\nabla \phi$.
- For a fixed $\beta$, $\frac{\partial \tilde{p}}{\partial x^{\beta}}=\nabla_{\beta} \tilde{p}$ is a one-form, $\frac{\partial \vec{V}}{\partial x^{\beta}}=\nabla_{\beta}\vec{V}$ is a vector, and  $\langle \tilde{p},\vec{V}\rangle=\phi=p_{\alpha}V^{\alpha}$ is a scalar.
- Taking derivative of the scalar: $\nabla_{\beta}\phi=\frac{\partial p_{\alpha}}{\partial x^{\beta}}V^{\alpha}+ p_{\alpha} \frac{\partial V^{\alpha}}{\partial x^{\beta}}$
- After substituting and renaming indices: $\nabla_{\beta}\phi=(\frac{\partial p_{\alpha}}{\partial x^{\beta}} -p_{\mu}\Gamma^{\mu}_{\alpha \beta})V^{\alpha} +p_{\alpha}V^{\alpha}_{;\beta}$ 
- Now, the term on the LSH is a one form, the term outside brackets on the RHS is a one form, solving for the one in the brackets suggests it should be a one form. Moreover, it is a 2 indexed term that is being contracted with a vector, giving out a one form. Also, it has the form of a covariant derivative. Hence, we regard the term inside the brackets as the covariant derivative of a one form $\tilde{p}$ :
- $\nabla \tilde{p}\rightarrow \nabla_{\beta}p_{\alpha}=\nabla p_{\alpha \beta}=p_{\alpha ; \beta}= p_{\alpha , \beta}-p_{\mu}\Gamma^{\mu}_{\alpha \beta}$ 
- This is a $\begin{pmatrix}0\\ 2\end{pmatrix}$ tensor when $\beta$ value is not specified. It needs a vector input to turn into a one-form field/one-form and then another vector to pick a specific component of that field/one-form
- Thus, we have the covariant derivative of a scalar: $\nabla_{\beta}(p_{\alpha}V^{\alpha})=p_{\alpha ; \beta}V^{\alpha} + p_{\alpha}V^{\alpha}_{;\beta}$  
- Thus, covariant differentiation obeys the same sort of product rule as ordinary differentiation: it must do this since in cartesian coordinates $\nabla$ is just partial differentiation of components which includes the product rule, so the above general form must reduce to it in the cartesian case. For that to be possible, there had to be a product rule (the reduction $V^{\alpha}_{;\beta}=V^{\alpha}_{,\beta}$ being already there).
- The two formulae for the components of the covariant derivative of a vector and a one-form are, respectively: $$V^{\alpha}_{;\beta}=V^{\alpha}_{,\beta}+V^{\mu}\Gamma^{\alpha}_{\mu \beta } $$$$p_{\alpha;\beta}=p_{\alpha,\beta}-p_{\mu}\Gamma^{\mu}_{\alpha \beta}$$
- The derivative index $\beta$ is the last one on $\Gamma$, the other indices are where they should be.
- Since the only reason the covariant derivative was different than a normal derivative was the basis vectors, it should coincide with a normal partial derivative on scalars and should satisfy the Leibniz rule:
	- $∇_{μ}(X^{ν}X_{ν})=(∇_{μ}X^{ν})X_{ν}+X^{ν}(∇_{μ}X_{ν})=∂_{μ}(X^{ν}X_{ν})=(∂_{μ}X^{ν})X_{ν}+X^{ν}(∂_{μ}X_{ν})$  
	- Now, since we knew the covariant derivative for a vector, the covariant derivative for a one-form followed.

- For covariant derivatives of tensors of higher types: For every up index, add a Christoffel symbol contracted with the tensor on that index. For every down index, _subtract_ such a term instead.
![[Pasted image 20231126114516.png]]

### 5.4 Christoffel Symbols And The Metric

- In Cartesian coordinates, the components of a one-form and its associated vector are equal, and since the components of $\nabla$ are acquired just through partial differentiation of components (in Cartesian coordinates), it follows that the components of the covariant derivative of a one-form and a vector must be equal in cartesian coordinates.
- Hence, the covariant derivatives themselves must only differ in the position of their indices (they would be tensors of different rank/ in different spaces), the metric tensor can be used to match the indices (connect the two via forming a map between the two spaces). 
- Hence, in cartesian coordinates,  if we have $\tilde{V}=$**g**$(\vec{V},\ )$, then $\nabla_{\beta}\tilde{V}=$**g**$(\nabla_{\beta}\vec{V},\ )$. However, this is a tensor equation- two tensors are equal to each other- they have the same components and are of the same type, so they are equal in one frame and transform in the same way from that frame to any other one. So, even though this was derived from some specific frame, they are equal in that frame and transform in the same manner (because they are of the same type), this relation must be true in all frames: its a tensor equation without any reference to components.
- Hence, $$V_{\alpha;\beta}=g_{\alpha \mu}V^{\mu}_{;\beta}$$
- The above argument another way:
	- Let the unprimed indices indicate cartesian coordinates and the primed ones indicate a general coordinate system.
	- The statement $V_{\alpha'}=g_{\alpha' \mu'}V^{\mu'}$ we know to be valid in all coordinate systems.
	- In Cartesian, $g_{\alpha \mu}=\delta_{\alpha \mu} \rightarrow V_{\alpha}=V^{\alpha}$ and the Christoffel symbols vanish so $V_{\alpha;\beta}=V_{\alpha,\beta}$ and $V^{\alpha}_{;\beta}=V^{\alpha}_{,\beta}$. So, $V_{\alpha, \beta}=V^{\alpha}_{,\beta}$. It follows that $V^{\alpha}_{;\beta}=V_{\alpha;\beta}$ 
	- Hence, in Cartesian, $V^{\alpha}_{;\beta}=g_{\alpha \mu}V^{\mu}_{;\beta}$ and coupling this with $V^{\alpha}_{;\beta}=V_{\alpha;\beta}$ , we have $V_{\alpha;\beta}=g_{\alpha \mu}V^{\mu}_{;\beta}$ which is a tensor equation valid in all coordinate frames.

- Lets take the $\beta$th covariant derivative of $V_{\alpha'}=g_{\alpha' \mu'}V^{\mu'}$:
	- We apply the Leibniz product rule that the covariant derivative obeys.
	- $V_{\alpha';\beta'}=g_{\alpha' \mu';\beta'}V^{\mu'}+g_{\alpha' \mu'}V^{\alpha'}_{;\beta'}$  
	- It follows (from the map provided by the metric between the covariant derivative of a vector and a one-form) that $g_{\alpha' \mu';\beta'}=0$  in all coordinate systems.

- In Cartesian, $g_{\alpha \mu;\beta}=g_{\alpha \mu;\beta}=g_{\alpha \mu,\beta}=\delta_{\alpha \mu, \beta}=0$
- Null tensors can not be transformed by transformation matrices but lets calculate the covariant derivative of the metric tensor explicitly in general coordinates:
	- Applying the product rule and keeping in mind the - sign because of the lower indices:
	- $(\nabla g)_{\alpha' \mu' \beta'}= g_{\alpha' \mu';\beta'}= g_{\alpha' \mu', \beta'} -g_{\alpha' \nu'}\Gamma^{\nu}_{\mu'\beta}-g_{\nu \mu'}\Gamma^{\nu}_{\mu' \beta'}=0$ 
	- These must evaluate to 0 after all the sums have taken place in a specific coordinate system.

*Calculating The Christoffel Symbols From The Metric*
- From the vanishing of the covariant derivative of the metric, we can find equations for the Christoffel symbols in terms of $g_{\alpha \beta, \mu}$ and vice versa, giving an easy way to derive the Christoffel symbols.
- First, we prove that the Christoffel symbols are symmetric in their two lower indices $T^{\mu}_{\alpha \beta}=T^{\mu}_{\beta \alpha}$:
	- Consider a scalar field $\phi$. Its first derivative $\nabla \phi$ is a one-form with components $\phi_{,\beta}$
	- Its second covariant derivative $\nabla \nabla \phi$ is a $\begin{pmatrix}0\\ 2\end{pmatrix}$ tensor with components $\phi_{,\beta;\alpha}$ 
	- In Cartesian coordinates, the covariant derivative is just the normal derivative so the components are $\phi_{,\beta;\alpha}=\phi_{,\beta,\alpha}= \frac{\partial}{\partial x^{\alpha}} \frac{\partial}{\partial x^{\beta}}\phi$  
	- These are symmetric in $\alpha$ and $\beta$.
	- This means, in Cartesian coordinates, $\nabla \nabla \phi(\vec{e}_{\alpha},\vec{e}_{\beta})=\nabla \nabla \phi(\vec{e}_{\beta},\vec{e}_{\alpha})$. Now, since tensors are linear functions, we can sneak in the components for some vectors and then this equation will become $\nabla \nabla \phi(\vec{A},\vec{B})=\nabla \nabla \phi(\vec{B},\vec{A})$.
	- This is a tensor equation and so must be true in all frames.
	- Hence, if a tensor is symmetric in one frame, it must be symmetric in all frames.
	- Therefore, we have, $\phi_{,\alpha;\beta}=\phi_{,\beta;\alpha}$  in all bases.
	- These are covariant derivatives of one-forms, so $\phi_{,\alpha,\beta}-\phi_{,\mu}\Gamma^{\mu}_{\alpha \beta}=\phi_{,\beta,\alpha}-\phi_{,\mu}\Gamma^{\mu}_{\beta \alpha}$  
	- Here, the two one-forms will cancel out, leaving the symmetry of the Christoffel symbols $$T^{\mu}_{\alpha \beta}=T^{\mu}_{\beta \alpha}$$
- Now, writing different permutations of the RHS of the equation $(\nabla g)_{\alpha' \mu' \beta'}= g_{\alpha' \mu';\beta'}= g_{\alpha' \mu', \beta'} -g_{\alpha' \nu'}\Gamma^{\nu}_{\mu'\beta}-g_{\nu \mu'}\Gamma^{\nu}_{\mu' \beta'}=0$ and adding them all up using symmetry of both the metric tensor and the Christoffel symbols: ![[Pasted image 20231129112919.png]]
- ![[Pasted image 20231129112939.png]]
- The first two terms on the RHS vanish to give ![[Pasted image 20231129113020.png]]
- Upon contraction with the inverse metric, we get the expression for Christoffel symbols in terms of the metric and its derivatives: ![[Pasted image 20231129113135.png]]

### 5.5 The Tensorial Nature Of The Christoffel Symbols

- Since $\vec{e}_{\alpha}$ is a vector, $\nabla \vec{e}_{\alpha}$ is a 1-1 tensor whose components are $\Gamma^{\mu}_{\alpha \beta}$ However, notice that here $\alpha$ is just a label to denote which tensor it is: $\alpha$ changes the tensor, while $\mu$ or $\beta$ changes only the component of a given tensor. There is one such tensor for each of the basis vectors.
- However, since some other frame will have a different set of basis vectors, that arent just transformed from some other set but are wholly different vectors and geometrical entities, we get that $\nabla \vec{e}_{\alpha'}$  The note on notation here is that the primed indices dont denote transformed basis vectors but a different set of basis vectors.
- Hence, $\nabla \vec{e}_{\alpha}$ and $\nabla \vec{e}_{\alpha'}$ are two different tensors and not just transformations of each other. This follows for their respective components as well, which are the Christoffel symbols. Hence, the Christoffel symbols of one frame cannot be obtained by a simple tensorial transformation, for the simple reason that they dont originate from the same set of geometrical quantities- basis vectors of different frames are different vectors, not just transformations of each other. Take Cartesian coordinates for example, where the Christoffel symbols are none. Those in polar coordinates are not null, and not null vectors cannot be obtained from null vectors via transformation, which points to the fact they are different entities.
- However, if we keep the $\alpha$ label, we do get that the $\mu$,$\beta$ components of the Christoffel symbols are components of one single tensor. However, there is no single tensor whose components are the whole of $T^{\mu}_{\alpha \beta}$ with $\alpha$ allowed to vary. The combination $V^{\beta}_{,\alpha} +\Gamma^{\beta}_{\mu \alpha}V^{\mu}$ are the components of one single tensor.

### 5.6 Noncoordinate Bases
