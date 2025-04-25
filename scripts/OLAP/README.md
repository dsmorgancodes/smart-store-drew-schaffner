# Section 1. The Business Goal
My business goal is to figure out which category was the most popular category in each region. 

# Section 2. Data Source
I will use my smart_sales.db. Specifically, the following tables will be used: 
customer, sales, products. 

# Section 3. Tools Used
I will use python, spark, a jupyter notebook, seaborn, and matlplotlib. 

# Section 4. Workflow & Logic
My data is somewhat segmented. The foreign ids in the sale database are used to form a joined table that contains all the data that is needed. Once this join occurs python is used to query the data and make calculations. The data for sale by category is rolled up into a summary for each cateogory. Then, this is further explored by breaking down each region and summing category sales by region. The results and then visualized using seaborn. 

# Section 5. Results (narrative + visualizations)
This image here shows that the most profitable region is the Eastern Region.

![This image shows that the Eastern Region is the most profitable region.](images/Profit%20by%20Region.png)

This image here shows that the profitable product category in the Eastern Region is: Electronics.

![This image shows the profitabilty of each category by region](images/Profit%20by%20Category%20By%20Region.png)

# Section 6. Suggested Business Action
There is a myriad of business actions that one could take based on these findings. But I think that the most important one is this: Collect more data. 

If I was given the data in this table to conduct a study on, I would ask for more data.

# Section 7. Challenges
SPARK. I'm not sure if there is another tool available to SPARK. But SPARK gives my computer an absolute bear of a time. It crashes, it's inconsistent. I would quite frankly love to have learned a different tool than this one. If other Mac Users have found one out there. I'd love to know about it. I've found the following tools: DASK, RAY, Google Cloud DataFlow. I've briefly used DASK. 

# Section 8. Ethical Considerations
I'm not sure if this data could be used to reinforce biases. But I know for a fact that AI has been used to reinforce biases. I think that one of the issues our generation will face is figuring out how to route out the unfair or innappropriate biases. For one, how do we even go about identifying these biases? I think that one of the ways we should do this is by examining our own biases. We built these models, naturally, whatever truth they do have, will be somehow tainted by our biases. 

There is truth out there, and biased or not, sometimes it takes a little bit of work to find it. 