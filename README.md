# Multicommodity_Multimodal_Transshipment_Network_Optimization
A MILP optimization problem, for optimizing a multicommodity, multimodal, transshipment network
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

This repository contains files from my internship project at one of India's largest steel-maker. 
Porject Title: - Optimizing the flow of Products in Multi-echelon, Multimodal transshipment network.

### Introduction - 
> The objective of this project was to develop an optimal design of outbound logistics network for a major steel-maker in India, The outbound logistics network of the steel maker had multiple products, which were to be routed from various facilities to multiple customer locations in the countries, using multiple modes of tansportation. To optimize the design of outbound logistics network, we developed an MILP optimization algorithm with an objective to minimize the cost-to-serve a customer order. The Problem is solved using Pyomo library in Python.

### Network Structure - 
> The outbound logistics network of the steel-maker consists of four stages, including the customer. These stages are - 
>> 1. Mills - Facilities which produce Crude Steel Products
>> 2. External Processing Agents (EPAs) - Sub-contracted Facilities which convert the crude steeel products to End Priducts
>> 3. Stockyards (SYDs) - Sub-contracted Facilities which store products for the customer as an on-site inventory
>> 4. Customers - Final Consumer of the products
>
> The steel-maker completely bares the carriage, insurance and freight costs for delivering a each custmer order.
>
> The Products are moved between facilities using three different modes of transportation - i.e., Railways, Roadways, and Waterways.
>
> Crude Steel Products at the EPAs, are converted to End Products based on a pre defined conversion rule. The coversion rule is defined in many to many type of matrix, where each End Product can be converted from multiple Crude steel products, and vice-versa.
>
> End Products manufactured at the EPA are either directly shipped to the customer or are stores at the stockyard as an on-site inventory for the customer. This routing is determined by the SLA agreement signed with customer, which specifies the precentage of total demand that the customer demands under direct shipment (i.e. Shipment from EPAs) and the percentage of total demand that the customer demands indirectly (i.e. Shipment from Stockyards).

### Costs in Outbound Logistis network - 
> Facility Costs -
>> 1. Variable handling at EPAs - Material Handling Cost, etc.
>> 2. Fixed cost of EPAs - Per annum Cost of Using a Facility
>> 3. Product conversion cost of EPAs - Per ton cost of Converting a Crude Steel Product to End Product at an EPA
>> 4. Variable handling cost of Stockyards - Material Handling Cost, etc.
>> 5. Fixed cost of Stockyards - Per annum Cost of Using a Facility
>> 6. Variable handling cost of Ports - Per ton cost of handling products at port

### Files in the Repo - 
> Jupyter notebook file - contains a Pyomo Code of a MILP problem to optime the multicommodity multimodal transshipment network.
> Excel File - Input data file used in Jupyter notebook
> Image File - Provides image of the Outbound Logistics network of the steel maker
