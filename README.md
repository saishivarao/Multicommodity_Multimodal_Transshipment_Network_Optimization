A MILP optimization problem for optimizing a multicommodity, multi-echelon logistics network
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Porject Title: - Optimizing the flow of Products in Multi-echelon, Multicommodity logistics network.

### Introduction - 
> The objective of this project  to optimize the flow of products in a multi-echelon manufacturing & distribution network. The network below represents flow of multiple steel products, which are transported - from two manufacturing facilities to multiple customer locations, through set of transshipment nodes - using multiple modes of tansportation. 
> 

### Network Structure - 
> ![Network Structure Diagram](https://github.com/saishivarao/Multicommodity_Multimodal_Transshipment_Network_Optimization/blob/main/image.png)
>
> The outbound logistics network of the steel-maker consists of four stages. These stages are - 
>> 1. Mills - Facilities which produce Crude Steel Products
>> 2. External Processing Agents (EPAs) - Facilities which convert the crude steeel products to End Priducts
>> 3. Stockyards (SYDs) - Facilities which store products for the customer as an on-site inventory
>> 4. Customers - Final Consumer of the products
>
> The company bares the carriage, insurance and freight costs.
>
> The Products are moved between facilities using three different modes of transportation - i.e., Railways, Roadways, and Waterways.
>
> Crude Steel Products are converted to End Products at the EPAs, based on a pre defined conversion rule. The coversion rule is defined in form of matrix, where the Crude steel products can be converted to multiple End Products based on the chemical composition.
>
> End Products manufactured at the EPA are either directly shipped to the customer or they are stored at the stockyard as an on-site inventory for the customer. This routing is determined by the SLA agreement signed with customer, which specifies the precentage of total demand that the customer wishes to procure directly (i.e. Shipment from EPAs) and the percentage of total demand that the customer wishes to procure indirectly (i.e. Shipment from Stockyards).


To optimize the flow of material in the network, I developed an MILP optimization algorithm with an objective to minimize the cost-to-serve a customer order. The Problem is solved using Pyomo library in Python.

### Files in the Repo - 
> 1. Jupyter notebook file - contains a Pyomo Code of the optimization problem
> 2. Excel File - Input data file used in Jupyter notebook
> 3. Image File - Provides image of the Outbound Logistics network of the steel maker
