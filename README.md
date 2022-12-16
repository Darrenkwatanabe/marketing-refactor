# marketing-refactor

## Technology Used

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)      |   
| Git | [https://git-scm.com/](https://git-scm.com/)     |    

# Project Description

[Visit the Deployed Site] (https://darrenkwatanabe.github.io/marketing-refactor/)

The goal of this project is to refactor the HTML AND CSS while utilizing the 
correct semantic elements, making the file organized and easy to read.

Horiseon is here to provide you with many things:
1. To help you utilize the internet to find what is best for your business.
2. To manage how your business is exposed to the public when being searched.
3. To assist you in optimally utilizing social media.


## Code Refactor Example

First we were given the starter code containing below:

```html
<div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>
```

I changed the non-semantic div header class to the header semantic element. 
As well as changing the non semantic div element to a nav element. 

```html
<h1>Hori<span class="seo">seo</span>n</h1>
        <nav>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </nav>
    </nav>
```

Since I had made these changes on HTML, I had to update the changes on CSS.

```css
.header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}

.header h1 {
    display: inline-block;
    font-size: 48px;
}
```

Since I wasn't target the class header and now targeting the element header, I updated as shown:

```css
header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}

header nav h1 {
    display: inline-block;
    font-size: 48px;
}
```

## Usage

To make sure this website displays correctly, we can look at the following:

```html
<id class="content">
        <section class="search-engine-optimization">
            <img src="./assets/images/search-engine-optimization.jpg" alt="search engine optimization" class="float-left" />
            <h2>Search Engine Optimization</h2>
            <p>
                The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
            </p>
        </section>
```

This shows that we are working with the content class in the html, so we find this class 
in the css file

```css
.content {
    width: 75%;
    display: inline-block;
    margin-left: 20px;
}
```

By looking at this, we see that the code under the class content will have a width of 75%,
the information within content will have top and bottom margins that are acknowledged, and
it will have a margin of 20 px to the left. 

In addition to that, we see that there is another class below that named "search-engine-
optimization". So we find that class in the css file as well.

```css
.search-engine-optimization {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}
``` 

We see that under the search-engine-optimization class, it will have a bottom margin of 
20 px, padding of 50px, and a height of 300 px all relating to the sizing. Also included
is the font-family, with a provided background color, and text color as well.

As we go through the html, we'll run into another section showing: 

```html
<id class="benefits">
        <section class="benefit-lead">
            <h3>Lead Generation</h3>
            <img src="./assets/images/lead-generation.png" alt="lead generation" />
            <p>
                Inbound strategies for lead generation require less work for your business, bringing customers directly to your website.
            </p>
        </section>
```

Again, this shows we are working with the benefits class in the html, so we look for this 
class in the css file.

```css
.benefits {
    margin-right: 20px;
    padding: 20px;
    clear: both;
    float: right;
    width: 20%;
    height: 100%;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #2589bd;
}
```

We see that in the benefits class, it will have a margin to the right of 20px and a padding 
of 20px. Also shows that this box will be clear and float to the right in terms of position.
It will have a width of 20% and a height of 100% related to the size. And includes the font-
family and background color as well.

## Learning Points

First and foremost, I learned how to utilize and link my html file to my css file. 
I also learned to properly utilize the semantic elements so that my file is much
more organized and easier to read. This project made constantly reminded me to save
my work as I go, using pushes on the CLI. 

## Author Info

### Darren Watanabe


*[Github](https://github.com/Darrenkwatanabe)
*[LinkedIn](https://www.linkedin.com/in/darren-watanabe-982526253/)
*[Email](watanabedarren@yahoo.com)

