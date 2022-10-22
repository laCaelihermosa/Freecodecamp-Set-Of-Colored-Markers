# TYPE OF COLORS
primary colors are colors that, when combined, create pure white. But for this to happen, each color needs to be at its highest intensity.
Secondary colors are the colors you get when you combine primary colors.
Tertiary colors are created by combining a primary with a nearby secondary color. 

Two colors that are opposite from each other on the color wheel are called complementary colors. If two complementary colors are combined, they produce gray. But when they are placed side-by-side, these colors produce strong visual contrast and appear brighter.

When colors are very bright right next to each other contrast can be distracting if it's overused on a website, and can make text hard to read if it's placed on a complementary-colored background.

#rgb
    Colors begin as black, and change as different levels of red, green, and blue are introduced.
    A function is a piece of code that can take an input and perform a specific action. The CSS rgb function accepts values, or arguments, for red, green, and blue, and produces a color:
    rgb(red, green, blue);
    rgb(0, 0, 0) = black
    rgb(255, 255, 255) = white
    Each red, green, and blue value is a number from 0 to 255. 0 means that there's 0% of that color, and is black. 255 means that there's 100% of that color.
#rgba
    The rgba function works just like the rgb function, but takes one more number from 0 to 1.0 for the alpha channel:
    rgba(redValue, greenValue, blueValue, alphaValue);

#hex
    Hex color values start with a # character and take six characters from 0-9 and A-F. The first pair of characters represent red, the second pair represent green, and the third pair represent blue. For example, #4B5320.
    With hex colors, 00 is 0% of that color, and FF is 100%. So #00FF00 translates to 0% red, 100% green, and 0% blue, and is the same as rgb(0, 255, 0)
#hsl
    The HSL color model, or hue, saturation, and lightness.
    The CSS hsl function accepts 3 values: a number from 0 to 360 for hue, a percentage from 0 to 100 for saturation, and a percentage from 0 to 100 for lightness.
    Saturation is the intensity of a color from 0%, or gray, to 100% for pure color.
    Lightness is how bright a color appears, from 0%, or complete black, to 100%, complete white, with 50% being neutral.

# GRADIENT COLORS
    Is a way to use color transitions when one color transitions into another.
        - The CSS linear-gradient function lets you control the direction of the transition along a line, and which colors are used.
        - this function actually creates an image element, and is usually paired with the background property which can accept an image as a value.

        Basic gradietn function: 
        linear-gradient(gradientDirection, color1, color2, ...);

            gradientDirection is the direction of the line used for the transition.
                values:
                    - 0 to 360 degres.
                    - to right, to left, to bottom, to top
                    - color1 and color2 are color arguments, so you can place any of the color types shown.     
        Color-stops allow you to fine-tune where colors are placed along the gradient line. They are a length unit like px or percentages that follow a color in the linear-gradient function. The first color is at the start (0%), the second is in the middle (50%), and the last is at the end (100%) of the gradient line.

# OPACITY
    Describes how opaque, or non-transparent, something is. 
    With the CSS opacity property, you can control how opaque or transparent an element is. With the value 0, or 0%, the element will be completely transparent, and at 1.0, or 100%, the element will be completely opaque like it is by default.
    Another way to set the opacity for an element is with the alpha channel. Similar to the opacity property, the alpha channel controls how transparent or opaque a color is.
# BOX-SHADOW
    The box-shadow property lets you apply one or more shadows around an element. Here is basic syntax:
        box-shadow: offsetX offsetY color;
        box-shadow: offsetX offsetY blurRadius color;

         if you wanted to expand the shadow out further? You can do that with the optional spreadRadius value:
            - box-shadow: offsetX offsetY blurRadius spreadRadius color;


# SHORTHANDS
    margin: w px; ( where = top w bottom w left w right w )
    margin: w px x px; ( where = (top, bottom) w px,  (left, right) x px )
    margin: w px x px y px; ( where = top w px,  (left, right) x px, bottom y px )
    margin: w px x px y px z px; ( where = top w px, right x px, bottom y px, left z px, )

    For Padding:
    This works similarly to the shorthand margin.

---------------------------------------------------------------------
The default display property for div elements is block. So when two block elements are next to each other, they stack like actual blocks. For example, your marker elements are all stacked on top of each other.
    To position two div elements on the same line, set their display properties to inline-bloc.

- In the last project, you learned a little bit about borders and the border-color property.

All HTML elements have borders, though they're usually set to none by default. With CSS, you can control all aspects of an element's border, and set the border on all sides, or just one side at a time. For a border to be visible, you need to set its width and style.
        border-left-style:
        border-left-width:

        The border-left shorthand property lets you to set the left border's width, style, and color at the same time. 
           border-left: width style color;
           border-left: 10px solid black;
         