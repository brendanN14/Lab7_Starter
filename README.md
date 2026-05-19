1. I would fit automated tests WIHTIN A GITHUB ACTION THAT RUNS WHENEVER CODE IS PUSHED. This is the best option because it automatically checks whether new changes break existing functionality before they are merged or submitted. For the Recipe project, specifically, this would help catch issues with recipe cards, localStorage, form inputs, and rendering early in the development process. Running tests automatically and systematically in this manner also makes the pipeline more reliable because developers do not have to remember to run the tests manually every time. It makes the testing process less tedious and more thorough. 

2. NO, I would not use an e2e test js to check if a function returns the correct output. That should usually be tested with a unit test because unit tests focus on small pieces of code, like individual funcs. End to end tests are better for testing a full user workflow, such as adding a recipe through the form and checking that it appears on the page.





