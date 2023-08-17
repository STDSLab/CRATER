# CRATER

This Julia code implements our efficient 'CRATER' approach to finding multipoles. 

Multipoles can be generated using the following sample code. The input to CRATER function is a covariance matrix, gain threshold, dependence threshold and a pairwise correlation threshold.

```
  using Multipoles
  cov = importData("covariance_mat.csv")
  multipoles = CRATER_PCG_CF(cov, 0.2, 0.5, 1.0)
```


In addition to CRATER, this code also include implementation of COMET and COMET_CF variants.
