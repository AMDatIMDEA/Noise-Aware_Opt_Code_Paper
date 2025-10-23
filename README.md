# Noise-Aware_Opt_Code_Paper

This repo contains the code for the paper on "Noise-Aware Optimization in Nominally Identical Measuring Systems for High-Throughput Parallel Workflows" by Schenk et al. (2025)

## Repo Structure:
The repo is organized as follows:
* Random_Initial_Data: Creates a random initial data set starting from one point, that served for initial data collection underlying the initial noise analysis studies
* Noise Analysis: Notebook and plots from paper for all the noise analysis 
* Convergence: Notebook and plots for convergence analysis of single and multi-device BO
* data: contains the main data files
* BO: contains the notebooks for running single and multi-device optimization, Metadata underlying the paper results, workflow as described in Readme_Workflow file. 

## Requirements:
The code builds on several python packages, especially gpCAM_8.1.6 https://github.com/lbl-camera/gpCAM. Other python packages as in the imports of the specific notebooks may need to be installed as well. 

## License

GPL-3

## Authors:
* Christina Schenk (IMDEA Materials Institute)
* Miguel Hernández-del-Valle (IMDEA Materials Institute, Universidad Carlos III de Madrid) 

## Acknowledgements:
* Marcus Noack (Berkeley Lab)
* Maciej Haranczyk (IMDEA Materials Institute)
* Luis Calero-Lumbreras (IMDEA Materials Institute, Universidad Carlos III de Madrid)

## Please cite
<br>
- C. Schenk, M. Hernández-del-Valle, Luis Calero-Lumbreras, Marcus Noack, Maciej Haranczyk (2025): Noise-Aware Optimization in Nominally Identical Measuring Systems for High-Throughput Parallel Workflows (under review)

