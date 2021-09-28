# (Python) Image to ANSI Converter

*Credit where credit is due.*

This python script is based off of original work by Micah Elliott (MicahElliott) located in Gist colortrans.py which was then used to create image-to-ansi.py by K Lange (klange) and subsequently improved on by Takumi Sueda (puhitaku). A big thanks to those foundations.

## Purpose

This script uses python libraries to provide a way to take image files and make them color compatible for use in a shell (ANSI). Which allows display of terminal art such as that contained in the demo.png file. The original colortrans.py file (not included here) provides a way to translate RGB values into ANSI compatible terminal codes (i.e. color included), find that script if you plan to do this all manually.

![alt text](https://github.com/torrycrass/image-to-ansi/blob/master/demo.png "demo converted cli image")

### Prerequisites
*Assumptions*

Yeah yeah, I'm aware about assumptions but this isn't subtaintial enough that I'm going to put in undue effort on this. So, all instructions, suggestions, and guidance assume that you're using Debian/Ubuntu. This will also assume you are using a newer version of either distro. If you are using an older version change **apt** to **apt-get** where you find it.

1. Python (if not already installed install by **apt install python**)
2. python-pip (**apt install python-pip**)
3. Pillow (**pip install pillow**)
4. Image (**pip install Image**)

### Usage
`python3 image-to-ansy.py <image>` or
`python3 image-to-ansy.py <image> | ./commandify` to create a command that will print the image.

### To-Do List

- [ ] Review sizing of output. Currently images larger than 50x50 are not very practical for console use.
- [x] Update script to display help information on run without variable or --help option

#### Additional References/Resources

- http://patorjk.com/software/taag/ (An online text to ASCII art converter)
- https://16colo.rs (A library of ANSI art)
- https://www.ansilove.org (A software library for ANSI file conversion)
- http://www.roysac.com (A collection of ANSI/ASCII art and tools)
- http://vectorpoem.com/playscii/ (An ANSI/ASCII art editing tool)
- https://github.com/atdt/escapes.js/ (A library for rendering ANSI art in HTML5/JS)

#### Prior Author Credits
- Micah Elliott (MicahElliott): https://gist.github.com/MicahElliott/719710
- K Lange (klange): https://gist.github.com/klange/1687427
- Takumi Sueda (puhitaku): https://gist.github.com/puhitaku/7eaf6142fa5a42425f55
