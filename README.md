# Art Book Next (ES-DE Version)
A simple theme for the version of EmulationStation used in [ES-DE](https://es-de.org/)

## **Preview**

| System View | Gamelist View |
|----|----|
| <img src="https://github.com/anthonycaccese/art-book-next-es-de/assets/1454947/b912e4c4-c255-48bf-a7c5-80fab62cb086"> | <img src="https://github.com/anthonycaccese/art-book-next-es-de/assets/1454947/67dec9b0-4460-4320-8bfb-3f524e344bd4"> |

## **Configuration Options**

- The theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE 
- `Theme Aspect Ratio` - sets the aspect ratio the theme will render at. If needed, this can be changed to match the aspect ratio of your screen (though it should happen automatically).
   - 16:9, 16:10, 4:3 and 19.5:9 are supported
- `Theme Variant` - sets the layout used for the gamelist view when media & metadata are scraped for your games.  There are 6 variants to choose from:
   - `List: Metadata &amp; Miximage` - A simple list that displays the miximage artwork and shows all game metadata
   - `List: Metadata &amp; Boxart'` - Same structure as above but it displays cover artwork instead of miximage
   - `List: Metadata, Screenshot &amp; Marquee` - A simple list that displays the cover, marquee and screenshot artwork and shows all game metadata
   - `List: Boxart` - A simple list that removes all gamemetadata and displays only a game's cover artwork
   - `List: Screenshot &amp; Marquee` - A simple list that removes all gamemetadata and displays the screenshot and marquee artwork
   - There is also a set of variants that remove the display of the help system.  You'll see those listed with the prefix of `[Help Off]`
- `Theme Color Scheme` - sets the color scheme that is used for the overall theme on all views.  There are 7 built in color schems to choose from:
   - `Art Book Next` - the default color scheme.  Its an update the previous color scheme I used for Art Book in 2017
   - `Art Book` - the original color scheme from Art Book built in 2017
   - `Steam OS` - based on the primary colors used in Steam OS
   - `SNES` - based on the Super Nintendo colors used in North America
   - `Famicom` - based on the Nintendo Famicom console colors
   - `Black` - A darker version of Art Book Next
   - `Grayscale` - A lightended version of the theme overall

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
* Other media is optional and may be used in cases where one of the above is missing

### Versions for other ES forks:
* If you use Retropie... then check out the version [here](https://github.com/anthonycaccese/art-book-next-retropie).
* If you use Batocera... then check out the version [here](https://github.com/anthonycaccese/art-book-next-es).  The Batocera version has all the same base features but simply makes them available to change through Batocera's menu UI.  It also adds some additional features such as the theming of the menu and the ability to toggle on/off the display of different media elements directly through the menu ui as well.

## **Acknowledgments**
* Most system logos were sourced and modified from the excellent work done by Dan Patrick [here](https://archive.org/details/console-logos-professionally-redrawn-plus-official-versions).  I modified each to be compatible with EmulationStation's current SVG support.
* ChangaOne font is by [Eduardo Tunni](https://www.fontsquirrel.com/fonts/changa)
* Oxygen font is by [Vernon Adams](https://www.fontsquirrel.com/fonts/oxygen)
* Auto-Collection Genre background art created by [@nautipuss](https://github.com/nautipuss)
* Metadata Icons sourced from [FontAwesome](https://fontawesome.com/search?o=r&m=free)
* Thank you to [GenoCL](https://genocl.carrd.co/) for the idea of the multi-artwork system view.  It got me to think about ES themes in a different way when building it out and it came out awesome.

## **License**
Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt this theme as long as you provide attribution back to me (and the above credits) as well share any updates you make under the same licence terms.

Thank you for taking a look at this 😄
