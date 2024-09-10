# PAL Custom Color Palette Editor (for Weather Radar Products)

The PAL Color Palette Editor is a powerful tool for customizing color schemes and creating visual palettes for weather radar products and similar applications.

## Why does this tool exist?

Weather visualization tools often use color palettes to represent different intensities or types of precipitation. Having a customizable palette allows users to tailor the visual representation to their specific needs or preferences. This editor enables you to start with existing schemes like The Weather Channel (TWC) color palette and modify it to your liking, or create entirely new palettes from scratch.

## How to use it?

Open the [PAL Color Palette Editor](https://rainviewer.github.io/pal-color-palete-editor/pal-color-palette-editor.html) in your browser. It's a safe, client-side tool built with vanilla JavaScript. No external dependencies or trackers. Your palettes are saved in your browser's local storage, so you won't lose your work if you accidentally close the tab.

## Features

- Start with the TWC color scheme
- Customize colors for different intensity levels
- Visual editor for intuitive color selection
- Import existing PAL files
- Export your custom palettes in PAL format

## What is important?

By default, PAL color palete editor is set to colorize Rain Viewer's weather radar reflectivity data, so the input is set to -32..95 dBZ and the output is 0..127 in colors (only colors corresponding for the rain). If you want to tune color scheme for Satellite IR data, use 0..255 in both input and output paramethers or use your own values sutable for your application.

## PAL Resources

Need inspiration or looking for existing palettes? Check out these resources:

- [WxTools Reflectivity Palettes](https://www.wxtools.org/reflectivity)
- [pykl3radar Color Tables](http://pykl3radar.com/colorTables/index.php)

Your custom palettes can be used in various weather visualization tools, including Rain Viewer.

## PAL Format Example

Here's a snippet of what a PAL file might look like:

```
; The Weather Channel
product: BR
Units: DBZ

Color: 5 99 235 99
Color: 10 99 235 99
Color: 15 61 198 61
Color: 20 31 158 52
Color: 25 17 103 25
SolidColor: 34 2 48 2
Color: 35 255 255 0  
Color: 40 255 127 0 
Color: 45 230 0 0
Color: 50 205 0 0
Color: 55 155 0 0
Color: 60 130 0 0
Color: 65 105 0 0 234 0 247
Color: 70 255 255 255 

```

For more details on creating custom color palettes, check out this [guide from RadarScope](https://radarscope.zendesk.com/hc/en-us/articles/4642122920722-Creating-a-Custom-Color-Palette-for-RadarScope).

## Any suggestions or ideas?

Feel free to create a pull request or fork. Your contributions are welcome!
