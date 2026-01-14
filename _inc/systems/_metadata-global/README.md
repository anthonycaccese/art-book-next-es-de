# System Metadata Files for ES-DE
This repo contains XML files that add system metadata variables for use in themes created for [ES-DE](https://es-de.org/)

The files leverage ES-DE variables to allow the values to be used in any theme agnostic of how the theme is structured.

It also includes a `_default.xml` that can be used as a temporary fallback for when new systems are added to ES-DE

Each file provides the following metadata variables:
- `systemDescription` - A description of the system
- `systemReleaseYear` - The year the system was released (when available)
- `systemReleaseDate` - The date the system was released in ISO 8601 (`YYYY-MM-DD`) format.  If only the month and year was known then the format is `YYYY-MM`.  If only the year was known then the format is `YYYY`.
- `systemReleaseDateFormated` - A formated version of the release date in `Month Day, Year` format.  If only the month and year was known then the format is `Month Year`.  If only the year was known then the format is `Year`.
- `systemManufacturer` - Represents the original Manufacturer of the system.
- `systemHardwareType` - A value to represent the systems type (e.g. `Console`. `Portable`, `Computer`, etc...)
- `systemColor` - A hex value to represent a systems primary color (can be used for things like backgrounds or navigation highlights)
- `systemColorPalette1...4` - 4 different hex values to represent other colors that can be used for a system (useful for things like color bands)
- `systemCoverSize` - Represents the common aspect ratio for a given system's cover artwork.  Can be used to customize the size of grids and carousels that display cover art.  
   - Current set of sizes: `landscape`, `square`, `portrait`, `1-2`, `3-5`, `5-7`.
   - Using these values you can define width/height for just this set and those sizes will apply automatically to a given system.

## **Usage**
1. Download the latest release of this repo and place it in a dedicated folder in your theme.  
   - I recommend a dedicated folder like this: `/_inc/systems/metadata-global/` 
   - This approach will make it easier to update when changes are made.
2. Include a reference to files at the top of your root theme.xml file
   - As an example; I add the following includes in my themes:
   - `<include>./_inc/systems/metadata-global/_default.xml</include>` - default file for fallback use cases
   - `<include>./_inc/systems/metadata-global/${system.theme}.xml</include>` - the system specific xml file
3. Reference a value using the variable names listed above
   - For example if you wanted to add system specific colors to a UI element you would refernece `${systemColor}` for that value
   
## **Contributions**
- If you see any existing values that should be updated with more accurate data; please submit an issue or PR to this repo.  Make sure to include the system, specific change and the reason for the change in your request.
- If you have an idea for a new variable to add; please submitt an issue to this repo with details of the variable and what it could be used for.

## **Examples**

| [CarAlt)](https://github.com/Weestuarty/caralt-es-de) | [Chicuelo (Revisited](https://github.com/anthonycaccese/chicuelo-revisited-es-de) |
| :---: | :---: |
| ![CarAlt](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/eebb8d45-b881-482f-bac0-31888ab12fcd) | ![chicuelo](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/74411202-1985-40ee-8cf6-8e9e1d4b9cc1) |
| Implements: `systemDescription` | Implements: `systemDescription`, `systemReleaseYear` and `systemHardwareType` | 

| [CodyWheel](https://github.com/Weestuarty/codywheel-es-de) | [CoinOPS](https://github.com/TheGrizzMD/coinops-es-de) |
| :---: | :---: |
| ![codywheel](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/6ea5c477-371e-4bb9-b090-a200a8588282) | ![coinops](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/50f75c6e-04e3-41a6-af74-358bb45403f8) |
| Implements: `systemDescription`, `systemReleaseYear`, `systemManufacturer` and `systemHardwareType` | Implements: `systemDescription` | 

| [Colorful (Revisited)](https://github.com/anthonycaccese/colorful-revisited-es-de) | [Colorful (Simplified)](https://github.com/anthonycaccese/colorful-simplified-es-de) |
| :---: | :---: |
| ![colorful-revisited](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/9b79ccc8-e0d7-43ae-b865-40f7bf740267) | ![colorful-simplified](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/35fcfbf4-eb08-4682-ae09-4fa3b5b8060b) |
| Implements: `systemColor`, `systemDescription`, `systemManufacturer`, `systemReleaseYear`, and `systemHardwareType` | Implements: `systemColor`, `systemDescription`, `systemManufacturer`, `systemReleaseYear`, `systemCoverSize`, and `systemHardwareType` | 

| [Diamond](https://github.com/Weestuarty/diamond-es-de) | [Epic Noir (Next)](https://github.com/anthonycaccese/epic-noir-next-es-de) |
| :---: | :---: |
| ![diamond](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/378c8a8a-2e9f-4cbc-aab6-6f269218699f) | ![epic-noir-next](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/bc45b7fa-874f-4107-852f-9c1c3a0dfcc3) |
| Implements: `systemManufacturer` and `systemReleaseYear` | Implements: `systemColor`, `systemDescription`, `systemReleaseYear`, and `systemHardwareType` | 

| [Epic Noir (Revisited)](https://github.com/anthonycaccese/epic-noir-revisited-es-de) | [ForAll](https://github.com/Weestuarty/forall-es-de) |
| :---: | :---: |
| ![epic-noir-revisited](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/98c74c60-42a7-4b3e-b129-ed4156dbc070) | ![forall](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/01b12f6f-f18d-4b9f-9a2d-842b10e3b3d0) |
| Implements: `systemDescription`, `systemReleaseYear`, and `systemHardwareType` | Implements: `systemDescription` | 

| [NSO Menu (Interpreted)](https://github.com/anthonycaccese/nso-menu-interpreted-es-de) | [Retrofix (Revisited)](https://github.com/anthonycaccese/retrofix-revisited-es-de) |
| :---: | :---: |
| ![nso-menu](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/f483899f-56f0-4230-8bca-afed9aab63d4) | ![retrofix](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/cda97089-7611-47be-8a19-bff469c69e42) |
| Implements: `systemColor` and `systemCoverSize` | Implements: `systemColor` | 

| [Showcase](https://github.com/Weestuarty/showcase-es-de) | [SimCar](https://github.com/Weestuarty/simcar-es-de) |
| :---: | :---: |
| ![showcase](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/2b27affe-ed6c-437b-9569-cf4ded74061d) | ![simcar](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/dc1dae0e-a452-4c4a-83c5-05ce81a22ed6) |
| Implements: `systemDescription` | Implements: `systemDescription` | 

| [TexGriddy](https://github.com/Weestuarty/texgriddy-es-de) |
| :---: |
| ![textgriddy](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/ff0dc121-a943-4096-9d96-27ddaeea974f) |
| Implements: `systemDescription` |


## **Credits**
* Some descriptions, release dates & manufacturer details were sourced from the wikipedia entries for each system
* Some descriptions were sourced from [ckau-book](https://github.com/CkauNui/ckau-book/tree/master)
* Some release date and manufacturer details were sourced from the [Launchbox](https://gamesdb.launchbox-app.com/) platforms list
* System colors were sourced from the great work done by [viking](https://forums.launchbox-app.com/profile/70421-viking/) from their work on the [Colorful](https://forums.launchbox-app.com/files/file/2081-colorful-bigbox-theme) theme for Launchbox and [@rogs123](https://github.com/rogs123) from their work on the [NSO Menu](https://github.com/anthonycaccese/nso-menu-interpreted-es-de) theme for ES-DE
* System Cover sizes were sourced from examples on screenscraper.fr

## **License**
Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt these files as long as you provide attribution back as well share any updates you make under the same licence terms.