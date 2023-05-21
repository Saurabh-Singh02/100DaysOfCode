## CSS Colors
* Colors are specified using predefined color names, or RGB, HEX, HSL, RGBA, HSLA values.

## CSS Color Names
* In CSS, a color can be specified by using a predefined color name:

* Tomato
* Orange
* DodgerBlue
* MediumSeaGreen
* Gray
* SlateBlue
* Violet
* LightGray

* CSS/HTML support more than **130** standard color names.

## CSS Background Color
* You can set the background color for HTML elements:
```
<h1 style="background-color:DodgerBlue;">Hello World</h1>
<p style="background-color:Tomato;">Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
```

## CSS Text Color
* You can set the color of text:

```
<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
<p style="color:MediumSeaGreen;">Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
```

## CSS Border Color
You can set the color of borders:

```
<h1 style="border:2px solid Tomato;">Hello World</h1>
<h1 style="border:2px solid DodgerBlue;">Hello World</h1>
<h1 style="border:2px solid Violet;">Hello World</h1>
```

## CSS Color Values
In CSS, colors can also be specified using RGB values, HEX values, HSL values, RGBA values, and HSLA values:

Same as color name "Tomato":
rgb(255, 99, 71)
#ff6347
hsl(9, 100%, 64%)


Same as color name "Tomato", but 50% transparent:
rgba(255, 99, 71, 0.5)
hsla(9, 100%, 64%, 0.5)
```
<h1 style="background-color:rgb(255, 99, 71);">...</h1>
<h1 style="background-color:#ff6347;">...</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>

<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1>
```
## CSS RGB Colors
* An RGB color value represents RED, GREEN, and BLUE light sources.
## RGB Value
**rgb(red, green, blue)**

* Each parameter (red, green, and blue) defines the intensity of the color between 0 and 255.

* For example, rgb(255, 0, 0) is displayed as red, because red is set to its highest value (255) and the others are set to 0.

* To display black, set all color parameters to 0, like this: rgb(0, 0, 0).

* To display white, set all color parameters to 255, like this: rgb(255, 255, 255).

## RGBA Value
* RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity for a color.

* An RGBA color value is specified with:

**rgba(red, green, blue, alpha)**

* The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all):

## CSS HEX Colors
* A hexadecimal color is specified with: #RRGGBB, where the RR (red), GG (green) and BB (blue) hexadecimal integers specify the components of the color.

## HEX Value
**#rrggbb**

* Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).

* For example, #ff0000 is displayed as red, because red is set to its highest value (ff) and the others are set to the lowest value (00).

* To display black, set all values to 00, like this: #000000.

* To display white, set all values to ff, like this: #ffffff.  

## 3 Digit HEX Value
* Sometimes you will see a 3-digit hex code in the CSS source.

* The 3-digit hex code is a shorthand for some 6-digit hex codes.
**#rgb**
* The 3-digit hex code can only be used when both the values (RR, GG, and BB) are the same for each component. So, if we have #ff00cc, it can be written like this: #f0c.

## CSS HSL Colors
* HSL stands for hue, saturation, and lightness.

## HSL Value
**hsl(hue, saturation, lightness)**

* Hue is a degree on the color wheel from 0 to 360. 0 is red, 120 is green, and 240 is blue.

* Saturation is a percentage value. 0% means a shade of gray, and 100% is the full color.

* Lightness is also a percentage. 0% is black, 50% is neither light or dark, 100% is white

## HSLA Value
* HSLA color values are an extension of HSL color values with an alpha channel - which specifies the opacity for a color.

* An HSLA color value is specified with:
**hsla(hue, saturation, lightness, alpha)**