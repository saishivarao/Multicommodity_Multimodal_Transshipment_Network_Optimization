# Multicommodity_Multimodal_Transshipment_Network_Optimization
A MILP optimization problem for optimizing a multicommodity, multi-echelon logistics network
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Porject Title: - Optimizing the flow of Products in Multi-echelon, Multicommodity transsportation network.

### Introduction - 
> The objective of this project  to develop an optimal design for outbound logistics network of a major steel-maker in India. The network represents flow of multiple steel products, which are transported - from two manufacturing facilities to multiple customer locations across the country - using multiple modes of tansportation. 
> 
> To optimize the flow of material in the network, I developed an MILP optimization algorithm with an objective to minimize the cost-to-serve a customer order. The Problem is solved using Pyomo library in Python.

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

### Costs in Outbound Logistis network - 
> Facility Costs -
>> 1. Variable handling at EPAs - Material Handling Cost, etc.
>> 2. Fixed cost of EPAs - Per annum Cost of Using a Facility
>> 3. Product conversion cost of EPAs - Per ton cost of Converting a Crude Steel Product to End Product at an EPA
>> 4. Variable handling cost of Stockyards - Material Handling Cost, etc.
>> 5. Fixed cost of Stockyards - Per annum Cost of Using a Facility
>> 6. Variable handling cost of Ports - Per ton cost of handling products at port

### Files in the Repo - 
> 1. Jupyter notebook file - contains a Pyomo Code of the optimization problem
> 2. Excel File - Input data file used in Jupyter notebook
> 3. Image File - Provides image of the Outbound Logistics network of the steel maker
