# data-visualization-challenge

OBSERVATIONS:

1. Look at "# Generate a line plot of tumor volume vs. time point for a single mouse treated with Capomulin"*
   
   In this line plot, we can observe the effectiveness of Capomulin treatment in our mouse 'l509'. As we can see, the volume of the tumor is increasing in the first 20 days. It's up to that moment when we start seeing the results of the treatment. For the first 15 days, we can see an exponential decrease in the volume of the tumor, reflecting the success of this drug regimen. Nevertheless, from day 35 onwards, the tumor starts growing in our mouse again. As a conclusion of this graphic, we can say that Capomulin treatment has a certain amount of success, but over time, the tumor has a tendency to grow.
   
2. Look at "Correlation and Regression"*

   The correlation between mouse weight and average tumor volume is 0.83. Since our number is very close to 1, we can conclude that these two variables have a strong relationship, meaning as one value increases, the other value also increases. We can see in our graphic that as the weight increases in our mice, the volume of the tumor also increases. 
   Our linear regression allows us to understand trends: the heavier the mouse, the larger the tumor. Additionally, by calculating these two variables, we can gain insight into how these factors are related in the context of Capomulin treatment. We were able to quantify how much the tumor volume changes with changes in mouse weight for mice treated with Capomulin.
   
3. Look at "# Generate a box plot that shows the distrubution of the tumor volume for each treatment group."*
 
   This graphic allows us to see the success in different drug regimes. As our first conclusion, we observe that 'Capomulin' and 'Ramicane' have the best rate of success when treating tumors, because the final tumor volume has a range of 20mm³ to 50mm³. On the other hand, our 'Infubinol' and 'Ceftamin' treatments have a greater range of final volume, although we find a noticeable outlier in the Infubinol treatment; this could be due to a response in one of the mice. This graphic gives us a clear insight into which treatments could be more useful due to their success.
   
   

  # References
  
  There is part of the code where I used ChatGPT.
  
  1. cleaned_df = combine_data[~combine_data['Mouse ID'].isin(duplicated_mouse_ids)]
cleaned_df.head()

I used AI to help me with "~", this is what it says:
   "So the goal of ~ in this part of the code is to select rows where the "Mouse ID" is not in the list of duplicated_mouse_ids, effectively removing those rows from the cleaned_df DataFrame."
   
   2. for treatment in treatments:
   
      tumor_volumes = merged_df.loc[merged_df['Drug Regimen'] == treatment, 'Tumor Volume (mm3)']
      
      tumor_vol.append(tumor_volumes)
   
I used AI to help me create the for loop since I was getting different errors

----------------------------------------------------------------------
