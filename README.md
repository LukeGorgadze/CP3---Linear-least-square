# CP3 Linear least square
 
## My ideas for this project:
* Predicting average lifespan of humans with the amount of their sleep and relevant life habits that are related to their health
* Predicting income based on age. The model could be used to make predictions about a person's income at different ages, or to understand the relationship between age and income depending on the time person dedicates to work or studying while constraining the index of individual's profession (In simple terms, how much it's related to tech on the scale of 0-10).

## Generating synthetic data
> I generate artificial data of people since it's not publicly available, as it would contain lifestyle of people and their life habits and revealing one's private information to public is nor ethical or morally correct.

> However, My program will work fine in case of being provided real data.

## Implementation Phase:
### Idea 1:
 For idea 1, I have created Human class with parameters fullName, gender, sleepTime, workOutHrs and I've came up with my own equation which tells me how long each person will probably live.

 Then, I generate 100 humans with random attributes and for each of them calculate their predicted age. I make matrix A out of all these people (I write their property values as rows) then solve x by normal equation,modified gram schmidt or HouseHolder depending on user's input.

 Running the program will make a prediction of maxium age - John Doe - (default character) will reach, then you'll see predictions for 50 new people by using our x vector.


### Idea 2:
For idea 2, I have a Human class with parameters: age, fullName, gender, workHrs, studyHrs, techIndex and an equation which tells me how much income a person has depending on these parameters.

I generate 100 humans and for each of them calculate income. Then i turn this humans into matrix A and solve x by modified gram schmidt or House holder with linear least squares with equality constrains.


 Running the program will make a prediction of income - John Doe - (default character) has, then you'll see predictions for 50 new people by using our x vector.

<hr/>

 ## Note
 **LukaUtils** is a python library i created for myself and this file includes all the necessary algorithms we had to implement for this computational project.

 I used Sauer's textbook to study and implement algorithms on my own.
