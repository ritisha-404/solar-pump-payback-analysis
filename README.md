# Solar Pump Payback Analysis

A Databricks-based analytical project comparing the indicative economics of a
5 kWp solar irrigation pump with a diesel pump across selected talukas in
Pune district.

> **Note:** This is an illustrative payback model. Cost, subsidy, operating,
> and performance inputs are assumptions and should not be interpreted as a
> site-specific engineering or financial feasibility study.

## Objective

The project estimates:

- Solar energy generation
- Solar energy coverage of pump demand
- Annual diesel operating cost
- Estimated annual savings from solar
- Farmer capital expenditure under a subsidy scenario
- Indicative payback period with and without subsidy

## Locations

The analysis covers four talukas in Pune district:

- Baramati
- Indapur
- Junnar
- Khed

## Data

Solar radiation data is obtained from the **NASA POWER API** and used to
estimate solar energy generation for the selected locations.

## Architecture

```text
NASA POWER API
      ↓
Bronze Layer
      ↓
Silver Layer
      ↓
Gold Analytical Table
      ↓
Databricks SQL
      ↓
Dashboard
