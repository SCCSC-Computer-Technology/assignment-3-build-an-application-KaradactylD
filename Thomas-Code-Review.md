***First Impression***<br/>
Upon running the program I found no major errors. I like how it is themed around turtles and was sort of game-like. I also like the details form design a lot.
<br/><br/>
***Form1 Code***<br/>
I found that everything is well documented. I saw your comment in the GetStates() method about pulling the state names from the database. It is possible to pull the names from the database, just select the combo box, click the arrow in the top-right, check the use data bound items, select your binding source, select the state name column for the display field, and select the state ID column for the value member field. 
<br/><br/>
***StateDetails Form Code***<br/>
I found that there was sufficient documentation for this form. In the prevBtn_Click and nextBtn_Click events, I noticed that the code could be turned into a method that accepts a lamba expression as an argument, which can be used to perform the index calculation. In the DisplayInfo() and LoadStateList() methods, I noticed a lack of try-catches for the SqlConnection and SqlCommand operations, which may lead to the program crashing.
<br/><br/>
***MoreDetails Form Code***<br/>
I found this form to be well-documented. I saw that there are two click events for button1, likely due to adding the event handler before renaming the button. To rename these events, right click on the name and click rename.
<br/><br/>
***Testing***<br/>
I noticed that when an invalid value, such as “ashdja” in the population column, is entered into the datagrid in the MoreDetails form, an error message displays that can be hard for a user to read. To fix this, handle the invalid value in the data error event.
I also noticed that when a change is made to the data in the datagridview, it does not save despite clicking the save button in the navbar.
<br/><br/>
***Comparing solutions***<br/>
In my solution, I used LINQ to SQL to work with the database. However, I do like the more hands-on approach to handling SQL used in the solution. In terms of tradeoffs, I find LINQ queries to be a little quicker to write and easier to read than using SqlCommands, so I will stick to my LINQ queries when I can.
<br/><br/>
***Additional Comments/Questions***<br/>
Is there a reason why you change the appearance of controls in your form constructors instead of in the properties pane, or is it just a preference?
