# Testing

> [!NOTE]  
> Return back to the [README.md](README.md) file.

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-START OF NOTES (to be deleted)

In this section, you need to convince the assessors that you have conducted enough testing to legitimately believe that the site works well.
Essentially, in this part, you should go over all of your project's features, and ensure that they all work as intended,
with the project providing an easy and straightforward way for the users to achieve their goals.

Feature-by-Feature Testing:

Go through each feature of your portfolio site and detail the testing process for each.

Explain the functionality and demonstrate how it aligns with the intended purpose. This could include:

- Navigation: Ensuring smooth transitions between pages, links directing to the correct destinations.
- Responsive Design: Checking for compatibility across various devices and screen sizes.
- Portfolio Display: Verifying that projects are properly showcased with accurate descriptions, images, and links.
- Contact Form: Testing the form submission process, ensuring the user receives a confirmation, and you receive the message.

User Experience Testing:

- Usability Testing: Have users (or simulated users) interact with the site and provide feedback. Document any issues encountered and the resolutions implemented.
- Accessibility Testing: Confirm compliance with accessibility standards (e.g., screen reader compatibility, proper alt text for images, keyboard navigation).

Compatibility Testing:

- Browser Compatibility: Testing on different browsers (Chrome, Firefox, Safari, Edge, etc.) to ensure consistent performance.
- Device Compatibility: Ensuring functionality across various devices (desktops, laptops, tablets, and mobile phones).

Regression Testing:

After implementing fixes or updates, ensure that previous features and functionalities still work as intended. This prevents new changes from breaking existing features.

Documentation and Logs:

Maintain records of testing procedures, results, and any bugs encountered along with their resolutions. This helps demonstrate a systematic approach to testing and problem-solving.
User Feedback Incorporation:

If applicable, mention how user feedback has been taken into account and implemented to enhance the user experience.

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-END OF NOTES (to be deleted)


As I ran throught the HTML validator I am suprised to see that I was not following many of the standards, but I will forgive myself. I am not yet an expert but after all: never quitting and always improving makes an expert. 

As you can see from this screenshot here:

![screenshot](documentation/validation/index_live.png) 

The first point was that the a element must not be nested inside a button element. Luckily, I did have to through away all of my code (jokes), instead, I removed the button element and styled the individual a elements to look like buttons instead. It worked well without losing much style but at the same time improving semantics and accessibility. 
I tested that the buttons on both pages work as intended. 

The second point was that the the list structure was incorrect. Suprsingly, it works, but the HTML Standard was not being followed in this regards. But to fix the list-structure issue, all I had to was to wrap ul inside li item instead of ul being a child of ol. Now its a child of li, which is the correct way, the funtionality and the looks of the index section seem not to have changed. 

The third point was that a p element was inside a table element. That is not correct as it cannot be a start-tag of table. So I moved it outside of table, above it. The changes cannot be seen or are very hard to notice and demonstrate, because it the browser (firefox) that I am using is pushing the p element outside of the table element in any case, whatsoever. 

For my second round of validating: 

![screenshot](documentation/validation/index_live_2nd.png) 

The most obvious point, that textarea should not include a type attribute... that makes sense is cool to know, that textarea expects a type of text per default. 

For the second point, I have to add headline (h) elements to improve for accessibility. I added those those, which the validator expected to see for accessibility purposed and you may see them in the comparisson table further down. 

After this he was satisfied with my code: 

![screenshot](documentation/validation/HTML/validation_complete.png)


I have been doing adjusting to the Swahili version alongside the corrections of the index.html every time, but now for the acutal validation, as well: 

![screenshot](documentation/validation/HTML/validating_swahili.png)

Apart from a p element that had gone lost, I also have to change the attribute in the html element responsible for the language, this is for the browser to know which language the document is written in. The correct setting needs to be lang="sw" for swahili, as the validator points out. 

This was all very helpful and increased my knowledge in HTML. 
And successful:
![screenshot](documentation/validation/HTML/validation_swahili_complete.png)

Here you may compare the visual results: 

| Issue | Before | After | Notes |
| --- | --- | --- | --- |
| Nested a inside button element | ![screenshot](documentation/validation/before_after/before_button.png) | ![screenshot](documentation/validation/before_after/after_button.png) | Improved semantics and accessibility|
| Missing headline | ![screenshot](documentation/validation/before_after/article_before.png) | ![screenshot](documentation/validation/before_after/article_after.png) | Improved Accessibility |
| Missing headline | ![screenshot](documentation/validation/before_after/copyright_before.png) | ![screenshot](documentation/validation/before_after/copyright_after.png) | Improved Accessibility |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |




## Code Validation

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-START OF NOTES (to be deleted)

Use the space to discuss code validation for any of your own code files (where applicable).
You are not required to validate external libraries/frameworks, such as imported Bootstrap, Materialize, Font Awesome, etc.

**IMPORTANT**: You must provide a screenshot for each file you validate.

**PRO TIP**: Always validate the live site pages, not your local code. There could be subtle/hidden differences.

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-END OF NOTES (to be deleted)

### HTML

I have used the recommended [HTML W3C Validator](https://validator.w3.org) to validate all of my HTML files.

| Directory | File | Screenshot | Notes |
| --- | --- | --- | --- |
|  | index.html | ![screenshot](documentation/validation/path-to-screenshot.png) | |
|  | swahili.html | ![screenshot](documentation/validation/path-to-screenshot.png) | |

### CSS

I have used the recommended [CSS Jigsaw Validator](https://jigsaw.w3.org/css-validator) to validate all of my CSS files.

| Directory | File | Screenshot | Notes |
| --- | --- | --- | --- |
| assets | styles.css | ![screenshot](documentation/validation/path-to-screenshot.png) | |

## Browser Compatibility

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-START OF NOTES (to be deleted)

Use this space to discuss testing the live/deployed site on various browsers.

Consider testing AT LEAST 3 different browsers, if available on your system.

You DO NOT need to use all of the browsers below, just pick any 3 (minimum).

Recommended browsers to consider:
- [Chrome](https://www.google.com/chrome)
- [Firefox (Developer Edition)](https://www.mozilla.org/firefox/developer)
- [Brave](https://brave.com/download)

**IMPORTANT**: You must provide screenshots of the tested browsers, to "prove" that you've actually tested them.

Please note, there are services out there that can test multiple browser compatibilities at the same time.
Some of these are paid services, but some are free.
If you use these, you must provide a link to the source used for attribution, and multiple screenshots of the results.

Sample browser testing documentation:

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-END OF NOTES (to be deleted)

I've tested my deployed project on multiple browsers to check for compatibility issues.

| Browser | Home | About | Contact | etc | Notes |
| --- | --- | --- | --- | --- | --- |
| Chrome | ![screenshot](documentation/browsers/browser-chrome-home.png) | ![screenshot](documentation/browsers/browser-chrome-about.png) | ![screenshot](documentation/browsers/browser-chrome-contact.png) | ![screenshot](documentation/browsers/browser-chrome-etc.png) | Works as expected |
| Firefox | ![screenshot](documentation/browsers/browser-firefox-home.png) | ![screenshot](documentation/browsers/browser-firefox-about.png) | ![screenshot](documentation/browsers/browser-firefox-contact.png) | ![screenshot](documentation/browsers/browser-firefox-etc.png) | Works as expected |
| Edge | ![screenshot](documentation/browsers/browser-edge-home.png) | ![screenshot](documentation/browsers/browser-edge-about.png) | ![screenshot](documentation/browsers/browser-chrome-edge.png) | ![screenshot](documentation/browsers/browser-edge-etc.png) | Works as expected |
| Safari | ![screenshot](documentation/browsers/browser-safari-home.png) | ![screenshot](documentation/browsers/browser-safari-about.png) | ![screenshot](documentation/browsers/browser-safari-contact.png) | ![screenshot](documentation/browsers/browser-safari-etc.png) | Minor CSS differences |
| Brave | ![screenshot](documentation/browsers/browser-brave-home.png) | ![screenshot](documentation/browsers/browser-brave-about.png) | ![screenshot](documentation/browsers/browser-brave-contact.png) | ![screenshot](documentation/browsers/browser-brave-etc.png) | Works as expected |
| Opera | ![screenshot](documentation/browsers/browser-opera-home.png) | ![screenshot](documentation/browsers/browser-opera-about.png) | ![screenshot](documentation/browsers/browser-opera-contact.png) | ![screenshot](documentation/browsers/browser-opera-etc.png) | Minor differences |
| repeat for any other tested browsers | x | x | x | x | x |

## Responsiveness

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-START OF NOTES (to be deleted)

Use this space to discuss testing the live/deployed site on various device sizes.

The minimum requirement is for the following 3 tests:
- Mobile
- Tablet
- Desktop

**IMPORTANT**: You must provide screenshots of the tested responsiveness, to "prove" that you've actually tested them.

Using the "amiresponsive" mockup image (or similar) does not suffice the requirements.
Consider using some of the built-in device sizes in the Developer Tools.

If you have tested the project on your actual mobile phone or tablet, consider also including screenshots of these as well.
It showcases a higher level of manual tests, and can be seen as a positive inclusion!

Sample responsiveness testing documentation:

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-END OF NOTES (to be deleted)

I've tested my deployed project on multiple devices to check for responsiveness issues.

| Device | Home | About | Contact | etc | Notes |
| --- | --- | --- | --- | --- | --- |
| Mobile (DevTools) | ![screenshot](documentation/responsiveness/responsive-mobile-home.png) | ![screenshot](documentation/responsiveness/responsive-mobile-about.png) | ![screenshot](documentation/responsiveness/responsive-mobile-contact.png) | ![screenshot](documentation/responsiveness/responsive-mobile-etc.png) | Works as expected |
| Tablet (DevTools) | ![screenshot](documentation/responsiveness/responsive-tablet-home.png) | ![screenshot](documentation/responsiveness/responsive-tablet-about.png) | ![screenshot](documentation/responsiveness/responsive-tablet-contact.png) | ![screenshot](documentation/responsiveness/responsive-tablet-etc.png) | Works as expected |
| Desktop | ![screenshot](documentation/responsiveness/responsive-desktop-home.png) | ![screenshot](documentation/responsiveness/responsive-desktop-about.png) | ![screenshot](documentation/responsiveness/responsive-desktop-contact.png) | ![screenshot](documentation/responsiveness/responsive-desktop-etc.png) | Works as expected |
| XL Monitor | ![screenshot](documentation/responsiveness/responsive-xl-home.png) | ![screenshot](documentation/responsiveness/responsive-xl-about.png) | ![screenshot](documentation/responsiveness/responsive-xl-contact.png) | ![screenshot](documentation/responsiveness/responsive-xl-etc.png) | Scaling starts to have minor issues |
| 4K Monitor | ![screenshot](documentation/responsiveness/responsive-4k-home.png) | ![screenshot](documentation/responsiveness/responsive-4k-about.png) | ![screenshot](documentation/responsiveness/responsive-4k-contact.png) | ![screenshot](documentation/responsiveness/responsive-4k-etc.png) | Noticeable scaling issues |
| Google Pixel 7 Pro | ![screenshot](documentation/responsiveness/responsive-pixel-home.png) | ![screenshot](documentation/responsiveness/responsive-pixel-about.png) | ![screenshot](documentation/responsiveness/responsive-pixel-contact.png) | ![screenshot](documentation/responsiveness/responsive-pixel-etc.png) | Works as expected |
| iPhone 14 | ![screenshot](documentation/responsiveness/responsive-iphone-home.png) | ![screenshot](documentation/responsiveness/responsive-iphone-about.png) | ![screenshot](documentation/responsiveness/responsive-iphone-contact.png) | ![screenshot](documentation/responsiveness/responsive-iphone-etc.png) | Works as expected |
| repeat for any other tested browsers | x | x | x | x | x |

## Lighthouse Audit

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-START OF NOTES (to be deleted)

Use this space to discuss testing the live/deployed site's Lighthouse Audit reports.
Avoid testing the local version (especially if developing in Gitpod), as this can have knock-on effects of performance.

If you don't have Lighthouse in your Developer Tools,
it can be added as an [extension](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk).

Don't just test the home page (unless it's a single-page application).
Make sure to test the Lighthouse Audit results for all of your pages.

**IMPORTANT**: You must provide screenshots of the results, to "prove" that you've actually tested them.

Sample Lighthouse testing documentation:

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-END OF NOTES (to be deleted)

I've tested my deployed project using the Lighthouse Audit tool to check for any major issues.

| Page | Mobile | Desktop | Notes |
| --- | --- | --- | --- |
| Home | ![screenshot](documentation/lighthouse/lighthouse-home-mobile.png) | ![screenshot](documentation/lighthouse/lighthouse-home-desktop.png) | Some minor warnings |
| About | ![screenshot](documentation/lighthouse/lighthouse-about-mobile.png) | ![screenshot](documentation/lighthouse/lighthouse-about-desktop.png) | Some minor warnings |
| Gallery | ![screenshot](documentation/lighthouse/lighthouse-gallery-mobile.png) | ![screenshot](documentation/lighthouse/lighthouse-gallery-desktop.png) | Slow response time due to large images |
| x | x | x | repeat for any other tested pages/sizes |

## User Story Testing

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-START OF NOTES (to be deleted)

Testing user stories is actually quite simple, once you've already got the stories defined on your README.

Most of your project's **features** should already align with the **user stories**,
so this should as simple as creating a table with the user story, matching with the re-used screenshot
from the respective feature.

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-END OF NOTES (to be deleted)

| User Story | Screenshot |
| --- | --- |
| As a new site user, I would like to ____________, so that I can ____________. | ![screenshot](documentation/features/feature01.png) |
| As a new site user, I would like to ____________, so that I can ____________. | ![screenshot](documentation/features/feature02.png) |
| As a new site user, I would like to ____________, so that I can ____________. | ![screenshot](documentation/features/feature03.png) |
| As a returning site user, I would like to ____________, so that I can ____________. | ![screenshot](documentation/features/feature04.png) |
| As a returning site user, I would like to ____________, so that I can ____________. | ![screenshot](documentation/features/feature05.png) |
| As a returning site user, I would like to ____________, so that I can ____________. | ![screenshot](documentation/features/feature06.png) |
| As a site administrator, I should be able to ____________, so that I can ____________. | ![screenshot](documentation/features/feature07.png) |
| As a site administrator, I should be able to ____________, so that I can ____________. | ![screenshot](documentation/features/feature08.png) |
| As a site administrator, I should be able to ____________, so that I can ____________. | ![screenshot](documentation/features/feature09.png) |
| repeat for all remaining user stories | x |

## Bugs

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-START OF NOTES (to be deleted)

This section is primarily used for JavaScript and Python applications,
but feel free to use this section to document any HTML/CSS bugs you might run into.

It's very important to document any bugs you've discovered while developing the project.
Make sure to include any necessary steps you've implemented to fix the bug(s) as well.

**PRO TIP**: screenshots of bugs are extremely helpful, and go a long way!

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-END OF NOTES (to be deleted)

- JS Uncaught ReferenceError: `foobar` is undefined/not defined

    ![screenshot](documentation/bugs/bug01.png)

    - To fix this, I _____________________.

- JS `'let'` or `'const'` or `'template literal syntax'` or `'arrow function syntax (=>)'` is available in ES6 (use `'esversion: 11'`) or Mozilla JS extensions (use moz).

    ![screenshot](documentation/bugs/bug02.png)

    - To fix this, I _____________________.

- Python `'ModuleNotFoundError'` when trying to import module from imported package

    ![screenshot](documentation/bugs/bug03.png)

    - To fix this, I _____________________.

- Django `TemplateDoesNotExist` at /appname/path appname/template_name.html

    ![screenshot](documentation/bugs/bug04.png)

    - To fix this, I _____________________.

- Python `E501 line too long` (93 > 79 characters)

    ![screenshot](documentation/bugs/bug04.png)

    - To fix this, I _____________________.

## Unfixed Bugs

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-START OF NOTES (to be deleted)

You will need to mention unfixed bugs and why they were not fixed.
This section should include shortcomings of the frameworks or technologies used.
Although time can be a big variable to consider, paucity of time and difficulty understanding
implementation is not a valid reason to leave bugs unfixed.

If you've identified any unfixed bugs, no matter how small, be sure to list them here.
It's better to be honest and list them, because if it's not documented and an assessor finds the issue,
they need to know whether or not you're aware of them as well, and why you've not corrected/fixed them.

Some examples:

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-END OF NOTES (to be deleted)

- On devices smaller than 375px, the page starts to have `overflow-x` scrolling.

    ![screenshot](documentation/bugs/unfixed-bug01.png)

    - Attempted fix: I tried to add additional media queries to handle this, but things started becoming too small to read.

- For PP3, when using a helper `clear()` function, any text above the height of the terminal does not clear, and remains when you scroll up.

    ![screenshot](documentation/bugs/unfixed-bug02.png)

    - Attempted fix: I tried to adjust the terminal size, but it only resizes the actual terminal, not the allowable area for text.

- When validating HTML with a semantic `section` element, the validator warns about lacking a header `h2-h6`. This is acceptable.

    ![screenshot](documentation/bugs/unfixed-bug03.png)

    - Attempted fix: this is a known warning and acceptable, and my section doesn't require a header since it's dynamically added via JS.

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-START OF NOTES (to be deleted)

If you legitimately cannot find any unfixed bugs or warnings, then use the following sentence:

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑-END OF NOTES (to be deleted)

> [!NOTE]  
> There are no remaining bugs that I am aware of.
