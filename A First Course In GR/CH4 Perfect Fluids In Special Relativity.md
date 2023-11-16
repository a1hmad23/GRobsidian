
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


