# P-10 Menu for EmulationStation

This is a tranlation of the Playchoice-10 menu interface for distributions that use this fork of [EmulationStation](https://github.com/batocera-linux/batocera-emulationstation).  Specifically [Batocera](https://batocera.org/) (v40 and above), [Knulli](https://www.knulli.org/), [RockNIX](https://rocknix.org/) and [RetroBat](https://www.retrobat.org/)

My work focused on tranlating the layout so that it could be buildable in the theme engine for EmulationStation.  Please refer to the `Changes Made` section below for additional details.

The original version of the UI can be found as part of the Playchoice-10 arcade hardware.

## Changes Made

- Used screenshots of Playchoice-10 menu to approximate the components that would be used build a theme compatible with EmulationStation.
- Changed the helpsystem to EmulationStation's native component and created a layout that tries to evoke the original helpsystem design (sadly it can't be a 1:1 translation due to differences in the theme engines)
- Added icons specific to EmulationStation functionality
- Created a custom set of pixel icons for the helpsystem
- Added a framework for adding additional color schemes

## **Preview**

![Preview](https://github.com/user-attachments/assets/3eee1c23-cf70-42e9-b3d2-d851e7b4b311)

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

| Off | Boxart |
|----|----|
| ![Game Artwork Off](https://github.com/user-attachments/assets/d22089b3-9f37-487c-bfec-e542ed2ca535) | ![Game Artwork Image](https://github.com/user-attachments/assets/319454f6-fde1-4996-a5fc-4ff2de3c3d30) |

### **Color Scheme:**

Sets the color scheme that is used for the overall theme on all views.
 
| Playchoice | Light Blue | Capcom Purple |
|----|----|----|
| ![Playchoice](https://github.com/user-attachments/assets/3eee1c23-cf70-42e9-b3d2-d851e7b4b311) | ![Light Blue](https://github.com/user-attachments/assets/33353d7c-b197-4697-8293-29f6ed02ff1c) | ![Capcom Purple](https://github.com/user-attachments/assets/6343d6f9-60e5-4bf5-92be-b7751280dbd4) |

| Dark Tan | OLED | Light |
|----|----|----|
| ![Dark Tan](https://github.com/user-attachments/assets/e26730ad-5db8-4a81-9da9-14232c31a85a) | ![OLED](https://github.com/user-attachments/assets/da12e5fd-54be-4678-8edf-6689452a4300) | ![Light](https://github.com/user-attachments/assets/7cb0862a-91cd-486a-8672-31c8513f62e8) |

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
