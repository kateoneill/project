### Project Title
Custom UI Component Library / CSS Framework

#### Attendees
Kate O'Neill
Deirdre O'Halloran

#### Week Ending
Sun 9 Oct 

#### Work Undertaken
##### CSS Frameworks comparison
*Tailwind vs Bootstrap vs Foundation*<br>

WHAT? <br>
*Tailwind*<br>
"Tailwind CSS is a utility-first CSS framework designed to enable users to create applications faster and easier. You can use utility classes to control the layout, color, spacing, typography, shadows, and more to create a completely custom component design — without leaving your HTML or writing a single line of custom CSS."(https://blog.hubspot.com/website/what-is-tailwind-css)

*Bootstrap*<br>
"Bootstrap is a free, open-source front-end development framework for the creation of websites and web apps. Designed to enable responsive development of mobile-first websites, Bootstrap provides a collection of syntax for template designs." (https://www.techtarget.com/whatis/definition/bootstrap)

*Bulma*<br>
Bulma is a free, open source framework that provides ready-to-use frontend components that you can easily combine to build responsive web interfaces.(https://bulma.io/)

HOW TO USE?<br>
*Tailwind*<br>
https://tailwindcss.com/docs/installation/framework-guides
- installable as an npm package
- can use as CDN
- yarn package ?? [not mentioned on that site but looked up on yarn site and was listed]

*Bootstrap*<br>
https://getbootstrap.com/docs/5.0/getting-started/download/
- CDN via jsDelivr
- install as npm package
- install as yarn package

*Bulma*<br>
- clone git repo
- installable w/ npm package manager
- Usable via CDN link

HOW IT'S MADE?<br>
*Tailwind*
- Tailwind is a PostCSS plugin (https://tailwindcss.com/docs/using-with-preprocessors)
- the only reference i could find for preprocessor tailwind uses was vague sentences in articles but most of them referred to the fact PostCSS was being used

*Bootstrap*
- v3.0 -> "Bootstrap ships with vanilla CSS, but its source code utilizes the two most popular CSS preprocessors, [Less](https://getbootstrap.com/docs/3.3/css/#less) and [Sass](https://getbootstrap.com/docs/3.3/css/#sass). Quickly get started with precompiled CSS or build on the source."[https://getbootstrap.com/docs/3.3/#:~:text=Preprocessors,or%20build%20on%20the%20source.]

- v4.0-> "**Moved from Less to Sass.** Bootstrap now compiles faster than ever thanks to Libsass, and we join an increasingly large community of Sass developers."[https://blog.getbootstrap.com/2015/08/19/bootstrap-4-alpha/

- Bootstrap has used both Less and SASS as their preprocessor of choice. Version 5 from what I can find is also written in SASS 
- https://thecodingmachine.com/en/getting-it-right-with-sass-and-bootstrap-5/#:~:text=Bootstrap%20package%20will%20ship%20with,and%20your%20custom%20CSS%20code.

*Bulma*
- written in sass
- spread over 39 sass files that you import as you want

WHY USE ANY OF THEM?
---What functionality and features are they bringing to the table?
<br>
 *Tailwind*
- no pre-styled components
- utility-first framework
- you add the utility classes to control every element 
- If you want a button with rounded edges :  ```
<button class="h-10 px-6 font-semibold rounded-md bg-black text-white" type="submit">Buy now</button>
- h10 is setting the height of the button
- px-6 is setting the padding
- font-semibold is setting font-weight
- rounded-md is adding rounded corners
- bg-black is adding a black background
- text-white is making the text white
example from : [here](https://blog.hubspot.com/website/what-is-tailwind-css#:~:text=Tailwind%20CSS%20makes%20it%20quicker,and%20more%20of%20your%20application.)
- adding custom colours is possible. I found [this article](https://www.geeksforgeeks.org/how-to-add-new-colors-to-tailwind-css-and-keep-the-originals-ones/#:~:text=You%20can%20easily%20add%20new,js%20file.)
- grid system : I watched [this video](https://www.youtube.com/watch?v=JITwwrVSteE) to understand it
- extensive docs to deal with literally everything : https://v1.tailwindcss.com/#what-is-tailwind

*Bootstrap*
I have experience using Bootstrap.
- pre-styled components 
- mobile-first so responsiveness takes centre stage
- it's 12-col grid system is one of the most popular 
- If you want a button with rounded edges:
- < button type="button" class="btn btn-secondary">Secondary</ button>
- way less code than Tailwind but also less cutomisation
- btn class adds the rounded edges
- secondary is adding a dark grey black colour as pre-set by Bootstrap
- example from [here](https://getbootstrap.com/docs/5.0/components/buttons/)
- Extensive docs that go into depth on all components: https://getbootstrap.com/docs/5.0/getting-started/introduction/

*Bulma*
- Modular: import as you need principle:
	- For example, let's say you only want the Bulma **columns.**  
	- The file is located in the `bulma/sass/grid` folder.  
	- Simply **import** the utilities dependencies, and then the files you need directly
- preset variables that you can override by updating before running a bulma import. ( i read about that [here](https://bulma.io/documentation/customize/variables/)
- mobile-first design
- optimised for vertical reading
- 4 breakpoints
- Column system using flexbox. I watched [this video](https://www.youtube.com/watch?v=feGMqVSRnmI)
- If you want a button with rounded edges:
- < button class="button is-black">Black</ button>
- button by default has some rounding
- is-black makes the button black
- Example from [here](https://bulma.io/documentation/elements/button/)
- slightly smaller docs than the extensiveness of the other 2 here: https://bulma.io/documentation/

=> commonalities between them 
=> differences
=>anything they're all missing
<br>
##### CSS 
WHAT IS CSS?<br>
https://www.w3schools.com/css/css_intro.asp
-   CSS stands for Cascading Style Sheets
-   CSS describes how HTML elements are to be displayed on screen, paper, or in other media
-   CSS saves a lot of work. It can control the layout of multiple web pages all at once
-   External stylesheets are stored in CSS files

PROBLEMS WITH CSS<br>
- self repetition is unavoidable 
- very static
- sometimes can have unexpected interactions (will change one thing and in turn change something unrelated)

WHAT'S A CSS PREPROCESSOR<br>
https://developer.mozilla.org/en-US/docs/Glossary/CSS_preprocessor
<br>
"CSS Preprocessors compile the code which is written using a special compiler. They then use that to create a CSS file, which can then be referenced by the main HTML document." (https://www.freecodecamp.org/news/css-preprocessors/)

- allow you to set variables, run loops or have if statements in your CSS code

"It offered an advanced way of writing CSS that extends the basic functionalities. This advanced code is later compiled as normal CSS code that the browser will understand".(https://sherocommerce.com/what-is-a-css-preprocessors-why-use-them/){{this link provides a good comparison between SASS, LESS and STYLUS}}<br>
WHY USE A PREPROCESSOR?
- creating variables and mixins makes code easier to maintain, change a colour variable in one place and it updates sitewide
- Not as much repetition 
- makes CSS coding more efficient and saves time

"CSS preprocessors make it easy to automate repetitive tasks, reduce the number of errors and code bloat, create reusable code snippets, and ensure backward compatibility"(https://www.emotionstudios.net/trending/6-reasons-you-should-use-a-css-preprocessor-2/#:~:text=CSS%20preprocessors%20make%20it%20easy,it%20on%20the%20client%20side.)

**Framework**<br>
WHAT'S A CSS FRAMEWORK?<br>
WHY USE A CSS FRAMEWORK?

CSS frameworks are tools used by UI developers to make their job easier. Rather than reinventing the wheel each time a new project comes up; frameworks give developers the tools to quickly spin-up user interfaces that can be tweaked and iterated on throughout a project instead of spending time starting from a blank document.(https://medium.com/html-all-the-things/what-is-a-css-framework-f758ef0b1a11)

PROS
- saves time 
- for bigger teams it can set standard (Bootstrap was created by Twitter to keep similar look and feel across all their associated platforms)
- some say they promote grid design which will mean better readability and expandability as well as creating more cohesive sites. (https://css-tricks.com/what-are-the-benefits-of-using-a-css-framework/)
- enables cross-browser functionality 

CONS
- can come with a lot of bloat, if you only want element from the entire framework but have to install the entire thing --We had an issue on my placement of long compiler times so much so that one of the senior developers had to start importing Bootstrap bit by bit to remove any bits he knew he 100% would not be using to try bring down the compiler time.
- initially using it and starting to use it can waste time as employees familiarise themselves with new frameworks, there are so many out there and while there can be commonalities across them, the 3 I looked into (Bootstrap, Tailwind and Bulma) couldn't be more different
- Sites can look the same thus removing any creative freedom. The issue of ages is sites and apps having the same look and feel, sites that only use Bootstrap and limit the custom CSS are undeniably going to have similar layouts and components which can give the web this unwanted uniformity.

=>I came across an [article](https://medium.com/codex/why-i-no-longer-use-css-frameworks-be356f10b0c9) that i thought was interesting and wanted to see if other people agreed to it

<br>
##### Dark Mode
BENEFITS
- reduces blue light which disrupts melatonin production to help you sleep
- extends battery life (https://mashable.com/article/iphone-dark-mode-battery-life-saving)
- better in low-light settings
- reduces eye strain and dry eyes in low-light condition
- helps people with light sensitivity or visual impairment 
- They conducted an experiment using the YouTube app with 50% of the brightness in Dark Mode and the battery saving compared to Light Mode was 15%. Compared to the screen with 100% active brightness, the Darkness interface saved 60% of the screen power (https://www.venturus.org.br/en/darkmode-and-the-benefits-for-the-user-experience/)

DISADVANTAGES
- not ALWAYS better for eye strain
- can be a challenge to read longer strings of text 
- difficult to see in bright sunlit areas
- Using a dark screen requires our pupils to dilate more to allow enough light to come in. The sharpness of your vision can be compromised this way, where details are harder to see clearly in dark mode. (https://vulcanpost.com/793823/dark-mode-pros-cons-eye-health/#:~:text=Disadvantages%20of%20dark%20mode,-Some%20may%20find&text=In%20a%20bright%20environment%2C%20the,enough%20light%20to%20come%20in.)
- not good for people with myopia or astigmatism 
- cause halation
- these struggles to read mean productivity can be affected.
<br>
- https://www.wired.com/story/do-you-need-dark-mode/
- https://blog.superhuman.com/why-do-people-use-dark-mode/
- https://www.forbes.com/uk/advisor/mobile-phones/what-is-dark-mode-and-should-you-be-using-it/
- https://www.vectornator.io/blog/dark-mode/

ARE PEOPLE CHOOSING DARK MODE?
- https://earthweb.com/how-many-people-use-dark-mode/
- According to data, 81.9% of people of smartphone users use dark mode

HOW TO DESIGN FOR DARK MODE
- https://blog.prototypr.io/how-to-design-a-dark-theme-for-your-android-app-3daeb264637
- It’s because Dark Theme works well with desaturated colors. Shades with tonal values that range from 50–400 are the most appropriate colors for dark theme
- https://uxplanet.org/8-tips-for-dark-theme-design-8dfc2f8f7ab6
- avoid pure black
- avoid saturated colours
- Use lighter tones (colors in the 200–50 range) because they have better readability on dark theme surfaces
- meet colour contrast standards
- communicate depth with varying dark colours - greys etc.
- https://compilezero.medium.com/dark-mode-ui-design-the-definitive-guide-part-1-color-53dcfaea5129

##### Unanswered Questions /  Questions to be looked into 
- further research into the preprocessors to narrow down which one to use
- outline commonalities explicitly regarding the frameworks to unlock potential USP
- look further into impact of dark mode on eyes 
- is full dark mode worth it / do i need a light mode option if there's more disadvantages
