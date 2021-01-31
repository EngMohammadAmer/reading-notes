[HOME](README.md)

# What CSS does

CSS allows you to create rules that specify how the content of an element should appear. For example, you can specify that
the background of the page is cream, all paragraphs should appear in gray using the Arial typeface, or that all level one
headings should be in a blue, italic, Times typeface.

## The key to understanding how CSS works
is to imagine that there is an invisible box around every HTML element.

## BLOCK & INLINE ELEMENTS
- Block level elements look like they start on a new line.
- Inline elements flow within the text and do not start on a new line. 


## CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
CSS Associates Style rules with HTML elements
p {
font-family: Arial;
}

## CSS Can be styled as per the following:
1- inline style
2- internal 
3- external

# css selectors:
[PDF FILE](./"css selectors.pdf")

# Summary
INTRODUCING CSS
* CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.
* Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
* Different types of selectors allow you to target yourrules at different elements.
* Declarations are made up of two parts: the properties of the element that you want to change, and the values
of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
* CSS rules usually appear in a separate document, although they may appear within an HTML page.

# Color

* rgb values
These express colors in terms of how much red, green and blue are used to make it up. For
example: rgb(100,100,90)
* hex codes
These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80
* color names
There are 147 predefined color names that are recognized by browsers. For example: DarkCyan

## opacity, rgba
rgba(0,0,0,0.5);

## hsl, hsla
* hsla(0,100%,100%,0.5);
- hue
This is expressed as an angle (between 0 and 360 degrees).
- saturation
This is expressed as a percentage.
- lightness
This is expressed as a percentage with 0% being white, 50% being normal, and 100% being black.
The hsla color property allows you to specify color properties using hue, saturation, and lightness as above, and adds a fourth value which represents transparency (just like the rgba
property). The a stands for:
- alpha
This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.

# Summary
# COLOR
Color not only brings your site to life, but also helps convey the mood and evokes reactions.
* There are three ways to specify colors in CSS: RGB values, hex codes, and color names.
* Color pickers can help you find the color you want.
* It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).
* CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
* CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.
