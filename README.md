# best-programming-club-2020-12-20

## Kim's BYO-Assignment: Add Detailed Cart View ##

I wanted to display what was inside the cart, by listing how many of each products were chosen. This was harder than I initially thought, to be honest, but I eventually got it to work! 

First, There is a `count` key in each product object in `itemsInCart`. As each product is added, the count goes up. So `itemsInCart` is no longer a list of objects that are sometimes multiples of the same, as we select multiple of one type of product. It is a short list with each objects its own counter. 

To add a prodcut to `itemsInCart`, we need to check if the cart is empty.
If it's not empty, then check if the selected product's type already exists in the cart. If we determine this is a new product, then we'll add a new product object. I keep track of all these different conditions with a boolean variable, `isInCart`.

<!-- Before going into datails of adding products to `itemsInCart`, there is a boolean variable `isInCart`. It shows whether the selected product has been counted. This will become helpful in keeping track when we are determing if the selected product's type already exists in `itemsInCart` or not. 

To add a product to `itemsInCart`, we first need to check if the cart is empty. If it is, then we add a new product object to `itemsInCart`, with initial `count: 1`. We also set `isInCart = true`. If it's not empty, then we start checking if each of the existing product matches with the selected. We do this with a for loop, that will initially set out to look through every single object, but it'll break if we find the matching product. If we find the matching product, we only increment the `count` key 

To add a prodcut to `itemsInCart`, we need to check if the cart is empty.
If it's not empty, then check if the selected product's type already exists in the cart. If we determine this is a new product, then we'll add a new product object. I keep track of all these different conditions with a boolean variable, `isInCart`.


When a button is clicked, it is automatically set to false. It'll increment itself when we either add the product object to `itemsInCart` or increment one of the existing product object. -->

### Challenges and shit ###

1. The biggest challenge was checking if the selected product already exists then adding the product accordingly. I kept getting stuck in a for loop. Having a boolean checker fixed my problem. 

2. I kept getting the HTML display of `itemsInCart` repeated every time a button was clicked. I ended up resetting and displaying the updated `itemsInCart` per button click. 

## Assignment

1. BYO-Assignment: Add a new feature to the Farmer's Market shop that would improve the user experience.
2. Come up with a nicer user interface design (in an Adobe program, [Figma](https://www.figma.com/), [Sketch](https://www.sketch.com/), etc) and add a screenshot of it to this README (See [GitHub guide on images in Markdown](https://guides.github.com/features/mastering-markdown/).)

### Getting the assignment

[Fork this repository](https://guides.github.com/activities/forking/)

[Install Prettier for VSCode](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

### Completing the assignment

Make sure to commit your changes as you're making progress on the assignment. You'll receive feedback on the commit messages. Remember, commit messages should be short and sweet, in present-tense with an imperative tone. For example:

```
rename cart variable
```

### Remember...

- Actively ask the Discord channels for help!
- Google as much as you can, using the keywords you've learned. For example, search _"how to create HTML from javascript"_ or _"what is javascript forEach"_ or _"what is javascript dataset"_. MDN is a great keyword to include in your searches for reference materal, for example _"MDN javascript array"_.
- Don't be afraid to commit code that's not working yet.
