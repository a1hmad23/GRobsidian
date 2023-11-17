
### 4.1 Fluids

- The source of the gravitational field can be taken as a perfect fluid as a first approximation.
- A fluid is a special kind of continuum- a collection of particles so numerous that the dynamics of individual particles cannot be followed, leaving only a description in terms of average quantities-number of particles per unit volume, energy density, density of momentum, temperature etc.
- The collection of particles must be large enough so that individual particles don't matter, but small enough so that it is relatively homogenous- average velocity, kinetic energy, interparticle spacing must be the same everywhere in the collection. Such a collection is called an element.
- The continuum approximations assigns to each element a value of density, temperature, etc. If such a collection does not exist, then the continuum approximation breaks down. Since the elements are regarded as small, this approximation is mathematically expressed by assigning to each point a value of density, temperature, etc. So a continuum is defined by various fields, having values at each point and each time.
- A fluid is a continuum that flows. Rigidity comes from forces parallel to the interface between two elements. Two adjacent elements can push and pull on each other, but the continuum wont be rigid unless they prevent each other from sliding along their common boundary. A fluid is characterized by the weakness of such forces compared to the push and pull forces which are called pressure. A perfect fluid has all anti slipping forces equal to 0, the only force between neighboring elements being pressure.

### 4.2 Dust: The Number-flux vector $\vec{N}$ 

- Relativistic description of a fluid
- Dust is a collection of particles, all of which are at rest in some Lorentz frame.

*The Number Density $n$* 
- Basic question: how many of these particles are there per unit volume?
- In their rest frame, just count them and divide by volume for different regions.
$$n\equiv number\ density\ in\ the\ MCRF\ of\ the\ element$$
- $n$ may be a function of the coordinates $x^{i}$, but in the rest frame, it will not depend on $t$. In other frames, the Lorentz transformations may bring a dependence on $t'$.
- The number density in some frame $O'$:
- They will all have the same velocity $v$ in $O'$. Total number of particles will not change, however, the same number of particles might occupy a different volume.
- Suppose, in the rest frame, some number of particles occupied a volume $\Delta x \Delta y \Delta z$. In $O'$, due to Lorentz contraction, they will occupy a volume  $\Delta x \Delta y \Delta z \sqrt{1-v^2}$.
- Hence, the number density in this frame is related to the rest frame by $\frac{n}{\sqrt{1-v^{2}}}$ 

*The Flux across a surface*
- When particles move, another basic question is how many of them move in a specific direction?
- The flux of particles across a surface is the number crossing a unit area of that surface in a unit time.
- Since area and time are frame dependent concepts, the flux clearly depends on the inertial reference frame used. It also depends on the orientation of the surface, since a surface parallel to the velocity of the particles will have no particles crossing it.
- In the rest frame of the dust, the flux is 0.
- in $O'$, suppose all particles move with the velocity $v$ in the $x$ direction. Consider a surface $\mathcal{L}$ that is oriented perpendicular to $x'$ which has are $A=\Delta y \Delta z$. All the particles within a distance $x=v \Delta t'$ will cross the surface in time $\Delta t'$. Since the particles are moving in the $x$-direction, the rectangular volume $\Delta y \Delta z v \Delta t'$ contains all and only those particles that will generate the flux. Hence, the total number of particles that will cross the surface is $\frac{n}{\sqrt{1-v^{2}}}\Delta y \Delta z v \Delta t'$.
- The flux (number crossing per unit volume per unit time) is then  $$(flux)^{x'}=\frac{nv}{\sqrt{1-v^{2}}}$$
- Suppose the particles also had a velocity in the y-direction. Even then, it will be the x component of the velocity that carries particles through the surface oriented perpendicular to it: $$(flux)^{x'}=\frac{nv^{x'}}{\sqrt{1-v^{2}}}$$
*The Number Flux Four Vector*
- Suppose in a frame $O$ there is a particle moving with velocity $v$ in the $x$ direction. The particle defines an inertial frame $O'$, which is its rest frame where the velocity vector is just the time basis vector $\vec{e_{0'}}$. Now that we know a vectors representation in one inertial frame, we can apply the Lorentz transformations to it to find its representation in any other frame we know the relative velocity with the rest frame of. Hence, in the frame $O'$, $\vec{U}\rightarrow_{O'} e_{0'}$, so $U^{\alpha'}=(1,0,0,0)$Then, in the frame $O$, $U^{\beta}= \Lambda^{\beta}_{\alpha'}U^{\alpha'}=\Lambda^{\beta}_{0'}$ 
  Hence, $\vec{U}\rightarrow_{O}(\Lambda^{0}_{0},\Lambda^{1}_{0},\Lambda^{2}_{0},\Lambda^{3}_{0})$
  The $v$ in the Lorentz transformations will be the same as the particles velocity.
- Let the particle have velocity ($v^{x},v^{y},v^{z}$) in the frame $O'$. Then, the 4-velocity $\vec{U}$ in the frame $O'$ has components: $\vec{U}\rightarrow_{O'}(\frac{1}{\sqrt{1-v^{2}}}, \frac{v^{x}}{\sqrt{1-v^{2}}}, \frac{v^{y}}{\sqrt{i-v^{2}}}, \frac{v^{z}}{\sqrt{1-v^{2}}})$ 
- Also, $\vec{U}\rightarrow_{O'}(\frac{dt}{d \tau},\frac{dx}{d \tau},\frac{dy}{d \tau}, \frac{dz}{d \tau})=(\frac{dt}{d \tau},\frac{dx}{dt} \frac{dt}{d \tau},...)$ which leads to the same result.

- The vector $\vec{N}$ defined by $\vec{N}=n \vec{U}$ then, in the frame $O'$ has components: $$\vec{N}\rightarrow_{O'}(\frac{n}{\sqrt{1-v^{2}}}, \frac{nv^{x}}{\sqrt{1-v^{2}}}, \frac{nv^{y}}{\sqrt{1-v^{2}}}, \frac{nv^{z}}{\sqrt{1-v^{2}}})$$
- Note that $n$ here denotes specifically the number density in the MCRF frame. Hence, the time component of the number flux vector $\vec{N}$ in any frame denotes the number density in that frame, while the spatial components thus become the flux in that frame.
- In Galilean physics, the number density was a scalar (no Lorentz contraction), and flux was a frame dependent concept since the three vector velocity was a frame dependent concept. However, here $\vec{N}$ is a vector, a tensor, a frame invariant/ independent geometrical object: it's action on a one-form to give a number is independent of a frame.
- A three vector is also frame independent in the sense that it isn't effected by the orientation of the axes. However, velocity was a frame dependent concept, and since flux was defined in terms of that, so the flux vector had to be defined relative to some velocity and hence some frame, and was a different vector in some other frame where the velocity of the particles generating the flux was different. To a relativist, there's only a single 4-vector $\vec{N}$, the frame dependence comes from missing one of its components.
- $\vec{N}\cdot \vec{N}=-n^{2}\rightarrow n=-\sqrt{\vec{N}\cdot \vec{N}}$ 
- Thus, $n$ is a scalar. Like rest mass, it is the scalar value of the number density in the MCRF.

### 4.3 One-Forms And Surfaces

*Number Density as a Timelike flux*
- ![[Pasted image 20231116193322.png]]
- The flux is the number of worldlines crossing the x-surface per unit time ($\Delta t=1)$. Taking into account the y and z directions of the x-surface, the flux can be regarded as the number of worldlines present in the unit cube $\Delta t=1, \Delta z=1, \Delta y=1$.
- Since time too is a coordinate no different than the spatial coordinates in these matters, we can think of a flux through time: imagine an ordinary cube with sides $\Delta x=\Delta y= \Delta z=1$ and regard the surface $L$ as constant in $t$. ![[Pasted image 20231116194048.png]]
- Then, the timelike flux is the number crossing the interval $\Delta x=1$ (since y and z are suppressed), But this is just the number contained in the unit volume at the given time: the number density. So, timelike flux is the number density.

 *A One-Form defines a surface*
 - To push our invariant picture further, we use one-forms to define the above surfaces.
 - In general, a surface is defined by $\phi(t,x,y,z)=C$. The gradient of the function $\phi$ is a normal one-form, which in a sense defines the surface as it uniquely determines the direction of its normal. However, any multiple would do so too, so it is customary to choose the unit normal one-form for surfaces that are not null: $\tilde{n}=\frac{\tilde{d}\phi}{|\tilde{d \phi}|}$, where |$\tilde{d \phi}$| is the magnitude of the normal one-form |$\tilde{d \phi}$| =$|\eta^{\alpha \beta} \phi_{,\alpha} \phi_{,\beta}|^{\frac{1}{2}}$ 
 - The surface element is defines as the unit normal times an area element. In this case, it is a volume element in three space in a three space whose coordinates are $x^{\alpha},x^{\beta}, x^{\gamma}$ can be represented by: $\tilde{n}dx^{\alpha}dx^{\beta}dx^{\gamma}$. A unit volume is $\tilde{n}$.

*The Flux Across The Surface*
- In 3D, the flux across the electric field is just $\vec{E}\cdot \vec{n}$. Here, it will be $\langle \tilde{n},\vec{N} \rangle$:
	- Let $\phi$ be a coordinate $x'$. Then, a surface of constant $x'$  (and $\phi$) has normal $\tilde{d}x'$, which is a unit normal since $\tilde{d}x' \rightarrow_{O'}(0,1,0,0)$ and magnitude is invariant. 
	- Then, $\langle \tilde{n},\vec{N} \rangle =N^{\alpha}(\tilde{d}x')_{\alpha} =N^{x'}$, which as we have seen is the flux across x-surfaces. Clearly, if we had chosen a surface of another constant coordinate, lets say $t'$, then we would have wound up with the flux across that surface, the timelike flux, number density in that frame $N^{0'}$.
	- Hence, given the vector $\vec{N}$, we can find its flux across a surface by contracting it with it unit normal one form $\tilde{n}$. Moreover, we have expressed everything frame invariantly and in a manner that separates the property of the system: $\vec{N}$ from that of the surface $\tilde{n}$.

*Representation Of A Frame By A One-Form*
- An inertial frame is defines by its four-velocity, the spatial components giving the velocity by which its spatial axes are moving and temporal component giving the rate at which its clocks are running (time dilation).
- But it can also be defined by the corresponding one-form, the one associated with the four velocity **g**$(\vec{U},)$. This has components $U_{\alpha}=n_{\alpha \beta}U^{\beta}$. In this frame then, $U_{0}=-1$ and $U_{i}=0$.
- Since the components of $\vec{U}$ equal the components $\vec{d}t$, and they are both vectors so transform in the same manner, the two are equal so a frame can also be defines by giving the vector $\vec{d}t$ in its own rest frame.
- Likewise, the above components of the one-form matches $-\tilde{d}t$ (derivative of t with respect to t) and so we could define a frame by giving $\tilde{d}t$. This is just the normal to the surface of constant t, and so can be pictured as surfaces of constant t, the surfaces of simultaneity. These clearly do defines a frame (a rigid one). Then, we have $E= \langle \tilde{d}t,\vec{p} \rangle$.


### 4.4 Dust Again: The Stress-Energy Tensor

- Dust particles also have energy and momentum, which are the source of the gravitational field in GR. So we must ask how to represent them in a frame invariant manner. Assume that all particles have the same rest mass m.

*Energy Density*
- In the MCRF of dust, each particle has energy $m$ and there are $n$ particles per unit volume. Thus, the energy density is $\rho = energy\ density\ in\ the\ MCRF = mn$, a scalar.
- In a frame $O'$ the number density is again Lorentz transformed since volume is, but since energy is just a component of four momentum, it too is transformed. So we have: 
		Energy density in a frame in which particles have velocity $v$: $\frac{\rho}{(1-v^{2)}}$ 
- Since this transformation involves two factors of $(1-v^{2})^{\frac{1}{2}}= \Lambda^{0'}_{0}$ , it cant be a component of a four-vector but rather of a $\begin{pmatrix}0\\ 2\end{pmatrix}$ tensor (one Lorentz factor for each index). To define energy requires a one-form: in order to select the 0th component of the four-vector of energy and momentum; to define a density also requires a one-form, since density is a flux across a constant time surface. Similarly, an energy flux (density) requires two one-forms, one to define energy and the other to define the surface.
- One can also speak of momentum density: again a one-form defines which component of momentum and another one-form defines density.
- By analogy, there is also a momentum flux: the rate at which momentum crosses some surface.
- So there is a tensor **T**, called the stress-energy tensor which has all these numbers as values when supplied with the appropriate one-forms as arguments.

*The Stress-Energy Tensor*
- The stress-energy tensor is defined by its components: $$T(\tilde{d}x^{\alpha}, \tilde{d}x^{\beta})=T^{\alpha \beta}= Flux\ of\ \alpha\ momentum\ across\ a\ surface\ of\ constant\ x^\beta$$
	- $\alpha\ momentum$ is just the $\alpha$ component of four-momentum: $\langle \tilde{d}x^{\alpha}, \vec{p} \rangle$ 
	- $T^{00}$=energy density (flux of 0 momentum across a surface of constant t)
	- $T^{0i}$= flux of energy across $x^{i}$ (=constant) surface
	- $T^{i0}$=momentum density
	- $T^{ij}$ flux of i momentum across j surface

- For any system, giving the components of **T** in some frame defines it completely. For dust in the MCRF: 
	- $(T^{00})_{MCRF}=\rho=mn$ 
	- All the other components are zero since there is neither any spatial flux nor any i momenta.
- The Tensor $\vec{p} \otimes \vec{N}$ has exactly these components in the MCRF too. Hence, dust: $$T=\vec{p} \otimes \vec{N}=mn\ \vec{U} \otimes \vec{U}= \rho \ \vec{U} \otimes \vec{U}$$
- Hence, $T^{\alpha \beta}=T(\tilde{w}^{\alpha},\tilde{w}^{\beta})=\rho \vec{U}(\tilde{w}^{\alpha})\vec{U}(\tilde{w}^{\beta})=\rho U^{\alpha}U^{\beta}$ 
	![[Pasted image 20231117222904.png]]
 These are what one would calculate for energy density, energy flux, momentum density, momentum flux from first principles
 - Notice that **T** is symmetric. This is true in general, not just for dust.




