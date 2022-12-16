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

