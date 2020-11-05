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

> The steel-maker is completely bares the carriage, insurance and freight costs for each custmer order.

> The Products are moved between facilities using three different modes of transportation - i.e., Railways, Roadways, and Waterways.

> Crude Steel Products at the EPAs, are converted to End Products based on a pre defined conversion rule. The coversion rule is defined in many to many type of matrix, where each End Product can be converted from multiple Crude steel products, and vice-versa.

> 


The Jupyter notebook file present in the repository contains a Pyomo Code of a MILP problem to optime the multicommodity multimodal transshipment network.
