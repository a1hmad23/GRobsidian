
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
- In general, $g_{\alpha \beta}$ will be a complicated functions of position, so the relation between, say, $V^{0}$ and $V_{0}$ might not be simple in an arbitrary coordinate system.
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

- By definition, differentiation is done through considering vectors at two distinct points (albeit they are infinitesimally close together). This notion might not be clear in a curved manifold, since the space might be curves between the two vectors and so the idea of the vectors pointing in the same direction is fuzzy. However, the local flatness of the Riemannian manifold helps us out. In the limit that is considered in the derivative of the vectors being close together, the space can be considered flat, and so vectors can point in the same direction, with their components being constant in this coordinate system, have there derivatives 0. That is, the derivatives of the basis vectors of the locally inertial coordinate system are 0 at $P$.
- This is a definition of the covariant derivative. Its justification lies in the physical fact in a locally inertial frame everything is like in SR, and in SR the derivatives of basis vectors are 0.
- Hence, the Christoffel symbols vanish, and the covariant derivatives has components equal to the partial derivative of the components: $V^{\alpha}_{;\beta}=V^{\alpha}_{,\beta}$ at $P$ in this frame.
- This is also true for the metric: $g_{\alpha \beta;\gamma}=g_{\alpha \beta,\gamma}=0$  at $P$. This is the equality in the local flatness theorem. Now, this is a tensor equation, and so must be true generally for any coordinates.
- Hence, if we have the symmetry of the Christoffel symbols, this will lead to the equation giving the Christoffel symbols in terms of the metric and its derivatives.
- Note that the derivative of the Christoffel symbols would depend on the second derivative of the metric, which means the derivatives of the Christoffel symbols are non zero. This implies that although we can find a coordinate system where the Christoffel symbols vanish at some point $P$, these symbols do not vanish everywhere in that coordinate system.
- This differs from flat space where such a coordinate system does exist. Hence, the difference between flat space and a curved manifold manifests itself in the Christoffel symbols.
- The equation for the Christoffel symbols in terms of the metric means that given the metric, one can calculate all covariant derivatives, since they depend only on the Christoffel symbols.