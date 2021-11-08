
# The New Yam Festival Website

This site hopes to enlighten the general public, especially people from outside Nigeria, on the cultural festival that is used to herald the harvesting and eating of new yams among the Igbo tribe in the South Eastern part of Nigeria. A brief mention is made of the history of the Igbo tribe. Yam and the festival is captured in colorful images and few videos of the festival is presented.

![Site Image on Different Screens](/docs/pp1_image.png)

## Design of the Site
I intended to have a three-page website having pages for the history, the festivals and Igbo tribe. We intended to have a logo, title and navigation bar as shown below.
![Design Wireframe Version 1](/docs/Yam_Festival_Main.png)

After the initial discussion with my mentor, the design was changed to having a navigation bar, banner image and banner text. I produced a revised wireframe below:
![Design Wireframe Version 2](/docs/Yam_Festival_Main_V2.png)

The main page was then produced according to the revised wireframe with two columns after the banner image. While reviewing the page, it seemed too crowded with information and not appealing to a user. I then decided to drop the idea of two columns and rather used flex technology to present the image gallery and information into necessary column depending on the device with of the user. 

## Features of the Site
The Site is is presented in three sections:
### 1. The Navigation Bar

The navigation bar has the main title of the site and has responsive navigation links to the Home, Festivals and Igbo Tribe sections which enables the user to easily navigate to the section of interest.

### 2. The landing page image

    The landing includes an image of a yam cutting action of a yam festival with text overlay to allow the user to have a feel of what the site would be presenting. An eye catchih animation grabs the users attention as the site is opening.
![Landing Page Image](/docs/landing_page_image.png)


### 3. The History of Yam Festivals

A brief description of yam is given here together with history of how the yam festival came into being among the Igbo tribe of the South Eastern Nigeria. This section is visible when the user visits the site or clicks on the Home navigation item.

The section also has a photo Gallery of Yam and Celebrations which is responsive to different sizes of screen. The full screen of a laptop or desktop gives a three-column image gallery while it reduces to two columns or single comlum as the device screen reduces.
![History Section](/docs/history_section.png)

### 4. Festivals Section
    
Thie Section has the Celebration Events in Video. The YouTube videos are are not on auto play and not muted which hands full control to the user. The two video clips uploaded in the site was set to autoplay and muted to enable a beautiful user interface to Iphone users, who otherwise would have only seen an blank section with a play arrow. 
![Festival Section](/docs/festival_section.png)

### 5. Igbo Tribe Section
This section give a brief description of the Igbo tribe and a video that enlightens the user about the Igbo tribe of Nigeria.
![Igbo Tribe Section](/docs/festival_section.png)

### 6. The Footer Section
The footer has the links to take the user backt to any of the three main sections of the site. n addition the Contact us part of the footer has the icons that links the user to the social network of the site designer.
![Igbo Tribe Section](/docs/footer_section.png)

### Features Left to Implement
It would have been nice to have a feedback form to obtain the users comments and find out if the user is interested in attending any future Yam Festival in Nigeria.

## Testing
* ### Image and Information Rendering

    I noticed that the banner image was not displaying when I deployed to Github pages. The issues was traced to a broken URL due to change of the benner display from background image to use of img element without adjusting the source accordingly. The source was adjusted to the correct URL and the image started displaying.

* ### Validity of the HTML

    The HTML text was validated using [W3C Markup Validation Service](https://validator.w3.org/). It was realised that the HTML had few errors which were identified and fixed as shown below:

    ![HTML Validation Result](/docs/html_validation.png)

    The errors due to few missing tags in the cause of rearrangement of elemnts were identified and corrected. After that the html validated without any errors.

* ### Validity of the CSS

* ### Performance Testing

* ### Browser Compatibility 

* ### Assebility by Different Device Widths

