### 1.1 Fundamental Principles of SR

- Regarding $(t,x,y,z)$ as 4-coordinates of a 4D space(time) began the geometrical point of view.
- Postulates of SR:
	 1. Principle of relativity: No absolute motion; all motion is relative; can only determine your motion with respect to something else. Physics in all inertial frames of reference is the same.
	2. Universality of the speed of light: All inertial observers measure the speed of light to be c.
- In Galilean relativity, a velocity v(t) of an object as measured by one observer becomes v(t) - V as measured by another observer moving with the constant speed V relative to the first observer. However, both the observers observe the same physics: Newtons laws are invariant under the Galilean velocity transformation.
- Newton argued for an absolute acceleration: an observer can extract information about its acceleration itself (train scenario). Hence, it is only for inertial observers that physics remain the same and is the reason why they are classed out.

### 1.2 Definition of an inertial observer in SR

- An inertial observer is a coordinate system for spacetime, which makes observations of $(x,y,z,t)$ for any event such that:
	1. **Rigidity (Constant Distance Between Points):** The distance between any two points within the observer's frame of reference remains constant in time. This ensures that the reference frame maintains its shape and size. In other words, it remains rigid. If the distance between points in the frame were changing, it would imply that the frame itself is undergoing some sort of deformation, which could be indicative of non-inertial effects.
	2. **Synchronized Clocks:** (only an unaccelerated observer can keep his clocks synchronized) All clocks within the observer's frame of reference are synchronized and show the same time for events happening at the same time within the frame. This condition ensures that measurements of time intervals are consistent across the entire frame of reference.
	3. **Euclidean Geometry:** The geometry of space within the observer's frame of reference at any time $t$ is Euclidean. This means that the spatial geometry follows the usual rules of flat, "classical" geometry as described by Euclid's postulates. This ensures that there are no inherent curvatures or distortions in the frame's spatial fabric. In the context of general relativity, this is a significant distinction because spacetime can be curved in the presence of mass and energy, leading to non-Euclidean geometries.
- The time coordinate of an event is the one as measured by the clock at the spatial coordinates $(x,y,z)$ of the event.

### 1.4 Spacetime Diagrams

- In spacetime diagrams, a point is an event of fixed $\vec{x}$ and fixed $t$.
- A line is a relation $x = x(t)$, which is a particles worldline.
- Slope is $\frac{dt}{dx} = \frac{1}{v}$. From this it can be deduced that light travels at 45 degrees in natural units.
### 1.5 Construction Of The Coordinates Used By Another Observer

- Since observers are just coordinate systems for the *same spacetime*, an event can have multiple coordinates corresponding to different observers. Hence coordinate lines of one observer can be drawn over the spacetime diagram of another, using the postulates of SR:
	- In any frame, the time axis represents the worldline for the observer at the origin, since all observers are stationary in their own frame (hence, only move through time). Hence, $t'$ axis is the same as the worldline for $O'$. Since the slope of a worldline is just the reciprocal of the velocity, and since $O'$ is just a particle moving with velocity $v$ in the frame $O$, it's worldline is a slanted straight line drawn at some angle with the $t-axis$ whose tangent is v. Hence, we have $t'-axis$ (in the frame $O$).
	- The $x'$ axis can be defined as the locus of events that reflect light rays to the $t$ coordinate $+a$ if they were emitted from $-a$, for any $a$. Choose an arbitrary point $a$ on the $t'$ axis, and mark $-a$. let a light ray go from $-a$ and let a light ray go to $+a$, via reflection (traveling at 45 degrees). Where the 2 intersect is a point on the $x'$-axis. Connect that point to the origin to get the $x'$ axis (since the two coordinate frames coincide at the origin).

### 1.6 Invariance Of The Interval

- We have found the coordinate axis of $O'$, now to find the length scale of $O'$ in $O$'s spacetime diagram:
- The interval between any 2 events is defined. For events on a light beam, the interval equals $0$: $\Delta s^2 = -\Delta t^2 + \Delta x^2 + \Delta y^2 + \Delta z^2 = 0 = \Delta s'^2$ (natural units so $d \vec{x}=dt$).
- Assume that the relation between the coordinates of $O$ and $O'$ is linear, so that $\Delta s'^2$ is some quadratic function of the unprimed coordinate increments $(\Delta t^2, \Delta x^2, \Delta y^2, \Delta z^2)$:
$$\Delta s'^2 = \Sigma_{\alpha,\beta = 3}^3 \hspace{0.1cm} M_{\alpha,\beta} \hspace{0.1cm} \Delta x^2_\alpha \Delta x^2_\beta$$
where $M_{\alpha,\beta}$ could depend on the relative velocity of the two frames.
- By expanding the above equation, we find only the sum appears, so $M_{\alpha,\beta}$ =  $M_{\beta,\alpha}$
- For a light beam, $\Delta s^{2}= 0$, so $\Delta t = \Delta r$. Hence, $$\Delta s'^{2}= M_{00} \Delta r^{2} + 2 \Sigma_{i=1}^{3} M_{0i}\Delta x^{i}\Delta r + \Sigma_{i,j=1}^{3} M_{i,j} \Delta x^{i} \Delta x^j$$
-  Under the transformation $\Delta x \rightarrow - \Delta x$, $\Delta s'^{2}= 0$ should remain invariant as it will still be events on the light beam that are considered (interval between events $a,b$ = interval between events $b,a$. This implies $M_{0,i} = 0$ since that's the only term that changes ($\Delta x$ changes sign, while $\Delta r=\sqrt{\Delta x^{2}+\Delta y^{2}+\Delta z^2}$ does not).
- Now, since the first and third term must cancel each other out, $-M_{00}= M_{ij}\delta^{ij}$
- Hence, generally (for all intervals, not just light), $$\Delta s^{2}= M_{00}(-\Delta t^{2}+\Delta x^{2}+\Delta y^{2}+ \Delta z^2)$$
- However, we haven't shown that $M_{00}$ is independent of the two observers, so let $M_{00} = \phi (v)$ 
- We have shown that the universality of the speed of light shows that for any two observers, $\Delta s^{2}=\phi (v) \Delta s'^2$

- Now we show that $\phi (v)$ can depend at most only on $|v|$:
	- let a rod be lying on the $y$-axis of the $O$'s frame. It's ends has $\Delta y$ as the only non-zero coordinate, hence it defines simultaneous events in $O$'s frame. Let $O'$ move in the $x$ direction relative to $O$, so that its word line lies in the $t-x$ plane, perpendicular to the events $A, B$ that define the ends of the rod. In $O'$ frame, pick out a clock that lies on the midpoint of the rod at t=0. Let the clock emit light rays before t = 0, at such a time that they (eventually) reach the events $A, B$. Since the distances and the speed of light for the two rays are equal, they will reach the two events simultaneously and be reflected and reach back the clock at the same instant. Reaching at the same instant means the two events of reflection we simultaneous as the clock being perpendicular to the rod means the two light rays cover the same distance and, they have the same speed. Hence, the two events A, B are simultaneous in $O'$ frame too, and so the interval there too has not time interval and so just equals the length of the rod, and so the equations for intervals just becomes an equation for lengths:
	$$(length\ of \ rod \ in \ O' \ frame )^{2}= \phi (v)(Length \ of \ rod \ in \ O \ frame)^2$$
	  But since the rod is perpendicular to the direction of velocity $v$, and only relative motion is of any significance (principle of relativity), then it doesn't matter which direction the velocity is in as long as its perpendicular (imagine running towards a rod such that its length is perpendicular to your velocity. now, as only relative motion counts, running towards the rod horizontally or from the above is equivalent). Hence, $$\phi (v) = \phi (|v|)$$
- Now, we show that $\phi (|v|) = 1$. Between any two events:
	- $\Delta s'^{2}= \phi (|v|)\Delta s^2$, $\Delta s^{2}= \phi(|v|)\Delta s'^2$ $\rightarrow$ $\Delta s'^{2}= (\phi(|v|))^{2} \Delta s'^2$ $\rightarrow \phi(|v|) = 1$

- Hence, the interval between any two events is the same when calculated by an inertial observer: $$\Delta s^{2}= \Delta s'^2$$
- Also, (we have shown that) the length of the rod is the same as measured by two inertial observers when it is oriented perpendicular to the relative velocity between the two.
- And, any two events that are simultaneous in one frame are simultaneous in another frame too if the other frame is moving perpendicular to the separation of the two events in the first frame.
- Since $\Delta s^{2}$ is independent of observers, it is a property of events itself, and can thus be used to classify them: 
	- If $\Delta s^{2} > 0$, then the events are spacelike separated, if $\Delta s^{2} < 0$, then the events are timelike separated, if $\Delta s^{2} = 0$, then the events are lightlike separated.
	- The events that are lightlike separated lie on a cone whose apex is one of the events. All events within the lightcone are timelike separated, while those outside are spacelike separated.
	- The events inside the forward lightcone of an event $A$ are called the absolute future of $A$, those in the backward lightcone are called the absolute past of $A$, those outside of it are called absolute elsewhere of $A$.
	- In SR, spacetime has three invariant divisions: s
	- 
	- Since the interval between any two events in invariant, it will be either spacelike, timelike, or lightlike for all observers. Hence, for an event $A$, all observers agree about what events are spacelike, timelike, or lightlike and hence agree about its absolute future, absolute past, absolute elsewhere.
	- Each different event has a different future, past, elsewhere although they can overlap.

### 1.7 Invariant Hyperbolae

- The curves $-t^{2}+ x^{2}= a^2$ is a hyperbola in the spacetime diagram of $O$. However, since it has the form of a spacetime interval, it represents all events whose spacetime interval with the origin is $a^2$ (since 1 event is the origin, we have $\Delta t=t$ and so on). By invariance, in the $O'$ frame, these same events have the same separation $a^2$ from the origin in $O'$ frame (since the origins coincide), so they lie on the curve $-t'^{2}+x'^{2}= a^2$. These are both spacelike Hyperbolae. The Hyperbolae $-t^{2}+ x^{2}= -b^2$ and $-t'^{2}+x'^{2}= -b^2$ are timelike.
- These Hyperbolae are asymptotic to the lines with $slope =_{+-}1$ which are light paths, since the timelike hyperbolae are valid for all events that are separated timelike from the origin and so lie inside the lightcone while the spacelike hyperbolae lie outside the lightcone.
- Calibration:
	- Consider a timelike hyperbola, it must intersect the $t$ axis at some point and also the $t'$ axis at some point, as points whose separation from the origin are timelike exist on both the axis. Consider the hyperbola $-t^{2}+ x^{2}= -1$. An event on the $t$ axis has $x = 0$, so $t = 1$. Where it intersects the $t'$ axis, $t' = 1$. 
	- The corresponding $t$ value for the event whose coordinates in $O'$ frame are $t' = 1$, $x'=0$, can be found by the intersection of the worldline for $O'$, the $t'$ axis (intersect $t=vx$ which is the $t'$ axis in $O$ with the hyperbola) and the invariant hyperbola, hence $t'$ can be calibrated. For this case, the value of $t$ is $t = \frac{1}{(1-v^2)^{\frac{1}{2}}}$. More generally, this gives the Lorentz transformation for $t$.
	- Similarly, considering spacelike hyperbolae lead to the calibration of the spatial axis.
- Since the only constraint is for the spacetime interval to be conserved, as long as it is, as is the case for the points on the invariant hyperbolae, the events can be shifted anywhere by choosing the appropriate Lorentz transformation, such as on the invariant hyperbolae.
- Space (section of spacetime at constant $t$ value) is Euclidean as posited by everyday experience, for which the normal Euclidean metric holds ($\Delta s^{2}=\Delta r^{2} +k$). In SR, the difference is, time must be considered in computations of distance.
- .....

### 1.8 Particularly Important Results

#### Time Dilation
 - The above Lorentz transformation equation for time can be considered as an interval transformation equation if the other event is taken to be the origin in the respective frames. The result holds for more general intervals too. $$\Delta t_{\ measured\ in\ O} =\frac{\Delta t'_{\ measured\ in\ O'}}{(1-v^{2)^{\frac{1}{2}}}}$$
 - For an event that's on the worldline of a clock on the origin, like the event B, $\Delta t'$ is measured by the same clock, but in frame O, $\Delta t$ is measured by two different clocks, one at the origin and one at the event B.
 - The proper time between two events is the time clicked off by a clock that passes through both the events. Let the clock be at rest in frame $O'$ so that the proper time is the same as the coordinate time. Then,$\Delta x = \Delta y = \Delta z = 0$, and so $$\Delta s^{2}= -\Delta t^{2}= -\Delta \tau^2$$
 - Since the interval between any two events is the same in all frames, this is an invariant recipe for defining/calculating proper time. In any frame, the negative of the square root of the interval gives the invariant proper time. By an observer in frame O, the proper time between any two events (or on a worldline) can be calculated as follows:
	 -  Negative of the square root of the interval: $\Delta \tau = -\Delta s^2 = (\Delta t^2 - \Delta x^2 - \Delta y^2 - \Delta z^2)^\frac{1}{2}$
	 - Upon dividing any multiplying by $\Delta t$: $$\Delta \tau = \Delta t (1-v^2)^\frac{1}{2}$$
- This equation holds for any frame. It could be interpreted as an expression for time dilation between any two events (or a worldline) in any frame other than the rest frame.

#### Length Contraction
- Consider a rod at rest in frame $O'$  with it's ends at the events $A: t'=0, x'=0$, and at $L: t'= 0, x'= l$. Since $\Delta t' = 0$, $\Delta s$ just becomes the usual Euclidean metric and hence equals the length of the rod: $L = \Delta s_{AL}$. Note that this is not a definition; this equation holds for a spacetime separation evaluated at constant $t'$.
- However, a similar equation holds for the length of the rod in frame $O$. Since length is a measurement of the spatial increment between two events at an instant of time, the length in frame $O$ can be found similarly:
	- Choosing the instant of $t = 0$ to make our length measurement in the frame $O$, we know the start of the rod lays at the event $A: t= 0,x = 0$, since the two frames align at $t = t' = 0$. Hence, the length of the rod in the frame $O$ will be the spatial increment at $t=0$ between the two events $A$ and $B$(corresponding to the end of the rod in frame $O$, both on the $x-axis$.
	- Since we know the $x'$ coordinate of the end of the rod, we can use an invariant hyperbola to find it's $x$ coordinate. 
	- *note:* we can do this since the (full) spacetime interval for the ends of the rod remains invariant. All we do is make an invariant Hyperbola for the spacetime interval of the rod (between the events that are its ends). Then we find it's coordinates in different frames.
	- In the frame $O'$, consider the hyperbola $-t'^{2}+x'^{2}= L^2$. Where this line intersects the x-axis gives the $x$ coordinate for the end of the rod in frame $O$: $x_{L}= (\frac{L}{(1-v^{2)^{\frac{1}{2}}}})$ 
	- .....

