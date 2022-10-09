### Project Title
Custom UI Component Library / CSS Framework

#### Attendees
Kate O'Neill
Deirdre O'Halloran

#### Week Ending
Sun 9 Oct 

#### Work Undertaken
**CSS Frameworks**
Tailwind vs Bootstrap vs Foundation

WHAT?
*Tailwind*
"Tailwind CSS is a utility-first CSS framework designed to enable users to create applications faster and easier. You can use utility classes to control the layout, color, spacing, typography, shadows, and more to create a completely custom component design — without leaving your HTML or writing a single line of custom CSS."(https://blog.hubspot.com/website/what-is-tailwind-css)

*Bootstrap*
"Bootstrap is a free, open-source front-end development framework for the creation of websites and web apps. Designed to enable responsive development of mobile-first websites, Bootstrap provides a collection of syntax for template designs." (https://www.techtarget.com/whatis/definition/bootstrap)

*Bulma*
Bulma is a free, open source framework that provides ready-to-use frontend components that you can easily combine to build responsive web interfaces.(https://bulma.io/)

HOW TO USE?
*Tailwind*
https://tailwindcss.com/docs/installation/framework-guides
- installable as an npm package
- can use as CDN
- yarn package ?? [not mentioned on that site but looked up on yarn site and was listed]

*Bootstrap*
https://getbootstrap.com/docs/5.0/getting-started/download/
- CDN via jsDelivr
- install as npm package
- install as yarn package

*Bulma*
- clone git repo
- installable w/ npm package manager
- Usable via CDN link

HOW IT'S MADE?
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


