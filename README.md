# Milica Radulovic - My Yoga Adventure


![Website responsive](assets/readme-img/respo.webp)

[Milica Radulovic - My Yoga Adventure](https://radule90.github.io/CI_PP_1/) website is set up as a personal yoga travel blog, where users can learn more about Milica and her love for yoga, and travel and connect. In terms of appearance, I tried to keep a minimalistic look with little detail that will embellish the site for visitors.


***
## Visual Design

### Colors

- For the base color, a shade of purple was chosen, a nice color that corresponds to the theme of the site.
- For the color of the letters, a shade of dark gray was chosen because it is not as intense as pure black, it has a more pleasant appearance and does not hinder readability and accessibility.
For the color of the letters, a shade of dark gray was chosen because it is not as intense as pure black, it has a more pleasant appearance and does not hinder readability and accessibility.
- Colour contrast was first verified on [WebAIM](https://webaim.org/resources/contrastchecker/).  
![Color Palette from coolors.co](assets/readme-img/palette.webp)

### Fonts

- I chose the font Open Sans, sans-serif letterform font from [Google Fonts](https://fonts.google.com), due to its clean appearance and readability, but it is not too serious for a website of this type.  
![Text Font](assets/readme-img/textfont.webp)

- Quicksand, also sans-serif letterform from [Google Fonts](https://fonts.google.com), alone to emphasize the specificity of the navigation bar without disturbing the appearance of the rest of the website.  
![Nav-bar Font](assets/readme-img/navfont.webp)

### Icons

- I have used [ICONS8](https://icons8.de) as a source for the decorative icons on the site, and adjusted the colors for website. Icons were selected that I thought complement the look of the website and do not disturb its essence.  
![Font Awsome Icons](assets/readme-img/icons8.webp)

- I have used [Font Awsome](https://fontawesome.com) for social media.  
![Font Awsome Icons](assets/readme-img/faw.webp)



### Images

- Images are a very important part of this site, because the theme of the site is yoga journey.
- All photos are the property of Milica Radulovic.
- I converted the images to [WebP](https://developers.google.com/speed/webp) format. After installing the libwep codec, the photos were converted in terminal with a command:

```sh
cwebp [options] -q input_file -o output_file.webp
```

***

## Styling / Formating

- In HTML I have used semantic elements in appropriate places and HTML entities. Whereas I used div (non-semantic) elements as container for decorative images and for positioning.
- Some time ago I came across this one [Write better CSS using logical properties](https://www.youtube.com/watch?v=kzvmaVik4mA), and because of the recommendation I started using logical properties.
- I did most of the positioning with Flexbox (learnd at [CSS-Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)), while I feel comfortable working with it.
- For embellishment and a kind of interactivity, I applied the transform property with the function scale ([Code Institute - Love Running Project](https://codeinstitute.net/de/)) and skew function ([MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/skew)) in several places.


### Header section

- The background image over the entire viewport seemed to me to be a fairly nice solution, because the user immediately gets to know the person whose journey they are going to read about.
- I also add the transparent mask to navigation bar in order to improve readability.  
![Website Header](assets/readme-img/header.webp)

### About section

- The heading is aligned left on purpose because the text is directly related to it and represents the whole.
- I used a light shade of purple as the background color, because it seemed calming and relaxing and in line with the images and theme of the site.
- The font color is a shade of gray and contrast with background-color is checkd with [WebAIM](https://webaim.org/resources/contrastchecker/).
- As an addition to the text, there is a firelog pose icon from [ICONS8](https://icons8.de). a decoration that fits in with the rest.
![Website About](assets/readme-img/about.webp)
- I kept most of that concept as well through the blog section of the site.
- Next comes image and is set as background with attachment proporty to fixed, in order to create an effect similar to [Parallax Scrolling](https://www.w3schools.com/howto/howto_css_parallax.asp) ([iOS Devices Bug](#bugs)).  


### Blog section

- I used a slightly modified concept in this section. I didn't want to deviate too much because these two are similar, they have a lot of text and images.
- Between articles there are background images that also represent the demarcation between different sections and articles.


### Gallery

- I decided for a white background in the next two sections of the site, in order to avoid monotony and make it clear to the user that the part of the site is finished (let's call it the "text part of the site") and the sections related to social networks and contact begin.
I used [W3Schools](https://www.w3schools.com/css/css3_flexbox_responsive.asp) code of the gallery to adapt it to the requiremnets of the project.
- The gallery is responsive. I decided that two columns should be displayed on small screens and three on large screens. I achieved this by setting the display of the last column container to none and using @media for a minimum width of 768px to display it again.
- I added the instagram button as a suggestion to the user that they can find more images on the instagram profile of site owner.  
![Website Gallery](assets/readme-img/gallery.webp)

### Connect section

- This section is separated from the rest with a border line, applied border image property with linear gradient (researched on [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/border-image)), it seemed like a nice and simple solution for dividing sections with a white background.
- Then, I added a box shadow to make the shape stand out.
- The form has validation and is responsive.  
![Website Connect](assets/readme-img/connect.webp)

### Footer

- For this section i chose dark gray background color, at first I thought it should be a shade of purple, but however the site would become boring, this is how it suggests that this is the end of the site.
- I included a short copyright text in it.
- Arrow to return to the top of the page, and when hovered over it scales itself as a suggestion that this is the link.
- Also included are links to social networks and the colors are inverted on the hover as a hint that this is the link to the user.


***

## Validation and testing

### HTML
- has been validated with [W3C Markup Validation Service](https://validator.w3.org).


### CSS
- has been validated with [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/).


### Accessibility

- Color contrast was verified on [WebAIM](https://webaim.org/resources/contrastchecker/).
- The following results were achieved on Chrome Lighthouse:

SLIKA REZULTATA!!!!!!!

- The site looks good on all common screen sizes, including 4k ([iOS Devices Bug](#bugs)).

- The navigation bar, header, about, blog, connect and footer sections are all readable and understandable with working internal and external links.

- The Connect form works, and requires input to every entry.


### Bugs

#### Partialy bugs
- Proporty background-attachment with value fixed does not work properly on iOS devices (iPads, iPhones). Tested with [BrowserStack](https://www.browserstack.com/).
 
  - Possible solutions 
    - The solution that is to change the value of    background-attachment to scroll for mobile phones and tablets sizes ([W3Schools](https://www.w3schools.com/howto/howto_css_parallax.asp)). But I didn't want to implement this solution, because the page was displayed normally on Android and HarmonyOS devices.
    - Rory (mentor) referred me to [this article](https://www.browserstack.com/guide/create-browser-specific-css) on [BrowserStack](https://www.browserstack.com/) to try to come up with a solution. After applying the CSS code for browser recognition and testing on a certain number of iOS devices on [BrowserStack](https://www.browserstack.com/), the browser, Safari, was recognized and the `background-attachment: scroll;` property was applied to it and the site worked, the problem remained with older models. Although it is not the best solution, I decided to implement it. In the future when I learn new technologies I will fix the bug.

***

## Credits

- [Code Institute](https://codeinstitute.net/de/)
- Rory Patrick Sheridan (Mentor) - Great advice and guidance
- [Mozilla Developer Networks](https://developer.mozilla.org/en-US/) - Additional learning resources
- [W3Schools](https://www.w3schools.com) - Additional learning resources
- [CSS-Tricks](https://css-tricks.com) - Additional learning resources
- [Dave Gray](https://www.youtube.com/c/DaveGrayTeachesCode) - Additional learning resources
- [Kevin Powell](https://www.youtube.com/@KevinPowell) - Additional learning resources
- [BrowserStack](https://www.browserstack.com/) - Website Testing on iOS
- [Coolors.co](https://coolors.co/) - Palette generator

***

## Content

- The base code for the "Parallax" Scrolling effect was taken from [W3Schools](https://www.w3schools.com/howto/howto_css_parallax.asp), and then adjusted for the needs of the site.
- The base code for the Gallery section was taken from [W3Schools](https://www.w3schools.com/css/css3_flexbox_responsive.asp), and then I adjusted it for the needs of the site.

***

## Media

- The images belong to Milica Radulovic.
- Decorative icons are taken from [ICONS8](https://icons8.de)
- Icons for social networks are taken from [Font Awsome](https://fontawesome.com).
