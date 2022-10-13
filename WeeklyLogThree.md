#### Weekly Log 3

- Installing The Live Sass compiler using VS Code and set up a local development environment using MAMP just to test out using some sass on basic divs and making use of the nested CSS.


##### Key Functionality
###### Grid
Any other frameworks have their own ***grid*** system which makes sense. *Mobile-first development* is such a huge area of any kind of app or web design. Popularised by Eric Schmidt in a Google conference. The reason it's mobile first is because of the amount of limitations you have on a smartphone screen, you start with the screen with the smallest area to play with and add more features and design as you work up to desktop. Mobile first design means you "focus on the core of your product and strip away the rest" [link](https://xd.adobe.com/ideas/process/ui-design/what-is-mobile-first-design/)The average smartphone size is 6.3" found [here](https://omdia.tech.informa.com/OM022757/Display-Dynamics--January-2022-Average-smartphone-display-size-stays-at-63-inches-while-the-resolution-can-be-potentially-enhanced#:~:text=Since%202021%2C%20the%20average%20has,6.3%2Dinch%20level%20since%202Q21.) where as the average laptop screen size is between 13.3 and 15" [here](https://voltfixer.com/average-laptop-screen-size/#:~:text=The%20average%20laptop%20screen%20size%20in%20the%20market%20is%2013.3,increase%20up%20to%2017.3%20inches.). That's a staggering difference in screen size and you want a memorable experience on either size. That's where grids come in. With mobile phone web usage only increasing year-on-year.  The need for this mobile-first approach is only increasing.![[Pasted image 20221013181349.png]]
[https://www.oberlo.com/statistics/mobile-internet-traffic] 
<br>
The grid systems we know with Bootstrap, Tailwind or Bulma as outlined previously allow you to more easily design and develop for various display sizes. Grid systems can hinders outside the box designs as you want to keep it rigid to certain column widths etc. but it's simply a different way of thinking about design, some might say a more mathematical approach to design with fixed number of columns (typically 12 as it allows you to deal with both even and odd numbers on top of the grid) and gutter width to think about. 

###### Stylised Components
The grid is intended to be the foundation everything is built on in this scenario. On top of that we need to add some components that have pre-styled elements. Of course, I want some level of customisability with the elements but also want an approach where if someone were to enter bare-minimum class names, something would appear, somewhere between the out of the box styles of Bootstrap and the customisability of tailwind. 

- **Buttons** : Every site has buttons on to redirect you to different internal pages or different sections of the same page, You want them to stand out on your page to make them easily identifiable.  For marketing purposes having internal linking on your site is essential to boost your SEO scoring which will have you preferential in being the top results. Googles crawl bot "arrives at the website’s homepage, renders the page, and follows the first link" [link here](https://yoast.com/internal-linking-for-seo-why-and-how/) It's attempting to figure out relationships between pages and posts.

![HM homepage](images/hm.png) The things highlighted in red are the internal linking buttons that are both linked very near the top of the homepage. In the second case it is integrated into the hero section of the webpage. This shows the importance of proper button styles.
- **Cards**: A huge part of web design is the idea of a Call To Action (CTA) section. It's usually an image and a sentence maybe a small description a
