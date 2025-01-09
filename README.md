# Smart Food Diary Application
Overview :
The Smart Food Diary is a web application developed to help users log their meals, track nutritional intake, and receive personalized dietary recommendations. The app integrates advanced machine learning models and nutritional databases to provide accurate food recognition, dietary insights, and interactive visualizations.

Features :
 User Authentication & Profile Management
Users can register, log in, and manage their profiles, including setting dietary goals such as calorie, protein, carb, and fat targets.

Food Logging & Image Recognition :
 Users can log their meals by uploading images. The app uses the dima806/indian_food_image_detection model integrated via Hugging Face Transformers to recognize food items and extract detailed nutritional information from the uploaded images.

Nutritional Breakdown & Analysis :
 The app calculates and displays the nutritional breakdown of each meal, including calories, proteins, carbs, and fats. The information is matched with recommended daily intake guidelines to help users stay on track.

Dietary Recommendations :
 The system provides personalized dietary suggestions based on user goals (e.g., weight loss, muscle gain) and past consumption patterns. The app uses the K-Nearest Neighbors (KNN) model to suggest healthier food alternatives.

Data Visualization :
 Nutritional trends are visualized using interactive Plotly charts, allowing users to analyze their intake over time. This helps them monitor progress and make informed decisions about their diet.

Custom Reports :
 Users can download their nutritional reports in PDF or CSV format, summarizing their daily intake, progress toward goals, and recommendations.

Admin Dashboard :
 The admin dashboard allows administrators to manage user profiles, food entries, and system settings. Admins can also perform user deletion and food entry additions.

Technologies Used :

 Django Framework: Backend framework for handling user authentication, session management, and meal logging functionalities.
Hugging Face Transformers: Used to integrate the dima806/indian_food_image_detection model for image-based food classification.
Pandas: A library for processing and normalizing nutritional data, enabling accurate comparisons and analysis.
Plotly: Used for creating interactive visualizations of nutritional intake trends.
K-Nearest Neighbors (KNN): Machine learning model used for meal recommendation based on the user’s dietary goals and previous entries.
How It Works
User Uploads Meal Image: The user uploads an image of their meal. The app uses the dima806/indian_food_image_detection model to classify the food items in the image.
Nutritional Information: After detecting the food, the app retrieves nutritional data (calories, protein, carbs, fats) and displays it in the user’s food diary.
Personalized Recommendations: The app analyzes the user’s dietary habits and provides meal recommendations using KNN based on the user’s preferences and goals.
Tracking & Analysis: Nutritional data is tracked and visualized in real-time, helping users monitor their intake and adjust their diet.


Conclusion :
 The Smart Food Diary application is an innovative tool that combines machine learning, real-time data visualization, and personalized dietary recommendations to help users manage their health effectively. It allows users to make informed decisions about their diet, track their progress, and stay motivated to achieve their nutrition goals.
