## EV-pricing

In this repository we include the code and data used in our experiments for the paper: **Why Pricing Rules Matter? Electricity Market Design with
Electric Vehicle Participants**.

This paper has been submitted to the special issue **Electric Vehicles Integration in Smart Grids** at the *World Electric Vehicle Journal*.


# Python libraries required

- pandas
- numpy
- matplotlib
- ortools
  > python -m pip install --upgrade --user ortools


# Data set

The file *Data_EV_Paper_.xlsx* contains the data used for our experiments:

- The 3-node structure is included here as per Figure 2. in the paper (Section 6). 
- Generation and demand resources are described there. They are also explained in Section 6 (see Table 2)
- Transmission lines (how nodes are connected and the respective capacities) are also included there.
- Electric vehicles parameters as per Table 3 (Section 6) are included here.  


# The notebook contains:

1. Loading the data (and selecting the correct scenario)
2. Allocation model (as described in Section 5 of the paper)
3. Pricing schemes (it also contains IP+ and CH pricing scheme, although we only use IP and ELM pricing for the experiments in the paper)
4. Results and plots

