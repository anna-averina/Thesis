# Supply chain networks and return predictability
## Master thesis by Anna Averina

### Overview

I use network theory to construct a set of long-short strategies for 65 companies, connected to the tire industry via trade relationships. I find that companies that are more central to the supply chain network earn higher returns that peripheral firms (Information Ratio of 0.72). A plausible explanation to this is that central firms are exposed to more shocks and, therefore, command a higher risk premium. Empirical evidence for this sector also suggests marginal return predictability for supply chain networks (for the revenues and market data), however, it does not outperform the benchmarks due to fast information diffusion across the network.

Please find my working file for the thesis in this repository (Thesis_AA) as well as the data used for the analysis (Thesis_AA.zip, Customers.zip, Suppliers.zip). I retreived my inputs from a commercial database of Bloombgerg, which is why my zip files are protected by a password. Please send me a message if you wish to download them.

To run this code, you will need the following packages: numpy, matplotlib, networkx, pandas, itertools, scipy. 

### Installation

To set up a Python environment, go to https://conda.io/miniconda.html. Choose the Miniconda installer (Python 3.6) according to your operating system.

Once Miniconda is installed, use the ‘conda’ command to create an environment called ‘green-roofs’ with the file ‘environment.yml’.  When you create an environment or install package, conda will ask you to proceed (i.e., ‘proceed ([y]/n)?‘). Type ‘y’.

To create the environment and install the necessary packages, open the terminal inside folder '0_install' and type:
- For Windows: ‘conda env create -f win_environment.yml -n greenroofs’;
- For Linux/macOS: ‘conda env create -f unix_environment.yml -n greenroofs’.

To activate the environment, type ‘activate greenroofs’ (Windows) or ‘source activate greenroofs’ (Linux/macOS). To deactivate the environment, type ‘deactivate’ (Windows) or ‘source deactivate’ (Linux/macOS).

You now have a working Python environment.

### Instructions

1. Open the terminal and activate the environment;

2. Open ‘create_features.py’:
    
    1. Set ‘BAG_Panden’ to the file with the building footprint polygons;
    2. Set ‘CIR’ to the file with the color-infrared imagery;
    3. Save ‘create_features.py’;

3. Run ‘create_features.py’ (i.e., type ‘python create_features.py’ in the command line);

4. Open ‘classify.py’ and:

    1. Save the IDs within the selected area of interest as ‘aoi_ids.csv’ and set it as the variable ‘AoI’;
    2. Save ‘classify.py’; and,

5. Run ‘classify.py’ (i.e., type ‘python classify.py in the command line’).

--- 
### Authors

Author: [Anna Averina](https://www.linkedin.com/in/annaaverina/)

Contributor: [Tiago Louro Alves](https://www.linkedin.com/in/tlouroalves/)

Supervisor: Goncalo Sommer Ribeiro 