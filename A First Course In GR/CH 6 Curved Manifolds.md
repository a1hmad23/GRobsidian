
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

