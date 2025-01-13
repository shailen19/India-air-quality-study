# India-air-quality-study
**Overview**

this project examined the air quality levels in India from 2015-2020, focusing on pollutant levels, their interactions, and their impact on air quality across different regions. We study key pollutants such as PM 2.5, PM 10, SO2 and CO, and studied their correlations and indivudal affects on the region. Using statistical methods like correlation tests, regression models and two-way ANOVA, the study identified  regional differences in air quality and highlighted relationships between pollutants like PM 2.5 and PM 10 and NO and O3.

**Key Features**
  1. **Box Plot Analysis**
     The box plot was used to examine PM 2.5 levels across different regions in India. A long plot was used to highlight regional varation: the        **North** had the highest level (4.46ug/m^3), East (4.08ug/m^3), Central (3.92ug/m^3), South (3.68ug/m^3), and **West** (3.55ug/m^3) recorded         the lowest level.
  2. **Correlation Matrix**
     The correlation matrix revealed key relationships between pollutants. The strongest correlation (0.87) was between PM 2.5 and PM 10, a 0.79 correlation between NO and NOx, and 0.67 between NO2 and NOx. The other pollutant pairs had p-values greater than 0.05, rejecting significant correlation.
  3. **Bootstrap Correlation**
     A boostrap correlation analysis was conducted to further investigate the correlation between PM 2.5 and PM 10. The bootstrap correlation closely followed a normal distribution. When comparing the theoretical confidence interval (CI) to the bootstrap CI, the theortical CI is notibly smaller, narrowing around 0.87 to 0.875.
  4. **Two Way ANOVA**
  The ANOVA test revealed that AQI Bucket (which classifies AQI into buckets like "Good", "Moderate",etc.) and Region have a signifcant impact on AQI as the p-values are extremely small. The test reveals that AQI Bucket and Region do interact, indicating that the relationship between AQI and region is not the same for all AQI buckets. The interaction explains the variation in air quality between regions.

**How to Run:**
To run this project, you will need to install the necessary libraries and set up your environment. The following instructions will guide you through the setup in RStudio.

1. **Set Up Your Environment** Make sure you have RStudio installed on your computer.
2. **Install Required Libraries In RStudio**, open a new R console and install the necessary libraries using the following code:
   ```{r}
   install.packages(c("dplyr", "lattice", "corrplot", "gplots", "car", "leaps"))
    ```
**3. Prepare the Data Files**
Make sure to place the necessary data files in the working directory (the folder where your R script is located)


     
