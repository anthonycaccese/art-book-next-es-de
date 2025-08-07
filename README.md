# Art Book Next (ES-DE Version)

A simple theme for [ES-DE](https://es-de.org/) based on the look of a coffee table art book.

## **Preview**

[![Art Book Next Overview](https://github.com/user-attachments/assets/d9a46907-2be3-430f-a841-96a1050c0461)](https://www.youtube.com/watch?v=vFmecuEw2As)

| System View | Gamelist View |
|----|----|
| <img src="https://github.com/user-attachments/assets/f49037ad-1b86-430f-a8ab-e00d8afa08d9" /> | <img src="https://github.com/user-attachments/assets/5ebd03a0-163d-4ca8-8371-7cfd0aa8052b" /> |

## **Configuration Options**

- The theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE 
- `Theme Variant` - Sets the layout used for the gamelist view when media & metadata are scraped for your games.  There are 7 variants to choose from:
   - `List: Metadata & Boxart` - A simple list that displays cover artwork and game metadata
   - `List: Metadata & Screenshot + Marquee` - A simple list that displays marquee, screenshot and game metadata
   - `List: Metadata & Screenshot + Boxart` - A simple list that displays the cover, screenshot and game metadata
   - `List: Metadata & Miximage` - A simple list that displays miximage artwork and game metadata
   - `List: Boxart` - A simple list that removes all game metadata and only displays a game's cover artwork
   - `List: Screenshot & Marquee` - A simple list that removes all game metadata and only displays the screenshot and marquee artwork
   - `List` - A simple list, nothing more 😊
   - There are also a set of variants that remove the display of the help system.  You'll see those listed with the prefix of `[Help Off]`.  They are the same as the above variants just with the help system turned off.
- `Theme Color Scheme` - Sets the color scheme, system artwork and system logo used on all views.  This can be customized by following the instructions in the [Customizations](#customizations) section below.
- `Theme Font Size` - Sets the font size to use. I've included font sizes built to scale well from small handheld screens all the way up through larger tv screens.
- `Theme Aspect Ratio` - Sets the aspect ratio that the theme will render at. This should happen automatically but if needed, this can be changed manually to match the aspect ratio of your screen.  16:9, 16:10, 4:3, 3:2, 8:7, 19.5:9, 21:9, 20:9, 32:9, 3:5, and 1:1 are supported

## **Customizations**

### **1. Creating your own color scheme**

A custom color scheme lets you to modify any of the colors, artwork and logos used in the theme while also allowing you to continue to get updates from the theme downloader.

#### Video Tutorial:

[![Customize Art Book Next](https://github.com/user-attachments/assets/5664b1be-793f-48c1-9363-49b941acbe15)](https://www.youtube.com/watch?v=gZTTwSI8QIc)

#### Instructions:

1) In the resources folder you will find a template file called [colors.xml](https://github.com/anthonycaccese/art-book-next-es-de/blob/main/resources/colors.xml)

2) Make a folder named in the Art Book Next folder called `theme-customizations` and place a copy of the `colors.xml` file inside that folder.  The folder structure should look like this when you are done:
   ```
   /ES-DE/themes/art-book-next-es-de/theme-customizations/colors.xml
   ```

3) Edit the properites in `colors.xml` to create your custom color scheme:
   - Here is a definition of each property:
      - `artworkSource` - Sets the path to where your custom artwork for system view is stored.  
         - If you want to create and display custom artwork then make sure `artworkSource` is set to point to `./theme-customizations/artwork`
         - There are mask files in the `resources/artwork-masks` that you can use to create your own custom artwork.
         - Export your artwork as a `.png` with nearest neighboor scaling and place it in `/theme-customizations/artwork/`.
         - For any system images you don't customize you can copy the source images from the theme the theme into `./theme-customizations/artwork`
      - `logoSource` - Sets the path to where your custom logos are stored.  
         - Make sure `logoSource` is set to point to `./theme-customizations/logos`
         - logos just need to be in SVG format, named the same as the system name and placed in the above folder.
      - `systemBackgroundColor` - Sets the color to be used for the background on System View. 
      - `systemArtSaturation` - Sets the saturation level for system artwork.  1 is full color and 0 is no color.
      - `systemArtColor` - Sets the color for system artwork.  You can use this to create consistent color across all artwork if you like.  If you leave it as `ffffff` then it will display the default color of the artwork.
      - `systemLogoColor` - Sets the color for system logos on System View.
      - `helpIconColor` - Sets the icon color for items in the included help system.
      - `helpTextColor` - Sets the text color for items in the included help system.
    
4) Set the `Theme Color Scheme` in ES-DE's UI Settings menu to `Custom` and you should see your custom color scheme display.  If you see an error check that the paths discussed above are correct and then check that the values you added for each property are correct and well formatted.

> [!NOTE]
> If you make a custom color scheme and are comfortable with sharing it, I would love to check it out 😊
> - Please feel free to create an issue in this repo called `Custom Color Scheme: [Name of your Color Scheme]`
> - Include the values you used for the properties above (xml is preferred), the artwork and logos you added (if any) and a screenshot of what it looks like.

### **2. Adding Custom Artwork & Logos for Custom Collections**

You can also add custom artwork and logos for any custom collections you create.  Please first follow the instructions for "Creating your own color scheme" above and then...

1) Make sure you have `Main Menu > Game Collection Settings > Group Custom Collections` set to `Never`
2) In your `theme-customizations/logos` folder add SVG logos for each custom collection you want to display.  They should be named the same as the collection.
3) In your `theme-customizations/artwork` folder add png images for each custom collection you want to display.  They should be named the same as the collection.

> [!NOTE]
> This image should help show how your image files should be named for custom collections.  Essentially they should be the same as your custom collection file names without the `custom-` prefix:
> 
> <img src="https://github.com/user-attachments/assets/4818d204-54db-435a-94ef-10525dddb354" />

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
* If you use Batocera, Rocknix or Knulli... then check out the version [here](https://github.com/anthonycaccese/art-book-next-es).  The Batocera version has all the same base features but simply makes them available to change through Batocera's menu UI.  It also adds some additional features such as the theming of the menu and the ability to toggle on/off the display of different media elements directly through the menu ui.
* If you use Retropie... then check out the version [here](https://github.com/anthonycaccese/art-book-next-retropie).

## **Credits**
* Most system logos were sourced and modified from the excellent work done by Dan Patrick [here](https://archive.org/details/console-logos-professionally-redrawn-plus-official-versions).  I modified each to be compatible with EmulationStation's current SVG support.
* ChangaOne font is by [Eduardo Tunni](https://www.fontsquirrel.com/fonts/changa)
* Auto-Collection Genre background art created by [@nautipuss](https://github.com/nautipuss)
* Metadata Icons sourced from [Phosphor Icons](https://phosphoricons.com/)
* The `Noir` System Artwork set was created and provided by [tenlevels](https://www.reddit.com/user/tenlevels/) with help from f8less and inspired by the artwork from the Epic Noir theme by chicuelo
* The `Outline` System Artwork set was created and provided by [Joppa Fallston](https://github.com/joppa-fallston), inspired by [denizonm's work](https://github.com/denizonm/Custom-Artbook-Next-Image-Replacements).
* Some System Artwork was created and provided by [theUnBurn](https://github.com/theUnBurn)
* Thank you to [GenoCL](https://genocl.carrd.co/) for the idea of the multi-artwork system view.  It got me to think about ES themes in a different way when building it out and it came out awesome.

## **License**
Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt this theme as long as you provide attribution back to me (and the above credits) as well share any updates you make under the same licence terms.

Thank you for taking a look at this 😄
