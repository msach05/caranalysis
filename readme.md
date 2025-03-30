# Practical Application – Module 11: Used Car Price Analysis

## Overview

This project explores what features influence the price of used cars, using a single consolidated dataset for analysis. After building an initial model, the dataset was segmented by **fuel type** to better understand consumer valuation differences across:

- **Gas**
- **Diesel**
- **Electric**
- **Hybrid**
- **Other**

Each segment was analyzed using linear regression, and the resulting model coefficients were compared to determine which features most impact resale value in each fuel category.

---

## Key Insights

### 1. Vehicle Condition
- **"Like new"** and **"good"** condition cars consistently fetch **higher prices**.
- **"Fair"** and especially **"salvage"** condition reduce price across all fuel types.

### 2. Vehicle Type
- **Pickup trucks**, **convertibles**, and **offroad vehicles** increase value, especially for **gas** and **diesel** cars.
- **Hatchbacks**, **mini-vans**, and **wagons** lower prices in most categories.

### 3. Manufacturer Group
- **Luxury brands** (e.g., BMW, Ferrari, Tesla) command strong **price premiums**, particularly in **electric** and **hybrid** markets.
- For **diesel vehicles**, luxury branding surprisingly shows a **negative effect**, possibly due to declining demand.

### 4. Transmission and Drive
- **"Other" or automatic transmissions** typically boost resale price in **electric** and **hybrid** segments.
- **Manual transmissions** show a small positive effect for **hybrids** but are neutral or negative elsewhere.
- **Front-wheel drive (FWD)** is consistently associated with **lower price**, while **RWD** and **AWD** often add value.

### 5. Cylinders (Not Applicable to Electric Vehicles)
- In **gas** and **diesel** cars, **6- or 8-cylinder** engines positively influence price.
- **Electric cars do not have cylinders**, and this feature was not relevant in their analysis.

### 6. Year and Odometer
- **Newer vehicles** are consistently more valuable across all fuel types.
- **Lower mileage** (odometer reading) is a strong price driver, especially for **gas**, **diesel**, and **hybrid** vehicles.

### 7. Paint Color
- **Red** and **yellow** sometimes boost value (notably in **hybrids** and **electrics**).
- **Custom**, **orange**, **green**, and **blue** colors generally reduce price.
- **Neutral colors** like **white**, **grey**, and **silver** vary in impact but are often safer choices.

---

## Strategic Recommendations

Used car dealerships should:

- Prioritize **newer**, **well-maintained** vehicles from **luxury manufacturers**, especially in the electric and hybrid space.
- Favor body types with high resale value (e.g., **pickup trucks** and **convertibles**).
- Avoid vehicles with **high mileage**, **salvage titles**, or **low-demand types/colors**.
- Use **fuel-type-specific insights** when sourcing inventory to align with consumer value drivers.

---

## Files Included

- [`Final_PracticalApplication_Module11.ipynb`](https://github.com/your-username/your-repo-name/blob/main/Final_PracticalApplication_Module11.ipynb): Notebook with the complete analysis.
- Regression coefficient summaries for each fuel type:
  - `coef_summarygas.txt`
  - `coef_summarydiesel.txt`
  - `coef_summaryelectric.txt`
  - `coef_summaryhybrid.txt`
  - `coef_summaryother.txt`
---
