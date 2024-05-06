# ML_Project_Humanitarian_supply_chain_network_Indonesian_Red_Cross_Society
This project aims to help the Indonesian Red Cross Society (Palang Merah Indonesia, PMI) optimize its operations and improve its performance through data analytics and artificial intelligence.

One of the most important tasks of PMI is the distribution of emergency supplies to victims in affected areas during humanitarian crises. PMI operates a humanitarian supply chain network to receive supplies from suppliers and donors, store them in its warehouses during normal times, and deliver them to victims during crises. PMI's warehouse network is divided into three levels, including 1 regional warehouse, 1 provincial warehouse, and 20 district warehouses.

![Screenshot 2024-05-06 at 2 53 31 PM](https://github.com/Hemin19/ML-Project---Humanitarian-supply-chain-network-Indonesian-Red-Cross-Society-/assets/88471700/17d0a1fa-7b6f-4195-bf1d-e609c56bbb99)

To operate this humanitarian supply chain network, PMI must manage sourcing, transport, replenishment, and distribution activities. And for each type of activity, PMI has two different policies.

![Screenshot 2024-05-06 at 2 55 33 PM](https://github.com/Hemin19/ML-Project---Humanitarian-supply-chain-network-Indonesian-Red-Cross-Society-/assets/88471700/37034acb-fba2-46a1-83c2-db100ae870f5)

PMI has developed a simulation model to simulate its operations and performance under different situations. The simulation is repeated 12,000 times, each corresponding to a specific scenario characterized by the following features:
- The sourcing, transport, replenishment, and distribution policies. (The combination of hierarchical sourcing and consolidated delivery is considered as infeasible.)
- Total demand: The total demand of the relief supplies to meet (unit: aid kit)
- Initial inventory: The initial inventory in each regional, provincial, and district warehouse (unit: aid kit)

Given a specific scenario, the simulation can output a curve over time of the percentage of demands fulfilled since the beginning of the humanitarian crisis. According to this output, the experts in PMI defined a performance indicator called readiness to evaluate the performance. The readiness ranges from 0% to 100% The higher the value, the better the performance. If the readiness is 100%, it indicates PMI is 100% ready to respond to the particular humanitarian crisis in the simulated situation. PMI now wants to use this simulated dataset (containing 12,000 simulated scenarios) to optimize its operations and performance

![Screenshot 2024-05-06 at 2 58 39 PM](https://github.com/Hemin19/ML-Project---Humanitarian-supply-chain-network-Indonesian-Red-Cross-Society-/assets/88471700/4563251d-24b5-48c0-ae69-c48e61d86ea5)
