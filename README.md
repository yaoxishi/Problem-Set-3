# Problem Set 3: Clustering via Partitioning

Remember to submit a single rendered PDF or HTML file (either from .Rmd or a Jupyter Notebook) via GitHub **by Friday at 5 pm** in this repo.

1. Load the state legislative professionalism data from the relevant subdirectory in this repo. See the codebook for reference in the same subdirectory and combine with our discussion of these data and the concept of state legislative professionalism from class for relevant background information. 

2. Munge the data: 
* select only the continuous features that should capture a state legislature’s level of "professionalism" (session length (total and regular), salary, and expenditures); 
* restrict the data to only include the 2009/10 legislative session for consistency; 
* omit all missing values; 
* standardize the input features;
* and anything else you think necessary to get this subset of data into workable form (_hint_: consider storing the state names as a separate object to be used in plotting later) 

3. Perform quick EDA visually or numerically and discuss the patterns you see.

4. Diagnose clusterability in any way you’d prefer (e.g., sparse sampling, ODI, etc.); display the results and discuss the likelihood that natural, non-random structure exist in these data.

5. Fit a k-means algorithm to these data and present the results. Give a quick, high level summary of the output and general patterns. Initialize the algorithm at k=2, and then check this assumption in the validation questions below.

6. Fit a Gaussian mixture model via the EM algorithm to these data and present the results. Give a quick, high level summary of the output and general patterns. Initialize the algorithm at k=2, and then check this assumption in the validation questions below.

7. Fit one additional partitioning technique of your choice (e.g., PAM, CLARA, fuzzy C-means, DBSCAN, etc.), and present and discuss results. Here again initialize at k=2.

8. Compare output of all in a visually useful, simple way (e.g., plotting by state cluster assignment across two features like salary and expenditures).

9. Select a single validation strategy (e.g., compactness via min(WSS), average silhouette width, etc.), and calculate for all three algorithms. Display and compare your results for all three algorithms you fit (k-means, GMM, X). 

10. Discuss the validation output. 
* What can you take away from the fit? 
* Which approach is optimal? And optimal at what value of k? 
* What are reasons you could imagine selecting a technically "sub-optimal" partitioning method, regardless of the validation statistics? 
