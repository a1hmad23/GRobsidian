### 3.1 The Metric Tensor

- Consider the representation of two vectors $A$ and $B$ in some frame $O$: $A=A^{\alpha}e_{\alpha}, B=B^{\beta}e_{\beta}$. Their scalar product in any frame can be found from these representations: $A\cdot B = (A^{\alpha}e_{\alpha})\cdot (B^{\beta}e_{\beta})$. Different indices are used to distinguish between the two sums.
- $\rightarrow A^{\alpha}B^{\beta}(e_{\alpha}\cdot e_{\beta}) = A^{\alpha}B^{\beta}\eta_{\alpha \beta}$ which is a frame invariant way of writing the invariant scalar product $-A^{0}B^{0}+A^{1}B^{1}+A^{2}B^{2}+A^{3}B^{3}$.
- The numbers $\eta_{\alpha \beta}$ are the components of the metric tensor (in the same frame as the one in which the components of the vectors are measured). Here, they give a rule for associating with two vectors a real number (their scalar product). This leads to the definition of tensors.

### 3.2 Definition Of Tensors

- A Tensor of type $\begin{pmatrix}0 \\ N\end{pmatrix}$ is a function of $N$ vectors into real numbers, which is linear in each of its $N$ arguments.
- The scalar product satisfies the condition for $\begin{pmatrix}0\\ 2\end{pmatrix}$ tensor.
- Linearity in the first argument means $(\alpha A\cdot B) = \alpha (A\cdot B)$ and $(A+B)\cdot C = A\cdot C +B\cdot C$.
- Let $g$ be the metric tensor. Then, $g(A,B)=A\cdot B$ and it is linear so that $g(\alpha A +\beta B, C) = \alpha g(A,C) +\beta g(B,C)$ 
- It is apparent that a tensor is a function of the vector themselves, and not their components, so that it returns the same real numbers for vectors represented in any frame.
- The components of a tensor in a frame $O$ are defined as the values it takes on input of the basis vectors of that frame. For the metric tensor, in a frame $O$ with basis vectors {$e_{\alpha}$}, the components are $g(e_\alpha,e_{\beta)}= e_{\alpha}\cdot e_{\beta} = \eta_{\alpha \beta}$ 

### 3.3 The $\begin{pmatrix}0\\ 1\end{pmatrix}$ Tensors: One-Forms

- Let $\tilde{p}$ be a one-form. Then, for a vector $A$, $\tilde{p}(A)$ is a real number. 
- Let $\tilde{q}$ be another one-form. Then, we define $\tilde{s}$ to be the one-form $\tilde{s} = \tilde{p}+\tilde{q}$ and $\tilde{r} = \alpha \tilde{p}$. For a vector argument $\vec{A}$, $\tilde{s}(\vec{A}) = \tilde{p}(\vec{A})+\tilde{q}(\vec{A})$ and $\tilde{r}(\vec{A})=\alpha \tilde{p}(\vec{A})$.
- With these definitions, the set of all vectors satisfy the axioms for a vector space. To distinguish it from the ordinary vector space, it's called the dual vector space.
- Since $\tilde{p}$ is a tensor, its components in some frame are $p_\alpha\equiv \tilde{p}(\vec{e_{\alpha}})$  
- By convention, a single lower index denotes a one-form component, while a single upper index denotes the component of a vector.
- $\tilde{p}(\vec{A}) = \tilde{p}(A^{\alpha}\vec{e_{\alpha}}) = A^{\alpha}p_\alpha$  (in terms of components). So the real number $\tilde{p}(\vec{A})$ is found to be $A^{0}p_{0}+A^{1}p_{1}+A^{2}p_{2}+A^{3}p_{3}$ , which is a contraction of $\tilde{p}$ and $\vec{A}$ (notice all the plus signs).
- The contraction is more fundamental in tensor analysis than the scalar product since it can be performed without reference to a third object.
- Components of a one-form in a basis {$\vec{e_{\beta'}}$}: $\tilde{p}(\vec{e_{\beta'}}) = \tilde{p}(\Lambda^{\alpha}_{\beta'}\vec{e_{\alpha}}) = \Lambda^{\alpha}_{\beta'} \tilde{p}(\vec{e_{\alpha}}) = \Lambda^{\alpha}_{\beta'}p_{\alpha}$ 
- The above transformation rule for 1-form components from one frame to another is the same as the transformation rule for basis vectors, and the opposite(inverse) for vector components. Hence, the contraction between one-form components and vector components is guaranteed to be frame invariant- they cancel each others transformation out: $A^{\alpha'}p_{\alpha'} = \Lambda^{\alpha'}_{\beta}A^{\beta}\Lambda^{\mu}_{\alpha'}p_{\mu} = \Lambda^{\alpha'}_{\beta}\Lambda^{\mu}_{\alpha'}A^{\beta}p_{\mu} =\delta^{\mu}_{\beta}A^{\beta}p_{\mu}=A^{\beta}p_{\beta}$  the first and the last expressions denote the same sum and hence are the same, so contractions in any frame are the same, albeit with different components (of the same geometrical quantities).

*Basis One-Forms*
- Since the set of all 1-forms is a vector space, any set of 4 linearly independent 1-forms can be a basis. In analogy to vectors, we want a set {$\tilde{\omega}^\alpha$} such that $\tilde{p} = p_{\alpha}\tilde{\omega}^{\alpha}$.
- Just like vectors, one-forms too are invariant geometrical quantities independent of their components and basis, which are just a representation in some frame $O$. Hence the contraction between the components $p_{\alpha}$ and the basis $\tilde{\omega}^{\alpha}$.
- To find the basis one-forms, we use the fact that for any vector $\vec{A}$, we have $\tilde{p}(\vec{A}) =p_{\alpha}A^{\alpha}$. Hence, $$\tilde{p}(\vec{A}) =p_{\alpha}A^{\alpha}=p_{\alpha}\tilde{\omega}^{\alpha}(\vec{A}) =p_{\alpha}\tilde{\omega}^{\alpha}(A^{\beta}\vec{e}_{\beta})=p_{\alpha}A^{\beta}\tilde{\omega}^{\alpha}(\vec{e_{\beta}})$$   which implies $$\tilde{\omega}^{\alpha}(\vec{e}_{\beta})=\delta^{\alpha}_{\beta}$$
- Since this equation gives the $\beta th$ component of the $\alpha th$ basis one-form, it defines the one-form basis. The components of a one-form basis are $(1,0,0,0), (0,1,0,0),(0,0,1,0),(0,0,0,1)$.
- The result $\tilde{\omega}^{\alpha}(\vec{e}_{\beta})=\delta^{\alpha}_{\beta}$ implies that a one-form basis acts on a vector in such a way that the $\alpha th$ one-form basis acting on a vector picks out the $\alpha th$ component of the vector in that frame: $\tilde{\omega}^{\alpha}(\vec{A})= \tilde{\omega}^{\alpha}(A^{\beta}\vec{e_{\beta}}) =A^{\beta}\tilde{\omega}^{\alpha}(\vec{e}_{\beta})=A^{\beta}\delta^{\alpha}_{\beta}=A^{\alpha}$. Note that in a different frame, although the components of the vector would change, but so would the one-form basis.
- By virtue of the above result, it is clear that the equation $\tilde{\omega}^{\alpha}(\vec{e}_{\beta})=\delta^{\alpha}_{\beta}$ signifies a relation between the sets {$\tilde{\omega}^{\alpha}$} and {$\vec{e}_{\beta}$}, rather then of individual pairs, since for example, changing the $\vec{e}_1$ basis vector would change the component in the direction of $\vec{e}_{2}$, and the same one-form basis $\tilde{\omega}^{2}$ acting on the same invariant vector would return a different result, which would not have been the case if $\tilde{\omega}^2$ was just related to $\vec{e}_{2}$, since $\vec{e}_{2}$ was left unchanged but $\tilde{\omega}^{2}$ changed.
- Components alone are insufficient to describe a geometrical quantity. Given a set of components, for a complete description, it is necessary to further specify if the the components are those of a vector or a one-form, and further specify the basis being used.
- The derivation for the transformation rule of one-form basis is analogous to those of the basis, and leads to the only equation that can be written down with the indices in their correct position: (same as components of a vector and opposite to one-form components and hence opposite to vector basis)
- $$\tilde{\omega}^{\alpha'}=\Lambda^{\alpha'}_{\beta}\tilde{\omega}^{\beta}$$
*Picture of a One-Form* 
- A series of surfaces that slices space. Contraction is the number of surfaces a vector pierces when drawn in space that the one-form has sliced.
- Does not define a unique direction in space, since it is not a vector. Rather, it defines a way of slicing space

*Derivative of a Function is a One-Form*
- Consider a scalar field $\phi (\vec{x})$ defined at every event $\vec{x}$ (in spacetime) and a some particle in spacetime. The worldline of this particle encounters a value of the scalar field at every event.
- The worldline can be parametrized by proper time $\tau$ (value of a clock moving on the line or the value of $-\sqrt{\Delta s^2}$ from some vantage point), through which the coordinates of events on the curve can be expressed as functions of $\tau$: $(t= t(\tau),x=x(\tau),y=y(\tau),z=z(\tau))$.
- The 4-velocity has components $\vec{U} =(\frac{dt}{d \tau}, \frac{dx}{d \tau}, \frac{dy}{d \tau}, \frac{dz}{ d \tau})$.
- Since $\phi$ is a function of $(t,x,y,x)$, which on the curve are functions of $\tau$, so $\phi$ is implicitly a function of $\tau$ on the curve: $\phi=\phi [t(\tau),x(\tau),y(\tau),z(\tau)]$ . Its rate of change on the curve is then: $$\frac{d \phi}{d \tau}=\frac{d\phi}{dt} \frac{dt}{d \tau} + \frac{d\phi}{dx} \frac{dx}{d \tau} +\frac{d\phi}{dy} \frac{dy}{d \tau} + \frac{d\phi}{dz} \frac{dz}{d \tau}\ \ =\ \ \frac{d\phi}{dt} U^{t} +\frac{d\phi}{dx} U^{x} +\frac{d\phi}{dy} U^{y} + \frac{d\phi}{dz} U^z$$
- In the last equation, it is clear that we have devised a means of producing from the vector $\vec{U}$ the number $\frac{d\phi}{d \tau}$ that represents the rate of change of $\phi$ on a curve on which $\vec{U}$ is tangent. Moreover, it clearly is a linear function of $\vec{U}$ ($\alpha$ can be taken common from the 4 terms, $U_{1} +U_{2}$ will lead to $U_{1}^{t}+U_{2}^t$ which can be distributed to $\frac{d\phi}{dt}$). Hence, we have defined a One-Form.
- By comparison with a generic contraction, we find from the above that the One-Form has components: $(\frac{d\phi}{dt},\ \frac{d\phi}{dx},\ \frac{d\phi}{dy}, \frac{d\phi}{dz})$. Hence, $$\tilde{d} \phi \rightarrow_{O} (\frac{d\phi}{dt},\ \frac{d\phi}{dx},\ \frac{d\phi}{dy}, \frac{d\phi}{dz})$$
are the gradient One-Form's components in some frame $O$.

![[Screenshot (16).png]]
- The Gradient enables us to justify our picture of 1-forms:
	- If h is the elevation, then the gradient $\tilde{d}h$ is clearly larger at A than B, where lines are spaced further apart. To find the elevation $\Delta h$ between two points, draw a vector and count the number of contours it passes, which is just the contraction of $\Delta h$ with $\Delta \vec{x}$: $\Sigma_{i} \frac{\partial{h}}{ \partial{x^{i}}} \Delta x^i$ (the value of $\tilde{d}h$ on $\Delta \vec{x}$).
	- Like a vector, a one-form's surfaces are straight and parallel and they are defined over a point: tangent one-forms in the same sense as tangent vectors.
	- In general, one cannot call the gradient a vector as the only plausible definition for a vector gradient would be a vector pointing up the slope such that it crosses the greatest number of contours per *unit length*, which requires a notion of distance and hence a metric. Geometrically, on its own (without the metric), the gradient is a one-form.
	- To check that the definition of the gradient being a one-form is a consistent one, the gradient's components that we found above (the partial derivatives) must transform like 1-form's components, that is, $(\tilde{d} \phi)_{\alpha'} = \Lambda^{\beta}_{\alpha'}\ (\tilde{d} \phi)_{\beta}$ :
		- $$\frac{\partial{\phi}}{ \partial{x^{\alpha'}}}=\frac{\partial{\phi}}{ \partial{x^{\beta}}} \frac{\partial{x^{\beta}}}{{\partial{x^{\alpha'}}}}  \rightarrow (\tilde{d}\phi)_{\alpha'}=\frac{\partial{x^{\beta}}}{{\partial{x^{\alpha'}}}} (\tilde{d}\phi)_{\beta}$$
		- Since the coordinates transform like $x^{\beta}= \Lambda^{\beta}_{\alpha'} x^{\alpha'}$, and $\Lambda^{\beta}_{\alpha'}$ are just constants (for 2 fixed frames), we can divide by $x^{\alpha'}$ and take the limit: $$\frac{\partial{x^{\beta}}}{{\partial{x^{\alpha'}}}} =\Lambda^{\beta}_{\alpha'}$$
		to get this identity.
		- Hence, the components of the gradient transform according to the inverse of the coordinates, (primed in terms of unprimed, with primed index being the lower one on Lambda). The gradient is the archetypal one-form.
