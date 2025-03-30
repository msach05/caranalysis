# Practical Application – Module 11: Used Car Price Analysis

## Overview

This project explores what features influence the price of used cars, using a single consolidated dataset. The dataset contains over **420K (originally)** used vehicle listings with information on:

- Vehicle **price**
- **Manufacturer**
- **Fuel type** (gas, diesel, electric, hybrid, other)
- **Condition** (new, like new, good, fair, salvage)
- **Year**, **odometer reading**, **body type**, **paint color**
- **Title status**, **transmission**, **drive type**, and more

### Data Cleaning Summary

To prepare the data for modeling:
- **Missing or irrelevant values** were removed, especially rows with null prices or odometers.
- **Categorical variables** (e.g., condition, manufacturer group, fuel type) were encoded for regression modeling.
- Outliers and unrealistic entries (e.g., prices at or below $100 or odometer readings at zero) were filtered out.
- The cleaned dataset was then segmented by **fuel type** to explore how pricing drivers vary across different kinds of vehicles.
- The data after cleaning up ended up with 380K rows.
---

## Key Insights

### 1. Vehicle Condition
- **"Like new"** and **"good"** condition cars consistently fetch **higher prices**.
- **"Fair"** and especially **"salvage"** condition reduce price across all fuel types.

### 2. Vehicle Type
- **Pickup trucks**, **convertibles**, and **offroad vehicles** increase value, especially for **gas** and **diesel** cars.
- **Hatchbacks**, **mini-vans**, and **wagons** lower prices in most categories.

### 3. Manufacturer Group
- **Luxury brands** (e.g., BMW, Tesla, etc) command strong **price premiums**, particularly in **electric** and **hybrid** markets.
- For **diesel vehicles**, luxury branding surprisingly shows a **negative effect**, possibly due to declining demand.

### 4. Transmission and Drive
- **"Other" or automatic transmissions** typically boost resale price in **electric** and **hybrid** segments.
- **Manual transmissions** show a small positive effect for **hybrids** but are neutral or negative elsewhere.
- **Front-wheel drive (FWD)** is consistently associated with **lower price**, while **RWD** and **AWD** often add value.

### 5. Cylinders (Not Applicable to Electric Vehicles)
- In **gas** and **diesel** cars, **6- or 8-cylinder** engines positively influence price.
- **Electric cars do not have cylinders**, and this feature was excluded from their analysis.

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
---

## Notebook

- 📘 View the full analysis in the Jupyter notebook:  
  [`Final_PracticalApplication_Module11.ipynb`](https://github.com/msach05/caranalysis/blob/main/Final_PracticalApplication_Module11.ipynb)

---