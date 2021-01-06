# HTML Book
# Chapter 5

* A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one.
* If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.
* The `<img>` element is used to add images to a web page.
* You must always specify a `src` attribute to indicate the source of an image and an `alt` attribute to describe the content of an image.
* `title` You can also use the title attribute with the `<img>` element to provide additional information about the image.
`<img src="image.jpg" alt="content" title="additional info" />`
* You should save images at the size you will be using them on the web page and in the appropriate format.
* `height` This specifies the height of the image in pixels.
* `width` This specifies the width of the image in pixels.
* There are three rules to remember when you are creating images for your website which are summarized below. We go into greater detail on each topic over the next nine pages.
1. Save images in the right format.
2. Save images at the right size.
3. Use the correct resolution.
* Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.

# Chapter 11
* Color brings the site to life and helps evokes reactions.
* Three ways to use colors in CSS:
    * RGB values => These express colors in terms of how much red, green and blue are used to make it up.Ex. ` color: rgb(100,100,90); `
    * hex codes => These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign.Ex.`color: #ee3e80;`
    * color name => There are 147 predefined color names that are recognized by browsers.Ex. ` color: DarkCyan; `
* Backgrounf color: By default, most browser windows have a white background, but browser users can set a background color for their windows, so if you want to be sure that the background is white you can use the background-color property on the `<body>` element. `background-color: rgb(200,200,200);`

* Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.
* When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.
* CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and lightness values.
    * hue =>This is expressed as an angle(between 0 and 360 degrees)
    * saturation => This is expressed as a percentage.
    * lightness => This is expressed as a percentage with 0% being white, 50% being normal, and 100% being black.
  
* CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
* CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.

# Chapter 12
* Typeface Terminology
1. Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.
2. Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.
3. Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)
* When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.
* The `font-family` property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.
* The `font-size` property enables you to specify a size for the font. There are several ways to specify the size of a font.
* `@font-face` allows you to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if it is not on the user's machine.
* The `text-transform` property is used to change the case of text giving it one of the following values: `uppercase `This causes the text to appear uppercase. `lowercase` This causes the text to appear lowercase. `capitalize` This causes the first letter of each word to appear capitalized.
* The text-decoration property allows you to specify the following values: `none`  This removes any decoration already applied to the text. `underline` This adds a line underneath the text. `overline` This adds a line over the top of the text. `line-through` This adds a line through words. `blink` This animates the text to make it flash on and off (however this is generally frowned upon, as it is considered rather annoying).
* The text-align property allowsyou to control the alignment oftext. The property can take oneof four values:`left`This indicates that the textshould be left-aligned.`right`This indicates that the textshould be right-aligned.`center`This allows you to center text.`justify`This indicates that every line ina paragraph, except the last line,should be set to take up the fullwidth of the containing box.
* There are properties to control t XX he choice of font, size, weight, style, and spacing.
* There is a limited choice of fonts that you can assume most people will have installed.
* If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.
* You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.
* You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.