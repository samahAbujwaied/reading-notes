# IMAGES
![](https://assets.digitalocean.com/articles/how-to-build-a-website-with-css/two-images.png)
* Controlling size of images in CSS
* Aligning images in CSS
* Adding background images
**Controlling the size and alignment of your images using CSS keeps rules that affect the presentation of your page in the CSS and out of the HTML markup.**

## How could controlling size of images in CSS ?
![](https://mbostock.github.io/protovis/docs/bar-bhlw.png)
*You can control the size of an image using the width and height properties in CSS, just like you can for any other box.*
*Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download.*


## How could aligning images using CSS ?
![](https://miro.medium.com/max/1804/1*b8DSnVjKVMRSlKLhml_d3w.png)
*Rather than using the ```<img>``` element's align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved:*
1. The float property is added to the class that was created to represent the size of the image.
2. New classes are created with names such as align-left or align-right to align the images to the left or right of the page. These class names are used in addition to classes that indicate the size of the image.

## How to centering images using CSS ?
![](https://i2.wp.com/css-tricks.com/wp-content/uploads/2011/10/centered.gif?resize=436%2C330)
*By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a block- level element using the display property with a value of block.*
*Once it has been made into a block-level element, there are two common ways in which you can horizontally center an image:*
1. On the containing element, you can use the text-align property with a value of center.
2. On the image itself, you can use the use the margin property and set the values of the left and right margins to auto.
*You can specify class names that allow any element to be centered, in the same way that you can for the dimensions or alignment of images.*

## Background Images
![](https://i.stack.imgur.com/IGGAv.jpg)
**The background-image property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box.**
### Repeating images 
* background-repeat
* background-attachment

**The background-repeat property can have four values:**
1. repeat
  >The background image is repeated both horizontally and vertically (the default way it
    is shown if the background- repeat property isn't used).
2. repeat-x
  >The image is repeated horizontally only.
3. repeat-y
  >The image is repeated vertically only.
4. no-repeat
  >The image is only shown once.

##  background-attachment
**The background-attachment property specifies whether a background image should stay in one position or move as the user scrolls up and down the page. It can have one of two values:**
1. fixed
  >The background image stays in the same position on the page.
2. scroll 
  >The background image moves up and down as the user scrolls up and down the page.

## Background position
*When an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed.*
*This property usually has a pair of values. The first represents the horizontal position and the second represents the vertical.*
![](https://i.pinimg.com/originals/a9/84/0a/a9840a7ddb1d028748759e8c47c5796f.gif)
## contrast of Background Images
**If you want to overlay text on a background image, the image must be low contrast in order for the text to be legible.**
![](https://i1.wp.com/css-tricks.com/wp-content/uploads/2014/03/conic-radial-gradient-compare.png?fit=2000%2C1000&ssl=1)
## Practical information 
* Search engine optimization
*  Using analytics to understand visitors
* Putting your site on the web

### search engine optimization (SEO)
* the Basics
**Search engine optimization (or SEO) is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers.At the heart of SEO is the idea of working out which terms people are likely to enter into a search engine to find your site and then using these terms in the right places on your site to increase the chances that search engines will show a link to your site in their results. In order to determine who comes first in the search results, search engines do not only look at what appears on your site. They also consider how many sites link to you (and how relevant those links are). For this reason, SEOis often split into two areas: on-page techniques and off-page techniques.**

#### on-Page techniques
![](https://digiwalebabu.com/wp-content/uploads/2018/06/on-page-seo.png)

**On-page techniques are the methods you can use on your web pages to improve their rating in search engines.The main component of this is looking at keywords that people are likely to enter into a search engine if they wanted to find your site, and then including these in the text and HTML code for your site in order to help the search engines know that your site covers these topics.Search engines rely very heavily on the text that is in your pages so it is important that the terms people are going to search for are in text. There are seven essential places where you want your keywords to appear. Ensuring that any images have appropriate text in the value of their alt attribute also helps search engines understand the content of images.**

#### off-Page techniques
![](https://www.expert-seo-training-institute.in/blog/wp-content/uploads/2019/01/Off-Page-SEO-Techniques.jpg)
**Getting other sites to link to you is just as important as on-page techniques. Search engines help determine how to rank your site by looking at the number of other sites that link to yours. They are particularly interested in sites whose content is related to yours. For example, if you were running a website that sold fish bait, then a link from a hairdresser is not likely to be considered as relevant as one from an angling community. Search engines also look at the words between the opening ```<a> ```tag and closing ```</a>```  tagin the link. If the text in the link contains keywords (rather than just click here or your website address) it may be considered more relevant. The words that appear in links to your site should also appear in the text of the page that the site links to.**


##### how to identify keyWords and Phrases?
**Determining which keywords to use on your site can be one of the hardest tasks when you start to think about SEO. Here are six steps that will help you identify the right keywords and phrases for your site.**
* Brainstorm 
* organiz
* research 
* compare 
* refine
*  map
## analytics: learning about your Visitors
**As soon as people start coming to your site, you can start analyzing how they found it, what they were looking at and at what point they are leaving. One of the best tools for doing this is a free service offered by Google called Google Analytics.**
* Signing up 
* How it works
* The tracking code

## how many PeoPle are coming to your site?
**The overview page gives you a snapshot of the key information you are likely to want to know. In particular, it tells you how many people are coming to your site.**
* Visits
* unique Visits
* Page Views
* Pages per visit
* average time on site
* date selector

## What are your Visitors looking at?
**The content link on the left-hand side allows you to learn more about what the visitors are looking at when they come to your site**
* Pages
* landing Pages
* top exit Pages
* Bounce rate

## Where are your Visitors coming from?
* referrers
* direct
* search terms
* advanced features

## domain names & hosting
* domain names 
*Your domain name is your web address (e.g. google.com or bbc. co.uk). There are many websites that allow you to register domain names. Usually you will have to pay an annual fee to keep that domain name. These sites usually have a form that allows you to check whether your preferred domain name is available, and because millions of domain names have already been registered, it might take you a while to find the one that is right for your site. A lot of sites that offer domain name registration also offer web hosting.*
* Web hosting
*So that other people can see your site, you will need to upload it to a web server. Web servers are special computers that are constantly connected to the Internet. They are specially set up to serve web pages when they are requested. With the exception of some very large sites, most websites live on web servers run by web hosting companies. This is usually far cheaper and more reliable than trying to run your own web servers. There are lots of different types of hosting on offer. We will now take a look at some of the key things that will help you choose which hosting company to use.*
![](https://www.fastwebhost.in/blog/wp-content/uploads/2017/03/domain_name_vs_website_hosting.png)

## FTP & third Party tools
*To transfer your code and images from your computer to your hosting company, you use something known as File Transfer Protocol.*
*As the name suggests, File Transfer Protocol (or FTP) allows you to transfer files across the Internet from your computer to the web server hosting your site.*
*There are many FTP programs that offer a simple interface that shows you the files on your computer alongside the files that are on your web server. These allow you to drag and drop files from your computer to the server or vice versa.*