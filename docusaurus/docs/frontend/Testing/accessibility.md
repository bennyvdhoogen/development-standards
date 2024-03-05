# Accessibility

## Why a standard for accessibility?
Op basis van de wet digitale overheid is de gemeente Amsterdam verplicht om haar websites en applicaties conform de Web Content Accessibility Guidelines (WCAG) te bouwen op niveau A en AA. Bij elkaar gaat het om 50 eisen, ook wel succescriteria genoemd, die betrekking hebben op toegankelijkheid. De succescriteria kunnen ingedeeld worden in vier principes.

**waarneembaar**

Alles op jouw website of app moet voor iedereen waarneembaar zijn. Een eis onder dit principe is bijvoorbeeld dat je een alternatieve tekst toevoegt aan een (informatieve) afbeelding. Iemand die de afbeelding niet ziet, kan deze dan toch waarnemen.

**bedienbaar**

Alles op jouw website of app moet door iedereen te bedienen zijn. Het navigatiemenu op jouw site moet bijvoorbeeld niet alleen met een muis, maar ook met het toetsenbord te bereiken zijn.

**begrijpelijk**

Alles op jouw website of app moet te begrijpen zijn door software en mensen. Je moet bijvoorbeeld de taal van een pagina aangeven in de code. Hulptechnologie zoals een schermlezer (screenreader) kan de tekst dan in de juiste taal voorlezen. Ook voor mensen moet je website of app begrijpelijk zijn. Zo moet je bij een formulier aangeven wáár de fout zit als iemand iets niet goed heeft ingevuld.

**robuust**

Jouw website of app moet door veel verschillende apparaten en hulptechnologie gebruikt kunnen worden. Een voorbeeld van een eis onder dit principe is dat je voor de elementen op jouw webpagina of in jouw app aangeeft wat hun naam, rol en waarde is.


## How to read this document

## When is this standard applicable?

De wet geldt voor alle websites en apps van de overheid. Daar vallen ook intranetten, extranetten en cloudapplicaties onder. Ook alle mobiele applicaties vallen onder de wet. Dat zijn dus zowel native, web- als hybride apps voor mobiele apparaten.

## What are good practices?

Thus while the techniques are useful for evaluating content, evaluations must go beyond just checking the sufficient technique tests in order to evaluate how content conforms to WCAG success criteria.


- Run your page through [WebAIM’s WAVE Accessibility Evaluation Tool](https://wave.webaim.org/standalone)
- Run Chrome’s Lighthouse on your page
- Run your page through an HTML Validator
- Ensure that all videos are captioned and audio described as needed and that audio-only files are transcribed.
- If you use style sheets, then disable style sheets to ensure content is in a usable order with style sheets turned off. This is the order that will be presented to screen readers.
- Attempt to operate your website with just the keyboard (but not with a screen reader). This test shows how well a mobility impaired user can access your page. The focus ring should always be visible, and the order of the page should make sense.
- View your page with a grayscale filter or color deficient vision simulator to ensure that content is not dependent on color.
- Make sure that all content is available in a screen reader.
- Translate your page and check if everything is translated.
- Translate your page and use a screenreader to check if everything is translated. Some content (like text in aria-label) isn’t always properly translated.
- Translate your page to a right-to-left language (like Arabic) and check if everything is still properly rendered and the content is flipped (a menu bar on the left should be on the right, etc.).
- Browsers can display text bigger than usual. Set your browser to the biggest text size, and check if this has an effect on your page, and that everything is still properly rendered.
- Zoom in 200% and check if everything is still properly rendered.
- Use High Contrast mode (a seperate plugin for Chrome) and check if everything is still properly rendered.
- Apply the following css snippet and check if everything is still properly rendered (WCAG 1.4.12). In Chrome you can use the Stylus plugin to easily do this. 
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

## What to avoid?

## Considerations

## Further reading

## Acknowledgments

> This page was last reviewed at 28th of February 2024. It needs to be reviewed again on the 28th of August 2024. 