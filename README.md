# QM/MM Benchmarking Data

Raw CP2K output logs produced by running benchmarks from the BioExcel QM/MM benchmark suite:

[https://github.com/bioexcel/qmmm\_benchmark\_suite](https://github.com/bioexcel/qmmm_benchmark_suite)


## Machines

### Cirrus@EPCC (HPE SGI ICE XA):
[https://www.cirrus.ac.uk](https://www.cirrus.ac.uk/)

- Infiniband interconnect
- CPU compute nodes:
	- 2 x 18-core Intel Xeon (Broadwell) E5-2695, 2.1 GHz
  - 256GB RAM
- GPU compute nodes:
	- 2 x NVIDIA Tesla V100 (Volta) SXM2-16GB
	- 2 x 20-core Intel Xeon (Cascade Lake) Gold 6248, 2.4 GHz
  - 384GB RAM


### ARCHER2@EPCC (HPE CRAY EX):
[https://www.archer2.ac.uk/](https://www.archer2.ac.uk/)

- Interconnect: HPE Cray Slingshot
- Compute nodes:
	- 2 x 64-core AMD EPYC (Zen2 Rome) 7742, 2.25GHz
	- 256GB RAM


## Benchmarking protocol
Repeated runs to rule out machine noise variability were performed for each benchmark on each machine for both 1 MD step and 6 MD steps. Subsequent analysis and visualisation of parallel scaling of average runtime per MD step and subroutine-level profiling was performed using our analysis script available from:

[https://github.com/bioexcel/qmmm_benchmark_script](https://github.com/bioexcel/qmmm_benchmark_script)

Results on Cirrus CPU nodes are for CP2K release version 8.1, whilst results on Cirrus GPU nodes and ARCHER2 are with CP2K version 8.2. 