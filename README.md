# Spoonacular API Guide

## What the API does
The Spoonacular API provides an interface to access data about food. This includes ingredients, recipes, products, and menu items.

*Requests to the API are limited to a rate of 1 requests per second for the free tier.*


## API Keys
To get started, you must get authorization to be able to use the Spoonacular API.

1. Create an account at https://spoonacular.com/food-api/console#Dashboard
2. Find API key under "MY CONSOLE" tab at the top right.
3. Copy API key to clipboard.

## Using the API
We can perform our CRUD requests by specifying the method (GET, DELETE, etc) in our query and by passing the API key we obtained above as a query parameter. This will authorize us to be able to make requests to the API.

## Examples
Using the API key that we got above, we can make some test calls to the API to query different sets of information.

To get a list of all the recipes in the database, we would do<br>```GET https://api.spoonacular.com/recipes/complexSearch?apiKey=YOUR-API-KEY```<br>
This request will return a paginated JSON response of recipes that looks something like this:
```json
{
    "results": [
        {
            "id": 716426,
            "title": "Cauliflower, Brown Rice, and Vegetable Fried Rice",
            "image": "https://spoonacular.com/recipeImages/716426-312x231.jpg",
            "imageType": "jpg"
        },
        {
            "id": 715594,
            "title": "Homemade Garlic and Basil French Fries",
            "image": "https://spoonacular.com/recipeImages/715594-312x231.jpg",
            "imageType": "jpg"
        },
        {
            "id": 715497,
            "title": "Berry Banana Breakfast Smoothie",
            "image": "https://spoonacular.com/recipeImages/715497-312x231.jpg",
            "imageType": "jpg"
        },
        {
            "id": 644387,
            "title": "Garlicky Kale",
            "image": "https://spoonacular.com/recipeImages/644387-312x231.jpg",
            "imageType": "jpg"
        },
        {
            "id": 716268,
            "title": "African Chicken Peanut Stew",
            "image": "https://spoonacular.com/recipeImages/716268-312x231.jpg",
            "imageType": "jpg"
        },
        {
            "id": 716381,
            "title": "Nigerian Snail Stew",
            "image": "https://spoonacular.com/recipeImages/716381-312x231.jpg",
            "imageType": "jpg"
        },
        {
            "id": 782601,
            "title": "Red Kidney Bean Jambalaya",
            "image": "https://spoonacular.com/recipeImages/782601-312x231.jpg",
            "imageType": "jpg"
        },
        {
            "id": 794349,
            "title": "Broccoli and Chickpea Rice Salad",
            "image": "https://spoonacular.com/recipeImages/794349-312x231.jpg",
            "imageType": "jpg"
        },
        {
            "id": 715446,
            "title": "Slow Cooker Beef Stew",
            "image": "https://spoonacular.com/recipeImages/715446-312x231.jpg",
            "imageType": "jpg"
        },
        {
            "id": 715415,
            "title": "Red Lentil Soup with Chicken and Turnips",
            "image": "https://spoonacular.com/recipeImages/715415-312x231.jpg",
            "imageType": "jpg"
        }
    ],
    "offset": 0,
    "number": 10,
    "totalResults": 5222
}
```
