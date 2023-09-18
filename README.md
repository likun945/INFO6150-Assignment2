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
15. [Mobile Adaptation](#mobile)

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
<link rel="icon" href="/assets/favicon.png" sizes="32x32" type="image/x-icon">
```
![image](https://github.com/likun945/INFO6150/assets/98712201/24fe26fa-b87f-42d4-aac3-bca4c90ba8b7)


This favicon represents the abbreviation "BG" for BoardGamer.

## Table <a name="table"></a>

```html
<table>
    <!-- Table content -->
</table>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/115d520e-41ba-4b81-b76f-654db6873d95)

Tables are used to organize and display tabular data. The table represents board game information.

## Form <a name="form"></a>

```html
               <form action="submit_registration.php" method="POST">
                    ...
                    <h2>Event Registration</h2>
                    <label for="date">Event Date:</label>
                    <input type="date" id="date" name="date" required><br><br>
                    <label for="comments">Comments:</label><br>
                    <textarea id="comments" name="comments" rows="4" cols="50"></textarea><br><br>
                    <input type="submit" value="Register">
                </form>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/2b40361b-c404-4e86-9723-77743b63fc3c)

A form for event registration. Users can input their event date and other information.

## Images <a name="images"></a>

```html
<img src="/assets/ticket.jpg" alt="Image Description">
```
![image](https://github.com/likun945/INFO6150/assets/98712201/86961355-6dac-424c-a594-f53c276bce28)

Images are embedded using the `<img>` element. The `src` attribute specifies the image file's path, and the `alt` attribute provides alternative text for accessibility.

## Hyperlink <a name="hyperlink"></a>

```html
<a href="https://boardgamegeek.com/boardgame/822" target="_blank">View on BGG</a>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/06e38e23-781c-4368-981c-b04ef897894d)

Hyperlinks are created with the `<a>` element. They link to other web pages or resources, and the `href` attribute defines the destination URL.

## Button <a name="button"></a>

```html
<button type="button" class="green" @click="tab = 0">BoardGame List</button>
```
<img width="234" alt="1694321162503" src="https://github.com/likun945/INFO6150/assets/98712201/6e407563-a7e1-455e-8b68-0ac4844e5926">

Buttons are created using the `<button>` element. They can trigger actions when clicked, we could switch the tab card by clicking the button.

## Audio <a name="audio"></a>

```html
<audio id="audio" controls>
   <source src="/assets/dancin.flac" type="audio/mpeg">
   Your browser does not support the audio element.
 </audio>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/3909b2c6-518d-4a5f-acc3-97759f49f3cf)

The `<audio>` element is used to embed audio content. The `controls` attribute adds audio controls (play, pause, volume) to the player.

## Video <a name="video"></a>

```html
<video controls>
  <source src="/assets/Ticket to Ride - How To Play.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/cceb8430-dcdf-488e-8537-a7481ad2e5b9)

The `<video>` element is used to embed video content. Like audio, it supports the `controls` attribute and multiple `<source>` elements for different video formats.


## Header <a name="header"></a>

```html
<header>
  <h1>Board Games</h1>
</header>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/ef9b9dba-ee24-449c-8cf2-4e0491825058)

The `<header>` element typically contains content that appears at the top of a webpage, such as navigation links, a site logo, or a page title.

## Footer <a name="footer"></a>

```html
<footer>
  <p>&copy; 2023 Created by KUN LI. All rights reserved.</p>
</footer>
```
<img width="922" alt="1694321213082" src="https://github.com/likun945/INFO6150/assets/98712201/f4fccb1c-505e-4a6f-b3fd-df6ddf021b8c">

The `<footer>` element usually contains content that appears at the bottom of a webpage, such as copyright information, contact details, or links to related pages.

## Summary <a name="summary"></a>
                      <details>
                        <summary>Contact Information</summary>
                        <div>
                            <p><strong>Name:</strong> Kun Li</p>
                            <p><strong>Email:</strong> <a href="mailto:kunli@example.com">kunli@example.com</a></p>
                            <p><strong>Phone:</strong> <a href="tel:+1234567890">+1 (234) 567-890</a></p>
                            <p><strong>Address:</strong> 123 Main Street, City, Country</p>
                            <p>
                                <strong>Introduction:</strong> Hello, I'm Kun Li, a board game enthusiast and event
                                organizer. I enjoy bringing people together to play and have fun with board games. Feel
                                free to reach out to me for any inquiries or event registrations!
                            </p>
                        </div>
                    </details>
![image](https://github.com/likun945/INFO6150/assets/98712201/6fd06bf5-2039-4b5d-9528-2a2bad2c8e04)

The summary of each section provides a brief information.

## Menu <a name="menu"></a>
```html
<menu id="frozen-btn">
   <button type="button" class="green" @click="tab = 0">BoardGame List</button>
   <button type="button" class="purple" @click="tab = 1">Event registration</button>
</menu>
```
![image](https://github.com/likun945/INFO6150/assets/98712201/f9938707-6252-4483-89f3-83660dbdf568)

The menu on the BoardGamer website is created using a `<menu>` element. It contains buttons that trigger tab switching when clicked.

## Contact <a name="contact"></a>
To provide contact information on my website, I use the following HTML code:

- Use `<a href="mailto:kunli@example.com">kunli@example.com</a>` for phone numbers. This creates a link that, when clicked on a mobile device, will prompt the user to make a call to the provided phone number.

- Use `<a href="tel:+1234567890">+1 (234) 567-890</a>` for email addresses. This creates a link that, when clicked, opens the user's default email client with the specified email address pre-filled in the "To" field.

![image](https://github.com/likun945/INFO6150/assets/98712201/d9bd8681-2662-4bb9-9568-4f0e1d753479)

## Mobile Adaption <a name="mobile"></a>
Ensuring my website looks and functions seamlessly on mobile devices is crucial for providing a user-friendly experience. I have optimized the website layout and elements to automatically adjust to different screen sizes and orientations.
![image](https://github.com/likun945/INFO6150/assets/98712201/f0186e54-cff5-4a97-8722-08f4bf431525)
![image](https://github.com/likun945/INFO6150/assets/98712201/73650bca-6c7e-4c31-833e-7d37df57ca70)
![image](https://github.com/likun945/INFO6150/assets/98712201/80385f4a-9525-458a-82cd-9a4be5f59465)


