# Huddle Landing Page 
Frontend Mentor is a website where front-end developers get a design and are asked to make it into a page to practice their skills. This repository is my approach for the following design: https://www.frontendmentor.io/challenges/huddle-landing-page-with-curved-sections-5ca5ecd01e82137ec91a50f2

If you want to see this repository live you can do it here: https://avoscanemile.github.io/huddle-third-page/

**I do not own this design. If you've any questions related to it you should clarify them in the Frontend Mentor website.** 

## Table of Contents
- [HTML Structure](#html-structure)
- [Layout and CSS Functions](#layout-and-css-functions)
- [Media Queries](#media-queries)
---

## HTML Structure <a name="html-structure"></a>

### Header (`.header`)
- The header contains the logo and a "Try it free" link.
  - `.header__flex`: Flex container for header content.
  - `.header__first-link`: Logo with hover effect.
  - `.header__second-link`: "Try it free" button with hover effect.

### Main (`.main`)
- The main content of the landing page.

#### First Section (`.first-section`)
- The first section includes a heading, text, a CTA button, and statistics.
  - `.first-section__first-flex`: Flex container for the first section.
  - `.first-section__second-flex`: Flex container for text content.
  - `.first-section__h1`: Heading with custom font.
  - `.first-section__txt`: Text content.
  - `.first-section__link`: CTA button with hover effect.
  - `.first-section__third-flex`: Flex container for statistics.
  - `.first-section__container`: Statistic container.
  - `.first-section__h2`: Large statistics numbers.
  - `.first-section__h3`: Statistic descriptions.

#### Second Section (`.second-section`)
- The second section features two content blocks.
  - `.second-section__first-flex`: Flex container for the second section.
  - `.second-section__second-flex`: Flex container for two content blocks.
  - `.second-section__third-flex`: Flex container for individual content blocks.
  - `.second-section__container`: Container for text content.
  - `.second-section__img`: Images with custom styling.
  - `.second-section__fourth-flex`: Flex container for the "Flowing Conversations" content block.
  - `.second-section__first-flex--second-background`: Flex container with background images.
  - `.second-section__5th-flex`: Flex container for the CTA section.
  - `.second-section__6th-flex`: Flex container for the CTA button and text.
  - `.second-section__call`: CTA text with custom styling.
  - `.second-section__link`: CTA button with hover effect.

### Footer (`.footer`)
- The footer section contains contact information, social links, and a newsletter subscription form.
  - `.footer__first-flex`: Flex container for footer content.
  - `.footer__second-flex`: Flex container for footer columns.
  - `.footer__container`: Individual footer column content.
  - `.footer__txt`: Footer text.
  - `.footer__third-flex`: Flex container for contact information.
  - `.footer__links`: Container for social links.
  - `.footer__link`: Individual social links with hover effect.
  - `.footer__social`: Social icons with hover effect.
  - `.footer__form`: Newsletter subscription form.
  - `.footer__email`: Email input field.
  - `.footer__submit`: Submit button with hover effect.

---

## Layout and CSS Functions Used <a name="layout-and-css-functions"></a>

### CSS Layout Tools

- **Flexbox**: Flexbox was used for creating flexible layouts in various sections of the landing page. It is primarily used for arranging content within containers.

  - In the header, `.header__flex` is a Flexbox container that horizontally aligns the logo and "Try it free" link.
  
  - In the first section, `.first-section__first-flex` uses Flexbox to center its child elements vertically and horizontally, creating a well-balanced design.
  - `.first-section__second-flex` applies Flexbox to vertically align its child elements and center text content.
  - In the first section statistics, `.first-section__fourth-flex` uses Flexbox for even distribution of two statistic containers.
  
  - In the second section, Flexbox is extensively used:
    - `.second-section__first-flex` applies Flexbox for positioning background images.
    - `.second-section__second-flex` utilizes Flexbox to center content.
    - `.second-section__third-flex` aligns text content and images side by side.
    - `.second-section__4th-flex` arranges the "Flowing Conversations" content.
    - `.second-section__5th-flex` aligns CTA content.
  
  - In the footer section:
    - `.footer__first-flex` is a Flexbox container for contact information.
    - `.footer__second-flex` arranges footer columns.
    - `.footer__container` within footer columns utilizes Flexbox for alignment.
    - `.footer__links` uses Flexbox for spacing social links.
    - `.footer__form` arranges the newsletter form elements.
  
### CSS Functions Used

- **Custom Properties (Variables)**: Custom properties (CSS variables) are used to define and reuse values for colors, fonts, and sizes throughout the styling of the landing page.

  - Custom properties like `--pink`, `--light-pink`, and `--ff-h` are used to maintain consistent design elements.

- **`clamp()` Function**: The `clamp()` function is employed to ensure that certain elements have responsive sizing based on viewport width.

  - For example, the `--section-width` variable uses `clamp()` to limit the section width to a range of 300px to 1500px, ensuring the content's responsiveness.
  
- **`url()` Function**: The `url()` function is used to specify background images and images in the landing page.

  - It is used for background images in the second section, such as `.second-section__first-flex` and `.second-section__first-flex--second-background`.
  - Images in the HTML, like `<img src="images/...">`, use the `url()` function to reference image files.

## Responsive Design with Media Queries <a name="media-queries"></a>

### Media Queries

Media queries are used in the Huddle landing page project to create a responsive design that adapts to different viewport widths. These queries allow for changes in layout, styling, and content presentation to ensure an optimal user experience on various devices.

### Impact on Layout

- **Max-width: 1200px**:
  - In the second section, `.second-section__third-flex` changes its layout from side by side to a vertical stack by switching to flex-direction: column.
  - `.second-section__container` elements are adjusted to a width of 80% and text alignment to center.
  - Images within `.second-section__img` are resized to 65% of the container's width.

- **Max-width: 800px**:
  - The first section statistics, `.first-section__fourth-flex`, change to a flex-direction of column, making them stack vertically.
  - `.first-section__container` padding is modified for better spacing.
  - In the second section, `.second-section__5th-flex` is adjusted for spacing.
  - `.second-section__call` and `.second-section__link` elements change their width to ensure text fits comfortably.

- **Max-width: 550px**:
  - In the header, `.header__flex` adjusts to a flex-direction of column for mobile devices.
  - `.header__second-link` text alignment is centered.
  - In the footer, `.footer__second-flex` changes to a flex-direction of column.
  - `.footer__container` elements adjust their width.
  - `.footer__container:nth-of-type(2)` receives additional margin for proper spacing.
  - `.footer__form` and its child elements adapt to a flex-direction of column.

**Please refer to the provided HTML/CSS code for detailed structure/styling information.**
