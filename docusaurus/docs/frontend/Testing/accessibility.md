# Accessibility
> This page was last reviewed at 6h of March 2024. It needs to be reviewed again on the 6th of December 2024. 
## Why a standard for accessibility?
In accordance with the Digital Government Act, the municipality of Amsterdam is required to build all its websites and applications in compliance with the Web Content Accessibility Guidelines (WCAG) at levels A and AA.
## When and for whom is this standard applicable?
This standard applies to front-end developers. The law is applicable to all government websites and applications, including intranets, extranets, and cloud applications. Additionally, it includes mobile applications, encompassing native, web, and hybrid apps for mobile devices.

## How to comply with the WCAG? 
The WCAG can be broken down into four key principles. If the website or application aligns with these principles, it meets the WCAG requirements. The four principles are:

1. **Perceivable:** Ensure that everything on the website or app is easily noticeable by everyone.
2. **Operable:** Make sure that everything on the website or app is accessible to everyone, including those who don't use a mouse or keyboard.
3. **Understandable:** Ensure that everything on the website or app, including error handling, is comprehensible for both software and users.
4. **Robust:** Guarantee that the website or app can be utilized across various devices and assistive technologies.

W3.org has offered [a concise guide](https://www.w3.org/WAI/WCAG22/quickref/?versions=2.0) detailing actions you can take to align with the four principles. Below are brief suggestions for each principle:

**Perceivable**
- Offer alternatives for time-based media, such as ensuring all videos have captions, providing necessary audio descriptions, and transcribing audio-only files.
- Supply text alternatives for non-text content to facilitate conversion into various formats, such as large print, braille, speech, symbols, or simpler language.
- Develop content that can be presented in diverse ways without compromising information or structure; for instance, provide guidance on the proper reading sequence of content.    
- Enhance accessibility for users by improving visibility and audibility of content, including distinguishing foreground from background; for example, allowing text to be resized up to 200%.

**Operable**
- Ensure that all functionality is accessible via a keyboard. 
- Allow users sufficient time to read and interact with content; for instance, enable users to postpone interruptions.
- Avoid designing content in a manner known to induce seizures or physical reactions, limiting flashing to no more than twice per second.
- Implement navigation aids to assist users in finding content and determining their location; for example, maintain a visible focus.
- Enhance usability by enabling users to operate functionality through diverse inputs beyond the keyboard.

**Understandable**
- Ensure that text content is both readable and easily understandable. 
- Design web pages to appear and function in consistent and predictable ways; for instance, employ the same navigation tools throughout the entire website or application. 
- Assist users in avoiding and rectifying mistakes, such as utilizing error suggestions.


**Robust**
- Maximize compatibility with present and future user agents, encompassing assistive technologies. Ensure, for instance, that all IDs are unique.

## How to test for accessibility
### in general?
- Manually test your application to ensure proper rendering by adjusting the text size to the maximum, zooming in at 200%, and verifying that all links feature descriptive link text.
- Evaluate your application by conducting tests without the use of a keyboard and/or mouse. Employ tools like screen readers, such as [JAWS](https://accessibility.psu.edu/screenreaders/jawscommands/), [VoiceOver](https://support.apple.com/guide/voiceover-guide/welcome/web) or the keyboard shortcuts when testing for usage without a mouse for this assessment. Pay attention to specific issues during testing, such as ensuring the focus ring remains consistently visible, confirming that the page's order is logical, and verifying that all content is accessible to the screen reader.

### on a web application?
- Validate your webpage using a dedicated tool like [WebAIM’s WAVE Accessibility Evaluation Tool](https://wave.webaim.org/standalone), [Markup Validation Service](https://validator.w3.org/) and [Lighthouse from Google](https://developer.chrome.com/docs/lighthouse/overview). WebAIM's WAVE Accessibility Evaluation Tool offers the option to disable stylesheets, allowing you to assess the content ordering as presented to screen readers.
- Manually test the rendering of your application by enabling high contrast mode on your website (you can use a plugin like High Contrast in Chrome). 
- Review your page using a grayscale filter or a color-deficient vision simulator, such as [Coblis](https://www.color-blindness.com/coblis-color-blindness-simulator/), to confirm that the content is not solely reliant on color.
- Translate your page into another language, including a right-to-left language like Arabic. Confirm the following: ensure accurate rendering of all elements, verify precise translation of all content (employ a screen reader to catch potential oversights, especially in aria-labels), and check for proper content orientation when translated to or from a right-to-left language.
- Apply the provided CSS snippet and confirm that all elements are still rendered correctly, adhering to WCAG 1.4.12. In Chrome, you can utilize the Stylus plugin for easy implementation. 
```css 
*{
  line-height: 1.5 !important;
  letter-spacing: 0.12em !important;
  word-spacing: 0.16em !important;
} p 
  {
  margin-bottom: 2em !important;
 }
```
### on a mobile app?
- For Android apps, employ the Accessibility Scanner app, and for iOS apps, activate the Xcode Accessibility Inspector within Xcode. These tools offer insights into unlabeled elements, clipped text, color contrast levels, and text size.
- Follow the tips and tricks provided on [Mobile A11y](https://mobilea11y.com/). 
- Utilize a screen reader to assess the element order in your app. For Android, you can use TalkBack, and for iOS, employ VoiceOver. 
- Utilize [Appium](http://appium.io/docs/en/latest/) to develop a test suite for a mobile app, incorporating accessibility testing.

### on a non-web application?
- Refer to the guidance provided in [Applying WCAG 2.2 to Non-Web Information and Communications Technologies (WCAG2ICT)](https://www.w3.org/TR/wcag2ict-22/#introduction) for additional tips and tricks.

## What to avoid?
Incorporate accessibility into the core design of your application rather than treating it as an add-on feature.

## Considerations
Testing accessibility thoroughly can be challenging. Consider collaborating with users, including those with disabilities, and invite them to test and provide feedback. 

## Further reading
- [Testing for Accessibility](https://accessibility.psu.edu/testing/protocol/)
- [Praktische toegankelijkheidstips](https://www.digitoegankelijk.nl/aan-de-slag/tips)

## Acknowledgments
Many thanks to [Aram Limpens](https://github.com/alimpens) and [Sirée Koolen-Wijkstra](https://github.com/SireeKoolenWijkstra)

