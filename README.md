# Nashville Housing Data Cleaning

**Project Type:** SQL Data Cleaning  
**Dataset:** Nashville Housing Dataset  

---

## Overview
This project demonstrates cleaning and organizing the Nashville Housing dataset using SQL. The goal was to ensure data consistency, remove duplicates, standardize values, and prepare the dataset for analysis.

---

## Steps Performed
1. **Initial Data Checks**
   - Reviewed all rows and columns
   - Counted total records
   - Checked for duplicate ParcelIDs and key columns
   - Identified missing or NULL values

2. **Data Cleaning**
   - Updated empty `PropertyAddress` fields by joining on `ParcelID`
   - Converted `SaleDate` to a proper DATE format
   - Split `PropertyAddress` into `PropertyStreet` and `PropertyCity`
   - Split `OwnerAddress` into `OwnerStreet`, `OwnerCity`, and `OwnerState`
   - Standardized `SoldAsVacant` values (`Y/N → Yes/No`)

3. **Removing Duplicates**
   - Identified duplicates based on `ParcelID`, `PropertyAddress`, `SalePrice`, `SaleDate`, `LegalReference`
   - Removed duplicate rows while preserving unique records

---

## How to Use
1. Open the SQL script in this repository: [`SQL`](SQL)  
2. Run the queries in your preferred SQL environment (MySQL recommended)  
3. Observe results for cleaned and validated data

---

## Tableau Dashboard

Interactive visualization created using the cleaned Nashville Housing dataset.

🔗 **View Interactive Dashboard:**  [https://public.tableau.com/app/profile/justincha/viz/NashvilleHousingDataCleaningVisualizationSQLTableau/Dashboard1?publish=yes]

---

## Portfolio Context
This project demonstrates key data analyst skills:
- SQL data cleaning and transformations  
- Handling NULLs and duplicates  
- Standardizing and parsing address data  
- Preparing datasets for analysis or visualization
- Visualization of dataset in Tableau
