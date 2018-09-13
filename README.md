# burial-mound-volume-tool

Tool to aid estimation of burial mound volume based on photographs.

### Installing and running

Steps to get running:

1. Download repository.
2. Copy one image of a mound into the root directory and rename it 1.jpg
3. Click on index.html
4. Process mound through the following steps:
	i. Type in height of human scale
	ii. Click no. 1 on feet of scale person
	iii. Click no. 2 on head of scale person
	iv. Click no. 3 on the centreline of the mound (to set x=0 to middle of mound)
	v. Click no. 4 somewhere along ground level (to set y=0 to base of mound)
	vi. Click a further 20 times along the curved surface of the mound. Start from the left and move to the right. This will automatically take you to the created table once all 20 clicks are done.
	vii. Review table to ensure it looks correct.
	viii. Either copy and paste table into excel or select the export to CSV button (currently not working in some cases)
5. Repeat process with each mount.

## To do list (functionality)
In priority order:

1. Get the export to .csv function working consistantly
2. Get a photo upload function working properly (either automatically cycle through photos and save .CSV with the same name if mound photos have a unique ID or allow user to select photos individually and choose output name)

## To do list (testing)

1. Check works with different browsers

## Built With

* [jquery](https://jquery.com/) - export to csv function

## License

See the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Built for research undertaken as part of the [Tundzha Regional Archaeology Project](https://www.fedarch.org/about/)
