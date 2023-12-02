
### 6.1 Differentiable Manifolds And Tensors

- The mathematical concept of a curved space begins with the idea of a manifold- a continuous space that locally looks Euclidean. To the concept of a manifold is added the idea of curvature itself.

*Manifolds*
- Basically, a manifold is any set that can be continuously parametrized. The number of independent parameters is the dimension of the manifold and the parameters are coordinates of the manifold.
- The surface of a sphere is parametrized by $\theta$ and $\phi$. The $m$ dimensional hyperplane has $m$ cartesian coordinates. The set of all rotations in a 3D Euclidean space is a manifold: two parameters describe the direction of rotation, and one describes the amount of rotation- it is a 3d manifold. Notice that the parametrization is indeed continuous. Each point is a rotation, and its coordinates are the three parameters.
- Mathematically, the association of points with the values of their parameters can be thought of as a mapping of points of a manifold into Euclidean space of the correct dimension. This is the meaning that a manifold looks locally Euclidean: it is smooth and has a certain number of dimensions. 
- The large scale topology might still be very different, but locally the correspondence is good: a small patch of the surface of a torus can be mapped onto the plane tangent to it.
- Hence, a manifold is a space with coordinates, that locally looks Euclidean but can globally can warp, bend, and do almost anything that is continuous.

*Differential Structure*
- We consider differentiable manifolds. These spaces are everywhere continuous and differentiable. 
- Roughly, this means that one can define a scalar field $\phi$ at each point of the manifold and be sure that it can be differentiated everywhere.
- This ensures that we can define one-forms and vectors everywhere: in a certain coordinate system on the manifold, the members of the set {$\phi_{,\alpha}$} are the components of the one form $\tilde{d}\phi$ and any set {$a \tilde{d}\phi +b \tilde{d}\psi$} is a one-form field. And that every curve with some parameter $\lambda$ has a tangent vector $\vec{V}$ defined as a function that takes the one form $\tilde{d}\phi$ into the derivative of $\phi$ along the curve, $\frac{d \phi}{d \lambda}$: (linear combinations are again vectors) $$\langle \tilde{d}\phi,\vec{V}\rangle =\vec{V}(\tilde{d}\phi)=\nabla_{V}\phi=\frac{d \phi}{d \lambda}$$
- Using one forms and vectors, we can define a whole set of tensors of any rank. Without the metric though, there is yet no correspondence. All of this comes from differentiability, so the set of all tensors are said to be part of the differential structure of the manifold.

*Review*
![[Pasted image 20231129181501.png]]

### 6.2 Riemannian Manifolds

- In our case the metric is essential since it will carry information about the rates at which clocks run and the distances between points, just as it does in SR.
- A differentiable manifold on which a symmetric $\begin{pmatrix}0\\2\end{pmatrix}$ tensor-field **g** has been singled out to act as a metric at each point is called a Riemannian manifold.
- By picking out a metric, we add structure to the manifold: the metric completely defines the curvature of a manifold. So, different metrics will lead to different curvatures.
- The differentiable manifold itself is primitive: an amorphous (without a clearly defined shape or form) collection of points, arranged locally like the points of Euclidean space, but not having any distance or shape defined. Giving the metric **g** gives it a specific shape.
- Note that it is possible to define the notion of curvature on a manifold without the metric-affine manifolds.

*The Metric And Local Flatness*
- Since the metric provides a mapping between vectors and forms, given a vector field at some point $\vec{V}(P)$, there is a unique one-form field $\tilde{V}(P)$.
- In general, $g_{\alpha \beta}$ will be complicated functions of position, so the relation between, say, $V^{0}$ and $V_{0}$ might not be simple in an arbitrary coordinate system.
- Since we have to study general curved manifolds, and a general curved manifold might have any coordinate system, we allow for any coordinate system.
- In SR we study Lorenz frames because they were simple. With gravity, since they are not allowed, we have to allow all coordinates, and thus all coordinate transformations that are non singular.
- The metric tensor is symmetric (by definition: inherits the symmetry of the scalar product). It is a theorem of matrix algebra that for a symmetric matrix, we can always find a transformation matrix such that the symmetric matrix becomes diagonal with +1,0, and -1 values only. The number of positive or negative values depend on the number of positive and negative eigenvalues. Since we choose there to be 1 negative eigenvalue and 3 positive eigenvalues, we have that, for some transformation matrix $\Lambda^{\alpha'}_{\beta}$, $$g_{\alpha' \beta'}=\begin{pmatrix}-1 &0&0&0\\0&1&0&0 \\ 0&0&1&0 \\ 0&0&0&1 \end{pmatrix}=\eta_{\alpha \beta}$$
- $\eta_{\alpha \beta}$ will denote only this metric-the metric of SR.
- This relied on choosing **g** to have the appropriate eigenvalues. The trace is called the signature of the metric, for SR and GR it is +2.
- This metric of SR was obtained here by a transformation at a point, hence the physical argument that it is always possible to construct a local inertial frame finds its mathematical grounding here: at a point we can obtain $\eta_{\alpha \beta}$  This in turn implies that the metric has to have +2 signature if it is to describe spacetime with gravity, since only then can we obtain the metric for SR.
- Moreover, the transformation matrix that produces this might not be a coordinate transformation...
- Having found a basis at some point $P$ for which the metric is $\eta$ , it is possible to find coordinates such that, in the neighborhood of $P$, the metric is nearly $\eta$  This is embodied in the theorem that having chosen a point $P$ of the manifold, a coordinate system {$x^{\alpha}$} can be found whose origin is at $P$ and in which $g_{\alpha \beta}(x^{\mu})=\eta_{\alpha \beta}+0[(x^{\mu})^{2}]$
- So the metric is nearly that of SR, the differences being second order in the coordinates. Such coordinate systems are referred to as local Lorentz frames.
- The above theorem can be put another way:
	- $g_{\alpha \beta}(P)=\eta_{\alpha \beta}$ for all $\alpha, \ \beta$
	- $\frac{\partial}{\partial x^{\gamma}}g_{\alpha \beta}(P)=0$  here a 2x term will appear which is 0 at the origin- x=0
	- $\frac{\partial^{2}}{\partial x^{\gamma} x^{\mu}}g_{\alpha \beta}(P) \neq 0$  for at least some values of $\alpha, \ \beta, \ \gamma, \ \mu$ if the manifold is not exactly flat. 

- The existence of local Lorenz frames is merely the statement that any curved space has a flat space tangent to it at any point. (that any curved space shares a region-albeit vanishingly small, with a flat space- the one tangent to it at a point).
- Straight lines in flat spacetime are the worldlines of free particles. The absence of first derivative terms mean that the metric doesn't change, the scalar product remain those of flat spacetime and so particles move in straight lines locally in this coordinate system. These coordinate systems are useful since in them the equations of physics will be nearly the same as those in flat spacetime.

*Lengths And Volumes*
- ![[Pasted image 20231129213313.png]]
- ![[Pasted image 20231129213344.png]]
- ![[Pasted image 20231129213400.png]]
- Volume is four dimensional: $dx^{0}dx^{1}dx^{2}dx^{3}$, where {$x^{\alpha}$} are the coordinates that give the nearly Lorenzian metric that was discussed above. From calculus of variations, in any other coordinate system {$x^{\alpha'}$}, we have  ![[Pasted image 20231130182940.png]]
- Where the $\partial$ denotes the Jacobian of the transformation: $\Lambda^{\alpha}_{\beta'}$ 
- In matrix terminology, the transformation of the metric components can be written as: $(g)=\Lambda \eta \Lambda^{T}$. The same relation follows for determinants, and using the fact that transposition does not change the determinant, along with the fact that $det(\eta)=-1$, we have that: $$det(g_{\alpha \beta})=g=-[det(\Lambda)]^{2}$$
- Hence, $det(\Lambda^{\alpha}_{\beta'})=(-g)^{\frac{1}{2}}$ 
- Therefore, $d^{4}x=(-g)^{\frac{1}{2}}d^{4}x'$ 
- The above argument stemmed from the fact that at a point spacetime is same as Minkowski spacetime, and so the volumes must be the same (In flat space the volume is just $d^{4}x$). This was possible by choosing the special coordinates at the point, the coordinates whose origin is at that point and so where the metric can be written as the Minkowski metric plus second order perturbations. Then, by using the general result from calculus of variations, we found an expression for the volume at any point in arbitrary coordinates, which depends on the determinant of the metric.
- The metric of course comes into it since it measures length. The result is that the square-root of the negative of the determinant of the metric is the thing to multiply by $d^{4}x'$ to get the true volume element at any point in any coordinate system.
- As an example, consider the spherical coordinate system for 3D space. From the line element one can deduce the metric, and then find its determinant. Multiply that by $d^{4}x$ for spherical coordinates and get the familiar result for the volume element in spherical coordinates.

*Proof Of The Local Flatness Theorem*

### 6.3 Covariant Differentiation

- By definition, differentiation is done through considering vectors at two distinct points (albeit they are infinitesimally close together). This notion might not be clear in a curved manifold, since the space might be curved between the two vectors and so the idea of vectors pointing in the same direction is fuzzy. However, the local flatness of the Riemannian manifold helps us out. In the limit that is considered in the derivative of the vectors being close together, the space can be considered flat, and so vectors can point in the same direction, with their components being constant in this coordinate system, have there derivatives 0. That is, the derivatives of the basis vectors of the locally inertial coordinate system are 0 at $P$. (presumably, this follows since the derivatives of the components constitute only one term, the other being the derivatives of the basis vectors, which also has to be 0 for the derivative of a vector to be 0).
- This is a definition of the covariant derivative. Its justification lies in the physical fact that in a locally inertial frame everything is like in SR, and in SR the derivatives of basis vectors are 0.
- Hence, the Christoffel symbols vanish, and the covariant derivatives has components equal to the partial derivative of the components: $V^{\alpha}_{;\beta}=V^{\alpha}_{,\beta}$ at $P$ in this frame.
- This is also true for the metric: $g_{\alpha \beta;\gamma}=g_{\alpha \beta,\gamma}=0$  at $P$. This is the equality in the local flatness theorem. Now, this is a tensor equation, and so must be true generally for any coordinates.
- Hence, if we have the symmetry of the Christoffel symbols, this will lead to the equation giving the Christoffel symbols in terms of the metric and its derivatives. (we do indeed have the symmetry of the Christoffel symbols-exercise)
- Note that the derivative of the Christoffel symbols would depend on the second derivative of the metric, which means the derivatives of the Christoffel symbols are non zero. This implies that although we can find a coordinate system where the Christoffel symbols vanish at some point $P$, these symbols do not vanish everywhere in that coordinate system.
- This differs from flat space where such a coordinate system does exist. Hence, the difference between flat space and a curved manifold manifests itself in the Christoffel symbols.
- The equation for the Christoffel symbols in terms of the metric means that given the metric, one can calculate all covariant derivatives, since they depend only on the Christoffel symbols. $\Gamma^{\alpha}_{\mu \nu}=\frac{1}{2} g^{\alpha \beta} (g_{\beta \mu,\nu}+g_{\beta \nu,\mu}-g_{\mu \nu,\beta})$.

*Divergence Formula*

### 6.4 Parallel-Transport, Geodesics, and Curvature

- Until now, we have used the local flatness theorem to develop as much mathematics as possible without considering curvature explicitly.
- There are 2 kinds of curvature: Intrinsic and extrinsic.
- Extrinsic curvature:
	- For a cylinder, it would be be the curvature it has in relation to the flat three dimensional space it is a part of.
	- Extrinsic curvature comes from considering a manifold as embedded in a space of higher dimensions.
	- Can be investigated by asking about lines that stay in the surface compared to straight lines that go off it.
- Intrinsic Curvature:
	- A cylinder can be made rolling a piece of paper, so intrinsically its geometry is flat.
	- Distance between points on the original paper remain the same on the cylinder.
	- Parallel straight lines remain so, so Euclid's parallelism axioms holds. In fact, all of Euclid's axioms hold for the surface of a cylinder.
	- A two dimensional ant would decide it was flat, only its global topology is funny, in that going in a straight line brings him back to where he was.

- Since we can only penetrate spacetime intrinsically- we cannot view it as embedded in higher dimensional space- all the worldlines stay in spacetime, we only talk about intrinsic curvature of spacetime.
- A Sphere has an intrinsically curved surface:
	- Lines that start parallel do not remain so, in fact they intersect. These are the great circles of a sphere, whose segments are the shortest routes between two points, as it is these only that stick to the surface- they only obey the curvature of the sphere and not add any of their own, they do not stray from their path.
	- In parallel transport on a sphere, the reason for not staying parallel is because you still have to obey the curvature of the sphere: you have to parallel transport as a 2D being walking on the sphere. With each new parallel vector added, the intrinsic curvature of the sphere somewhat modifies the vector.
	- Upon returning, the vector are found to have not stayed parallel. Since this does not happen in a flat space, this must be an effect due to the curvature of the sphere.
	- If you imagine a small circle, each parallel straight line must end at the north pole when extended, hence they curve to the direction of the north pole.

- The result of parallel transport between vectors depends on the path taken. Therefore, we cannot assert that two vectors are the same or parallel. Hence, on a curved manifold, it isn't possible to define globally parallel vector fields. Local parallelism can still be defined, a vector can be kept parallel and of the same length from one point to the next.

*Parallel Transport*
- Suppose a vector field $\vec{V}$ is defined on the sphere, and we examine how it changes along a curve. If the vectors at infinitesimally close points of the curve are parallel and of equal length, then the vector is said to be parallel-transported along the curve.
- If $\vec{U}=\frac{d \vec{x}}{d \lambda}$ is the tangent to the curve (not necessarily normalized), then in a locally inertial coordinate system at $P$, the components of $\vec{V}$ must be constant along the curve at $P$: (since the vectors dont change when the are infinitesimally close to each other and they are on the curve) $\frac{dV^{\alpha}}{d \lambda}=0$ at $P$
- Now, each of the components defines a scalar field on the curve, and we know that the derivative of a scalar field along a curve can be written in terms of the scalar product between the derivatives of the scalar field (with the coordinates) and the (vectors tangent to it: usually the 4-velocity), or $\frac{dV^{\alpha}}{d \lambda}= \frac{dx^{\beta}}{d \lambda} \frac{\partial V^{\alpha}}{\partial x^{\beta}}= U^{\beta} V^{\alpha}_{,\beta}=U^{\beta} V^{\alpha}_{;\beta}=0$   at $P$, where the 2nd last equality follows from using the locally flat coordinate system, where the Christoffel symbols are 0.
- The last equality is a tensor equation, the LHS has a permissible tensor operation: contraction between tensor components, those of the covariant derivative and a 4-vector.
- Hence, we have a frame invariant definition of the parallel transport of $\vec{V}$ along $\vec{U}$ (how $\vec{V}$ changes as it is transported along the curve, imagine they are sufficiently close enough so that they are in the local Lorenz frame, so that the first derivative of the metric is 0 and the Christoffel symbols vanish and the covariant derivative reduce to the normal derivative, and so the derivative of the components are 0 and so the components are help constant as the vector is slides from one point to another (transported)): $$U^{\beta} V^{\alpha}_{;\beta}=0 \iff \frac{d}{d\lambda}\vec{V}=0=\nabla_\vec{U}$$
*Geodesics*
- By a straight line, Euclid means to keep on going in the direction it has been going. More precisely, the tangent to the curve at a point is parallel to the tangent to the curve at the next point.
- In Euclidean space, a straight line is the only curve that parallel transports its own tangent vector. In a curved space, we can draw lines that are as straight as possible by demanding parallel transport of the tangent vector. By demanding that the tangent vector doesn't change, we enforce that the curve doesn't stray more than is necessary- that is to only stray to account for the curvature of the manifold.( moving straight in a curved spacetime means to take the tangent to a worldline-the 4 velocity, and move it parallel to itself ) These are called geodesics: $$\vec{U}\ is\ tangent\ to \ a\ geodesis \iff \nabla_\vec{U}\vec{U}=0$$
- In a locally inertial coordinate system, these are straight lines.
- In component notation: $$U^{\beta}U^{\alpha}_{;\beta}=U^{\beta}U^{\alpha}_{,\beta} + \Gamma^{\alpha}_{\mu \beta}U^{\mu}U^{\beta}=0$$Here, $U^{\alpha}=\frac{dx^{\alpha}}{d \lambda}$ so $U^{\alpha} \frac{\partial}{\partial x^{\beta}}= \frac{d}{d \lambda }$ and we get
- ![[Pasted image 20231203004702.png]]
- This is a second order differential equation for $x^{\alpha}(\lambda)$  with a unique solution for when the initial position and the initial velocity are given. The solution is a geodesic.


### 6.5 The Curvature Tensor


