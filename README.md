# Code-Refactor-c1 
Challenge one: HTML, CSS, Git challenge code refactor 

## Technology Used 

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) , [https://www.w3schools.com/cssref/css_selectors.php](https://www.w3schools.com/cssref/css_selectors.php)   |   
| Git | [https://git-scm.com/](https://git-scm.com/)     |    

## Description 

[Visit the Deployed Site](https://sheaschwenn.github.io/Code-Refactor-c1/)

This refactoring of the Horiseon marketing agency's webpage allows the page to be optimized for search engines and follow accessibility standards. This was done by adding alt text, semantic HTML elements, and generally tidying up (including the concolidation and deletion of classes, ids and elements) the HTML and CSS files. 


![Site Langing Page](./images/horiseon-finished.gif)


## Table of Contents 


* [Code Refactor Example](#code-refactor-example)
* [Usage](#usage)
* [Learning Points](#learning-points)
* [Author Info](#author-info)
* [Credits](#credits)
* [License](#license)



## Code Refactor Example

```html
 <div class="benefits">
        <div class="benefit-lead">
            <h3>Lead Generation</h3>
            <img src="./assets/images/lead-generation.png" />
            <p>
                Inbound strategies for lead generation require less work for your business, bringing customers directly to your website.
            </p>
        </div>
        <div class="benefit-brand">
            <h3>Brand Awareness</h3>
            <img src="./assets/images/brand-awareness.png" />
            <p>
                Users find your business through paid and organic searches, increasing the search ranking and visibility for your business.
            </p>
        </div>
        <div class="benefit-cost">
            <h3>Cost Management</h3>
            <img src="./assets/images/cost-management.png" />
            <p>
                As the search ranking for your business increases, your advertising costs decrease, and you no longer need to advertise your page.
            </p>
        </div>
    </div>
```

Converting the above non-semantic div element into the semantic HTML elements, aside and section, to improve the accesibility and seo of the page.  [See this page on semantic elements](https://www.w3schools.com/html/html5_semantic_elements.asp)

```html
    <aside class="benefits">
        <section class="benefit">
            <h3>Lead Generation</h3>
            <img src="./images/lead-generation.png" alt=""/>
            <p>Inbound strategies for lead generation require less work for your business, bringing customers directly to your website.</p>
        </section>
        <section class="benefit">
            <h3>Brand Awareness</h3>
            <img src="./images/brand-awareness.png" alt=" "/>
            <p>Users find your business through paid and organic searches, increasing the search ranking and visibility for your business. </p>
        </section>
        <section class="benefit">
            <h3>Cost Management</h3>
            <img src="./images/cost-management.png" alt="" />
            <p>As the search ranking for your business increases, your advertising costs decrease, and you no longer need to advertise your page.</p>
        </section>
    </aside>

```

The three different benefit-[variable] classes were then edited down to a since class of benefit. [See this page on CSS selectors](https://www.w3schools.com/cssref/css_selectors.php)

```css
.benefit-lead {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-brand {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
```

This changed allowed for the CSS to be edited down to a single CSS function instead of three, reducing the repetition of the CSS file. 

```css
.benefit {
    margin-bottom: 32px;
    color: #ffffff;
}
```

## Usage 


![Updated Horiseon marketing webpage](./images/horison-full-screen.png)



## Learning Points 

This project was a great induction to the ways that HTML and CSS work together to create a webapplication.  I was taught the importance of semantics and specificity within HTML and CSS. Getting too specific will create a lot of repetition with in the CSS file but being too broad causes a lack of appropriate style and function.  I also learned that you can preview your readme in VS code, this happened toward the end of my work flow, as you can see by all of my README commits. I decided to not include alt text for the icons included in the webpage since they were simply there for style and design and would not add anything function for seo or accesibility. 



## Author Info

### Shea Schwennicke 

* [LinkedIn](https://www.linkedin.com/in/shea-schwennicke-76a378210/)
* [Github](https://github.com/sheaschwenn)




## License

Please refer to the LICENSE in the repo


---

© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.