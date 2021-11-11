
# The New Yam Festival Website 
[Hosted Live Here](https://polyanyanwu.github.io/yam-festival-pp1/)

This site hopes to enlighten the public, especially people from outside Nigeria, on the cultural festival that is used to herald the harvesting and eating of new yams among the Igbo tribe in the South Eastern part of Nigeria. A brief mention is made of the history of the Igbo tribe. Yam and the festival is captured in colorful images and few videos of the festival is presented.

![Site Image on Different Screens](/docs/pp1_image.png)

## Design of the Site
I intended to have a three-page website having pages for the history, the festivals and Igbo tribe. We intended to have a logo, title and navigation bar as shown below.
![Design Wireframe Version 1](/docs/Yam_Festival_Main.png)

After the initial discussion with my mentor, the design was changed to having a navigation bar, banner image and banner text. It became apparent that the Search functionality was out of scope as that would require JavaScript, therefore it was removed from the design. I produced a revised wireframe below:
![Design Wireframe Version 2](/docs/Yam_Festival_Main_V2.png)

The main page was then produced according to the revised wireframe with two columns after the banner image. While reviewing the page, it seemed too crowded with information and not appealing to a user. I then decided to drop the idea of two columns and rather used flex technology to present the image gallery and information into necessary column depending on the device width of the user. 

## Features of the Site
The Site is is presented in three sections:
### 1. The Navigation Bar

The navigation bar has the main title of the site and has responsive navigation links to the Home, Festivals and Igbo Tribe sections, which enables the user to navigate easily to the section of interest.

### 2. The landing page image

The landing includes an image of a yam cutting action of a yam festival with text overlay to allow the user to have a feel of what the site would be presenting. An eye-catching animation grabs the user’s attention as the site is opening.
![Landing Page Image](/docs/landing_page.png)

### 3. The History of Yam Festivals

A brief description of yam is given here together with history of how the yam festival came into being among the Igbo tribe of the South Eastern Nigeria. This section is visible when the user visits the site or clicks on the Home navigation item.

The section also has a photo Gallery of Yam and textual descriptions, which is responsive to different sizes of screen. The full screen of a laptop or desktop gives a two-column image gallery/text while it reduces to single column as the device screen reduces.
![History Section](/docs/history_section.png)

### 4. Festivals Section
    
Thie Section has the Celebration Events in Video. The YouTube videos are are not on auto play and not muted which hands full control to the user. The two video clips uploaded in the site was set to autoplay and muted to enable a beautiful user interface to Iphone users, who otherwise would have only seen an blank section with a play arrow. 
![Festival Section](/docs/festival_section.jpg)

### 5. Igbo Tribe Section
This section give a brief description of the Igbo tribe and a video that enlightens the user about the Igbo tribe of Nigeria.
![Igbo Tribe Section](/docs/igbo_section.jpg)

### 6. The Footer Section
The footer has the links to take the user back to any of the three main sections of the site. In addition, the Contact us part of the footer has the icons that links the user to the social network of the site designer.

![Igbo Tribe Section](/docs/footer_section.png)

### Features Left to Implement
It would have been nice to have a feedback form to obtain the users comments and find out if the user is interested in attending any future Yam Festival in Nigeria.

## Testing
* ### Image and Information Rendering

    I noticed that the banner image was not displaying when I deployed to Github pages. The issues was traced to a broken URL due to change of the banner display from background image to use of img element without adjusting the source accordingly. The source was adjusted to the correct URL and the image started displaying.

* ### Validity of the HTML

    The HTML text was validated using [W3C Markup Validation Service](https://validator.w3.org/). It was realized that the HTML had few errors, which were identified and fixed as shown below:

    ![HTML Validation Result](/docs/html_validation.png)

    The errors due to few missing tags in the cause of rearrangement of elements were identified and corrected. After that the html validated without any errors.

* ### Validity of the CSS

    The CSS text was validated using [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/validator). It was realized that the CSS had two errors, which were identified and fixed as shown below: The first error 0.5% 1% 0.5 1% for padding was resolved by using the shorthand 0.5% 1% and the second error was resolved by deleting the 0.

    ![CSS Validation Result](/docs/css_validation.png)

* ### Accessibility & Performance Testing

    Performance test was carried out using Lighthouse tool provided by the Chrome Development tool. Initial performance result pointed to deficiencies in the size and type of images on the site - most were .jpg and .png. The images were converted to .webp using  [cloud convert](https://cloudconvert.com/) and then  [tiny png](https://tinypng.com/) was used to compress the images further. Issue of non-caching of static images was also observed. Cache Control was added to the header with properties content="max-age=31536000" and content="public". After these changes to the images and caching, the Lighthouse produced the result below:
    ![Performance Result](/docs/performance_test.png)


* ### Browser Compatibility 

    The website was tested with the major browsers available and found to work as expected: Chrome, Firefox, Safari, and Microsoft Edge. It was while testing on Safari on the Iphone that I noticed that the .mp4 videos were not playing. To resolve this I had to specify the type="video/mp4", gave it an autoplay and mute attribute in order to have the video show a picture instead of being blank. However, the mute attribute ensures the voice is not out until the user chooses to hear it. Apart from the iPhone, Android phones had no issues with playing the videos.

* ### Accessibility with Different Device Widths

    Using the Chrome Development tools, the responsiveness of the site to various screen sizes was simulated. This led to the adjustment of the CSS until the site supports numerous device widths from the smallest hand held devices to full computer monitor screens.
    ![Responsive Screens](/docs/various_screen_sizes.png)
    The first image above shows a full screen of three image columns and two video columns dsiplayed on a laptop computer screen. The images below the laptop screen are simulations on the ipad (with two image columns) and small screen of Moto G4 and Iphone X displaying single column for both video and images.

## Deployment
The site was deployed to GitHub pages. The following steps were used to effect the deployment:
1. In the GitHub click on repositories, and select yam-festival-pp1
2. Click on the Settings tab
3. From the settings page, click on Pages
4. In the source section drop-down menu, select the Main Branch
5. Once the Main branch has been selected, the page will be refreshed with a detailed ribbon display to indicate the successful deployment.
6. The live site can be found at [New Yam Festival] (https://polyanyanwu.github.io/yam-festival-pp1/)

## Credits
### i. Design
Inspiration on the banner and cover text was drawn from the Love Running Essentials project. Criticism and guidance from my Mentor (Brian O'Hare) and class coordinator (Simen Daehlin) assisted immensely in my continual adjustment of the design until it got to this likeable and informative state.
The lectures from the Learning Management System of the Code Institute was the origin most of the knowledge on HTML5 and CSS which were used in this project.

### ii. Content
Text content on the mythology of the yam festival was taken from [Juju Medium](https://medium.com/@emailthisjuju/iwa-ji-new-yam-festival-a7b204fc3bf6). Information on The Yam Crop Growing on Sticks was obtained from [Ogidi Olu Farms](https://www.ogidiolufarms.com/tag/modified-trellis-method/). 
    
The icons in the footer were copied from the Font Awesome.
### iii. Media
The beautiful pictures of celebrations were downloaded from the following sources, converted, compresssed and used on this site:
*   [IITA](https://www.iita.org/test-yam/) 
* [Peoples Gazette](https://gazettengr.com/igbos-in-ghana-to-celebrate-new-yam-festival/) 
* [Wikipedia](https://en.wikipedia.org/wiki/New_Yam_Festival_of_the_Igbo#/media/File:NewYam-IgboFestival-Dublin.jpg)
* [Umuzu Mainland Develoment Association](https://umdaokija.org/festivals/) 
* [Guardian Newspapers](https://guardian.ng/life/iwa-ji-the-new-yam-festival-in-igbo-land/)
* [Moving across cultures](https://clairekavculturestudiescom.wordpress.com/2020/01/15/nigerias-new-yam-festival/)
* [Juju Medium](https://medium.com/@emailthisjuju/iwa-ji-new-yam-festival-a7b204fc3bf6)

    The clip that plays on the first video on the Yam Celebrations were curated from [Channels Television](https://www.youtube.com/watch?v=awBHeFO3228) on YouTube. The video on Enugu People celebrating New Yam Festivals was embedded from their YouTube [Enugu Celebration](https://youtu.be/ZrPPYXIdAZg).

    Thanks to God and my family for their support and understanding while I stayed hours on the Laptop.
