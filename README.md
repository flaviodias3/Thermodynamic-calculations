# SEPR Calculation Application

This application is designed to calculate the Seasonal Energy Performance Ratio (SEPR) for process chillers based on the EN14825:2022 standard. The application uses various libraries such as Pandas and Numpy for data manipulation and analysis.

## Features

1. **Data Handling and Processing**:
   - Utilizes Pandas for data manipulation and analysis.
   - Supports various data formats including DataFrames.

2. **SEPR Calculation**:
   - Calculates SEPR based on the EN14825:2022 standard.
   - Includes calculations for part load conditions, cooling demand, efficiency ratios, and degradation coefficients.

3. **Power Input Correction**:
   - Corrects power input based on EN14511-3:2018 standard.
   - Includes calculations for pump efficiency and power input correction factors.

4. **Degradation Coefficient Calculation**:
   - Calculates degradation coefficient (CD) based on EN14825:2022 and EN14511-3:2018 standards.
   - Includes calculations for corrected power input during compressor-off state.

## Libraries Used

- pandas
- numpy

## Application Structure

The application is structured into various sections including:

1. **Introduction**: Provides an overview of the SEPR calculation.
2. **Parameters Input**: Defines the input parameters for the calculations.
3. **Part Load Conditions**: Calculates cooling capacity, pump flow rate, external static pressure, and power input for different part load conditions (A, B, C, D).
4. **Bin Temperature and Hours**: Defines bin temperature and hours based on EN14825:2022.
5. **Process Cooling Load**: Calculates process cooling load at a given temperature.
6. **Efficiency Calculation**: Defines functions to calculate pump efficiency based on power.
7. **Power Input Correction**: Calculates power input correction factors based on pump efficiency.
8. **Degradation Coefficient Calculation**: Calculates degradation coefficient (CD) based on corrected power input during compressor-off state.
9. **Capacity Ratio Calculation**: Calculates capacity ratio (CR) based on part load ratio and declared capacity.
10. **Efficiency Ratio Calculation**: Calculates efficiency ratio (EER) based on declared capacity and corrected power input.
11. **SEPR Calculation**: Calculates SEPR based on bin hours, cooling demand, and efficiency ratios.

## Usage

To run the application, execute the following command:

```bash
python app.py
