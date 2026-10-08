# NASA Task Load Index (NASA-TLX)
========

An implementation of the NASA Task Load Index (NASA-TLX).

## General information
From the respective [Wikipedia article](http://en.wikipedia.org/wiki/NASA-TLX):
> The NASA Task Load Index (NASA-TLX) is a subjective, multidimensional assessment tool that rates perceived workload, in order to assess a task, system, or team’s effectiveness or other aspects of performance. It was developed by the Human Performance Group at NASA’s [Ames Research Center](http://en.wikipedia.org/wiki/Ames_Research_Center) over a three year development cycle that included more than 40 laboratory simulations. It has been cited in over 550 studies and a recent search for “NASA-TLX” on Google Scholar revealed over 3,660 articles. These statistics highlight the large influence the NASA-TLX has had in [Human Factors](http://en.wikipedia.org/wiki/Human_Factors) research.

Learn more about it at the official [NASA-TLX website](http://humansystems.arc.nasa.gov/groups/TLX/). You can also take a look at the original paper [<cite>Development of NASA-TLX (Task Load Index): Results of Empirical and Theoretical Research</cite>](http://humansystems.arc.nasa.gov/groups/TLX/downloads/NASA-TLXChapter.pdf) (PDF format, 1.4 MB).

## Custom Modifications for Relish Food Memories Workshop
This fork has been specifically modified to run the **Relish Food Memories Workshop Cognitive Load Test**. 

Key features added to this version:
- **Simplified Participant Input**: Removed complex "Proband" and "Task" creation in Step 1. It now just asks for the Participant's Name.
- **CSV Download**: Researchers can instantly download a CSV file containing all test results recorded in the local browser session.
- **Google Sheets Integration (Optional Backend)**: Seamlessly configured to automatically push results to a Google Sheet via Google Apps Script the moment a participant completes the test. This enables remote testing where participants use their own devices.

## Installation / Usage
No server installation is required. This is a static HTML/JS web app.
1. Download the code or clone the repository.
2. Open `index.html` in your browser.
3. **Optional (Google Sheets Setup):** 
   - Create a Google Apps Script Web App to handle POST requests.
   - Insert your Web App URL into `var scriptURL = '...'` located around line 258 of `setup/js/default.js`.

## Tested browsers
At this point I tested the implementation with the latest versions of
- Chrome
- Firefox
- Opera
- Safari

## Author
- [Francesco Schwarz](https://github.com/isellsoap/)

## Used libraries and utilities
- [jQuery](http://jquery.com/) ([MIT license](https://github.com/jquery/jquery/blob/master/MIT-LICENSE.txt))
- [jQuery UI](http://jqueryui.com/) ([MIT license](http://www.opensource.org/licenses/mit-license) or [GPL v2](http://opensource.org/licenses/GPL-2.0))
- [Highcharts JS](http://www.highcharts.com/) (non-commercial use with [CC BY-NC 3.0](http://creativecommons.org/licenses/by-nc/3.0/) license)

## License
This NASA-TLX implementation is published under the [MIT license](http://www.opensource.org/licenses/mit-license) and [GPL v3](http://opensource.org/licenses/GPL-3.0).

## Other implementations of the NASA-TLX
You can also take a look at how others implemented the NASA-TLX:
- [Keith Vertanen](http://www.keithv.com/software/nasatlx/) (implemented with HTML and JavaScript)
- [Jonathan Polom ](https://github.com/jmpolom/NASA-TLX) (implemented with Python and wxPython)