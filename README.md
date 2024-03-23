# Art Book Next (ES-DE Version)
A simple theme for the version of EmulationStation used in [ES-DE](https://es-de.org/)

## **Preview**

| System View | Gamelist View |
|----|----|
| <img width="1392" alt="Screenshot 2023-12-10 at 3 59 43 PM" src="https://github.com/anthonycaccese/art-book-next-es-de/assets/1454947/cea9e784-def2-4339-96ed-41f866166b21"> | <img width="1392" alt="Screenshot 2023-12-10 at 3 59 50 PM" src="https://github.com/anthonycaccese/art-book-next-es-de/assets/1454947/1a9c0ce1-31e2-4c5a-9eb2-4ed84c67a7e3"> |

## **Configuration Options**

- The theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE 
- `Theme Aspect Ratio` - sets the aspect ratio the theme will render at. If needed, this can be changed to match the aspect ratio of your screen (though it should happen automatically).
   - 16:9, 16:10 and 4:3 are supported
- `Theme Variant` - sets the layout used for the gamelist view when media & metadata are scraped for your games.  There are 6 variants to choose from:
   - `List` - A simple list that displays the miximage artwork and shows all game metadata
   - `List (Immersive)` - A simple list that displays the cover, marquee and screenshot artwork and shows all game metadata
   - `List (No Metadata)` - A simple list that removes all gamemetadata and displays the screenshot and marquee artwork
- `Theme Color Scheme` - sets the color scheme that is used for the overall theme on all views.  There are 7 built in color schems to choose from:
   - `Art Book Next` - the default color scheme.  Its an update the previous color scheme I used for Art Book in 2017
   - `Art Book` - the original color scheme from Art Book built in 2017
   - `Steam OS` - based on the primary colors used in Steam OS
   - `SNES` - based on the Super Nintendo colors used in North America
   - `Famicom` - based on the Nintendo Famicom console colors
   - `Black` - A darker version of Art Book Next
   - `Grayscale` - A lightended version of the theme overall

### Preview of the Theme Variants

| Theme Variant | Preview |
|----|----|
| List | <img width="1392" alt="Screenshot 2023-12-10 at 4 01 33 PM" src="https://github.com/anthonycaccese/art-book-next-es-de/assets/1454947/e869ee33-b0e0-4c4c-b1e0-fbe9eb632af6"> |
| List (Immersive) | <img width="1392" alt="Screenshot 2023-12-10 at 3 59 50 PM" src="https://github.com/anthonycaccese/art-book-next-es-de/assets/1454947/1a9c0ce1-31e2-4c5a-9eb2-4ed84c67a7e3"> |
| List (No Metadata) | <img width="1392" alt="Screenshot 2023-12-10 at 4 02 30 PM" src="https://github.com/anthonycaccese/art-book-next-es-de/assets/1454947/063f0b4a-ea9f-46f3-b567-d7a90cb43d3b"> |

## **Additional Notes**

### Scraping:
* Please make sure the following are set to be scraped under Scraper > Content Settings:
   * Game Names
   * Ratings
   * Other Metadata
   * Videos
   * Screenshots
   * Box Cover Images
   * Marquee (Wheel) Images
* Other media is optional and will be used in cases where one of the above is missing (for example Title Screen images will be used if screenshots are missing)

### Versions for other ES forks:
* If you use Retropie... then check out the version [here](https://github.com/anthonycaccese/art-book-next-retropie).
* If you use Batocera... then check out the version [here](https://github.com/anthonycaccese/art-book-next-es).  The Batocera version has all the same base features but simply makes them available to change through Batocera's menu UI.  It also adds some additional features such as the theming of the menu and the ability to toggle on/off the display of different media elements directly through the menu ui as well.

## **Acknowledgments**
* Most system logos were sourced and modified from the excellent work done by Dan Patrick [here](https://archive.org/details/console-logos-professionally-redrawn-plus-official-versions).  I modified each to be compatible with EmulationStation's current SVG support.
* ChangaOne font is by [Eduardo Tunni](https://www.fontsquirrel.com/fonts/changa)
* Oxygen font is by [Vernon Adams](https://www.fontsquirrel.com/fonts/oxygen)
* Auto-Collection Genre background art created by [@nautipuss](https://github.com/nautipuss)
* Metadata Icons sourced from [FontAwesome](https://fontawesome.com/search?o=r&m=free)

## **License**
Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt this theme as long as you provide attribution back to me (and the above credits) as well share any updates you make under the same licence terms.

Thank you for taking a look at this 😄
