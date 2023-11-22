
### 4.1 Fluids

- The source of the gravitational field can be taken as a perfect fluid as a first approximation.
- A fluid is a special kind of continuum- a collection of particles so numerous that the dynamics of individual particles cannot be followed, leaving only a description in terms of average quantities-number of particles per unit volume, energy density, density of momentum, temperature etc.
- The collection of particles must be large enough so that individual particles don't matter, but small enough so that it is relatively homogenous- average velocity, kinetic energy, interparticle spacing must be the same everywhere in the collection. Such a collection is called an element.
- The continuum approximations assigns to each element a value of density, temperature, etc. If such a collection does not exist, then the continuum approximation breaks down. Since the elements are regarded as small, this approximation is mathematically expressed by assigning to each point a value of density, temperature, etc. So a continuum is defined by various fields- having values at each point and each time.
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


### 4.5 General Fluids

- Until now we have dealt with the simplest possible collection of particles: not interacting and all at the same constant velocity. To generalize this to real fluids, we have to take into account that besides the bulk motion of a fluid, each particle can have some random motion and various forces between the particles can contribute potential energies to the total.

*Definition Of Macroscopic Quantities*
- For each fluid element, we go to the frame where it is at rest- its total spatial momentum is zero. This is its MCRF. However, a fluid moment can accelerate, so a moment later a different frame will be its MCRF. Different fluid elements can be moving at different velocities, so an MCRF is not shared. Thus, the MCRF is specific to a single fluid element, and which frame is the MCRF is a function of position and time. All scalar quantities associated with a fluid element in relativity are defined to be their values in its MCRF.
- ![[Pasted image 20231118133103.png]]

*First Law Of Thermodynamics*
- Conservation of Energy.
- In an MCRF, a fluid element can exchange energy by either heat or work: $\Delta E=\Delta Q -p \Delta V$ 
- If an element contains $N$ particles, and $n$ is the number density, then $V=\frac{N}{n}$ or $\Delta V=\frac{-N}{n^{2}}\Delta n$.
- From the definition of $\rho$ : $E=\rho V =\rho \frac{N}{n}$ or $\Delta E=\rho \Delta V +\Delta \rho V$.
- $\rightarrow \Delta Q=\frac{N}{n} \Delta \rho -N(\rho +p) \frac{\Delta n }{n^{2}}$ 
- Heat absorbed by particle $q=\frac{Q}{n}$ is then: $nq=\Delta \rho - \frac{\rho + p}{n} \Delta n$ 
- Suppose the changes are infinitesimal. It can be shown in general that a fluid's state can be described by two parameters, say $\rho$ and $n$. Everything else is then a function of these, such as the RHS of the above equation. The general theory of first order differential equation then says that for such an equation there are always present two functions of the two parameters such that:
	$d \rho -(\rho + p) \frac{dn}{n}= A dB$     is an identity for all $rho$ and $n$.
- It is customary in Thermodynamics to define temperature T as $A/n$ and entropy S as B: $d \rho -(\rho + p) \frac{dn}{n}=nTdS \rightarrow \Delta q=T \Delta S$         
- The heat absorbed by a fluid element is proportional to its increase in entropy.

*The General Stress-Energy Tensor*
- The earlier definition of the **T** was perfectly general. Then, in the MCRF of general fluid element, we have:
	- $T^{00}=\rho= energy\ density$
	- $T^{0i}=energy\ flux$. There is no motion but energy may be transmitted by heat conduction, so this is a heat conduction term in the MCRF. 
	- $T^{i0}=momentum\ density$. Particles have no momentum, but if heat is being conducted, then the energy will carry momentum. (argument below for $T^{0i}=T^{i0}$)
	- $T^{ij}=stress$.

*The Spatial components of T, $T^{ij}$
- Flux of i momentum across j surface.
![[Pasted image 20231118164124.png]]
	Consider two fluid elements A and B. In general they exert forces on each other. Let the force exerted by A on B be F. Let the common interface shared by them be L. B of course exerts an equal and opposite force on A. Since this is the MCRF where velocities are 0, newtons second law is perfectly valid here which say that force equals the rate of change of momentum. Hence, if A is exerting a force on B, A is pouring momentum onto B. Of course, other fluid elements might be doing the same to B, and the total momentum poured into B might be 0 so it wont move. There is therefore a flow of momentum from A to B across L, at the rate F. If L has area A, then the flux of momentum is F/A. If L is a surface of constant $x^j$, then $T^{ij}$ for the fluid element A is $\frac{F^{i}}{A}$.
	 
- So $T^{ij}$ represents forces between adjacent fluid elements. These forces need not be perpendicular to the interface (such as rigidity because of parallel forces), but if they are, then clearly $T^{ij}=0$ unless $i=j$.

*Symmetry Of $T^{\alpha \beta}$
- If a tensor is symmetric in one frame, that means in that frame for any $\tilde{r},\tilde{q},T(\tilde{r},\tilde{q})=T(\tilde{q},\tilde{r})$. But that is a tensor equation, with no reference to a specific frame, involving only geometric quantities. Hence, it implies symmetry in all frames.

![[Pasted image 20231120222434.png]]
- The cube of side $l$ is a fluid element. Since $T^{ij}$ is the flux of momentum across j surface, and flux of momentum is momentum per unit time per unit area, while force is momentum per unit time so momentum flux is just force per unit area and $T^{ij}$ is momentum flux so $T^{ij}$ is force per unit area. Therefore, force across surface 1 is: $F^{i}_{1}=T^{ix}l^{2}$. Since F is not necessarily perpendicular to the surface, i runs from 1 to 3.
- Similarly, force emanating from 2 to some neighbor is $F^{i}_{2}=T^{iy}l^{2}$ and there's $F^{i}_{3}$ and $F^{i}_{4}$.
- We are considering small fluid elements where $l \rightarrow 0$. Then, in order for infinitesimal mass to not have infinite acceleration which any finite force would produce, the total force on the fluid element must vanish.
- From Newtons 3rd law, the force on the fluid in the x direction is: $-F^{i}_{1} - F^{i}_{3}$. Hence, we must have $F^{i}_{3}=-F^{i}_{1}$. With this knowledge, we compute torques about the z-axis through the center of the fluid element (which is why we ignored the top and bottom forces as they don't contribute to this torque).
- find total torque, find an equation for angular acceleration which would depend inversely on the size of the fluid element which must be 0 which would give the symmetry of **T** (partially, repeat argument, as it was arbitrary, for other axes for full symmetry).
- Since energy flux is the speed at which energy density is flowing, and since energy and mass are the same thing, energy flux is the speed at which mass density is flowing which is just momentum density. Therefore, $T^{0i}=T^{i0}$ .

*Conservation Of Energy Momentum*
- Since **T** represents the momentum and energy content of a fluid, it can be used to represent the law of conservation of energy and momentum:
	- Lets take a cubic element (we are gonna take the limit $l\rightarrow 0$ where the shape would become irrelevant so it doesn't effect the generality of the argument). ![[Pasted image 20231122184549.png]]
	- The energy flowing in at the side 4 is $T^{0x}(x=0)$. It follows:
	- ![[Pasted image 20231122185132.png]]
	- Dividing by $l^{3}$ and taking the limit as $l\rightarrow 0$, we see that the RHS becomes the definitions of partial derivatives:
	- $\frac{\partial}{\partial t}T^{00}=\frac{\partial}{\partial x}T^{0x} + \frac{\partial}{\partial y}T^{0y} + \frac{\partial}{\partial z}T^{0z}$ $\rightarrow$   $T^{00}_{,0}=T^{0x}_{,x}+T^{0y}_{,y}+T^{0z}_{,z}$  $$T^{0 \alpha}_{,\alpha}$$ which is the law of conservation of energy.
- Similarly, for the conservation of $\alpha$ momentum: $$T^{\alpha \beta}_{,\beta}$$
- These are just divergences.

*Conservation Of Particles*
- $N^{\alpha}_{,\alpha}=nU^{\alpha}_{,\alpha}=0$

### 4.6 Perfect Fluids

- No viscosity and no heat conduction in the MCRF.

*No Heat Conduction*
- For any fluid element, in the MCRF, the only mode of energy transfer is heat conduction since no movement takes place. There is no head conduction in perfect fluids, therefore $T^{0i}=T^{i0}=0$. This means that entropy is constant, via the heat transfer and change in entropy relation.

*No Viscosity*
- This means forces should always be perpendicular to the interface. Hence, $T^{ij}=0\ unless\ i=j$, meaning that $T^{ij}$ should be a diagonal matrix.
- Since no viscosity is a general statement independent of the spatial axes, it must be that $T^{ij}$ is diagonal in all MCRF frames. The only such matrix is a multiple of the identity.
- Thus an x-surface will have it across only a force in the x-direction, similarly for y and z. All of these forces per unit are are equal (no preferred direction), and are called the pressure $p$.
- Hence, $T^{ij}=p\delta^{ij}$
- ![[Pasted image 20231122211827.png]]
- Hence, in the MCRF $\rightarrow T^{\alpha \beta}=(\rho +p)U^{\alpha}U^{\beta}+p\eta^{\alpha \beta}$ 
- Since this is a frame invariant formula: $$T=(\rho + p)\vec{U}\otimes \vec{U} +pg^{-1}$$The Stress-Energy Tensor for a perfect fluid.

*Asides On The Meaning Of Pressure*
- Comparing the above formula with for dust, we see that dust is a pressure free special case of a perfect fluid. Pressure comes from the flux of momentum, whether that comes from forces or particles crossing a boundary doesn't matter.

*The Conservation Laws*
- $T^{\alpha \beta}_{,\beta}=[(\rho +p)U^{\alpha}U^{\beta}+p\eta^{\alpha \beta}]_{,\beta}$ 
- Assuming conservation of particles $N^{\beta}_{,\beta}=nU^{\beta}_{,\beta}=0$, we write the first term as $[\frac{\rho +p}{n}  U^{\alpha}nU^{\beta}]_{\beta}$. By the produce rule of derivatives, we have $\frac{\rho +p}{n}  U^{\alpha}_{,\beta}nU^{\beta} + \frac{\rho +p}{n}  U^{\alpha}nU^{\beta}_{,\beta}=\frac{\rho +p}{n}  U^{\alpha}_{,\beta}nU^{\beta}=nU^{\beta}( \frac{\rho +p}{n} U^{\alpha})_{, \beta}$.
- As for the second term, $\eta^{\alpha \beta}$ is a constant matrix so $\eta^{\alpha \beta}_{,\gamma}=0$ 
- Moreover, we have $U^{\alpha}U_{\alpha}=-1 \rightarrow (U^{\alpha}U_{\alpha})_{,\beta}=0=(U^{\alpha}U^{\gamma}\eta_{\alpha \gamma})_{,\beta}=(U^{\alpha}U^{\gamma})_{,\beta}\ \eta_{\alpha\gamma }=2U^{\alpha}_{,\beta}U^{\gamma}\eta_{\alpha\gamma}$   notice that the last step follows from symmetry (equal footing of the two live indices).
- Hence, we have $T^{\alpha \beta}_{,\beta}=nU^{\beta}( \frac{\rho +p}{n} U^{\alpha})_{, \beta} + p_{,\beta}\eta^{\alpha \beta}$. Now, contracting it with $U_{\alpha}$ (feeding **T** the one-form)