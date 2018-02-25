# How to customize this fork to suit your needs:

## Custom boot screen
Simply swap the image with yours. Use the converter mentioned inside `_Bootscreen.h` file, copy the code and paste it between `{` and `}` then compile. In my version, it shows the logo for 2 seconds. Modify the delay to suit your needs.

## Custom name for printer
Change the line `#define CUSTOM_MACHINE_NAME` to whatever name you want.

## Splash screen text
`#define STRING_SPLASH_LINE2 "Message"`. I suggest leaving first splash text intact so people can read the firmware version.

### What is `#define STRING_CONFIG_H_AUTHOR`?
It's just a line where you write your (nick)name to. That's to show who changed this version of firmware. Some software will pull this info and display it.

## Different screen type
By default, this uses 128x64 RepRapDiscount Full Graphic Smart Controller. To change this to stock 4-line character LCD, go to `//#define ULTRA_LCD` and uncomment it, then comment out the line below. For even more different display, scroll a bit down and you'll see the settings.

## Summary
There you go, a guide on how to modify the cosmetics of Marlin. Please respect GPL.
