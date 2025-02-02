# Additions

Created a front end for Chowdown. This front end can add new recipes and post. The functionality is all included in additem.php. This file must be placed in your webserver root (or any subfolder).
The front end also adds additional fields to the recipe.
- yield (the amount of food the recipe will make)
- cookTime (the amount of time if will take to bake / cook the items
- prepTime (amount of time needed to prepare ingrients before cooking can start)
- nutritional information
  - servingSize (the amount of food relating to the nutritioal information)
  - calories (cal or kcal amount)
  - cholesterolContent (Cholesterol in mg)
  - fatContent (Fat in grams)
  - sodiumContent (Sodium in mg)
  - carbohydrateContent (Carbohydrate n grams)
  - sugarContent (Sugar in grams)
  - fiberContent (Fiber in grams)
  - proteinContent (Protein in grams)
  - saturatedFatContent (Saturated Fat in grams)
  - unsaturatedFatContent (Un Saturated Fat in grams)

The nutritional information can be adjusted in the _data/nutrients.yml file. The nutritioal information was added by another fork.

# Chowdown

A simple, plaintext recipe database for hackers

[http://chowdown.io](http://chowdown.io)

# Getting Started

This is a Jekyll build. Make sure you have Jekyll [installed](https://jekyllrb.com/). To install, run this command in the terminal (or iTerm, etc):

```gem install bundler jekyll```

or to check if you've got it installed already:

```jekyll -v```

Clone or download this repo. Navigate to the folder in terminal (or iTerm, etc), and then run:

```jekyll serve```

With default settings, you should be able to view the site locally at `http://127.0.0.1:4000/`

# Writing a Recipe

The recipes are stored in the collection "Recipes" (the folder /_recipes).

They are written in Markdown and contain a few special sections:

- The frontmatter, which contains:
 - Title, Image, and Layout (which is "recipe")
 - Ingredients (a list of things in the dish)
 - Directions (a list of steps for the dish)
- Body content (for intros, stories, written detail)

If you need help with Markdown, here's a [handy cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

# Writing a component recipe

A component recipe is a special recipe made up of other recipes. To make a new component recipe:

- place your smaller, single recipes into the /_components folder
- make a new recipe like normal in the /_recipes folders
- in the frontmatter of this new recipe, include your recipes from the /_components folder (instead of the usual Ingredeints list)

You can an example on the Red Berry Tart recipe. 

- [example Markdown](https://raw.githubusercontent.com/clarklab/chowdown/gh-pages/_recipes/red-berry-tart.md)
- [example recipe page](http://chowdown.io/recipes/red-berry-tart.html)
