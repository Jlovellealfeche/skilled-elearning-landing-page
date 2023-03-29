# Frontend Mentor - Skilled e-learning landing page solution

This is a solution to the [Skilled e-learning landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/skilled-elearning-landing-page-S1ObDrZ8q). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [ https://github.com/Jlovellealfeche/skilled-elearning-landing-page](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned


*** <b>Notes on media queries breakpoints </b> *** 

```
@media screen and (max-width: 767px) {
<p>This is for mobile</p>
}

@media screen and (min-width: 768px) and (max-width: 1023px) {
    <p>This is for tablet</p>
}


@media screen and (min-width: 1024px) {
    <p>This is for desktop</p>
  
}

```

*** <b>Notes on usage of @use and @forward in sass partials </b> *** 

### Folder name Sass

  ||--<b>Abstract</b>--- _index.scss-->
  ```
   @forward './colors'; 
   @forward './breakpoints';
   @forwards './mixins';
  ```

  ||--<b>base</b>---_index.scss--> 
  ```
  
  @forward './base-styles'; 
  
  ```
            |--- _index.scss 

              ```
                  @forward './base-styles';
              ```

            |--- _base-styles.scss --> 
  
                ```
                  @use '../abstracts' as a; 

                  @use '../components' as c; 
                ```  

  ||--<b>components</b>
  |
  |

  ||<b>style.scss</b>----
    
      @use 'abstracts';
      @use 'base';
      @use 'components';



### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.


## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

