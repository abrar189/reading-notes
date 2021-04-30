# Images
## Adding Images
< img > 
To add an image into the page you need to use an < img > element. This is an empty
element (which means there is no closing tag). It must carry the following two attributes:

- src :This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. (Here you can see that the images are in a child folder called images — relative URLs

- alt: This provides a text description of the image which describes the image if you cannot see it.

- title:  You can also use the title attribute with the < img > element to provide additional information about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image.

**Height This specifies the height of the image in pixels.**

**Width This specifies the width of the image in pixels.**

## Where to Place Images in Your Code
1. Before a paragraph
2. Inside the start of a paragraph
3. In the middle of a paragraph

# Color
The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
 - rgb values: These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)

 - Hex codes: These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80

- color names: There are 147 predefined color names that are recognized by browsers. For example: DarkCyan.

## Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.

![image](https://www.pngkey.com/png/full/34-348874_red-green-and-blue-used-to-create-other.png)

## example color :

![image](https://steemitimages.com/DQmSeqka7ChoKqsaBRHghteSSoPv25TuFm51bmkGBPWE7b2/Example.png)

# Text

1. There are properties to control the choice of font, size, weight, style, and spacing.
2. There is a limited choice of fonts that you can assume most people will have installed.
3. If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.
4. You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.
5. You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.

# JPEG vs PNG vs GIF

- Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth.
- Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. 
- Use GIF format for images that contain animations.

## Compression
Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size.
 
 1. JPEG is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality. Beyond this, the compression artefacts become more prominent. JPEG images are best suited for photographs and paintings of natural scenes where the variations in colour and intensity are smooth

 2. PNG is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper, it would also occupy more space on the disk. This makes it unsuitable for storing or transferring high-resolution digital photographs but a great choice for images with text, logos and shapes with sharp edges.

 3. GIF is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. Given that PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.

 ## Transparency

 - JPEG images don’t support transparency and are hence not usable for such cases.
 
- PNG images support transparency in two ways — inserting an alpha channel that allows partial transparency or by declaring a single colour as transparent (index transparency). Partial transparency makes the edges blend smoothly into the background. PNG8 images (discussed in the “Colours” section below) can support only index transparency whereas PNG24 images can support alpha channel transparency.

- GIF images support transparency by declaring a single colour in the colour palette as transparent (index transparency). Because of absence of partial transparency, the edges (specially rounded or too-detailed edges) get a poor jagged effect. Though this can be solved to some extent using dithering, with improved PNG support, GIF is unsuitable for images with transparent backgrounds.
