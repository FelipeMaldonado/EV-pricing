## EV-pricing

In this repository we include the code and data used in our experiments for the paper: **Why Do Pricing Rules Matter? Electricity Market Design with
Electric Vehicle Participants**.

This paper has been submitted to the special issue **Electric Vehicles Integration in Smart Grids** at the *World Electric Vehicle Journal*.


# Python libraries required

- pandas
- numpy
- matplotlib
- ortools
  > python -m pip install --upgrade --user ortools


# Data set

In the folder *data*, there are 4 different data files, one per each scenario from the paper:

	1.  *Data_EV_Paper_S1.xlsx* for Scenario 1, used as reference (no EVs, no demand response)
	2.  *Data_EV_Paper_S2.xlsx* for Scenario 2 (EVs, no demand response)
	3.  *Data_EV_Paper_S3.xlsx* for Scenario 3 (EVs and demand response).
	
Additionally the file *Data_Khodayar.xlsx* is included. We used this dataset (associated to the paper: **Electric Vehicle Mobility in Transmission-Constrained Hourly Power Generation Scheduling**, Khodayar et al (2013)) to adapt it for the settings in  our experiments, detailed as below:

- The 3-node structure is included here as per Figure 2. in the paper (Section 6). 
- Generation and demand resources are described there. They are also explained in Section 6 (see Table 2)
- Transmission lines (how nodes are connected and the respective capacities) are also included there.
- Electric vehicles parameters as per Table 3 (Section 6) are included here.  


# The notebook contains:

1. Loading the data (and selecting the correct scenario)
2. Allocation model (as described in Section 5 of the paper)
3. Pricing schemes (it also contains IP+ pricing scheme, although we only use IP and ELM pricing for the experiments in the paper)
4. Results and plots

