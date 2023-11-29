
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
- Using one forms and vectors, we can defines a whole set of tensors of any rank. Without the metric though, there is yet no correspondence. All of this comes from differentiability, so the set of all tensors are said to be part of the differential structure of the manifold.

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
- Since we have to study general curved manifolds, and a general curved coordinate system might have any coordinate system, we allow for any coordinate system.
- In SR we studies Lorenz frames because they were simple. With gravity, since they are not allowed, we have to allow all coordinates, and thus all coordinate transformations that are non singular.
- The metric tensor is symmetric (by definition: inherits the symmetry of the scalar product). It is a theorem of matrix algebra that for a symmetric matrix, we can always find a transformation matrix such that the symmetric matrix becomes diagonal with +1,0, and -1 values only. The number of positive or negative values depend on the number of positive and negative eigenvalues. Since we choose there to be 1 negative eigenvalue and 3 positive eigenvalues, we have that, for some transformation matrix $\Lambda^{\alpha'}_{\beta}$, $$g_{\alpha' \beta'}=\begin{pmatrix}-1 &0&0&0\\0&1&0&0 \\ 0&0&1&0 \\ 0&0&0&1 \end{pmatrix}=\eta_{\alpha \beta}$$
- $\eta_{\alpha \beta}$ will denote only this metric-the metric of SR.
- This relied on choosing **g** to have the appropriate eigenvalues. The trace is called the signature of the metric, for SR and GR it is +2.
- This metric of SR was obtained here by a transformation at a point, hence the physical argument that it is always possible to construct a local inertial frame finds its mathematical grounding here: at a point we can obtain $\eta_{\alpha \beta}$  This in turn implies that the metric has to have +2 signature if it is to describe spacetime with gravity, since only then can we obtain the metric for SR.
- Moreover, the transformation matrix that produces this might not be a coordinate transformation...
- Having found a basis at some point $P$ for which the metric is $\eta$ , it is possible to find coordinates such that, in the neighborhood of $P$, the metric is nearly $\eta$  This is embodied in the theorem that having chosen a point $P$ of the manifold, a coordinate system {$x^{\alpha}$} can be found whose origin is at $P$ and in which $g_{\alpha \beta}(x^{\mu})=\eta_{\alpha \beta}+0[(x^{\mu})^{2}]$
- So the metric is nearly that of SR, the differences being second order in the coordinates. Such coordinate systems are referred to as local Lorentz frames.
- The above theorem can be put another way:
	- $g_{\alpha \beta}(P)=\eta_{\alpha \beta}$ for all $al$
	- 