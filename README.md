# ML_Project_Humanitarian_supply_chain_network_Indonesian_Red_Cross_Society
1. Context
In recent years, the frequency and intensity of humanitarian crises have escalated due to various factors such as COVID-19 epidemics, regional wars, climate change, and so on. Humanitarian organizations play an important role in this context.
This project aims to help the Indonesian Red Cross Society (Palang Merah Indonesia, PMI) to optimize its opera- tions and improve its performance through data analytics and artificial intelligence.
One of the most important tasks of PMI is the distribution of emergency supplies to victims in affected areas dur- ing humanitarian crises. PMI operates a humanitarian supply chain network to receive supplies from suppliers and donors, store them in its warehouses during normal times, and deliver them to victims during crises. PMI's warehouse network is divided into three levels, including 1 regional warehouse, 1 provincial warehouse, and 20 district warehouses.
To operate this humanitarian supply chain network, PMI must manage sourcing, transport, replenishment, and distribution activities. And for each type of activity, PMI has two different policies.
  Activity
Sourcing
Transport Replenishment
Distribution
Definition
Assign a warehouse to meet a particular demand of relief supplies, move relief supplies from other warehouses to the assigned warehouse as needed.
Transport relief supplies from warehouses to affected areas and delivering them to victims.
Procure relief supplies from suppliers to maintain adequate inventory levels in the warehouse network.
Decide the order of fulfillment of different demand
                
  Activity
Policy 0
Policy 1
     Sourcing
Transport
Replenishment
Distribution
Hierarchical sourcing: Assign the closest warehouse to meet the particular demand. If needed, the relief supplies can be moved only from upstream to downstream (from regional warehouses to provincial warehouses and from provincial warehouses to district warehouses).
Dedicated delivery: Each transport only have one destination.
Slow replenishment: It takes 15 days to complete the replenishment. The price of the replenishment is cheaper.
First in first out (FIFO): The first received demand is fulfilled first.
Matrix sourcing: Assign the closest warehouse to meet the particular demand. The relief supplies can be moved from any warehouse to the assigned warehouse as needed.
Consolidated delivery: Each transport can have multiple destinations.
Fast replenishment: It takes 3 days to complete the replenishment. The price of the replenishment is more expensive.
Equity: All demands are partially fulfilled by sharing the available relief supplies.
                 PMI has developed a simulation model to simulate its operations and performance under different situation. The simulation is repeated 12,000 times, each corresponding to a specific scenario characterized by the following fea- tures:
The sourcing, transport, replenishment, and distribution policies. (The combination of hierarchical sourcing and consolidated delivery is considered as infeasible.)
Total demand: The total demand of the relief supplies to meet (unit: aid kit)
Initial inventory: The initial inventory in each regional, provincial, and district warehouse (unit: aid kit)
Given a specific scenario, the simulation can output a curve over time of the percentage of demands fulfilled since the beginning of the humanitarian crisis.
According to this output, the experts in PMI defined a performance indicator called the readiness to evaluate the performance. The readiness ranges from 0% to 100% The higher the value, the better the performance. If the readi- ness is 100%, it indicates that PMI is 100% ready to respond to the particular humanitarian crisis in the simulated situation.
PMI now wants to use this simulated dataset (containing 12,000 simulated scenarios) to optimize its operations and performance.
2. Task
1. Develop a deep learning model, predict the final readiness value in advance, up to 10 days after the start of a humanitarian crisis.
Information you can use: the policies, total demand, initial inventory, and the first 10 days demand cov- erage curve
Expected prediction: the readiness.
 
2. Develop a deep learning model, predict the subsequent demand coverage curve, up to 10 days after the start of a humanitarian crisis.
Information you can use: the policies, total demand, initial inventory, and the first 10 days demand cov- erage curve
Expected prediction: the demand coverage curve after the first 10 days, from the 11th day to the end of the crisis (the 24th day).
3. (Optional) Can you develop models that require the shorter wait time after the start of the crisis? For exam- ple, waiting only 5 days instead of 10 days to get the prediction.
