1. I would fit automated tests WIHTIN A GITHUB ACTION THAT RUNS WHENEVER CODE IS PUSHED. This is the best option because it automatically checks whether new changes break existing functionality before they are merged or submitted. For the Recipe project, specifically, this would help catch issues with recipe cards, localStorage, form inputs, and rendering early in the development process. Running tests automatically and systematically in this manner also makes the pipeline more reliable because developers do not have to remember to run the tests manually every time. It makes the testing process less tedious and more thorough. 

2. NO, I would not use an e2e test js to check if a function returns the correct output. That should usually be tested with a unit test because unit tests focus on small pieces of code, like individual funcs. End to end tests are better for testing a full user workflow, such as adding a recipe through the form and checking that it appears on the page.

3. Navigation mode analyzes the page right after it loads. thus, it is useful for testing the initial page load experience, including performance metrics like First Contentful Paint, Largest Contentful Paint, Total blocking time, cumulative layout shify, and speed index. Snapshot mode, on the other hand, analyzes the page at one specific point in time after it has already loaded. It is better for checking the curr state of the page, especially accessibility issues, but it does NOT measure the full page-loading process.

4. Three improvements we could make are:

- Add a `lang` attribute to the `<html>` element, such as `<html lang="en">`, because Lighthouse reported that the page is missing a lang attribute in the Accessibility section. It states that doing so would "improve the interpretation of your content by users in different locales".

- Add a meta description in the HTML, such as `<meta name="description" content="CSE 110 shop site with product cards and cart functionality.">`, because Lighthouse reported that the document does not have a meta description in the SEO section. This way, crawlers such as LLMS would better understand the app's content.

- LASTLY, improve performance by reducing unused JavaScript and using more efficient cache lifetimes. The navigation report showed estimated savings from reducing unused JavaScript and also suggested improving cache lifetimes.






