# MealDB

- [Api docs](https://themealdb.com/api.php)
- [WireFrames](https://whimsical.com/meals-db-L2Q6N79JbBY6AqaskSWcdY)



#Acceptance Criteria:

- While the splash screen is being shown, check to see whether or not the user has used the app before. If so, pass the last selected filter option (Category, Area, Ingredients, Saved) to the HomeScreen fragment so it can pass the last selected category to the filtered list fragment to immediately be displayed. If not, just send them to the HomeScreen fragment to select how they would like to filter the meals.
- At the homescreen fragment, if there was a filtering option sent, move directly to the filter list fragment, sending the last selected category along.
If there is no filtering option sent, display the welcome screen with the list of filtering options for the user to choose from. Upon selection, save the user's selection (key-value pair) for next time they open the app and send the user to the filter list fragment along with their selection.
- In the filter list fragment, display the filtering option at the top of the page. Take the list of filtered options from the network and display them in a recycler view for the user to choose from, user should be able to see all data attributes (individual string or object), if the text of the data attribute  doesnt fit in 3 lines, place an ellipses at the end to indicate to the user they need to press it to get more information. When the user clicks on the recycler view item, the user should be able to view a list of meals that fit the filter in the Meal List Fragment
- In the meal list Fragment, the chosen filter (ex. the "Beef" Category) should be displayed at the top with the full description that was cut off in the previous fragment. Below the description should be a list of the meals in that category with a picture to show what it looks like along with the name of the meal. Clicking on any of the meal items should send the user to the meal detail fragment with details of the selected dish and how to make it.
- The meal detail fragment should take a meal as an argument and display its contents. It should have a picture of what it should look like, the ingredients necessary to make the dish as well as the instructions on how to cook the dish. User should be able to select this meal as one of their favorites to be viewed later.
- Each Fragment after the home screen should have the ability to go to the previous fragment.
- Use Retrofit for your network requests and add a logging interceptor so you can see the actual network requests made in your logcat.
- User should be able to save their favorite meals from the details screen and view them whenever they select the "Saved" filtering option on the home page.
- Be sure to leverage Kotlin's features like scope functions, extension functions and higher order functions as well as data classes and sealed classes/ enums to help manage state.
- Make sure that your code follows the SOLID principles and has been refactored to be DRY.
