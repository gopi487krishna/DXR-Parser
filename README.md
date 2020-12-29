# DXR-Parser 🐱‍🏍

> A sphinx extension for converting doxygen **XML** output to stylesheet friendly RST files

# Reason behind this project 🤔

There are two main sphinx extensions that can generate RST files from doxygen / autodoc XML output

* [Breathe](1) (Bridge between Sphinx and Doxygen System)
* [Exhale](2) ( Built on top of breathe for automating stuff )

These extensions are quite rich in nature and provide a lot of customizablity for the user to render the output.

I personally wanted to use them in one of our C++ projects but came across some problems with the rendered output. Basically i was using [RTD theme](3) but did not like the color scheme of it so i decided to hack the CSS to meet my own expectations. 

This turned out to be really a big disaster 💥 . Due to lack of reference for the elements and large chunks of CSS it became very difficult to modify the look and feel of the docs. I had to try a lot of things to make the site look as I wanted and even then the results were not satisfactory. 

Thats when i gave a look at [Godot Docs](4) . The API documentation looked great and they did it by using their own extension for generating RST output from doxygen XML output. 

This gave me the idea for **DXR parser** 😋

[1]: https://github.com/michaeljones/breathe
[2]: https://github.com/svenevs/exhale
[3]: https://github.com/readthedocs/sphinx_rtd_theme
[4]: https://docs.godotengine.org/en/stable/index.html