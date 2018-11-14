# This homework assignment was to make a "Friend Finder" application. 
*I themed this app to "Find an "evil genius" finder just to make it fun.*

The application is to first take in the name and the image URL of a new "friend".
Then 10 questions are asked of this person. 10 Questions where they have the ability to choose how strongly they agree or disagree (from 1 to 5) with the question.

When the user finishes the quiz, the answers are compared to the 10 "evil" friends stored in the friends.js file. The evil friend that is most compatable will be displayed in a modal.

The server.js file will make the  connections with port and set up the two requires, express and path. Server.js will also require the two route files, API and html.

*The apiRoutes.js has to handle the get and post requests as well as handle the logic.*
The new user input has to be made into an object, then the results of the quiz has to be compared to the scores of the 10 preloaded "evil" friends. 
The math.abs() method is the way we will obtain the absolute value difference between the user input and the evil friend scores. 
We need to make a for loop to iterate through the array of evil friends, then another for loop that will iterate the evil scores. These values are parsed as intergers and the absolute value of each answer is totalled for each evil person vs the user scores.
The lowest absolute value of the evil person will be conisderd the best match and that value is posted to the body. The modal will grab the AJAX post and place the name and the URL of the bestmatch and display it. 






