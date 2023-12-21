# SpatialDieaseSim
Repository accompanying the manuscript "Catching a wave: on the suitability of traveling-wave solutions in epidemiological modeling" (DOI: https://doi.org/10.1101/2023.06.23.546298; or  2023.06.23.546298v1.full.pdf in this repository). 

Three classic compartmental disease transmission models implemented in SLiM4 (https://messerlab.org/slim/)


SI.slim   individual-based simulation framework of an S(usceptible)-I(nfective) Model 

SIS.slim  individual-based simulation framework of an S(usceptible)-I(nfective)-S(usceptible) Model

SIR.slim  individual-based simulaiton framework of an S(usceptible)-I(nfective)-R(ecovered) Model


## Model Parameters:
D=Diffusion Coefficient

R=averave number of contacts per tick

ALPHA=disease establishment proportion

INFTICKS=number of infectious ticks (SIS.slim, SIR.slim)

N=population size

STORE=index for output files (if no GUI is used)

## Runtime Performance:
For this project, we conducted individual-based simulations on Cornell’s BSCB computing cluster (https://biohpc.cornell.edu/lab/lab.aspx). The run-time of individual simulations varied considerably: from a few seconds in the case of no successful disease establishment to a few hours in the case of disease establishment in highly structured populations. For the latter, we run one simulation on a local machine to obtain a reference value: A simulated disease outbreak in the SI model in a highly structured population (i.e., $D=10^{-10}$) run for 15,126 ticks, took 3 hours and 8 minutes, and had a peak memory usage of 102.4 Mb (MacBook Pro, 2.7GHz Dual-Core Intel Core i5, 8 GB 1867 MHz DDR3 Memory)

This project has received funding from the European Union’s Horizon2020 research and innovation program under the Marie SklodowskaCurie grant agreement No. 101025586.
