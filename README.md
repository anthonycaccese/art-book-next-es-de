# Art Book Next (ES-DE Version)
A simple theme for the version of EmulationStation used in [ES-DE](https://es-de.org/)

## **Preview**

| System View | Gamelist View |
|----|----|
| <img src="https://github.com/anthonycaccese/art-book-next-es-de/assets/1454947/b912e4c4-c255-48bf-a7c5-80fab62cb086"> | <img src="https://github.com/anthonycaccese/art-book-next-es-de/assets/1454947/67dec9b0-4460-4320-8bfb-3f524e344bd4"> |

## **Configuration Options**

- The theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE 
- `Theme Aspect Ratio` - sets the aspect ratio the theme will render at. If needed, this can be changed to match the aspect ratio of your screen (though it should happen automatically).
   - 16:9, 16:10, 4:3, 19.5:9 and 1:1 are supported
- `Theme Variant` - sets the layout used for the gamelist view when media & metadata are scraped for your games.  There are 6 variants to choose from:
   - `List: Metadata &amp; Miximage` - A simple list that displays the miximage artwork and shows all game metadata
   - `List: Metadata &amp; Boxart'` - Same structure as above but it displays cover artwork instead of miximage
   - `List: Metadata, Screenshot &amp; Marquee` - A simple list that displays the cover, marquee and screenshot artwork and shows all game metadata
   - `List: Boxart` - A simple list that removes all gamemetadata and displays only a game's cover artwork
   - `List: Screenshot &amp; Marquee` - A simple list that removes all gamemetadata and displays the screenshot and marquee artwork
   - There is also a set of variants that remove the display of the help system.  You'll see those listed with the prefix of `[Help Off]`
- `Theme Color Scheme` - sets the color scheme and system artwork that is used for the overall theme on all views.

## **Additional Notes**

### **Creating your own color scheme:**

1) In the resources folder you will find a template file called [colors-custom.xml](https://github.com/anthonycaccese/art-book-next-es-de/blob/main/resources/colors.xml)

2) Make a folder named `theme-customizations` and place a copy of the `colors.xml` file inside that folder.  The folder structure should look like this when you are done:
   ```
   /ES-DE/themes/art-book-next-es-de/theme-customizations/colors.xml
   ```
   *Note: This structure will allow you to continue to get updates for the theme from the theme downloader while also retaining your customizations.*

3) Edit the properites in `colors.xml` to create your custom color scheme:
   - Here is a definition of each property:
      - `artworkSource` - Sets the path to where your custom artwork for system view is stored.  
         - You shouldn't need to change this from the value that is set in the template you copied in step 2.  
         - There are mask files in the `resources/artwork-masks` that you can use to create artwork your own custom artwork for system view.
         - Export any custom artwork you create a `.png` with nearest neighboor scaling and place them in `/ES-DE/themes/art-book-next-es-de/theme-customizations/artwork-custom/`.
      - `systemBackgroundColor` - Sets the color to be used for the background on System View. 
      - `systemArtSaturation` - Sets the saturation level for system artwork.  1 is full color and 0 is no color.
      - `systemArtColor` - Sets the color for system artwork.  You can use this to create consistent color across all artwork if you like.  If you leave it as `ffffff` then it will display the default color of the artwork.
      - `systemLogoColor` - Sets the color for system logos on System View.
      - `helpIconColor` - Sets the icon color for items in the included help system.
      - `helpTextColor` - Sets the text color for items in the included help system.
    
4) Set the `Theme Color Scheme` in ES-DE's UI Settings menu to `Custom` and you should see your custom color scheme display.  If you see an error check that the paths discussed above are correct and then check that the values you added for each property are correct and well formatted.

If you make a custom color scheme and are comfortable with sharing I would love to check it out 😊
- Please feel free to create an issue in this repo called `Custom Color Scheme: [Name of your Color Scheme]`
- Include the values you used for the properties above (xml is preferred), the background image and fonts you added (if any) and a screenshot of what it looks like.

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
* The `Noir` System Artwork set was created and provided by [tenlevels](https://www.reddit.com/user/tenlevels/) with help from f8less and inspired by the artwork from the Epic Noir theme by chicuelo
* The `Outline` System Artwork set was created and provided by [Joppa Fallston](https://github.com/joppa-fallston), inspired by [denizonm's work](https://github.com/denizonm/Custom-Artbook-Next-Image-Replacements).
* Some System Artwork was created and provided by [theUnBurn](https://github.com/theUnBurn)
* Thank you to [GenoCL](https://genocl.carrd.co/) for the idea of the multi-artwork system view.  It got me to think about ES themes in a different way when building it out and it came out awesome.

## **License**
Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt this theme as long as you provide attribution back to me (and the above credits) as well share any updates you make under the same licence terms.

Thank you for taking a look at this 😄
