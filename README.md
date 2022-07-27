# MealDB

- [Api docs](https://themealdb.com/api.php)
- [WireFrames](https://whimsical.com/meals-db-L2Q6N79JbBY6AqaskSWcdY)



#Acceptance Criteria:

- While the splash screen is being shown, check to see whether or not the user has used the app before. If so, pass the last selected filter option (Category, Area, Ingredients, Saved) to the HomeScreen fragment so it can pass the last selected category to the filtered list fragment to immediately be displayed. If not, just send them to the HomeScreen fragment to select how they would like to filter the meals.
- At the homescreen fragment, if there was a filtering option sent, move directly to the filter list fragment, sending the last selected category along.
if there is no filtering option sent, display the welcome screen with the list of filtering options for the user to choose from. Upon selection, save the user's selection (key-value pair) for next time and send the user to the filter list fragment along with their selection.
- In the filter list fragment, display the filtering option at the top of the page. Take the list of filtered options from the network and display them in a recycler view for the user to choose from, user should be able to see all data attributes (individual string or object), if the text data  doesnt fit in 3 lines, place an ellipses at the end to indicate to the user they need to press it to get more information. When the user clicks on the recycler view item, the user should be able to view a list of meals that fit the filter in the Meal List Fragment
- In the meal list Fragment,
