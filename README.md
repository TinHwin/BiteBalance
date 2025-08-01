# BiteBalance

https://github.com/UML-COMP4630-LIN/project-bitebalance

**Description**
BiteBalance is an all-in-one meal planning mobile app designed for college students and budget-conscious individuals to promote healthy, affordable home cooking. Developed by Team 08, the project aimed to address the challenges of expensive and unhealthy dining out by providing a free, user-friendly app that suggests personalized recipes based on dietary preferences, budget, and calorie goals. The app was built using React Native with TypeScript for cross-platform compatibility, Firebase Firestore for user data storage, Google Authentication for secure login, and the Spoonacular API for recipe data. Key features include recipe search with filtering system, recipes recommendation based on user preferences, weekly meal planning, nutritional and cost tracking, and an ingredient checklist. The project faced challenges with API integration and development setup but was enhanced through user feedback, incorporating improved readability and a dynamic calendar system. The team learned technical skills like React Native and Firebase, and non-technical skills like collaboration, overcoming obstacles through regular communication and iterative testing. This report details the project's purpose, methodology, results, challenges, and lessons learned, highlighting BiteBalance's potential to simplify meal planning for its target audience. And we hope to improve this over time with more refinement and debugging of the app.

**Features**

<img width="545" height="410" alt="Screenshot 2025-08-01 at 5 21 47 PM" src="https://github.com/user-attachments/assets/ab3270aa-d1f1-41de-82e7-23fe6e1b36c7" />

<img width="538" height="808" alt="Screenshot 2025-08-01 at 5 22 12 PM" src="https://github.com/user-attachments/assets/036ae0ac-4c76-48e4-b8f0-393195cfb67a" />

**Recipe Search**
Users can search for any recipes by writing in the search bar. The search results will be filtered based on user preferences they’ve entered. This means that if the users  had a certain diet or intolerances, the recipe will not contain those ingredients that can affect the user. However, if the user entered ingredients they liked, the recipe will have ingredients they liked in the recipe. The recipe will be fetched using the Spoonacular API.

**Recipe Recommendations**
Users can generate recipe recommendations for Breakfast, Lunch, and Dinner. These recipes will be filtered based on user preferences, which means it can filter out what they can’t eat or don’t want and add ingredients they want. 

**Dynamic Calendar System**
Displays recipes on a calendar with 7-day/full-month toggle, synced across screens using `currentMonth` in `AppContext`.

**Saving Recipes and User Preferences to storage**
Saves recipes to specific dates and user preferences in AsyncStorage and Firebase Firestore to allow data persistent when the user logs back in or switches back to the app.

**Nutritional Tracking**
Tracks daily/weekly calorie intake on `MealsScreen`, comparing to user calories intake goals.

**Budget Tracking**
Calculating recipe costs on `CartScreen`, compared to user budget goals.

**User Authentication**
Implements Google Authentication for secure login, storing user information such as their name, image, and UID in Firebase Firestore. This allows us to easily use their UID for searching their saved recipes and user preferences in our database.

**Ingredient Checklist**
Provides a checkbox list for ingredients on `CartScreen` for shopping.

