# Art Book Next (ES-DE Version)
A simple theme for the version of EmulationStation used in [ES-DE](https://es-de.org/) v2.x.  
*(If you are using ES-DE v1.x or earlier please download [this version](https://github.com/anthonycaccese/art-book-next-retropie) instead)*

## **Preview**

| System View | Gamelist View |
|----|----|
| ![Screenshot 2023-03-02 at 12 32 40 PM](https://user-images.githubusercontent.com/1454947/222508403-0d97b557-40e1-45df-b797-ba8ed1ff4247.png) | ![Screenshot 2023-03-02 at 12 33 13 PM](https://user-images.githubusercontent.com/1454947/222508431-d301835c-c3a7-47e9-b94a-90a93ed6a0e9.png) |

## **Configuration Options**

- The theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE 
- `Theme Aspect Ratio` - sets the aspect ratio the theme will render at. If needed, this can be changed to match the aspect ratio of your screen (though it should happen automatically).
   - 16:9, 16:10 and 4:3 are supported
- `Theme Variant` - sets the layout used for the gamelist view when media & metadata are scraped for your games.  There are 6 variants to choose from:
   - `List` - A simple list that displays the miximage artwork and shows all game metadata
   - `List (Immersive)` - A simple list that displays the cover, marquee and screenshot artwork and shows all game metadata
   - `List (No Metadata)` - A simple list that removes all gamemetadata and displays the screenshot and marquee artwork
   - `Carousel` - a cover art focused carousel view with all game metadata
   - `Carousel (Immersive)` - similar to the carousel variant but also displays video
   - `Carousel (No Metadata)` - Removes all metadata and simply displays a cover artwork carousel
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
| List | ![Screenshot 2023-03-02 at 12 33 29 PM](https://user-images.githubusercontent.com/1454947/222512099-89b111a5-d1e3-456b-90b8-d442cd4004ea.png) |
| List (Immersive) | ![Screenshot 2023-03-02 at 12 33 13 PM](https://user-images.githubusercontent.com/1454947/222512152-623df201-0733-4ea5-80f2-a660941676af.png) |
| List (No Metadata) | ![Screenshot 2023-03-02 at 12 33 36 PM](https://user-images.githubusercontent.com/1454947/222512196-246d5e3a-d3ab-483a-a69e-173fb1695f1f.png) |
| Carousel | ![Screenshot 2023-03-02 at 12 33 45 PM](https://user-images.githubusercontent.com/1454947/222512248-08a48aac-9c4f-406d-b32c-ca491e3e8752.png) |
| Carousel (No Metadata) | ![Screenshot 2023-03-02 at 12 33 54 PM](https://user-images.githubusercontent.com/1454947/222512311-3a9adf96-3894-444a-a6b7-b8adbb098ac8.png) |


### Preview of the Theme Color Schemes

| Theme Color Scheme | Preview |
|----|----|
| Art Book Next | ![Screenshot 2023-03-02 at 12 33 13 PM](https://user-images.githubusercontent.com/1454947/222511503-7a2b8402-5f83-4932-8f39-e1f0e60cf91f.png) |
| Art Book (based on my original theme from [2017](https://retropie.org.uk/forum/topic/11728/theme-art-book)) | ![Screenshot 2023-03-02 at 12 34 17 PM](https://user-images.githubusercontent.com/1454947/222511554-cc4a5bab-b364-4def-9773-e240fae99485.png) |
| Steam OS (being used as the default for [RetroDeck](https://github.com/XargonWan/RetroDECK/)) | ![Screenshot 2023-03-02 at 12 34 23 PM](https://user-images.githubusercontent.com/1454947/222511616-c6ce979a-bc81-444c-a64d-105a032694d0.png) |
| SNES (simply made for fun as the SNES was my first console) | ![Screenshot 2023-03-02 at 12 34 28 PM](https://user-images.githubusercontent.com/1454947/222511713-247ad1a2-6a5b-4952-a9bd-730e830cad37.png) |
| Famicom | ![Screenshot 2023-03-02 at 12 34 34 PM](https://user-images.githubusercontent.com/1454947/222511749-d8f7e610-53da-4210-994f-2a1c8aad91c4.png) |
| Black | ![Screenshot 2023-03-02 at 12 34 39 PM](https://user-images.githubusercontent.com/1454947/222511766-3583a8ac-64b3-4b35-9bc2-5e392ef34846.png) |
| Grayscale | ![Screenshot 2023-03-02 at 12 34 46 PM](https://user-images.githubusercontent.com/1454947/222511794-65c863d0-a006-459e-9980-9a83c39f4e4e.png) |

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
* If you use Retropie or ES-DE v1.x or eariler... then check out the version [here](https://github.com/anthonycaccese/art-book-next-retropie).
* If you use Batocera... then check out the version [here](https://github.com/anthonycaccese/es-theme-art-book-next/archive/2.0.zip).  The Batocera version has all the same base features but simply makes them available to change through Batocera's menu UI (i.e. you don't need to touch the XML as discussed above).  It also adds some additional features such as the theming of the menu and the ability to toggle on/off the display of different media elements directly through the menu ui as well.

## **Acknowledgments**
* Most system logos were sourced and modified from the excellent work done by Dan Patrick [here](https://archive.org/details/console-logos-professionally-redrawn-plus-official-versions).  I modified each to be compatible with EmulationStation's current SVG support.
* ChangaOne font is by [Eduardo Tunni](https://www.fontsquirrel.com/fonts/changa)
* Oxygen font is by [Vernon Adams](https://www.fontsquirrel.com/fonts/oxygen)

## **License**
Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt this theme as long as you provide attribution back to me (and the above credits) as well share any updates you make under the same licence terms.

Thank you for taking a look at this 😄
