# Spoonacular API Guide

## What the API does
The Spoonacular API provides an interface to access data about food. This includes ingredients, recipes, products, and menu items.

*Requests to the API are limited to a rate of 1 requests per second for the free tier.*


## API Keys
To get started, you must get authorization to be able to use the Spoonacular API.

1. Create an account at https://spoonacular.com/food-api/console#Dashboard
2. Find API key under "MY CONSOLE" tab at the top right.

## Using the API
Using the API key that we got above, we can make a test call to the API to query a list of recipes with ```GET https://api.spoonacular.com/recipes/complexSearch?apiKey=991ca57d17d54a84a35ce07c00e6dafe```
