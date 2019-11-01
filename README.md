# Anastasiia Vasylenko Resume
Stream-One-Project: User-Centric Frontend Development - Milestone Project

This is my Resume Website designed to showcase to potential employers the example of the websites I can build.
The website contains brief information about myself, the range of the programming languages I work with, highlights three of my projects
as an example of my work, and a contact form.

## UX
The goal of my project design was to make it minimalistic and user-friendly while giving the potential employer the exact
information they would be looking for without overwhelming them with unnecessary information. 

**User Story:**

> *As a potential employer, I want to find a candidate for an open position and to familiarize myself with who they are, their skills
as well as view what type of work they've done in the past. That way I can hire somebody who I know will be able to do the job 
required for my business.*

To help the above user achieve his goal, I designed my website to contains an overview of who I am as well as my photo on the background
to create a friendly and personable experience for the user. I also listed all of my programming skills and gave each of them a grade
based on my self-assessment. In the "Work Samples" section a user would be able to familiarize himself with the projects I've done in the past,
view their code source and deployed versions. The very last section allows the user to conveniently contact me if he chooses to. 
I also included links to my professional Social Media such as LinkedIn in the footer, along with my GitHub profile where the user can view my
repositories and the link the printable version of my resume should the user want to have it in hand.

## Features 
### Existing Features
* The website has a "collapsed" menu bar into a button in all versions that will open up menu options after a click on it. 
This is done to minimize the amount of content on the page so the user can find the information he needs easier and faster.
* The cards in the "Work Samples" section change their color when the user hovers over them.
* All the icons on the website including the ones in the footer use the same transition and change in size when the user hovers over them or clicks on them.
* Contact form fields are recognizable by the browser because each of them has its unique input type. This was if the user's information is saved in the browser, it will pop up in the fields automatically when the user start filling them out.
* The "paper airplane" in the "Contact" section is a .png image with a transparent background. This allowed me to add it as a background image while mantaining the custom color scheme of my website created by me.
### Features Left to Implement 
* In the future, I would like to add more projects as I work on them to the "Work Samples" section.  I would also like to include
a live demo preview of them within the cards that would only start once the user hovers over them.

## Technologies
1. HTML
2. CSS
3. Bootstrap (4.3.1)
4. Hover.css

## Testing
The employer user story has achieved the desired outcome. In the "About Me" section the employer can read an overview of who I am,
he can review my skills and how I assess my proficiency in each one of them. He also can view the projects I've done the past,
their code sources, deployed versions and read a brief overview of what those projects are. The employer can also view
my GitHub repositories and my Social Media to familiarize himself with me as a potential candidate even better, by clicking on the icons in the footer. If the employer chooses to contact me, he can conveniently leave his contact information and a brief message
in the "Contact" Section and also download a printable version of my resume from the icon in the footer.

Some manual testing has been done to ensure the website works well:
* If you try to submit an empty form in the "Contact" section, it will prompt a message and point out a field that is required
to be filled out. This field will prompt the user to one field at a time starting from the top one. This rule works for "Name",
"Email" and "Massage" fields. I left the "Phone Number" optional as it is more desirable for me to connect first via Email.

* All the links have `<target='_blank'>` attribute to ensure that should the user choose to click on them, the website he left from won't be closed in his browser. All links have been tested and respond properly.

The website is written for different screen versions with some elements hidden or re-aligned on smaller screens to ensure positive UX and to not overwhelm the user with the amount of elements on the screen. All versions for different screen sizes have been tested in Desktop Versions
(Google Chrome, Safari), Tablet Versions (iPad, iPad Pro) and Mobile Versions (iPhone X, iPhone 6, Samsung Galaxy).

An interesting bug has been found during developing a mobile version of the website in the Chrome browser. Mobile version of Safari
does not interpret correctly `<background-attachment='fixed'>` while Chrome Developer tools "Mobile view" show the background correctly.
To fix this bug, I used a media query for my `<top-section-container>` and resized a copy of the same image to ensure that the
correct part of it is being shown on the Mobile view. As for the `<contact-container>`, I changed the property of `<backgroung-attachment>` 
to 'scroll'. This ensured the correct positioning of the element on all three versions.

Another problem was encountered for the Mobile view caused by Bootstrap form. It appears it had set width parameters that were larger than 100% of the Mobile View Version. I resolved it by overwriting the width parameter in my style.css sheet and aligning 
items to the center of the container in index.html.

## Deployment

My website was deployed directly from the master branch via GitHub platform. All the new commits will update the repository
automatically without changing the link address. It can be viewed via this link: https://aavasylenko.github.io/milestone-project-1/ 

To run it locally, the user can clone this repository directly into his editor by pasting the following into the terminal:

`<git clone https://github.com/aavasylenko/milestone-project-1.git>`
## Credits
### Contents

All content in the "Work Samples" section was written by me following the video instructions of the Code Institute instructor.

### Media 

The background  picture of the `<top-section-container>` was taken from https://www.pexels.com/

The "paper-airplane" in the Contact section was taken from https://www.pngfly.com/

The picture of myself is owned by me.

### Acknowledgements

All the code was inspired by previous lessons in Code Institute.


