# Level Travel Static Website

<p align="center">
  <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
</p>

# 🌍 A Travel Agency Static Website

## 📖 Table of Contents
1. 🤖 [Introduction](#introduction)
2. 🔧 [Tech Stack](#tech-stack)
3. 🛠 [Features](#features)
4. 🚀 [Quick Start](#quick-start)
5. 🕸️ [Snippets (Code to Copy)](#snippets)
6. 🖼 [Assets](#assets)
7. 📌 [More](#more)

<a id="introduction"></a>
## 🤖 Introduction
This travel agency app, named Level, is a static website project crafted to deliver a sleek and modern user experience for exploring and discovering destinations around the world. The user interface is built using **HTML, CSS, and JavaScript**, enhanced with **jQuery** for interactive features such as sliding images via the **Slick Carousel** and date selection using the **Datepicker** plugin. The design is further polished with **Bootstrap**, ensuring a responsive and visually appealing layout. Level is designed to provide users with an intuitive and engaging platform for browsing travel destinations seamlessly.

<a id="tech-stack"></a>
## 🔧 Tech Stack
- **JavaScript**
- **Jquery**
- **Bootstrap CSS (Styling)**

<a id="features"></a>
## 🛠 Features
👉 **Navigation Menu :** Smooth scrolling to different sections (e.g., Search, Services, Recommended Places, Contact).</br></br>
👉 **Search Form :** Form fields are styled with Font Awesome icons for better visual appeal.</br></br>
👉 **Video Section :** Users can play or pause the video using Font Awesome icons.</br></br>
👉 **Responsive Design:** Ensures a seamless user experience across all devices.</br>

and many more, including code architecture and reusability

<a id="quick-start"></a>
## 🚀 Quick Start
Follow these steps to set up the project locally on your machine.

**Prerequisites**

Make sure you have the following installed on your machine:
- **[VS Code](https://code.visualstudio.com/download)**
- **[Git](https://git-scm.com/)**
- **[Modern web browser](#) (Chrome, Firefox, Safari, Edge)**
**Clone the repository**
```bash
git clone https://github.com/your-username/level-travel-website.git
cd level-travel-website
```
**Installation**
For development, you may want to install dependencies locally instead of using CDNs:
```bash
npm install bootstrap jquery jquery-ui slick-carousel font-awesome
```
## 🕸️ CSS Snippets

<details >
<summary style="background-color: gray; border-radius: 6px; padding: 10px; cursor: pointer;">View Full CSS Code</summary>

```css
:root {
    /* COLORS */
    --color-primary: #ee5057;
    --color-secondary: #111;
    --color-text: #898989;
    --color-light: #f4f4f4;

    /* FONTS */
    --font-primary: 'Open Sans', Helvetica, Arial, sans-serif;
    --font-bold: 700;
    --font-light: 400;
    --font-size-text: 13px;
    --font-size-title: 20px;
    --font-size-section-title: 48px;

    /* SIZE */
    --size-primary: 25px;
    --size-half: calc(var(--size-primary) / 2);
    --size-double: calc(var(--size-primary) * 2);
    --margin-primary: var(--size-primary);
    --margin-half: calc(var(--size-primary) / 2);
    --margin-double: calc(var(--size-primary) * 2);
    --padding-primary: var(--size-primary);
    --padding-half: var(--size-half);
    --padding-double: var(--size-double);
    --height-primary: 120px;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 0px;
}

a {
    color: inherit;
    text-decoration: none;
}

/* VIDEO */
.video-container {
    overflow: hidden;
    width: 100%;
    height: 257px;
    position: relative;
}

.video-overlay {
    position: absolute;
    background-color: rgb(0 0 0 / 50%);
    width: 100%;
    height: 257px;
    z-index: 1;
    justify-content: center;
    align-items: center;
    display: flex;
}

.video-control-play , .video-control-pause {
    color: white;
    font-size: var(--font-size-section-title);
    cursor: pointer;
}

.video-control-pause {
    display: none;
}

.video-container video {
    width: 100%;
}

@media (min-width: 768px) {
    .navbar {
        height: var(--height-primary);
    }

    .navbar .navbar-nav .level-nav-link.nav-link {
        padding: var(--padding-double) var(--padding-primary);
    }

    .video-container {
        height: 515px;
    }

    .video-overlay {
        height: 515px;
    }
}

/* NABVAR */
.navbar .navbar-nav .level-nav-link.nav-link {
    padding-right: var(--padding-primary);
    padding-left: var(--padding-primary);
}

.navbar .navbar-nav .level-nav-link.nav-link.active,
.navbar .navbar-nav .level-nav-link.nav-link:hover {
    background-color: var(--color-primary);
    color: white;
}

.navbar-brand {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.navbar-brand h1 {margin: 0px;}

/* HERO */
.hero {
    position: relative;
    background: url('../images/bg-img-1.jpg') no-repeat center center;
    height: 515px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.search-form {
    background-color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    gap: var(--size-half);
    padding: var(--padding-double) var(--padding-primary);
}

.form-group {
    flex: 1 25%;/*flex-grow=1, flex-shrink=1, flex-basis=25%*/
    position: relative;
    display: flex;
    align-items: center;
}

.form-group .form-control {
    padding-left: var(--padding-double);
    border-radius: 0;
}

.form-group i {
    position: absolute;
    font-size: var(--font-size-title);
    color: var(--color-primary);
    left: var(--size-half);
}

.btn-primary {
    background-color: var(--color-primary);
    border-radius: 0;
    border: none;
    width: 100%;
    text-transform: uppercase;
    font-weight: var(--font-bold);
}

.btn-primary:hover {
    background-color: #c3343d;
}

.need-help {
    background-color: white;
    padding: 0 var(--padding-double) var(--padding-half);
    font-size: .8rem;
}

/* SUBSCRIBE */
section {
    padding: var(--padding-double) 0;
    position: relative;
}

.section-color {
    background-color: var(--color-primary);
    color: white;
}

.section-title {font-size: var(--font-size-section-title);}
.section-subtitle {font-size: var(--font-size-title);}

.btn-white {
    border: 2px solid white;
    background-color: inherit;
    color: white;
    padding: var(--padding-half) var(--padding-primary);
}

.btn-white:hover {
    background-color: white;
    color: var(--color-primary);
}

/* SERVICES */
.section-down-arrow {
    position: absolute;
    top: 0;
    width: 100%;
    height: var(--height-primary);
}

.article {
    text-align: center;
    margin-top: var(--size-double);
    transition: all .2s ease-in;
    color: var(--color-primary);
    padding: var(--padding-primary);
}

.article:hover {
    scale: 1.1;
    box-shadow: 0 0 7px 0 var(--color-text);
}

.article-icon {
    font-size: 4rem;
    margin-bottom: var(--margin-primary);
}

.article p {
    font-size: var(--font-size-title);
}

.btn-fit {
    width: max-content;
}

/* SLIDER */
.section-gray {
    background-color: var(--color-light);
}

.level-slider-item {
    background-color: white;
    margin-right: var(--margin-half);
}

.level-slider-item img {
    width: 100%;
}

.level-slider-item-container {
    padding: var(--padding-primary);
}

.level-slider-item-container h3 {
    font-size: var(--font-size-title);
    color: var(--color-primary);
}

.level-slider-item-container p {
    font-size: var(--font-size-text);
    color: var(--color-text);
}

/* STAR PLACES */

.star-places {
    background-color: white;
}

.star-places-header {
    background-color: var(--color-primary);
    color: white;
    padding: var(--padding-half);
}

.star-places-header h3 {
    font-size: var(--font-size-title);
    font-weight: var(--font-light);
}

.star-places-header p {
    font-size: var(--font-size-text);
    font-weight: var(--font-light);
    margin: 0;
}

.star-places-body {
    padding-bottom: var(--padding-half);
}

.star-places-body a{
    background-color: var(--color-light);
    display: flex;
    justify-content: flex-start;
    gap: var(--size-primary);
    margin: var(--size-primary);
    align-items: center;
    color: var(--color-secondary);
    transition: all .2s ease-in;
}

.star-places-body a:hover {
    background-color: hwb(0 69% 22%);
}

.star-places-body h4 {
    font-size: var(--font-size-title);
    text-transform: uppercase;
}

/* CONTACT */
.contact-form {
    margin: auto;
    width: 100%;
}

.contact-form .form-control {
    background-color: var(--color-light);
    border: none;
    margin-bottom: var(--size-half);
}

.contact-form .form-group i {
    top: var(--size-half);
}

.map-container {
    padding-bottom: var(--size-half);
    width: 100%;
    height: 100%;
    cursor: grab;
}

/* FOOTER */
.footer {
    background-color: var(--color-secondary);
}

.footer p {
    padding: var(--padding-half) 0px;
    color: white;
    text-align: center;
    margin-bottom: 0px;
}

.footer a {
    color: var(--color-primary);
}
</details> ```
