### Project Description

#### Problem Statement
You are working for "GlavRosGosOil", a mining company, and your task is to decide where to drill a new oil well. The typical steps for selecting a location are as follows:
1. Collect characteristics for wells in the chosen region: oil quality and reserves.
2. Build a model to predict the volume of reserves in new wells.
3. Select wells with the highest predicted values.
4. Determine the region with the highest total profit from the selected wells.

You have samples of oil wells in three regions. The characteristics for each well in the region are already known. Build a model to determine the region where extraction will bring the highest profit. Analyze potential profit and risks using the Bootstrap technique.

#### Data Description
- Geological exploration data for three regions are located in:
  - `/datasets/geo_data_0.csv`
  - `/datasets/geo_data_1.csv`
  - `/datasets/geo_data_2.csv`
  
- **Columns:**
  - `id` — unique well identifier
  - `f0`, `f1`, `f2` — three features of points (important for model training)
  - `product` — volume of reserves in the well (thousand barrels)

#### Task Conditions
- Only linear regression is suitable for model training.
- During exploration, 500 points are studied, from which 200 best are selected using machine learning for development.
- The budget for well development in each region is 10 billion rubles.
- At current prices, one barrel of oil brings 450 rubles in revenue. Hence, revenue from a unit of product is 450,000 rubles (since volume is in thousand barrels).
- After assessing risks, retain only regions where the risk of losses is less than 2.5%. Among these, select the region with the highest average profit.

#### Note
The data provided is synthetic, and specific details of contracts and deposit characteristics are not disclosed.
