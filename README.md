# INFO6150 - Portfolio Readme

## Overview

The **Portfolio** HTML page serves as a user interface for showcasing my work and accomplishments. This document provides an overview of the HTML page and explains the purpose of various HTML elements and tags used in its structure.


## Table of Contents

1. [Page Structure](#page-structure)
2. [Favicon](#favicon)
3. [Table](#table)
4. [Form](#form)
5. [Images](#images)
6. [Hyperlink](#hyperlink)
7. [Button](#button)
8. [Audio](#audio)
9. [Video](#video)
10. [Header](#header)
11. [Footer](#footer)
12. [Summary](#summary)
13. [Menu](#menu)
14. [Contact](#contact)

## Page Structure <a name="page-structure"></a>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Meta tags, title, stylesheet, and favicon -->
</head>
<body>
    <!-- Page content -->
</body>
</html>
```

The HTML page is structured with the standard `<!DOCTYPE html>` declaration. It includes metadata, a title, external stylesheets, vue framwork, and a favicon.

## Favicon <a name="favicon"></a>

```html
    <link rel="icon" href="/assets/favicon-32x32.png" sizes="32x32" type="image/x-icon">
```
![image](https://github.com/likun945/INFO6150/assets/98712201/5bfd8a7f-7451-482b-8d2c-48470e9bb89b)

This favicon represents the abbreviation "KL" for KUN LI.

## Table <a name="table"></a>

```html
<table>
    <tr>
        <td>LinkedIn</td>
        <td>
            <a
                href="https://www.linkedin.com/in/kun-li-355638249/"
                target="_blank"
            >
                https://www.linkedin.com/in/kun-li-355638249/
            </a>
        </td>
    </tr>
    ...
</table>;

```
![image](https://github.com/likun945/INFO6150/assets/98712201/2b2fde95-bff9-468f-9402-93bb52e2ef6a)
This table serves as a structured way to present links to online profiles, with each row containing the name of the platform and the corresponding URL.

## Form <a name="form"></a>

```html
                        <form id="form" v-if="!hasRating" @submit="submitForm">
                            <div class="rate-content">
                                <span style="margin-right: 8px"><b>Rate my website</b></span>
                                <div class="rating">
                                    <div>
                                        <input type="radio" name="rate" @click="rating='Excellent'">
                                        <label>Excellent</label>
                                    </div>
                                    <div>
                                        <input type="radio" name="rate" @click="rating='Very Good'">
                                        <label>Very Good</label>
                                    </div>
                                    <div>
                                        <input type="radio" name="rate" @click="rating='Good'">
                                        <label>Good</label>
                                    </div>
                                    <div>
                                        <input type="radio" name="rate" @click="rating='Fair'">
                                        <label>Fair</label>
                                    </div>
                                </div>
                            </div>
                            <div style="margin-top:10px">
                                <input type="submit" class="custom-button" value="Submit">
                            </div>
                        </form>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/37a373f7-a2de-4856-9a54-c97436cf9eb4)
This form is designed to gather user ratings of a website, allowing them to choose a rating category (Excellent, Very Good, Good, or Fair) and submit their feedback.

## Images <a name="images"></a>

```html
                                <div class="gallery">
                                    <figure>
                                        <a target="_blank" href="/assets/cargurus.jpg">
                                            <img src="/assets/cargurus.jpg" alt="Cinque Terre" width="276" height="195">
                                        </a>
                                        <figcaption class="desc">First day at Cargurus</figcaption>
                                    </figure>
                                </div>
```
<img width="826" alt="1694999466447" src="https://github.com/likun945/INFO6150/assets/98712201/a924d2f4-02c5-4b6d-8088-88beadccc1f5">

The src attribute specifies the path to the image file, and the alt attribute provides alternative text for accessibility purposes. In this example, the image is associated with the description "First day at Cargurus."

## Hyperlink <a name="hyperlink"></a>

```html
<a href="https://www.linkedin.com/in/kun-li-355638249/" target="_blank">https://www.linkedin.com/in/kun-li-355638249/</a>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/e5083c0a-b86f-416f-ac96-0705130347a5)

In this code, the <a> element is used to create a hyperlink. The href attribute specifies the destination URL, which, in this case, links to a LinkedIn profile .The target="_blank" attribute ensures that the link opens in a new browser tab or window.

## Button <a name="button"></a>

```html
        <div class="mask_btns">
            <button class="selected">Home</button>
            <button id="showDialogButton2" @click="mask = false">Video</button>
            <button @click="toWork">Work</button>
        </div>
```
![image](https://github.com/likun945/INFO6150-Assignment2/assets/98712201/ae4bdb98-4898-4791-a26d-b66c00e1423b)

The first button represents the active "Home" tab.
The second button opens a dialog when clicked.
The third button triggers navigation to the "Work" section.
These buttons enhance user interaction and navigation on the page.

## Audio <a name="audio"></a>

```html
    <audio ref="audio" @play="startAnimation" @pause="stopAnimation">
        <source src="/assets/name_audio.m4a" type="audio/mp4">
    </audio>
                ...
                <div @click="toggleAudio" class="animated-element" :class="{ pulsating: isPlaying }">
                     <svg t="1694982031490" class="icon" viewBox="0 0 1024 1024" version="1.1" ... //use icon
                </div>
```
<img width="26" alt="1695000376222" src="https://github.com/likun945/INFO6150/assets/98712201/573e4b4e-ad81-44b5-b5e2-47a7cea7b536">

The <audio> element is used to embed an audio file with the src attribute pointing to the audio source file. The @play and @pause event listeners are used to trigger animation when the audio playback starts and stops, respectively. The accompanying <div> element with the animated-element class contains an SVG icon that users can click to toggle audio playback, and it features a pulsating animation when audio is playing.

## Video <a name="video"></a>

```html
                <video controls width="200px" height="300px" ref="video">
                    <source src="/assets/intro - Compressed with FlexClip.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
```
<img width="890" alt="1695000313148" src="https://github.com/likun945/INFO6150/assets/98712201/c0e2b4b0-9eca-4975-9fa1-940f86882711">

The `<video>` element is used to embed video content. Like audio, it supports the `controls` attribute and multiple `<source>` elements for different video formats.


## Header <a name="header"></a>

```html
            <header class="header">
                <div class="name">
                    <!-- <p>Kun Li</p> -->
                    <img width="32" height="32" src="/assets/android-chrome-192x192.png" />
                </div>
                <div class="tabs">
                    <menu class="menu">
                        <button>Home</button>
                        <button id="showDialogButton">Video</button>
                        <button @click="toWork">Work</button>
                    </menu>
                </div>
                <div class="mobile_tab_btn">
                    <svg t="1694919187348" class="icon" viewBox="0 0 1024 1024" version="1.1"
                        xmlns="http://www.w3.org/2000/svg" @click="clickMask" p-id="6534" width="28" height="28">
                        <path
                            d="M113 224h800c26.5 0 48-21.5 48-48s-21.5-48-48-48H113c-26.5 0-48 21.5-48 48s21.5 48 48 48z m800 240H433c-26.5 0-48 21.5-48 48s21.5 48 48 48h480c26.5 0 48-21.5 48-48s-21.5-48-48-48zM243.7 355.6L78.6 499.9c-6.7 5.8-7.3 15.9-1.5 22.6 0.5 0.5 1 1.1 1.5 1.5l165.1 144c3.3 2.9 8.4 2.6 11.3-0.8 1.3-1.5 2-3.3 2-5.3V361.6c0-4.4-3.6-8-8-8-1.9 0-3.8 0.7-5.3 2zM913 800H113c-26.5 0-48 21.5-48 48s21.5 48 48 48h800c26.5 0 48-21.5 48-48s-21.5-48-48-48z"
                            p-id="6535"></path>
                    </svg>
                </div>
            </header>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/cf048bc6-c471-4940-81b2-0bab0761b03d)

The `<header>` element typically contains content that appears at the top of a webpage, such as navigation links, a site logo, or a page title.

## Footer <a name="footer"></a>

```html
<footer>
  <p>&copy; 2023 Created by KUN LI. All rights reserved.</p>
</footer>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/5e5e7bb5-55d2-4ea8-ac21-1b20814b0b84)

The `<footer>` element usually contains content that appears at the bottom of a webpage, such as copyright information, contact details, or links to related pages.

## Summary <a name="summary"></a>
```html
                            <details>
                                <summary><b>Education</b></summary>
                                <div class="education">
                                    <div class="school">
                                        <img src="/assets/neu.jpg" />
                                    </div>
                                    <div class="school_info">
                                        <div><b>Northeastern University</b></div>
                                        <div>Master of Science - MS, Management Information Systems, General</div>
                                        <div class="date">Jan 2022 - Dec 2023</div>
                                        <div>Grade: 3.34</div>
                                    </div>
                                </div>
                                <div class="education">
                                    <div class="school">
                                        <img src="/assets/zstu.jpg" />
                                    </div>
                                    <div class="school_info">
                                        <div><b>Zhejiang Sci-Tech University</b></div>
                                        <div>Bachelor's degree, Management Information Systems, General</div>
                                        <div class="date">Aug 2016 - Jun 2020</div>
                                        <div>Grade: 3.28</div>
                                    </div>
                                </div>
                            </details>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/cca088a5-6dd9-4bf3-ad86-3592af1787ea)

Each summary serves as a brief overview of the enclosed educational information.

## Menu <a name="menu"></a>
```html
                    <menu class="menu">
                        <button>Home</button>
                        <button id="showDialogButton">Video</button>
                        <button @click="toWork">Work</button>
                    </menu>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/e7fd9d27-c527-4e0d-9221-18b0897633ac)

The menu on the BoardGamer website is created using a `<menu>` element. It contains buttons that trigger specific function when clicked.

## Contact <a name="contact"></a>
To provide contact information on my website, I use the following HTML code:

- Use `<a href="tel:+17819578803" target="_blank">Tel(+1)781-957-8803</a>` for phone numbers. This creates a link that, when clicked on a mobile device, will prompt the user to make a call to the provided phone number.

- Use `<a href="mailto:li.kun1@northeastern.edu" target="_blank">li.kun1@northeastern.edu</a>` for email addresses. This creates a link that, when clicked, opens the user's default email client with the specified email address pre-filled in the "To" field.
![image](https://github.com/likun945/INFO6150/assets/98712201/9f6efa11-9331-403b-b6fd-7b008808cd14)
