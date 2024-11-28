# P-10 Menu for EmulationStation

This is a tranlation of the Playchoice-10 menu interface for the version of EmulationStation used in [Batocera (v40 and above)](https://batocera.org/).

This version of the theme only works with distributions that use the latest Batocera (v40 and above) fork of EmulationStation.  Specifically [Batocera](https://batocera.org/), [Knulli](https://www.knulli.org/), [RockNIX](https://rocknix.org/) and [RetroBat](https://www.retrobat.org/)

My work focused on tranlating the layout so that it could be buildable in the theme engine for EmulationStation.  Please refer to the `Changes Made` section below for additional details.

The original version of the UI can be found as part of the Playchoice-10 arcade hardware.

## Changes Made

- Used screenshots of Playchoice-10 menu to approximate the components that would be used build a theme compatible with EmulationStation.
- Changed the helpsystem to EmulationStation's native component and created a layout that tries to evoke the original helpsystem design (sadly it can't be a 1:1 translation due to differences in the theme engines)
- Added icons specific to EmulationStation functionality
- Created a custom set of pixel icons for the helpsystem
- Added a framework for adding additional color schemes

## **Preview**

![Preview](https://github.com/user-attachments/assets/111926a1-2ff1-4fb8-b184-b8f975000d8a)

## **Configuration Options**

The following options can be changed directly from the main menu under `User Interface Settings > Theme Configuration`

### **Distribution:**

Used to define which folder to look in for Theme Customization files.

Options:
- `Batocera/Knulli`
- `RockNIX`
- `RetroBat`

### **Aspect Ratio:**

Sets the aspect ratio to match your display. This should happen automatically but can also be set manually if needed.

Options:
- `Automatic`
- `16:9`
- `16:10`
- `4:3`
- `1:1`
- `3:2`

### **Game Artwork:**

Defines the type of artwork used to represent a game. The artwork is sourced from the the selections you make in the scraper menu. Image will display the image you selected to scrape for `Image Source`. Boxart will display the image you selected to scrape for `Box Source`, Logo will display the image you selected to display for 

Options: 
- `Off`
- `Image`
- `Boxart`
- `Logo`

| Off | Image |
|----|----|
| ![Game Artwork Off](https://github.com/user-attachments/assets/d6538d34-8f87-4a9b-b7ac-3dd60f57edd1) | ![Game Artwork Image](https://github.com/user-attachments/assets/d2b27ac6-7fa4-4009-8aa3-1060ba0873ad) |

### **Color Scheme:**

Sets the color scheme that is used for the overall theme on all views.
 
| Playchoice | Light Blue | Capcom Purple |
|----|----|----|
| ![Playchoice](https://github.com/user-attachments/assets/111926a1-2ff1-4fb8-b184-b8f975000d8a) | ![Light Blue](https://github.com/user-attachments/assets/1ccef710-6178-43b6-9d8e-9769cb82240b) | ![Capcom Purple](https://github.com/user-attachments/assets/57f4d03e-36c5-4e27-9c14-780d97c56e7e) |

| Dark Tan | OLED | Light |
|----|----|----|
| ![Dark Tan](https://github.com/user-attachments/assets/8f577b07-fbca-4f6a-81a0-524aa95e8cff) | ![OLED](https://github.com/user-attachments/assets/f316036e-95f9-4586-b163-3409355f7732) | ![Light](https://github.com/user-attachments/assets/33fe0d65-a959-44f1-ab73-53d5b69bc804) |

You can also create your own custom color scheme by following the instructions under "[Creating your own color scheme](#creating-your-own-color-scheme)"
 
## Theme Customizations

P-10 Menu allows customizations to color schemes without the need to edit the source XML.  This enables you to change the look of the theme and still retain your changes when the theme is updated.

### Start Here
- Make sure the `Distribution` setting is set to the correct value for your current OS (e.g. Batocera/Knulli, RockNIX or RetroBat)
- This value determines the folder where you will add your customizations
    - Batocera/Knulli = `/userdata/theme-customizations/p-10-menu/`
    - RockNIX = `/roms/_userdata/theme-customizations/p-10-menu/`
    - Retrobat = `C:\RetroBat\emulationstation\.emulationstation\theme-customizations\p-10-menu\`
- Create the folders that match your distribution and then move on to the options below...

### Color Schemes

* Download this template: https://github.com/anthonycaccese/p-10-menu-es/blob/main/resources/customizations/colors.xml
* Upload it to the path you created above and make sure its called `colors.xml`
* Change any values in the template to the colors you prefer.
* I tried to make the values as self explanatory as possible but if you have questions regarding which property does what please don't hesitate to ask.
* After your colors are defined; in theme configuration change `Color Scheme` to `Custom`

If you make a custom color scheme and are comfortable with sharing I would love to check it out 😊
- Please feel free to create an issue in this repo called `Custom Color Scheme: [Name of your Color Scheme]`
- Include the values you used for the properties above (xml is preferred) and a screenshot of what it looks like.

## **Additional Notes**

### Versions for other ES forks:
* If you use ES-DE... then the ES-DE version [here](https://github.com/anthonycaccese/p-10-menu-es-de) will work out of the box with that distribution.  When used with ES-DE the theme comes with additional support for navigation sound sets.

### **Credits:**

- The included font is called ["A Goblin Appears!"](https://www.dafont.com/a-goblin-appears.font)

## **License**
Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt this theme as long as you provide attribution back to me (and the above credits) as well share any updates you make under the same license terms.