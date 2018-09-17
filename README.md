# burial-mound-volume-tool

Tool to aid estimation of burial mound volume based on photographs with human scales. The current iteration of the tool allows you to plot a table of coordinates following the horizon of the mound and find horizon polynomial coefficents in excel. Postprocessing (currently done in Excel) is used to generate an approximation of the horizon of the mound (using linest polynomial coefficents to model trendline of the coordinates) of which is used to estimate mound volume using the cylindrical shells method (rotate around y axis). This volume value is to be used in research into burial mound construction methodology.

### Installing and running

Steps to get running:

**1. Clone repository**
**2. Run Part A: [Process Image Tool](https://jserc.github.io/burial-mound-volume-tool/PART_A_ProcessImagesTool.html)** - *(to use locally, file is [PART_A_ProcessImagesTool.html](PART_A_ProcessImagesTool.html))*  <br />
	i. Import mound images individually <br />
	ii. Follow the steps as directed within the web app<br />
	ii. Export table and save to CSV file with unique mound identifier as the name eg. 8046.csv <br />
**3. Run Part B: Post Processing Tool** - *(must be used locally, file is [PART_B_PostProcessingTool.xlsm](PART_B_PostProcessingTool.xlsm))*  <br />
	i. Ensure [macros are enabled](https://support.office.com/en-us/article/enable-or-disable-macros-in-office-files-12b036fd-d140-4e74-b45e-16fed1a7e5c6) in the spreadheet <br />
	ii. Follow instructions in tool to import and process data<br />
	iii. Use cylindrical shells method to estimate volume of mound. (TO BE ADDED IN SPREADSHEET VERY SOON)<br />

## To do list (functionality)
In priority order:

1. ~~Replace initial 4 clicks with popup prompts and add instruction and examples within the popups.~~ 16/09/18 Complete
2. Get the export to .csv function working consistantly - 16/09/18: inconsistantly working in some cases
3. ~~Get a photo upload function working properly (either automatically cycle through photos and save .CSV with the same name if mound photos have a unique ID or allow user to select photos individually and choose output name). Naming of photos will be fixed as part of this process.~~  16/09/18 Complete
4. Build all postprocessing data calculations for mound volume in (rather then relying on postprocessing data manually)<br />
	i. ~~Importing CSV en-mass import macro~~  16/09/18 Complete <br />
	ii ~~Populate data summary macro~~  16/09/18 Complete <br />
	iii. ~~Use Linest to calculate polynomial coefficients of a trendline of the xy data.~~ 18/09/18 Complete <br />
	iv. Use cylindrical shells method to estimate volume of mound. (TO BE ADDED IN SPREADSHEET VERY SOON) <br />
	iv ~~Refresh data macro~~  16/09/18 Complete <br />
	v. Erosion volume calculations to be added <br />

## To do list (testing)

1. ~~Check works with different browsers~~  16/09/18 Complete <br />
2. Do comparison test with mounds modelled from 0.5m or less LIDAR data so we can estimate margin of error. Calculate exact volume using GRASS.
3. ~~create test image for confirmation of output calibration~~ 18/09/18 Complete

## Built With

* [jquery](https://jquery.com/) - export to csv function

## License

Any code that I wrote within this repository is licenced under [GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/), refer to the [LICENSE.md](LICENSE.md) file for details. All sample photographs are have been sourced and licenced seperately from the [Tundzha Regional Archaeology Project](http://www.tundzha.org/). Out of interest, I would appreciate if you let me know what you are working on if you use this tool.

## Acknowledgments

* Built for data collected with [FAIMS](https://www.fedarch.org/about/) and for research undertaken as part of the [Tundzha Regional Archaeology Project](http://www.tundzha.org/)
