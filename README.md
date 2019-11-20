# TriExponential-Solver
Analytical Algorithm for Computing 3-timepoint Nuclear Medicine Time Activity Curves

Pharmacokinetics backend of the VRAK Voxel dosimetry software reported in Med Phys. 2013 Nov;40(11):112503. doi: 10.1118/1.4824318.
https://www.ncbi.nlm.nih.gov/pubmed/24320462

Curves are solved analytically to pass through measurements via linear fit of log-transformed data. Each phase depletes to very near zero as it approaches subsequent measurements.

![](animated_triexp.gif)
