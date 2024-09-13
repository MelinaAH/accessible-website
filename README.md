Web Accessibility

As part of the Web Accessibility 1 course at Tampere University, the assignment 
was to “Create an accessible website (five documents in HTML format) that 
includes titles, paragraphs, images, and links (e.g., navigation between documents). 
The content and topic can be anything.” My prior knowledge of accessibility was 
primarily theoretical, and I had little experience in creating accessible 
websites. Through this project, I have learned a great deal, enhancing my 
understanding of the importance of landmarks and semantic elements, and how to 
make websites more accessible and user-friendly for those using screen readers 
and keyboards for navigation.

Explanation of Choices

In designing the website, I focused on ensuring accessibility for users who rely 
on screen readers and keyboard navigation. I believe the site is accessible to 
these users, as I have implemented landmarks, semantic elements, and other best 
practices mentioned in WCAG 2.1. However, I recognize that other users have 
different needs, such as those who use voice recognition software, 
eye-tracking technology, or switch devices to interact with their computers or 
mobile devices. These aspects were not explicitly addressed in my project. 
Nevertheless, I’m confident that the accessibility improvements made for screen 
reader and keyboard users will also benefit those using other assistive 
technologies. Ensuring a solid foundation of accessibility can often enhance 
usability across various devices and methods of interaction.

Accessibility Features

Language Attribute: All the documents include a lang attribute, which specifies 
the language of the document. This is crucial for screen readers to pronounce 
the text correctly.

Clear Language: The texts are copied from visittampere.fi/en/ and tampere.fi/en 
pages. This may lead to accessibility issues, as I didn’t verify if the texts 
are in clear language. To make text easy to understand, sentences should be as 
short as possible. Additionally, abbreviations, slang words, and jargon should 
be avoided. These kinds of issues may arise in the documents.

Responsive Design: I have implemented media queries to ensure that the website 
adapts seamlessly to various screen sizes, from mobile devices to large desktop 
monitors. By using Flexbox layouts, I have ensured that the content remains 
accessible and user-friendly regardless of the device being used. This approach 
aligns with accessibility standards by making the website usable for people with 
different devices and screen resolutions.

Headings and Structure: Headings are used correctly to create a logical document 
structure. This makes it easier for screen reader users to navigate and 
understand the relationship between different sections. Proper use of headings 
ensures that the content is organised hierarchically, which is crucial for 
accessibility.

Landmarks and Semantic Elements: Landmarks and semantic elements are used to 
enhance the user experience for those who use screen readers. They make the 
document’s structure logical, understandable, and easier to navigate. Semantic 
elements, such as article, nav, and footer, provide meaningful context to 
the content, unlike generic <div> tags, which don’t convey any specific meaning. 
Unlike semantic elements, <div> tags lack built-in accessibility features, 
making it harder for assistive technologies to interpret the content.

Colour Contrast: The colour contrast is at least 4.5:1, which is the required 
ratio for accessibility. Sufficient colour contrast makes the content accessible 
for people with low vision and other vision impairments, except total blindness.

Links: A link should clearly explain what information the reader will get by 
clicking on it. Based on that knowledge, the links are descriptive, 
understandable, and available for assistive technologies. For this reason, 
aria-label attributes are not needed here. However, I have added aria-label and 
aria-current attributes to the navigation bar. Aria-current attributes are used 
to highlight the current page. They ensure that users using screen readers know 
on which page they are.

Link States: I have used “Hover”, “Focus”, and “Visited” states for the links. 
“Hover” helps sighted people and “Focus” helps people using the keyboard for 
navigation to notice which link they are about to activate. A visited state may 
help people with short-term memory loss to remember which content has already 
been read. However, this feature benefits only sighted people.

Underlined hyperlinks: For users to notice which text snippets are links, I kept 
the underline in them. I just edited the CSS properties of text-underline-offset 
and text-decoration-color.

Visual Focus and Hover: The Focus and Hover states help people notice 
interactive components. The Focus state is seen when using a keyboard for 
navigation and the Hover state when operating with a mouse. I modified the 
default focus state a bit by increasing the offset of the focused state of the 
link, making it more readable. Additionally, I modified the colour of the Hover 
feature to ensure sufficient colour contrast. I also ensured that the contrast 
between the Hover and Normal state is sufficient.

Link Text: Good link text makes sense without context. It should explain clearly 
what information the reader will get by clicking on the link. On the navigation 
menu, I used short descriptive link names, and for text links, I tried to keep 
them as short as possible but still descriptive.

Skip Links: To make navigation easier and faster for people using a keyboard, 
screen readers, switch controls, or other assistive technologies, I added a skip 
links feature.

Images: All images on the website have descriptive alt attributes. Alt 
attributes should explain the content of an image as clearly as possible, 
keeping in mind that people using screen readers cannot see the image. However, 
they still need to be short but descriptive. Meaningless images should be 
defined as background or decorative images using an empty alt attribute 
(alt=""). If an image lacks an alt attribute, screen readers may read the file 
name, which can be confusing.

Zooming: The ability to zoom webpages is crucial for people with low vision. 
Webpages need to be zoomable for the entire content or only for text. I have 
taken this into account by using em units for defining text sizes. Unlike font 
sizes in pixels, em and rem units are scalable, allowing the text to resize 
proportionally based on the user’s settings.
