# Read Me

This is a code block I wrote to help me achieve some fitness goals. I wanted to run a half marathon in two hours, and to squat 500 pounds in the same year. I started the year at about 200 pounds and knew that it would be easier to meet that running goal if I lower my body weight to about 180 pounds, once my 1/2 marathon training was done, I knew that it would be easier for me if I bulked to help me get to that 500 pound squat.
This program has a few global variables.
1. Your chat GPT key is essential for getting the nutritional information for the grocery list I created.
2. the total number of daily calories you want to eat
3. the total number of Fats
4. Total number of Carbs
5. Total number of Proteins
6. A weekly budget for the program to stay within.
7. The Zip code you live in.
How this program works is it asks chat GPT for the nutritional and price information for each specific good from within the zipcode you have inputted into the model. It searches Walmart for the information and populates the dictionary. (Because this function costs money by hitting the API, i have my most recent dictionary saved and the function commented out). The function then optimizes over the number of ingredients that it can buy to hit the daily calorie goals. It is not allowed to recommend more than 4 servings of any given good ( i was getting suggestions of lentils and milk for basically everything) and I made the function optimize over the number of ingredients so to have variety.
The program also gives you recipe recommendations by again hitting the OpenAI API, and giving you a list of recipes, and it also recommends whatever else you need to buy to make those.
The program saves the nutritional information from the OpenAI APi call so as to not have to continuously charge the API and also saves the recipe list so as again, to save money.
