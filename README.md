__**Code Institute User-Centric Frontend Development - Shadow Racing AI**__

The goal of this website is to create leads for an artificial intelligence-based horse racing tipping service.

Given that the tipping service is based on artificial intelligence, the website needs to have a modern slick design
which gives the right impression to potential users.

**Technologies**

1. html
2. css
3. jquery
4. javascript
5. bootstrap 4.3.1

**External sources**

1. Font-Awesome
2. Google Fonts

__**Features**__

The site has a modern navigation using the fa-ellipsis-v (three vertical dots) which is always collapsed to give the
website the clean design is requires. It has smooth scrolling using the scroll-behaviour: smooth; attribute. Modern,
but popular fonts were selected and imported from google fonts. I have used uniform icons from font awesome for each
section of the site to give it continuity. A favicon has been added using a 16x16 version of the logo png.

**Features Left to Implement**

As present the site is purely for advertising purposes, in the future I will add sign up and login features behind a
pay wall, a user section where they can see the day tips and also add a chart which automatically updates from results
rather than a static image and will be interactive for users.

__**User Story**__

As a user I am looking for a relaiable horse tipping service, that can provide me with daily tips with a simple user
experience.

I want a service that can provide me with consistant monthly profits, for a minimum of effort.

__**Testing**__

The website has an enticing home page which draws the user in. As the home page occupies the whole screen on loading there's
a chevron indicating more information below which takes the user down to the about us section when clicked. It uses smooth
scrolling so there’s no jerky movements to the site and it navigates well.

The toggler dropdown menu provides the user with the option to scroll to the other sections of the website, this also uses
the smooth scroll-behaviour attribute. The menu automatically closes when navigated away from using some additional javascript.

There is a description of the team behind the service as well as details of the timing and type of tips the service provides.
There is also a chart showing the systems results over time, satisfying the users questions about how the service works.
Below this there is a contact form for the user to find out more information about the service if they still have questions.

The contact form is not yet functional, the submit button currently opens the users default email. However the form includes
validation that each section has been completed.

The bookmaker logos in the affiliate section link directly to their websites and open in a separate browser window using
'target="_blank"', as do the social icons in the footer (these only link to the home page of the sites as no social sites
currently exist for Shadow Racing). User Guide, Disclaimer and T&Cs can be downloaded from the footer using the download
attribute. All links have been tested multiple time to ensure they link to the correct site / document.

I have tested the website on all the main browsers including IE, Chrome, Firefox, Safari and Opera. It has also been tested
on smaller screens from ipad pro down to iphone5 using the inspect function in google chrome and an IOS device. Media queries
have been extensively used to re-size the text and icons when used on smaller devices.

During the testing phase, it became apparent that the logo and chart images were not re-sizing dependent on device, rather
than use a media query I opted for the following code which force the images to resize as the screen size is reduced.

display: flex;
justify-content: center;

However despite the website working perfectly on all sizes in google chromes inspect feature, the was not the case when viewed
on an actual IOS device. Addtional code was required in order to stop the logo from mis-shaping on all devices.
```
    display: -webkit-box;
    display: -moz-box;
    display: -ms-flex;
    display: -webkit-flex;
    display: flex;
    justify-content: center;
    -webkit-box-align: center;
    -webkit-flex-align: center;
    -ms-flex-align: center;
    -webkit-align-items: center;
```
__**Deployment**__

This site is hosted using GitHub pages, deployed directly from the master branch. The deployed site will update automatically
upon new commits to the master branch. In order for the site to deploy correctly on GitHub pages, the landing page must be
named index.html. The site is published at https://richep365.github.io/ShadowRacingAI/

__**Credits**__

**Content**

All content was written by me, including the disclaimer and terms & conditions, which I wrote and adapted from my website
i-betuk.com for this project.

**Media**

The 2 horse racing photos were taken from pixabay.com, they have both had opaque overlays added. The logo was designed by
me using Brandmark.io

**Acknowledgements**

Addition of smooth scrolling was found at CCS-Tricks

https://css-tricks.com/snippets/jquery/smooth-scrolling/

This doesn't not work on IE or Safari it requires javascript to fix this issue, but that's outside te scope of this project.

The short peice of javascript to close the toggle icon when navigating away, was taken from the following stackoverflow answer
```
    <script>
        $(document).on('click', function() {
            $('.collapse').collapse('hide');
        })
    </script>
```
https://stackoverflow.com/questions/21496304/bootstrap-collapse-component-not-closing-menu-on-clicking-away/32608307

The following code to remove the border from the toggle icon, when clicked, was also taken from stack overflow
```
    .navbar-toggler:focus,
    .navbar-toggler:active {
        outline: none;
        box-shadow: none;
    }
```
https://stackoverflow.com/questions/50668594/removing-the-border-color-of-the-navbar-toggler-hamburger-icon-bootstrap-4

The code to change the focus colour of the active form cells was found at the following link.

https://blog.blakesimpson.co.uk/read/71-changing-the-twitter-bootstrap-input-outline-color
```
    .center-form input:focus,
    .center-form textarea:focus,
    .center-form select:focus {
        border-color: #e0443c;
        box-shadow: 0 0 1px #e0443c inset;
        }
```
I also had to look up how to add a favicon, and found the simple answer here.

https://stackoverflow.com/questions/9943771/adding-a-favicon-to-a-static-html-page








