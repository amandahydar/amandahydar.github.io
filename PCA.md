## Advanced Statistical Analysis for Bioenergy Supply Chains

**Project description:** The data obtained from pre-processing two types of biomass, with varying moisture content, are used to develop conclusions on how variables such as throughput, grinding energy, and logistics costs are related to the aforementioned factors, as well as to each other. Test data from Idaho National Laboratory was obtained and Principal Component Analysis (PCA) was used to investigate the correlation between selected factors and the overall performance of the system.

### 1. What is Biomass?

Biomass is, organic matter, especially plant matter, and it can be converted to fuel.

<img src="images/biomass.JPG?raw=true"/>

_First generation_: edible crops such as sorghum and corn

_Second generation_: non-edible crops such as wood chips, switchgrass, Miscanthus, organic waste, and food crop waste (e.g., corn stover)

Biomass is the largest single source of renewable energy in the United States and was found to have the potential to replace 30% of the current petroleum demand (Goss, Thesis, and Rials). Used to produce fuels such as charcoal, ethanol, and renewable diesel, biomass is a versatile renewable source. 

### 1. Data Collection

A major participant in enhancing research of biomass-to-biofuel supply chain logistics is Idaho National Laboratory (INL). INL has taken major strides in investigating the economics and sustainability of moving biomass from harvest to the throat of the biomass conversion process; these advances have been made possible, in part, through development of a full-scale, integrated feedstock preprocessing system called the Process Demonstration Unit (PDU). Through utilization of the PDU, extensive experimentation and data collection has been made possible which may provide insight on how to adapt control parameters to account for variability. Figure 1 shows a block flow diagram of the biochemical conversion process, which is the process the biomass used in PDU experiments undergoes. The data used to further understand how preprocessing variables affect throughput was taken from the preprocessing operations of Stage I and II grinding blocks.

<img src="images/preprocessing.png?raw=true"/>

### 2. Principal Component Analysis (PCA)

Principal Component Analysis is a dimension-reducing technique used to linearly transform a large set of data into a smaller number of uncorrelated components, called “principal components”, which represent most of the information in the original variables and allows for an enhanced understanding of the data.


This method of analysis is useful to uncover patterns and can reduce a large amount of data into a subset of significant relationships.

<img src="images/pca1.png?raw=true"/>

<img src="images/pca2.png?raw=true"/>

PCA essentially works in steps toward solving an eigenvalue/eigenvector problem to reduce the dimensions of a dataset. 

<img src="images/PCAmethod1.JPG?raw=true"/>


### 3. Using PCA to Understand Biomass Preprocessing Variables

PCA essentially works in steps toward solving an eigenvalue/eigenvector problem to reduce the dimensions of a dataset. Beginning with a calculation of the first principal component, a linear combination of x1,x2, …., xp ,  such that the variance of y1 is maximized. . In a similar fashion, moving to the next set of variables, y2 will be calculated and account for the second largest percentage of variance between all components. Further, the PCA will find the optimal weight vector for the first component and its' associated variance; this calculation will be performed for each principal component found and will be maximized, subject to the constraint that it must be uncorrelated with the previous components. From these variable weight vectors and associated variances for each principal component, an indication of how each variable contributes to the variance is seen. Reducing the dataset in this way can considerably simplify data analysis and further exploration of the implications found can provide valuable insight.

_Step 1: Calculate Eigenvectors_

<img src="images/pcastep1.png?raw=true"/>

_Step 2: Evaluate Scree and Score Plot_

<img src="images/pcastep2.JPG?raw=true"/>

_Step 3: Generate Biplots_

<img src="images/pcastep3.png?raw=true"/>

<img src="images/pcastep4.png?raw=true"/>

### 4. Conclusions

Results indicate that type of biomass and percentage of moisture strongly influence the throughput, energy consumption, preprocessing cost, and logistics cost.
PCA results show segregation when testing corn stover as opposed to switchgrass and varying the amount of moisture. The graphical results indicate that decreasing costs and energy, while increasing throughput, may be achieved when switchgrass is used rather than corn stover. The PCA results for moisture content show that lower moisture content between 0-15% increase throughput and decrease logistics cost, energy consumption, and preprocessing cost; these correlations can be seen in the biplots shown in Step 3. To further quantify the impact of these factors, a cost comparison of using these recommended settings versus the opposition may be analyzed; using a moisture content between 0-15% results in preprocessing cost reductions of $2.54 per dry ton, which is a 15.7% preprocessing cost reduction from using a higher moisture content. Data from type of biomass used may also be quantified as an 18% preprocessing cost reduction when using switchgrass as opposed to corn stover. It is therefore recommended for improved operations, to use switchgrass with lower moisture content (between 0-15%), which returns the highest possible throughput and lower logistics and preprocessing costs
