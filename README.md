# Iris Flower Classification Dashboard

## Project Overview

This project demonstrates data analysis, transformation, and visualization skills using the classic Iris flower dataset. The goal was to explore the morphological characteristics (sepal and petal dimensions) of three different Iris species and build an interactive Power BI dashboard to highlight their distinguishing features.

## Dataset

The Iris dataset contains 150 samples of Iris flowers, with measurements for sepal length, sepal width, petal length, and petal width, along with the corresponding species (Iris-setosa, Iris-versicolor, Iris-virginica).
- `Dataset link- (https://archive.ics.uci.edu/dataset/53/iris)
- `iris.data`: Raw dataset. 
- `iris.names`: Dataset description and attribute information.

## Tools Used

* **Power BI Desktop**: For data transformation (Power Query), data modeling, and interactive dashboard creation.

## Data Transformation & Analysis Highlights

1.  **Data Loading & Cleaning**: Loaded the `iris.data` file into Power BI, manually assigned headers (Sepal Length (cm), Sepal Width (cm), Petal Length (cm), Petal Width (cm), Species), and corrected data types.
2.  **Feature Engineering**: Created new calculated columns in Power Query to derive more insightful metrics:
    * `Petal Area (sq cm)` = `Petal Length (cm)` * `Petal Width (cm)`
    * `Sepal Area (sq cm)` = `Sepal Length (cm)` * `Sepal Width (cm)`
    * `Petal Aspect Ratio` = `Petal Width (cm)` / `Petal Length (cm)`
    * And others like `Petal Volume`, `Length Difference`, etc.
3.  **Key Performance Indicators (KPIs)**: Implemented DAX measures for summary statistics, such as `Total Irises`, `Avg Sepal Length`, and `Sum of Petal/Sepal Volume`.
4.  **Data Quality Checks**: Utilized Power Query's column quality and distribution features to ensure data integrity.
5.  **(Optional: If you did scaling/PCA)**: Integrated Python scripts within Power Query to perform data scaling (e.g., StandardScaler) and Principal Component Analysis (PCA) to reduce dimensionality and highlight key variance.

## Dashboard Insights (Power BI Dashboard)

The Power BI dashboard provides a visual narrative of the Iris dataset:

* **Interactive Species Slicer**: Allows users to filter and focus on individual Iris species, dynamically updating all visuals.
* **Petal vs. Petal Scatter Plot**: This is the most differentiating visual. It clearly shows `Iris-setosa` as a distinct cluster with smaller petals, while `Iris-versicolor` and `Iris-virginica` form separate, albeit slightly overlapping, clusters based on their larger petal dimensions. This highlights the strong predictive power of petal characteristics.
* **Sepal vs. Sepal Scatter Plot**: In contrast, this plot demonstrates more overlap between species based on sepal measurements, indicating they are less distinct for classification compared to petals.
* **Distribution Charts**: Bar charts and histograms provide insights into the distribution of each morphological feature across the selected species.
* **Summary Cards (KPIs)**: Provide quick overviews of total counts, average measurements, and calculated volumes.
  
## Result

![WhatsApp Image 2025-06-05 at 22 48 56_515ad452](https://github.com/user-attachments/assets/045d3ff5-822a-4a55-904d-0e1f912cdeac)

