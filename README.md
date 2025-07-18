7/18/2025, Shahinul

To run the coupled UEDGE and heat transport codes self-consistently, execute the following command:


python -i coupling_UEDGE_heat.py


Before running the script, the UEDGE simulation was manually executed using the emitted lithium flux (only physical sputtering) until convergence was achieved. 
This step is necessary since obtaining a converged solution with higher impurities (evaporation and ad-atom) is often challenging.

Once a fully converged solution with lithium atoms and ions is available, the coupling_UEDGE_heat.py script will run both codes over a specified time duration (e.g., t = 5 s).

Each iteration outputs results from both codes in CSV and HDF5 formats for analysis and plotting.

Several plotting scripts are also provided in this directory, including:

data_analysis.py

plot2d.py

plot_case.py

power_balance.py

These can be used to visualize plasma parameters, heat fluxes, and power balance metrics.
