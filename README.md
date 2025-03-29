# Web Accessibility Project

## Project Description
**What was done:** 
As part of the Web Accessibility course at Tampere University, the assignment was to create an accessible website (five documents in HTML format) that includes titles, paragraphs, images, and links (e.g., navigation between documents). The content and topic could be anything.

**Why:** 
The purpose of the project was to enhance my understanding of accessibility and learn practical ways to make websites more user-friendly, particularly for those using screen readers and keyboard navigation.

**How:** 
I used WCAG 2.1 guidelines and best practices, such as landmarks and semantic elements, to ensure the website's accessibility.

**My Role:** 
I completed the project independently, handling all design and implementation stages.

## Explanation of Choices
In designing the website, I focused on ensuring accessibility for users who rely on screen readers and keyboard navigation. I implemented landmarks, semantic elements, and other best practices mentioned in WCAG 2.1. Although I did not address all possible accessibility needs, such as voice recognition software and eye-tracking technology, I believe the improvements made for screen reader and keyboard users will also benefit those using other assistive technologies.

## Accessibility Features
**Language Attribute:**
All the documents include a lang attribute, which specifies the language of the document. This is crucial for screen readers to pronounce the text correctly.

**Clear Language:**
The texts are copied from visittampere.fi/en/ and tampere.fi/en pages. This may lead to accessibility issues, as I didn’t verify if the texts are in clear language. In an understandable text, sentences should be as short as possible. Additionally, abbreviations, slang words, and jargon should be avoided. These kinds of issues may arise in the documents.

**Responsive Design:**
I have implemented media queries to ensure that the website adapts seamlessly to various screen sizes, from mobile devices to large desktop monitors. Using Flexbox layouts, I ensured that the content remains accessible and user-friendly regardless of the device being used. This approach aligns with accessibility standards by making the website usable for people with different devices and screen resolutions.

**Headings and Structure:**
Headings are used correctly to create a logical document structure, making it easier for screen reader users to navigate and understand the relationship between different sections.

**Landmarks and Semantic Elements:**
Landmarks and semantic elements are used to enhance the user experience for those who use screen readers. They make the document’s structure logical, understandable, and easier to navigate. Semantic elements, such as /<article/>, /<nav/>, and /<footer/>, provide meaningful context to the content, unlike generic /<div/> tags, which don’t convey any specific meaning. Unlike semantic elements, /<div/> tags lack built-in accessibility features, making it harder for assistive technologies to interpret the content.

**Colour Contrast:**
The colour contrast is at least 4.5:1, which is the required ratio for accessibility. Sufficient colour contrast makes the content accessible for people with low vision and other vision impairments.

**Links:**
Links are descriptive, understandable, and available for assistive technologies. They clearly explain what information the reader will get by clicking onthem. Even though aria-label attributes are not needed in this case, I used them and aria-current attributes to highlight the current page in the navigation bar. They ensure that users using screen readers know on which page they are.

**Link States:**
I have used “Hover”, “Focus”, and “Visited” states for the links. “Hover” helps sighted people and “Focus” helps people using the keyboard for navigation to notice which link they are about to activate. A visited state may help people with short-term memory loss to remember which content has already been read.

**Underlined hyperlinks:**
To ensure users notice which text snippets are links, I kept the underline in them. I just edited the CSS properties of text-underline-offset and text-decoration-color.

**Visual Focus and Hover:**
The Focus and Hover states help people notice interactive components. The Focus state is seen when using a keyboard for navigation and the Hover state when operating with a mouse. I modified the default focus state by increasing the offset, making it more readable. Additionally, I ensured sufficient colour contrast between the Hover and Normal states.

**Link Text:**
Good link text makes sense without context. It should explain clearly what information the reader will get by clicking on the link. In the navigation menu, I used short descriptive link names, and for text links, I kept them as short as possible but still descriptive.

**Skip Links:**
To make navigation easier and faster for people using a keyboard, screen readers, switch controls, or other assistive technologies, I added a skip links feature.

**Images:**
All images on the website have descriptive alt attributes. Alt attributes should explain the content of an image as clearly as possible, keeping in mind that people using screen readers cannot see the image. However, they still need to be short but descriptive. Meaningless images should be defined as background or decorative images using an empty alt attribute (alt=""). If an image lacks an alt attribute, screen readers may read the file name, which can be confusing.

**Zooming:**
I used em units for defining text sizes to ensure that the website content is zoomable.  Unlike font sizes in pixels, em and rem units are scalable, allowing the text to resize proportionally based on the user’s settings.
