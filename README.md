# Fork-it: Hostel Mess Menu Generator 🥗📅

**Fork-it** is a Python-based automated weekly menu planner designed for college hostel messes. It dynamically generates diverse, nutritionally balanced meal plans while factoring in dietary preferences and constraints.

## 🔍 Project Overview

Fork-it was built to streamline the tedious and repetitive process of manually creating weekly food menus in college messes. It aims to:
- Reduce planning effort for hostel admins and cooks
- Promote healthier, more varied meals
- Respect user-defined dietary preferences (e.g., vegetarian, low-carb, high-protein)

## 🧠 Key Features

- 🍽️ **Automatic Meal Plan Generator**  
  Generates complete weekly menus using recipe metadata from open food APIs.

- 📊 **Nutritional & Dietary Filtering**  
  Integrates filters for dietary needs (veg/non-veg, calorie limits, macro ratios).

- 🔗 **API Integration with Foodoscope's RecipeDB and FlavorDB**  
  Retrieves structured recipe data and flavor profiles via HTTP requests.

- ⏱️ **Efficiency**  
  Reduces planning time by ~40% compared to manual methods.

## 🛠️ Tech Stack

- **Language:** Python  
- **APIs Used:**  
  - [RecipeDB](https://cosylab.iiitd.edu.in/recipedb/)  
  - [FlavorDB](https://cosylab.iiitd.edu.in/flavordb/)

- **Libraries:**  
  - `requests`, `json`, `datetime`, `random`, `pandas`, `matplotlib` (for optional visualizations)

## 📁 Project Structure

