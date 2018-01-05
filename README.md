# Surface Smoothing
The diffusion equation f_t = µ∆f describes how a function f changes over time by a scalar coefficient µ times its spatial laplacian. In mesh processing, this equation is used to smooth out geometrical details on a mesh by replacing the regular Laplace operator by the Laplace Beltrami operator and the function f by vertex positions. Since the Laplace Beltrami operator of vertex positions corresponds to the mean curvature geometrically the equation moves all vertices in the normal direction by a strength proportional to the mean curvature. This repo implements this (implicit) mean curvature flow scheme.

![](smoothing.png)

Note: Requires Eigen 3.2.4 and assumes it is in /usr/local/Cellar/eigen/3.2.4/include/eigen3/
