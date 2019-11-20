# TriExponential-Solver
Analytical Algorithm for Computing 3-timepoint Nuclear Medicine Time Activity Curves

Pharmacokinetics backend of the VRAK Voxel dosimetry software reported in Med Phys. 2013 Nov;40(11):112503. doi: 10.1118/1.4824318.
https://www.ncbi.nlm.nih.gov/pubmed/24320462

![](fig2-ideal_case_3phase.jpg)

Curves are solved analytically to pass through measurements via linear fit of log-transformed data. Each phase depletes to very near zero as it approaches subsequent measurements. Priority is given to the final measurement as this is considered most important for accurately approximating the time integral with long half-life therapeutic isotopes. Some error handling conditions are applied to reasonably fit a curve through early time points which don't obey common physiological patterns as could be observed due to misalignment between voxels in serial imaging. The method accepts three post-treatment imaging timepoints and employs the convention to decay correct measurements before performing pharmacokinetics processing. The method has been validated for Lu-177 therapies.

![](animated_triexp.gif)
