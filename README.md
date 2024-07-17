# Abstract
Approximating solutions to the complex mathematical equations that underpin our physical
systems is an incredibly energy-intensive process. Finding solutions to these equations
becomes increasingly difficult as dimensionality increases and data becomes more sparse,
with the scientific community turning to machine learning (ML) methods to try and alle-
viate these issues. Approximations of Ordinary Differential Equations (ODEs) and Partial
Differential Equations (PDEs) via traditional methods are both faster and more accurate,
but computationally expensive. ML-based methods have the potential to offer efficient,
scalable and real-time approximations to these equations, with the environmental cost of
simulations/training models under scrutiny as the impact of high-performance computing
on the environment is evaluated. From a climate perspective, improving computational
efficiency in regard to resource utilisation also becomes important for increasing the accu-
racy of modelling complex and nonlinear physical systems; allowing researchers to develop
more powerful physics-based models for ocean surface or climate modelling.

This report focuses on one proposed solution for a generalised solution for solving ODEs
and PDEs, named physics-informed neural networks (PINNs). This extension of artificial
neural networks (ANNs), whilst benefiting from real-time approximations, is simple in its
implementation, easy to parallelise using ML-libraries and can be run directly on graphics
processing units (GPUs). Their implementation involves an extension of a fully-connected
neural network (FCNN), via an added term of the loss function. PINNs utilise the prior
knowledge of physical systems by calculating the PDE residual as this added term, which
in turn constrains the network to obey the underlying physical equation and generalise
well outside of training data.

This research study sets out to investigate the training times of these extended neural
networks when used to approximate ODEs via a PINN-based model comparative to a
traditional numerical solver.
