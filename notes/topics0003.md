### Blount Identity

<p>
Bloch function is expressed as follows
</p>

$$
\begin{align}
\psi_{n{\bf k}}({\bf r}) &= e^{i{\bf k}\cdot{\bf r}}u_{n{\bf k}}({\bf r}) \tag{1}
\end{align}
$$

<p>
where $u_{n{\bf k}}$ has the periodicity of Hamiltonian.
Bloch functions are normalized to one unit cell    
</p>

$$
\begin{align}
\int_{V} d{\bf r}\hspace{0.5mm} \psi^{*}_{m{\bf k}}({\bf r})\psi_{n{\bf k}}({\bf r}) &= \delta\_{mn} \tag{2}
\end{align}
$$

<p>
where $V$ is the real-space primitive cell volume.
When the number of the primitive cell in the supercell is $N$,
the volume of the supercell, $V_{\rm all}$, is $V_{\rm all}=NV$.
Bra-ket notation in this paper is related to Bloch functions as follows,     
</p>

$$
\begin{align}
\ket{\psi_{n{\bf k}}} &= \int d{\bf r} \hspace{0.5mm} \psi_{n{\bf k}}({\bf r}) \ket{\bf r} \tag{3} 
\end{align}
$$

<p>
This notation is different from one in Ref.~\cite{PhysRevB.56.12847}.    
</p>

$$
\begin{align}
\braket{\psi_{m{\bf k}}|\psi_{n{\bf k}'}}
&= \int d{\bf r} \int d{\bf r}' \hspace{0.5mm} \psi^{*}_{m{\bf k}}({\bf r}) \psi_{n{\bf k}'}({\bf r}') 
    \braket{{\bf r}|{\bf r}'}  \\\\
&= \int d{\bf r} \int d{\bf r}' \hspace{0.5mm} \psi^{*}_{m{\bf k}}({\bf r})
    \psi_{n{\bf k}'}({\bf r}') 
    \delta({\bf r}-{\bf r}') \nonumber \\
&=& \int d{\bf r} \hspace{0.5mm} 
    \psi^{*}_{m{\bf k}}({\bf r})
    \psi_{n{\bf k}'}({\bf r}) \nonumber \\
&=& \sum_{\bf R} \int_{V} d{\bf r} \hspace{0.5mm}
    \psi^{*}_{m{\bf k}}({\bf r}+{\bf R})
    \psi_{n{\bf k}'}({\bf r} + {\bf R}) \nonumber \\
&=& \sum_{\bf R} e^{i({\bf k}'-{\bf k})\cdot{\bf R}}
    \int_{V} d{\bf r} \psi^{*}_{m{\bf k}}({\bf r})
    \psi_{n{\bf k}'}({\bf r}) \nonumber \\
&=& N \delta_{{\bf kk'}}\delta_{mn} \nonumber \\
&=& \frac{(2\pi)^{3}}{V} \delta({\bf k}-{\bf k}')\delta_{mn} 
    \label{eq:braket_norm}
\end{align}
$$

<p>
When deriving Eq.~\ref{eq:braket_norm}, the following property 
of Bloch function is used.    
</p>

$$
\begin{align}
\psi_{n{\bf k}}({\bf r}+{\bf R}) &= e^{i{\bf k}\cdot{\bf R}} \psi_{n{\bf k}}({\bf r}) \tag{4}
\end{align}
$$

<p>
Kronecker delta formula is expressed as,    
</p>

\begin{eqnarray}
\frac{1}{N} \sum_{\bf R} e^{i({\bf k}'-{\bf k})\cdot{\bf R}} 
&=& \delta_{{\bf kk}'} 
\label{eq:Kronecker_delta}
\end{eqnarray}
Kronecker delta is switched to Dirac delta function using the following correspondence,
\begin{eqnarray}
\sum_{\bf k} \delta_{{\bf kk}'}
= 1 &\rightarrow& \int d{\bf k} \delta({\bf k}-{\bf k}') = 1 \nonumber \\
\frac{1}{\Delta k_{x} \Delta k_{y} \Delta k_{z}}
\sum_{\bf k} \delta_{{\bf kk}'} \Delta k_{x} \Delta k_{y} \Delta k_{z} 
&=& \sum_{\bf k} \frac{V_{\rm all}}{(2\pi)^{3}} \delta_{{\bf kk}'} \Delta {\bf k} \nonumber \\
\frac{V_{\rm all}}{(2\pi)^{3}} \delta_{{\bf kk}'} 
= \frac{NV}{(2\pi)^{3}} \delta_{{\bf kk}'} &\rightarrow& \delta({\bf k}-{\bf k}')  \nonumber \\
N \delta_{{\bf kk}'} &\rightarrow& \frac{(2\pi)^{3}}{V} \delta({\bf k}-{\bf k}')
\label{eq:Kronecker_dirac_delta}
\end{eqnarray}

\section{Bra-ket notation of Marzari et al. \cite{PhysRevB.56.12847}}
Bra-ket notation is sometimes written as~\cite{PhysRevB.56.12847}
\begin{eqnarray}
\ket{\psi_{n{\bf k}}}
&=& e^{i{\bf k}\cdot{\bf r}} \ket{u_{n{\bf k}}}.
\label{eq:braket_marzari}
\end{eqnarray}
This notation leads to the inconsistent with Eq.~\ref{eq:braket_ryo}
\begin{eqnarray}
\ket{\psi_{n{\bf k}'}}
&=& \int d{\bf r} \hspace{0.5mm} \psi_{n{\bf k}}({\bf r}) \ket{\bf r} \nonumber \\
&=& \int d{\bf r} \hspace{0.5mm} e^{i{\bf k}\cdot{\bf r}}u_{n{\bf k}}({\bf r}) \ket{\bf r} \nonumber \\
&\neq& e^{i{\bf k}\cdot{\bf r}}
\int d{\bf r} \hspace{0.5mm} u_{n{\bf k}}({\bf r}) \ket{\bf r}
=e^{i{\bf k}\cdot{\bf r}}\ket{u_{n{\bf k}}}
\label{eq:inconsistency_of_marzari}
\end{eqnarray}
We, thus, employ the bra-ket notation of Eq.~\ref{eq:braket_ryo}
for the formulation of Wannier functions.

\section{Wannier function}
Wannier functions are constructed through the Fourier transform of 
Bloch functions,
(Eq.(3) of Marzari2012),
\begin{eqnarray}
\ket{{\bf R}n} 
&=& \frac{V}{(2\pi)^{3}}\int_{\rm BZ}
e^{-i{\bf k}\cdot{\bf R}} \ket{\psi_{{\bf k}n}}, \\
&=& \frac{1}{N} {\sum_{\bf k}}' e^{-i{\bf k}\cdot{\bf R}} \ket{\psi_{n{\bf k}}}
\label{eq:wannier_function}
\end{eqnarray}
where the integral is carried over the Brillouin zone (BZ).
Normalization of the Wannier functions is checked as, 
\begin{eqnarray}
\braket{{\bf R}m|{\bf R}'n} 
&=& \int d{\bf r} \hspace{0.5mm} \braket{{\bf R}m|{\bf r}}
\braket{{\bf r}|{\bf R}'n} \nonumber \\
&=& \biggl(\frac{1}{N}\biggr)^{2} 
{\sum_{{\bf kk}'}}' e^{-i{\bf k}\cdot {\bf R}}
e^{i{\bf k}'\cdot{\bf R}'} \int d{\bf r}\hspace{0.5mm}
\braket{\psi_{m{\bf k}}|{\bf r}}\braket{{\bf r}|\psi_{m{\bf k}'}} \nonumber \\
&=& \biggl(\frac{1}{N}\biggr)^{2} {\sum_{{\bf kk}'}}'
e^{-i{\bf k}\cdot {\bf R}}e^{i{\bf k}'\cdot{\bf R}'}
N\delta_{mn}\delta_{{\bf kk}'} \nonumber \\
&=& \frac{1}{N} {\sum_{{\bf k}}}'
e^{-i{\bf k}\cdot {\bf R}}e^{i{\bf k}\cdot{\bf R}'}
\delta_{mn} = \delta_{mn}\delta_{{\bf RR}'}
\label{eq:wannier_function_norm}
\end{eqnarray}

%The following formula derived by Blount, 
%called Blount identity, 
%is necessary for the determination of Maximally 
%localized Wannier functions (MLWFs).
%\begin{eqnarray}
%\braket{{\bf R}n|\hat {\bf r}|{\bf 0}m}
%&=& i \frac{V}{(2\pi)^{3}} \int_{\rm BZ} d{\bf k}
%\exp(i{\bf k}\cdot{\bf R})
%\braket{u_{{\bf k}n}|\nabla_{\bf k}|u_{{\bf k}m}},
%\label{eq:BlountIdentity}
%\end{eqnarray}
%where $\hat {\bf r}$ is position operator 
%(Eq.(23) of Marzari2012).

\section{Blount Identity}

\begin{eqnarray}
\hat{\bf r} \ket{{\bf 0}m}
&=& {\bf r} \ket{{\bf 0}m} \nonumber \\
&=& \frac{V}{(2\pi)^{3}} \int_{\rm BZ}
d{\bf k}' {\bf r}\ket{\psi_{{\bf k}'m}} 
\label{eq:Deriv_Step1}
\end{eqnarray}
The gradient of the Bloch orbital with respect to ${\bf k}$ is
\begin{eqnarray}
\nabla_{{\bf k}'} \ket{\psi_{{\bf k}'m}}
&=& \nabla_{{\bf k}'} (\exp(i{\bf k}'\cdot{\bf r}) 
\ket{u_{{\bf k}'m}}) 
\nonumber \\
&=& i{\bf r}\ket{\psi_{{\bf k}'m}}+\exp(i{\bf k}'\cdot{\bf r})
\nabla_{{\bf k}'} \ket{u_{{\bf k}'m}}.
\label{eq:Deriv_Step2}
\end{eqnarray}
Solvint Eq. \ref{eq:Deriv_Step2} yields
\begin{eqnarray}
{\bf r}\ket{\psi_{{\bf k}'m}}
&=& i\exp(i{\bf k}'\cdot{\bf r})\nabla_{{\bf k}'}
\ket{u_{{\bf k}'m}}-i\nabla_{{\bf k}'}\ket{\psi_{{\bf k}'m}}.
\label{eq:Deriv_Step3}
\end{eqnarray}
And Eq. \ref{eq:Deriv_Step1} becomes
\begin{eqnarray}
{\bf r} \ket{{\bf 0}m} 
&=& \frac{V}{(2\pi)^{3}} \int_{\rm BZ}
d{\bf k}' \biggl\{
i\exp(i{\bf k}'\cdot{\bf r})\nabla_{{\bf k}'}
\ket{u_{{\bf k}'m}}-i\nabla_{{\bf k}'}\ket{\psi_{{\bf k}'m}}
\biggr\}.
\label{eq:Deriv_Step4}
\end{eqnarray}
We focus our attention on 
the first term in Eq.~\ref{eq:Deriv_Step4}
since the 2nd term is expected to be zero.

\section{Divergence Theorem}
For arbitrary vector ${\bf a}$, the divergence
theorem is expressed as follows,
\begin{eqnarray}
\int (\nabla \cdot {\bf a}) \enskip d{\bf V}
&=& \int ({\bf a}\cdot {\bf n}) \enskip d{\bf S}
\label{eq:divergence_theorem}
\end{eqnarray}
where ${\bf n}$ is the outward-pointing normal.
We can define the vector ${\bf a}$ as $\phi{\bf b}$,
where $\phi$ and ${\bf b}$ are a scalar function 
and constant vector, respectively.
Then Eq.~\ref{eq:divergence_theorem} 
becomes,
\begin{eqnarray}
{\bf b} \cdot 
\int (\nabla \phi) \enskip d{\bf V}
&=& {\bf b} \cdot \int ({\phi}{\bf n}) 
\enskip d{\bf S}.
\label{eq:divergence_theorem_2}
\end{eqnarray}
From Eq.~\ref{eq:divergence_theorem_2},
the relation used in Blount1962 is obtained.
\begin{eqnarray}
\int (\nabla \phi) \enskip d{\bf V}
&=& \int ({\phi}{\bf n}) 
\enskip d{\bf S}.
\label{eq:divergence_theorem_3}
\end{eqnarray}

</p>

---
