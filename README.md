# 🍲 Recipe Finder | World Flavors

Discover delicious recipes from across Africa and around the world with **Recipe Finder**, a Python desktop application built with PyQt5.

The application features a collection of traditional African dishes, recipe search, step-by-step cooking instructions, and a favorites system. It can also connect to the API Ninjas Recipe API to search for recipes online.

## ✨ Features

- 🌍 **African Cuisine:** Explore traditional dishes from different African countries.
- 🇳🇬 **Nigerian Jollof Rice:** Find ingredients and step-by-step cooking instructions for this popular Nigerian dish.
- 🇬🇭 **Ghanaian Jollof Rice:** Explore a Ghanaian version of jollof rice.
- 🔎 **Recipe Search:** Search for recipes by name or country.
- 🎲 **Surprise Me:** Discover a random recipe.
- ❤️ **Favorites:** Save your favorite recipes and view them later.
- 💾 **Persistent Storage:** Store favorite recipes in a local JSON file.
- 🌐 **API Integration:** Search online using the API Ninjas Recipe API.
- 📴 **Offline Recipe Collection:** Browse built-in recipes even when the API is unavailable.
- 🎨 **Modern GUI:** Enjoy a dark-themed interface with separate navigation, search results, and recipe details panels.

## 🍛 Included African Recipes

The application includes these built-in recipes:

| Recipe | Country |
|---|---|
| Nigerian Jollof Rice | Nigeria 🇳🇬 |
| Ghanaian Jollof Rice | Ghana 🇬🇭 |
| Egusi Soup | Nigeria 🇳🇬 |
| Suya | Nigeria 🇳🇬 |
| Waakye | Ghana 🇬🇭 |
| Puff-Puff | Nigeria 🇳🇬 |
| Injera with Misir Wat | Ethiopia 🇪🇹 |
| Chicken Yassa | Senegal 🇸🇳 |
| Bobotie | South Africa 🇿🇦 |
| Ndole | Cameroon 🇨🇲 |

Each built-in recipe includes ingredients and cooking instructions.

## 🛠️ Technologies Used

- **Python** — Main programming language.
- **PyQt5** — Desktop graphical user interface.
- **Requests** — HTTP requests to the recipe API.
- **API Ninjas** — Online recipe search.
- **JSON** — Saving and loading favorite recipes.
- **OS and Environment Variables** — Secure API key configuration.
- **Random** — Selecting surprise recipes.

## 📋 Requirements

Before running the application, make sure you have:

- Python 3 installed.
- An internet connection for online recipe searches.
- An API Ninjas API key for online searches.
- The required Python libraries.

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/recipe-finder.git
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Open the project folder

```bash
cd recipe-finder
```

### 3. Install dependencies

```bash
pip install PyQt5 requests
```

### 4. Configure your API key

The application reads your API key from an environment variable named `NINJAS_API_KEY`.

**Windows Command Prompt:**

```cmd
set NINJAS_API_KEY=YOUR_API_KEY
```

**Windows PowerShell:**

```powershell
$env:NINJAS_API_KEY="YOUR_API_KEY"
```

Replace `YOUR_API_KEY` with your own API Ninjas key. These commands set the variable for the current terminal session.

Never publish your real API key in your GitHub repository.

### 5. Run the application

```bash
python main.py
```

Replace `main.py` with your actual Python filename if it is different.

## 🖥️ How to Use

1. Launch the Recipe Finder application.
2. Browse the built-in recipes in the search results panel.
3. Select a recipe to view its ingredients and cooking instructions.
4. Use the search box to search by recipe name or country.
5. Select **Surprise Me** to discover a random dish.
6. Choose **African Foods** to browse the built-in African recipe collection.
7. Select **Nigerian Jollof** or **Ghanaian Jollof** to find either jollof recipe quickly.
8. Click **Add to Favorites** to save a recipe.
9. Select **Favorites** to view your saved recipes.
10. Use **Save Favorites** to save your collection to a JSON file.

## 🌐 API Integration

Recipe Finder uses the API Ninjas Recipe API to search for recipes online.

The application sends an HTTP GET request to the recipe endpoint with the search term and your API key.

If online searching is unavailable, the application attempts to display matching built-in recipes instead.

To use online searching, you need a valid API key and access to the relevant API endpoint.

## 💾 Data Storage

Favorite recipes are stored locally in:

```text
recipe_favorites.json
```

This file is created when favorites are saved. It allows the application to load previously saved favorites when you reopen it, as long as the file remains available.

## 📁 Project Structure

```text
recipe-finder/
│
├── main.py
├── recipe_favorites.json
└── README.md
```

- `main.py` — The main Python application.
- `recipe_favorites.json` — Local storage for favorite recipes, created when needed.
- `README.md` — Project documentation.

The filenames above are examples; use the actual filename of your Python script.

## 🔐 Security

- Keep your API key private.
- Use the `NINJAS_API_KEY` environment variable instead of hardcoding your key.
- Do not commit API keys or other secrets to GitHub.
- Consider adding generated local data files to `.gitignore` if you do not want them tracked.

## 🎯 Project Goals

This project demonstrates practical Python programming skills, including:

- Building a desktop application with PyQt5.
- Working with external APIs.
- Sending HTTP requests and handling API errors.
- Searching and filtering recipe data.
- Reading and writing JSON files.
- Using environment variables for configuration.
- Organizing application functionality into methods.
- Creating an interactive graphical user interface.

## 🔮 Future Improvements

Possible future upgrades include:

- Adding more African recipes and cuisines from other regions.
- Displaying food images.
- Adding ingredient-based searches.
- Filtering recipes by country or cuisine.
- Adding preparation and cooking times.
- Including serving-size adjustments.
- Improving recipe recommendations.
- Adding unit tests and more detailed error messages.

## 👨‍💻 Author

**Created as a Python project to explore APIs, desktop application development, and African cuisine.**

## 📜 License

Choose a license for your project before distributing it publicly. For example, you could use the MIT License if it suits your goals.
