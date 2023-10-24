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

*Notation for Derivatives*
- $\frac{\partial{\phi}}{ \partial{x}} \equiv \phi_{.x}$ 
-  $\frac{\partial{\phi}}{ \partial{x^\alpha}} \equiv \phi_{,\alpha}$ 
- To be consistent with the transformation properties, the superscript in the denominator is a subscript.
- $x^{\alpha}_{,\beta} = \delta^{\alpha}_{\beta}$ 
- Since the components of a vector are just scalars, the set of all $\alpha th$ components of a vector field is a scalar field. Hence, their gradient can be taken, which would be a one-form as we showed for a general scalar field: $\frac{\partial{x^{\alpha}}}{ \partial{x^{\beta}}} \equiv \tilde{d}x^{\alpha} \equiv x^{\alpha}_{,\beta} = \delta^{\alpha}_{\beta} \rightarrow$ $\tilde{d}x^{\alpha} \equiv \delta^{\alpha}_{\beta} \rightarrow$
$$\tilde{d}x^{\alpha} \equiv \tilde{\omega}^{\alpha}$$
- This result shows that the basis one-form is just $\tilde{d}x^{\alpha}$ ,the gradient of the coordinates.
- For any function $f$, we know the components of the gradient One-Form are $\frac{\partial{f}}{ \partial{x^{\alpha}}}$. If we couple this with a one-form basis, we will get the complete One-Form. We found that the basis One-Forms are equivalent to the gradient One-Form of the coordinates, hence: $$\tilde{d}f = \frac{\partial{f}}{ \partial{x}} \tilde{d}x^{\alpha}$$
- Although the notation has been chosen partly to suggest the physicists sloppy way of writing differentials, it is one-forms (tensors) instead that are present in the above equation. Tensors can have small value if acted on infinitesimal vectors.

*Normal One-Forms* 
- Like the gradient, the concept of normal vector requires a scalar product and hence a defined metric. However, the concept of a normal One-Form is more natural: it is the one-form that returns $0$ when acted upon any vector tangent to a surface. An outward normal one-form would further return a positive value for vectors that point outward from a surface.

### 3.4 The $\begin{pmatrix}0\\ 2\end{pmatrix}$ Tensors
- Tensors (linear functions) of two vector arguments (that return a scalar), such as the metric tensor.
- Can be formed from one-forms by a kind of product:
	- If $\tilde{p}$ and $\tilde{q}$ are two one-forms, then the (outer) product $\tilde{p} \otimes \tilde{q}$ is the $\begin{pmatrix}0 \\ 2\end{pmatrix}$ tensor that when supplied with two vectors $\vec{A}, \vec{B}$ returns the value $\tilde{p}(\vec{A})\tilde{q}(\vec{B})$.
	- The outer product $\otimes$ is not commutative:  $\tilde{p} \otimes \tilde{q}$ is different from $\tilde{q}\otimes \tilde{p}$ in that the first one returns $\tilde{p}(\vec{A})\tilde{q}(\vec{B})$ while the second one returns $\tilde{q}(\vec{A})\tilde{p}(\vec{B})$, that is, the vectors are supplied to different one-forms.

*Components*
- The most general $\begin{pmatrix}0\\2 \end{pmatrix}$ tensor is not a simple outer product, but it can be represented as a linear sum of such tensors (below). 
- The components of a general $\begin{pmatrix}0\\2 \end{pmatrix}$ tensor are $f_{\alpha \beta}=$f$(\vec{e_{\alpha}},\vec{e_{\beta}})$. Since each index can have four values, there are 16 components (can be thought of as arrayed in a matrix).
- The value of **f** on two arbitrary vectors is f$(\vec{A},\vec{B}) =$f$(A^{\alpha}\vec{e_{\alpha}},B^{\beta}\vec{e_{\beta}})=A^{\alpha}B^{\beta}$ f$(\vec{e_{\alpha}},\vec{e_{\beta}})=A^{\alpha}B^{\beta}f_{\alpha \beta}$ (contraction, the value a tensor takes when supplied with vectors is always a contraction of their components, in whatever frame). Notice two different dummy indices are used to keep track of two different summations.
- A basis for these tensors would have to be a(for each of the 16 components) 16 element set        {$\tilde{w}^{\alpha \beta}$} such that f$=f_{\alpha \beta}\tilde{\omega}^{\alpha \beta}$ (a geometrical invariant object).
- Since we can write an equation for the components, in it we can express the LHS in terms of the basis one-forms and see if that leads anywhere: 
	- $f_{\mu \nu}=$f$(\vec{e}_{\mu}\vec{e}_{\nu})=f_{\alpha \beta}\tilde{\omega}^{\alpha \beta}(\vec{e_{\mu}},\vec{e_{\nu}})$  $$\rightarrow \tilde{\omega}^{\alpha \beta}(\vec{e_{\mu}},\vec{e_{\nu}}) = \delta^{\alpha}_{\mu}\delta^{\beta}_{\nu}$$
- Hence, $$\tilde{\omega}^{\alpha \beta}= \tilde{\omega}^{\alpha}\otimes \tilde{\omega}^{\beta}$$
are the basis for all $\begin{pmatrix}0\\2 \end{pmatrix}$ tensors and so we write, for a general tensor: f$=f_{\alpha \beta}\tilde{\omega}^{\alpha}\otimes \tilde{\omega}^{\beta}$ 
- This is a sum of simple outer product tensors (each value of $\alpha$ and $\beta$ corresponds to a term(which is an outer product one form) in the sum).
- So, if you have got two general one-forms, you can make a general 2nd rank tensor by their linear sum.

*Symmetries*
- A $\begin{pmatrix}0\\2\end{pmatrix}$ tensor takes two arguments, and as we have seen, their order is important. The behavior of a tensor under an interchange of its arguments is an important property.
- A tensor is symmetric if **f**$(\vec{A},\vec{B})=$ **f**$(\vec{B},\vec{A})$,  $\forall \vec{A},\vec{B}$. To see the behavior of it's components, set $\vec{A} = \vec{e}_{\alpha}$ $\rightarrow$ $f_{\alpha \beta} =$f$(\vec{e_{\alpha}},\vec{e}_{\beta})=(\vec{e_{\beta}},\vec{e}_{\alpha})=f_{\beta \alpha}$. This is the same condition for a symmetric matix: corresponding rows and columns are the same.
- An arbitrary tensor **h** can define a new symmetric tensor: $h_{(s)}(\vec{A},\vec{B}) =\frac{1}{2}h(\vec{A},\vec{B})+ \frac{1}{2} h(\vec{B},\vec{A})$. Replacing the vectors with basis vectors, we find the corresponding relation for the components: $h_{(s) \alpha \beta}= \frac{1}{2} (h_{\alpha \beta} + h_{\beta \alpha })$. For this (the components of a symmetric tensor), a special notation is used: $h_{(\alpha \beta)}= \frac{1}{2} (h_{\alpha \beta} + h_{\beta \alpha })$. (Components of a symmetric tensor defined from the components of a general tensor).
- Similarly, an antisymmetric tensor can be defined, with the symbol A used for it. For the components, square brackets are used: $h_{[\alpha \beta]}$.
- $\rightarrow$  any tensor can be expressed as a sum of a symmetric and anti symmetric tensors defined from it. For the components (and similarly for the tensor): $h_{\alpha \beta}=h_{(\alpha \beta)} + h_{[\alpha \beta]}$. So any $\begin{pmatrix}0\\2\end{pmatrix}$ tensor can be split uniquely into its symmetric and antisymmetric parts.
- The metric tensor **g** is symmetric.

### 3.5 Metrics as a Mapping of vectors into One-forms

- The fundamental role of a metric in differential geometry is to act as a mapping between one-forms ands vectors:
	- Consider **g** and a single vector $\vec{V}$, the expression g$(\vec{V}, )$. Since this is a linear function of 1 vector input, it is a one-form: g$(\vec{V}, )\equiv \tilde{V}()$.
	- $\tilde{V}$ is a one-form whose value on a vector is $\vec{V}\cdot \vec{A}$: $\tilde{V}(\vec{A}) \equiv g(\vec{V},\vec{A}) =\vec{V}\cdot \vec{A}$. Since **g** is symmetric g$(\ ,\vec{V})\equiv \tilde{V}()$.
	- The components of $\tilde{V}$ are: $\tilde{V}(\vec{e}_{\alpha})=\vec{V}\cdot \vec{e}_{\alpha}=V^{\beta}\vec{e}_{\beta}\cdot \vec{e}_{\alpha}=V^{\beta}\eta_{\alpha \beta}=V_{\alpha}\rightarrow$ $$V_{\alpha}=\eta_{\alpha \beta}V^{\beta}$$ 
	- The components of the above one-form are distinguished from the components of the vector only by the positioning of the index.
	- These one-forms can be used to return a scalar product when contracted with a vector.
	- Due to the metric tensor components $\eta_{\alpha \beta}$ , if the components of a $\vec{V}$ are {$V^{\alpha}$}=$(a,b,c,d)$, then the components of the one-form $\tilde{V}$ are {$V_{\alpha}$}=$(-a,b,c,d)$.
	- In this case only the sign of the time component can be changed to change between the components of a vector and the corresponding one form obtained by inputting that vector into the metric tensor. However, since this result was obtained by using the components of the metric tensor, the result will be different in other frames where the components of the metric tensor are different.
	- In the above discussion, the metric tensor took in a vector and returned a one-form. 
	- Hence, the metric tensor **g**,and in some frame, its components $\eta_{\alpha \beta}$ provides a mapping that takes a vector and returns a one-form

	*The inverse*
	- The equation $V_{\alpha}=V^{\beta}\eta_{\alpha \beta}$  suggests that a way of going from one-form components to the related vector components if an inverse of the metric tensor exists, which it does.
	- Hence, given {$A_{\beta}$}, we can find{$A^{\alpha}$}: $$A^{\beta}=\eta^{\alpha \beta} A_\beta$$where $\eta^{\alpha \beta}$ are the components of the inverse of the metric tensor.
	- Hence, the inverse metric tensor, and in some frame, its components $\eta^{\alpha \beta}$ provide a mapping that takes in a one-form and returns a vector.

- Similarly, we can associate a vector $\vec{d}\phi$ with the gradient one-form $\tilde{d}\phi$:
	- Since the gradient vector points in the direction of the greatest increase of function, in a direction where the function does not increase at all (be constant), it must have no component. For example, take your function to be height, and imagine yourself on a mountain. Here the gradient points in the z direction. If you travel on a vector that points (lays) in the x-y plane, the gradient vector is orthogonal to it and its dot product with it zero.
	- One can see that the vector $\vec{d}\phi$ is orthogonal to surfaces of constant $\phi$ as follows:
		- By this mapping (feed in a vector to the metric tensor and get a one form, feed the one-form a vector and it returns the scalar value of this vector with the first one) Its inner product with any vector is the same as the contraction of the gradient one-form with that vector.
		- For a vector on a surface of constant $\phi$, the value $\tilde{d}\phi(\vec{V})=0$, since, from earlier discussions, the gradient one-form's components are the rate of change of the function $\phi$, which in the direction of a vector which is in the direction of zero(constant) change of the function are equal to zero.
- $\eta^{\alpha \beta}$ is identical to $\eta_{\alpha \beta}$, hence, in going from one-form to vector also just change the sign of the time component.
- A scalar product between two vectors is equivalent to contraction between the one form produced by inputting in one of the vectors into the metric and then contracting the other vector with the one-form. (also, in the scalar product, you can contract one set of components with he metric tensor components to obtain a contraction between oneform components and vectors.)

*Why distinguish One-Forms from vectors?*
- Since it is the metric that provides the mapping from one-forms to vectors and vice versa, and since in Euclidean space, in Cartesian coordinates, the metric is just the identity $\delta^{i}_{j}$ , one-form and vector components are equivalent and no distinction is made. In SR, however, the components differ (by that one change of sign of the time component).
- Therefore, whereas the gradient has components $\tilde{d}\phi \rightarrow_{O}(\frac{\partial{\phi}}{\partial {t}},\frac{\partial{\phi}}{\partial{x}},...)$, the associated vector that is orthogonal to surfaces of constant $\phi$ has components $\vec{d}\phi \rightarrow_{O}(-\frac{\partial{\phi}}{\partial {t}},\frac{\partial{\phi}}{\partial{x}},...)$
- Vectors and One-forms act in complimentary ways, you can operate on one to produce the other. Such ideas lead to the saying that vectors and one-forms are dual to each other.
- Such dual spaces are found elsewhere in physics too (the operation of finding the element of one space from an element of the other is called the adjoint and is 1-1 and invertible):
	- Row vectors as one forms matrix multiplying with column vectors to produce a number(linearly).
	- In Quantum Mechanics, the wavefunction is a complex scalar field $\psi(\vec{x})$, drawn from the *Hilbert space* of all such functions, which, since it satisfies the axioms for a vector space, is one. Since it is either the metric or a one-form that lets us evaluate the inner product between two vectors, the Quantum Mechanical inner product suggests that the complex conjugate of the elements of the Hilbert space make the space of one-forms, dual to the Hilbert space, with the value it returns when acted upon a vector is the integral with it (analogous to the sum). The operation of complex conjugation acts like our metric tensor, transforming a vector (of the Hilbert space) to a one-form.
	- The same idea is reflected in Dirac's bras and kets.
- The concept of a dual vector space arises very frequently in advanced mathematical physics.

*Magnitudes and scalar products of one-forms*
- The metric tensor provides a (bijective) map from the space of all one-forms to the space of all vectors. Hence, with every one-form, we can associate a vector (the one obtained by contracting the one-form with one of the indices of the metric tensor).
- Hence, the magnitude of a one-form is defined as the magnitude of the corresponding vector: $\tilde{p}^{2}=\vec{p}^{2}=\eta_{\alpha \beta}p^{\alpha}p^{\beta}$.
- This would involve(to find the magnitude of the one-form) finding the set {$p^\alpha$} from {$p_{\beta}$}, but $\eta_{\alpha \beta}p^{\alpha}p^{\beta}=\eta_{\alpha \beta}(\eta^{\alpha \mu}p_{\mu})(\eta^{\beta \nu}p_{\nu})$.   notice the use of different indices for each independent summation.
- Since $\eta_{\alpha \beta}\eta^{\beta \nu} =\delta^{\nu \alpha}$,(summation over beta) since the two are inverses of each other and the LHS is just a matrix product. Using this, the above equation reduces to: $\tilde{p}^{2}=\eta^{\alpha \beta}p_{\alpha}p_{\beta}$.
- Using the components of the metric tensor in Euclidean space, in Cartesian coordinates, we find the magnitude for one-forms has the same form as that of the vector and thus that of a spacetime interval, and so is invariant. One-forms are timelike, spacelike, or lightlike as their associated vectors are.
- From writing an expression for the magnitude of the sum of two one forms, we can define the scalar product for one-forms. It is the same as that for vectors.
- ....

### 3.6 Finally: $\begin{pmatrix}M\\N\end{pmatrix}$ Tensors
 *Vector as a function of One-Forms* 
 -  we can also define vectors as functions of one-forms that return a scalar: $\vec{V}(\tilde{p})\equiv \tilde{p}(\vec{V})\equiv p_{\alpha}V^{\alpha}\equiv \langle \tilde{p},\vec{V} \rangle$ 
 - This dethrones vectors as from their special position as things acted on by tensors and places them on an equal footing with one-forms.

*$\begin{pmatrix}M\\0\end{pmatrix}$ tensors*
- A linear function of M one-forms into the real numbers.
- A simple $\begin{pmatrix}2\\0\end{pmatrix}$ tensor is $\vec{V} \otimes \vec{W}$, which can be supplied with two one-forms and is generally not commutative. Writing out the contraction shows that it has components $V^{\alpha}W^{\beta}$ with a basis $\vec{e}_{\alpha} \otimes \vec{e}_{\beta}$. 
- The components of an $\begin{pmatrix}M\\0\end{pmatrix}$ tensor are the values it takes when supplied with basis one-forms $\tilde{\omega}^{\alpha}$. The components all have indices that are superscripts.

*$\begin{pmatrix}M\\N\end{pmatrix}$* tensors
- A linear function of M one-forms and N vectors into the real numbers.
- Let R be a $\begin{pmatrix}1\\1\end{pmatrix}$ tensor. Then it requires an input one One-form $\tilde{p}$ and one vector$\vec{A}$ to produce the real number $R(\tilde{p};\vec{A})$. It has components $R^{\alpha}_{\beta}\equiv R(\tilde{\omega}^{\alpha};\vec{e}_{\beta})$. In a new frame, the components are $R^{\alpha'}_{\beta'}=R(\tilde{\omega}^{\alpha'};\vec{e}_{\beta'})=R(\Lambda^{\alpha'}_\mu \tilde{\omega}^{\mu};\Lambda^{\nu}_{\beta'} \vec{e}_{\nu})=\Lambda^{\alpha'}_{\mu}\Lambda^{\nu}_{\beta'}R(\tilde{\omega}^{\mu};\vec{e}_{\nu})=\Lambda^{\alpha'}_{\mu}\Lambda^{\nu}_{\beta'}R^{\mu}_{\nu}$ 
- The transformation of components is such that each index transforms by bringing in $\Lambda$ whose indices are arranged as permitted by the summation convention.

*Circular Reasoning?*
- We defined One-Forms in terms of vectors but now we define vectors in terms of one-forms. This duality is at the heart of theory, but it is not circularity. We picked up an object (the displacement) and identified a vector with it and then generated all general tensors, which pick their meaning from the original meaning that we gave vectors. But we could have equally well associated one-forms with some physical object such as the gradient and gotten the same results. The power of mathematics is that it doesn't need to say what the original vectors or one forms are, it just gives rules for manipulating them. The association of a physical object, lets say momentum $\vec{p}$ with a vector, is at the interface of physics and mathematics: it is how we make a mathematical world of the physical world.
- A geometer adds to these abstract tensor spaces what a notion of a vector in a curved space is.

### 3.7 Index Raising and Lowering

- In the same way that the metric tensor maps a vector onto a one-form, it maps a $\begin{pmatrix}M\\N\end{pmatrix}$ tensor to a $\begin{pmatrix}M-1\\N+1\end{pmatrix}$ tensor, conversely for the inverse.
- The resulting tensor will have one fewer dimension. This is akin to how the scalar product of two vectors results in a scalar, effectively "summing out" the vector dimensions. In essence, when working with the metric and higher-rank tensors, contractions generalize the concept of the scalar product, allowing for the reduction of tensor rank and often leading to quantities with specific physical or geometric interpretations.
- Suppose $T^{\alpha \beta}_{\gamma}$ are the components of a $\begin{pmatrix}1\\2\end{pmatrix}$ tensor, then $T^{\alpha}_{\beta \gamma} \equiv \eta_{\beta \mu}T^{\alpha \mu}_{\gamma}$ are the components of a $\begin{pmatrix}1\\2\end{pmatrix}$ tensor, obtained by mapping the second one-form argument onto a vector argument. note that this means it can be contracted with one more vector argument instead of a one-form argument.
- Whenever an index is raised ow lowered, it is the map generated by the metric doing the work. In SR, when raising or lowering the 0th index, the sign is changed, when raising or lowering the 1,2,3 indices, they remain unchanged (the components).

*Mixed Components of Metric*
- Suppose we raise an index of the metric tensor components using the components of the inverse metric tensor: $\eta^{\alpha}_{\beta} \equiv \eta^{\alpha \mu}\eta_{\mu \beta}$. Since the RHS is the matrix product of two inverses, we must have $\eta^{\alpha}_{\beta}\equiv \delta^{\alpha}_{\beta}$.
- Raising the other index: $\eta^{\alpha \beta}\equiv \eta^{\beta \gamma}\delta^{\alpha}_\gamma$ is an identity.
- So the matrix inverse of the covariant metric tensor is the same as the contravariant metric tensor.

*Metric and Non-Metric vector Algebras*
- Why does the metric and not some other $\begin{pmatrix}0\\2\end{pmatrix}$ tensor generate the correspondence between one-forms and vectors?
- First, the correspondence is needed since it gives us the inner product and we want the inner product since in physics, they are useful. In QM and classical mechanics, a metric for the vector space is not required.
- It is the metric that generates the mapping, so if it was some other tensor that did that, then that would have been the metric. The metric is an added bit of structure in the vector space. Different spaces in mathematics can have different metric structures. we are dealing pseudo-Riemannian, where the magnitude given to vectors by the metric could both be positive and negative.

### 3.8 Differentiation of Tensors

- A function $f$ is a tensor of $\begin{pmatrix}0\\0\end{pmatrix}$ rank, while its gradient $\tilde{d}f$ is function of $\begin{pmatrix}0\\1\end{pmatrix}$ rank. Differentiation of a function produces a tensor of one higher (covariant) rank. This applies to differentiation of tensor of any rank.
- 