# Launching Jupyter Notebooks on SDSC HPC Systems 
Updated: 4/25/24

For more questions, contact consult@sdsc.edu.

All applications running on all SDSC HPC systems (Expanse, Voyager, Comet, TSCC) must be secure (hosted with HTTPS connection). By default, Jupyter notebooks launch in the browser with an insecure _HTTP_ connection. SDSC has developed a utility to help you launch Jupyter notebooks on high-performance computing (HPC) systems with an _HTTPS_ connection. 

## Galyleo shell script:  https://github.com/mkandes/galyleo

The Galyleo script works with SDSC's [Satellite reverse proxy service](https://github.com/sdsc-hpc-training-org/satellite) and a batch job scheduler (e.g. Slurm) to provide each Jupyter notebook or Jupyter Lab server you start with its own one-time, token-authenticated HTTPS connection between the compute resources of the HPC system the notebook server is running on and your web browser. This secure connection affords both privacy and integrity to the data exchanged between the notebook server and your browser, helping protect you and your work against network eavesdropping and data tampering.

See the Galyleo reference pages for more information
