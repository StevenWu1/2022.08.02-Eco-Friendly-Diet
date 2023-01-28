We introduce a framework for recommending environment-friendly diets for average Americans and forecasting the effectiveness of such an approach if it is widely accepted by society. This framework consists of the following major steps: diet optimization, prediction of individual food consumption and US population forecast. 


![image](framework.PNG "Diet Recommendation and Prediction of CO2 Emission Reduction")

- Linear Programming based Diet Optimization: 


In this step, the algorithm determines the optimal environment-friendly diet to meet the basic nutrient requirements of individuals and minimize its CO2 emission. Such an optimization problem can be formulated as a linear programming process, in which we define the essential nutrient consumption as optimization constraints and designate the CO2 emission amount as the optimization goal.   


Assume the major food items in our daily lives include beef, lamb, potatoes and so on. We define variable $X_i$ to represent annual consumption amount of each food item $i$, and $C_i$ to represent the CO2 emission footprint of the food item $i$. Then, $C_i×X_i$ denotes the CO2 emission caused by the food item i every year. The main goal of the algorithm is to minimize the total emission of all the food items in our daily diet $Min(\sum(C_i×X_i)$. 


Let us assume that each unit of the food item i contain a certain amount of nutrient ingredients such as protein and vitamins. We donate $S_i^k≥0$  as the nutrient constitute  $k$ of the food $i$. Nutrient requirement for the ingredient $k$ can be formalized as $n_k≤\sum S_i^kX_i≤n_k^'$, where $n_k$ and $n_k^' represent the lower bound and upper bound for the daily consumption of the ingredient $k$. US Food and Agriculture department releases diet guidelines ever year, which recommends the approximate amount for each ingredient. 
