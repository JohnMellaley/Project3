# Foodie code institute 
## Overview

The foodie web site was set up to allow people to look up recipes and also add recipes of there own. This could be used as
centrial depository for all ones favourite recipes.


## UX

### What is this website for?
This website was created for anyone with an interest in cooking to allow them to look up recipes based on a number of different search
criteria  example name, meal type, ingredients, origin, (without) allegrns etc. The user can add also add their own recipes to the website as well 
as update and delete them if required. The site will also allow other users to try there recipe out. Users should also be able to 'like' other 
peoples recipes. There will also be statistics page that will provide information on the most popular recipes, authors,  recipes per meal type,
recipes per country and meal type with the most allergens. Everypne that registereds, will have there own username and password and once logged in
will be directed to there own profile page which will contain all there recipes that they have added.

### User Stores
This site is used by anyone looking for some new recipes ideas for cooking at home for the family or special ocassions etc.. Someone wishing to 
store there favorite recipes for future use, either by themself or another user on the website. Chefs\Cooks could also use the site to get feedback on there
own recipe through the like functionality

**Existing and New fans.**

* Users should be able to search recipes based on recipe name.
* Users should be able to search recipes based on counrty of orgin.
* Users should be able to search recipes based on meal type.
* Users should be able to search based on ingredents.
* Users should be able to search, discounting any recipes with certain allgerns
* Users should be able to add there own recipes
* Users should be able to like other users recipes
* Users should be able to update or delete the own recipes.
* User should be registered and have the own id.
* Users should have there own profile page with there own recipes displayed if any
* There should be page with all recipes sorted by the most likes at the top.


In the design of this web page I decided to use Balsamiq to create my wire frames. I did two sets of screens one for mobile and the other for 
desktop. For mobile I only did screen that were significantly different from large screens. Both can be seen under assets\wire frames folder
within the project.

### How does it work

## Features
 
### Existing Features

* register
    - Can only log in if registered. Index page allows you to do this. ONce registered will redirect to 
      the home page.

* login 
    - login in form. One logged in will direct to the login page.

* Home link
    -  each user as there own home page with there own recipes order by the most likes

* All recipes
    - This page provides all recipes from all users and again order by the most likes

* Cards
    - All recipes are displayed with Cards with image, title and link to view a more detailed page with 
      all the recipes information. The back of the card has information for Author, Origin, Type, 
      Prep Time, Cooking Time, Services, Likes and allergens.

* Show recipe
    - Displays all the detials on the cards on one HTML page
    - If are the Author of the recipe you will see two buttons one for updating the recipe and the
      second one allows you delete the recipe.
    - If you are not the Author of the recipe then you can click the like button. This will increase the
      count. Each person can only like each recipe once only.

* Update page
    -   This page allows you add, update and delete any of the attributes of your recipe. The page is
        is display with a form and a submit button

* Delete Button
    -   Activates a modal, which asks you to confirm if you would like to Delete the recipe. If you
        click yes then the recipe is deleted and you are direct back to your home page. If you click no
        then the modal closes and you back on the recipe page.

* Add Recipe
    -   This page allows you to add a new recipe

* Search Recipes
    - on this page you have three search options
    - Search by name. If you know the name then you can search and if found will display a card with 
      recipe below. The card functions like all cards on the site with the same options
    - Search by ingredients and or Allergen. For this search you must select at lest two ingredients
      with the option of choosen an allergen. Once submitted a list of all the recipes with both ingredients
      and if allergen selected then it will remove any recipes from this list containing this recipe.
    - The third option allows you to searh by type and origin. Both options must be selected and again results
      are shown as list of cards at the bottom of the page 

* Dashboard
    - This page contains 6 graphs. This page is interactive for example if you click on Authors bar,
      then all the other graphs will respond and the information will change to show how that persons 
      recipes are split up.Example on the dish with most likes, bar chart you will only see the authors
      recipes and the rest will disappear.
    - Authors with the most likes.
    - Dish with the most likes.
    - Country with the most dishes
    - Recipes By Type. 
    - Which Meals Is Most Likely To Contain Allergens
    - Which Cusines Contains The Most Allergens

* Logout
    - This page allows the user to logout and directs user back to the index page



### Features Left to Implement
    - Would like to add autocomplete to the name search.

## Some the tech used includes:
- **HTML**, **CSS**.
  - Base languages used to create website

  - [Cloud9](https://aws.amazon.com/cloud9/)
    - We use **Cloud9** to build our web pages
  - [Google-fonts](https://fonts.google.com/m)
    - Using **Google-fonts** to get use of fonts
  - [GitHub](https://github.com/)
    - Using **GitHub** a web-based hosting service for version control using Git


## Testing
### Manual testing
- All internal links have been checked and work correctly.
   - **Home** Brings user to home page
   - **All Recipes** Brings user All recipes page
   - **Search Recipes** Brings user to search page
   - **Add Recipes** Brings user to add recipe page
   - **Dashboard** Brings user to dashboard page
   - **Logout** Logs out user and bring to index page
   - **Cooking instructions** Link in cards bring you to the recipe view page
   - **Social Media** 

- Register Modal
    - If password not the same, error message display.
    - If User name already in Database then error message display
    - If everything okay user moved home page.

- login form
    - if Password or user name incorrect error message displayed
    - if user allready in session error message display
    - If everything okay then page directed to home page
    - 
- cards
    - cards display correctly in home page, all recipes page and search page
    - Front of card display image, link to show recipe page and back displays all attributes correctly

- Profile page
      - All the users recipes are display here and order from most like down.
      
- Recipes page.
      - All recipes displayed here correctly in order from most liked down.

- show recipe
    - Recipe details displays as expected
    - Likes button if clicked by Author of recipe, pop up error message appears
    - Likes button if clicked and user that already liked the recipe then popup message appears
    - Otherwise  likes count is incremented by one.
    - Update and Delete button only show if its the Author viewing the recipe

- delete Button
    - modal pops us when pressed. click yes button on model and recipe deletes okay
    - Click no and returns back to show recipe page
    
- update button
    - update form pops up with recipes detials

- Update form test
    - Form page is displayed correctly
    - All required fields work as expeceted cannot submit form without Name, image, prep time, cook time, servers.
    - Type and country of origin no option to leave blank
    - Can add, edit and delete Ingredients,Steps allergns okay.
    - Buttons to add extra fields work okay
    - Submit button works as expected


- Search page
    - Dish Name Search
        - Recipe card pops up if name correct. Check in different cases and all work okay. Can't leave blank.
        - If name not correct error message displays as expected.
    - Ingredients and allergen Search
        - Two ingredient fields are required.
        - Can search with two ingredients and returns all recipes that have the two ingredients mentioned
        - If allergen added, will check recipes to make that allergen is not included on the results
        - if not recipes found that match the creteria then the message no recipes found is displayed
    - Dish type and Country of Origin Search
        - If Counrty or origin not selected the an alert message box pop up telling the user to fill them in
        - If both options are selected it will return the matchs else display message no recipes found is displayed
        
- add recipes
    - Form display as expected.
    - All required fields work as expeceted, cannot submit form without Name, image, prep time, cook time, servers.
    - type and country select, need to add validation in python to display error message.
    - need at least one Ingredient and one step to submit the recipe
    - can submit with no allergens.
    - Submit button clears the form and displays a message that your recipe has been added successfully if everything was okay

- Dashboard
      - All chart display as expected
      - This is an interactive chart so click on a bar or section of pie chart, then all charts will represent only the portion of the chart you clicked.
        click a second time then it reverts back to show the complete set of data

- Logout
      - works okay, logs user out ans redirects to index page.
- 
    
- Site viewed and tested in the following browsers (all work as expected):
  - Google Chrome       dsiplays okay
  - Mozilla Firefox    displays okay
  - Opera               not displaying
  - Internet explorer

### Automatic testing
- Automatic testing not required

### Site has been tested on mobile, tablet and laptop devices as well as testing on chrome for the different sizes.

### Index page
-Stays the same for all devices

### Navbar: 
- On medium to large screens the the nav-items are display on the righ hand side of the navbar. On Small screens these items are displayed under
  a hambuger icon which when click a side nav opens with a list of the item underneath each other.

### Home page (Profile.html).
- Recipes on large screen are displayed 3 per row.
- Recipes on medium screens are displayed 2 per row.
- Recipes on small screens are displayed 1 per row.

### All Recipes page (Recipe.html)
- Recipes on large screen are displayed 3 per row.
- Recipes on medium screens are displayed 2 per row.
- Recipes on small screens are displayed 1 per row.

### add recipe (add_recipe.html)
- Display the sames on all screens

### update recipe (edit_recipe.html)
- Display the sames on all screens

### show_recipe
- On small screens Detials, Image, ingredients and steps display under each other. On medium to large screen it detials and image at top, with
  Ingredients and steps at the bottom.

### Dashboard
- Pie charts on small screen one at a time, and on medium to large screens one at time



### search_recipes




### Footer 
- Stays the same for all devices


# Deployment

This web site is deployed on the Heroku platform.
https://recipe-book-jm.herokuapp.com/

# Credits

# Media
## Photos       
### Image background on search form   
- travel.png was obtained from www.freepik.com
- plane.png was obtained from www.flaticon.com 
