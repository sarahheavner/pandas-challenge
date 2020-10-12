# pandas-challenge - Heroes of Pymoli Analysis

    OBSERVABLE TRENDS:
    
        1 - Heroes of Pymoli (HOP) is far more popular amongst players who identify as Male then it is amongst players who identify as                   Female or other/Non-Disclosed. 84% of HOP players identify as Male. Male indentified players also lead considerably in HOP game             purchases, both in number of purchases and dollars spent - 652 out of the 780 total purchases (equaling 83.5% of the game                   purchases), as well as $196,764 out of $237,977 (82.6%  of game purchase revenue).
        2 - HOP is most popular amongst the age ranges of 15-29 (76.74% total) - with 44.79% of total players between 20-24 in age, 18.58%               between 15-19, and 13.37% between 25-29. Dollars spent per age range also follow a similar trend - 46.8% for 20-24, 17.3% for               15-20, and 12.3% for 25-29.
        3 - "Final Critic", "Oathbreaker, Last Hope of the Breaking Storm", and "Fiery Glass Crusader" are amonsgt the most commonly                     purchased items, as well as most profitable. 
        
        
        
        
        
        
# pandas-challenge - Heroes of Pymoli Homework Notes

        - Assignment Goals
           -Import csv file and create dataframe
           - Purchasing analysis
               - Calculated # of items, total purchases, average price, total revenue
               - Created dataframe to display results
           - Count total number of players
               - Used nunique() function in case there were duplicate values in SN field
           - Determine count and percentage of players based on gender
               - Used drop_duplicates() function to create new dataframe with correct count
               - percentage = (gender count / number of players) * 100
               - Created new data frame to display results
               - Added formatting to % for percentage column
           - Calculate purchase count, avg. purchase price, avg. purchase total per person by gender, avg purchase per person
               - Used pre-"drop_duplicates" dataframe 
                   - groupby Gender to calculate count of purchases per gender
                   - groupby Gender to calculate average purchase price per gender 
                   - total gender purchases = count of gender purchases * average purchase price
                   - avg purchase per person = (total gender purchase / number of players) 
               - Created new dataframe to display results
               - Added formatting to $ and 2 decimal places
           - Determine count and percentage based on age
               - Created bins for age ranges specified on assignment
               - Created group names for my bin ranges 
               - Used pd.cut to assign a bin to each row based off of age 
               - Calculated count for each age group
               - percentage = (age count / number of players) * 100
               - Created new dataframe to display results
               - *Note* had to sort dataframe by index, if not the summary was displaying out of order and sorting descending by                             count/percentage
               - Added formatting to % for percentage column
           - Calculate purchase count, avg. purchase price, avg. purchase total per person by gender, avg purchase per age group
               - Used pre-"drop_duplicates" dataframe 
                   - groupby Age Group to calculate count of purchases per gender
                   - groupby Age Group to calculate average purchase price per gender 
                   - total Age Group purchases = count of gender purchases * average purchase price
                   - avg purchase per person = (total Age Group purchase / number of players)  
               - Created new dataframe to display results
               - Added formatting to $ and 2 decimal places
           - Calculate to obtain purchase count, average purchase price, and Total Purchase Price per SN
               - Used pre-"drop_duplicates" dataframe 
                   - groupby SN to calculate count of purchases per player
                   - groupby SN to calulcate average purchase per player
                   - total purchase = count of SN purchases * average purchase per SN
               - Created new dataframe to display results
               - Sorted ascending by purchase count
               - Added formatting to $ and 2 decimal places
           - Calculate popularity of items 
               - Created new dataframe with only Item ID, Item Name, and Item Price columns
               - Group by Item ID and Item Name. Perform calculations to obtain purchase count, average item price, and total purchase value
                   - Groupby Item ID and Item Name to calculate count of purchases per Item
                   - Groupby Item ID and Item Name to calculate average item price
                   - Total purchase value = purchase count * average item price
               - Created dataframe to display results
               - Sorted descending by purchase count
               - Added formatting to $ and 2 decimal places
           - Calculate most profitable item
               - Used un-sorted dataframe created above
                   - Changed sort to total purchase value
               - Created new dataframe to display results
               - Added formatting to $ and 2 decimal places
               
              
                   
                  

                
                
                   
                
                
                    
              
                
               
           
      
        

