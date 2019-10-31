# UCoCoS Software Package

The UCoCoS Software package integrates a collection of tools for the analysis and control of complex systems and networks, and constitutes the main result of Work Package 4 on computational tools and software.  The developed analysis tools concern the detection of oscillatory patterns in networks,  the computation of partial synchronization manifolds in delay-coupled networks, as well as the assessment of the robustness of stability of a controlled system against feedback delays and a sampled data implementation of the controller. The synthesis tools allow to design structured controllers, including decentralized and distributed controllers, for large-scale systems and networks with delays.

The software was developped in the framework of the project UCoCoS, funded by the European Unions Horizon 2020 research and innovation programme under the Marie Sklodowska-Curie Grant Agreement No 675080.

### Availability:

To use the package extract [UCoCoS_Package.zip](https://github.com/UCoCoSH2020/UCoCoS-Software-Package/blob/master/UCoCoS_Package.zip) file in one directory, and open the file index.html. This package is released under the GNU GPL v3.0 license. For complete details see [here](http://www.gnu.org/licenses/gpl-3.0.html).

# Contribution of the Early Stage Researchers

The package includes software tools developed by ESR1, ESR3, ESR5 and ESR6 as part of their doctoral project, under supervision of their PhD advisers. They are as follows.
 
## MHB_EA (Kirill Rogov, ESR1)
 This software tool implements a method aiming at pattern prediction and computation in networks of diffusively coupled Lur’e systems.    Interconnecting several globally asymptotical stable systems into a network via diffusion may induce a diffusion-driven instability    phenomenon, which on its turn may lead to pattern formation in coupled systems. As the  oscillations can be shown to appear via a Hopf    bifurcation,  the describing function method can be used in order to replace a nonlinearity and then to analyze the system of linear    equations by means of the multivariable harmonic balance method. The software is based on an extension of this method to systems having a network structure. The approach is particularly powerful for detecting equal amplitude oscillations.

## compute_manifolds (Libo Su, ESR3)
Due to weak couplings, large time-delays, etc., a network of interconnected dynamical systems may exhibit a form of incomplete synchronization where some but not all systems behave synchronously. The phenomenon is called partial synchronization or cluster synchronization. To describe the patterns of partial synchronization, so-called partial synchronization manifolds are used, which are linear invariant subspaces of  the state space. Based on a recently proposed existence criterion for partial synchronization manifolds in terms of the block structure of a reordered adjacency matrix,  the software tool computes all partial synchronization manifolds in networks of systems interacting via linear diffusive delayed coupling, where both the cases of invasive and non-invasive coupling may be considered.  The software  includes the additional feature of computing system matrices corresponding to the synchronization error dynamics, as well as the adjacency matrix of a reduced network corresponding to the dynamics on the partial synchronization manifold.

## TDS_HIOPT-NSE  (Deesh Dileep, ESR5)
The software implements a novel methodology  for the design of robust controllers for  linear time-invariant (LTI)  delay systems of both retarded and neutral type, focusing on decentralized and overlapping fixed-order controllers for Multiple Input Multiple Output (MIMO) systems. The methodology is grounded in a direct optimization approach as it relies on the minimization of the spectral abscissa and H-infinity based cost functions with respect to the controller or design parameters.  The software can be applied to  generic MIMO systems,  where specifications on the structure of the controller are automatically translated into a sparsity pattern on the controller.  For the design of decentralized controllers for a class of networks consisting of identical systems, the software can also exploit the network structure, thereby significantly improving computational efficiency and scalability with the number of subsystems. 

## Dec_sampling_LTI (Jijju Thomas, ESR6)
This software tool concerns the stability analysis of decentralized sampled-data LTI control systems with asynchronous sensors and actuators. The general case is considered where each controller in the decentralized setting has its own sampling and actuation frequency, which translates into asynchrony between sensors and actuators.  The software allows to compute bounds on the delays and the sampling rates in such a way that preservation of stability of the closed-loop system is guaranteed.

