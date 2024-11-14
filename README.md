# font-compare-word-list

Simple browser tool for comparing two local fonts using a .txt file word list.

Shows each word in a cell, and shows the two fonts overlaid.

For more detailed view: https://github.com/MattMatic/hbfontcompare

## Live Demo
https://mattmatic.github.io/font-compare-word-list/

## Usage
- Drag a .txt file onto the "Word List" drag-and-drop site
	- File should be one word per line
- Drag each font onto the drag-and-drop heading sites
- Choose the text alignment with radio buttons
- Use the Prev / Next buttons to scroll through the word list
	- Prev = Alt-2
	- Next = Alt-3
- Type in a "Start" position and click "Go" to jump to a location

## CheckList Usage
After loading the word list...

- Drag a .txt file of words to the "CheckList" drag-and-drop site
	- For each word in the checklist file, the first matching word will be checked
	- Note: any checks already in place will be left
- Click "Download" to save a file `CheckList.YYYYMMDD_HHMMSS.txt` file with the words
- Click "Invert" to toggle all checkboxes
- Click "Delete Unchecked" to permanently remove words

## HarfBuzz addition
HarfBuzz is used to populate the "Diff" column.

HINT: Click on the "Diff" to show/hide the icon legends.

The Diff column will help you quickly identify differences in the HarfBuzz output between the two fonts.

- If the GIDs, cluster, advance, and offsets match you will see a green checkbox.
- If only the GIDs are different (because the font has auto assigned GIDs when building), this field will be blank.
- Other differences are shown with icons.

### Check Similar
The "Check Similar" button will iterate through all words in the list,
and check entries that are identical, or only have GID differences.

NOTE: This process is time consuming, and there will be a red progress update underneath the "Show Lang/Script" link at the bottom of the page.

You can then use "Invert" and "Delete Unchecked" to manage and prune the list.

### Sequences
To remove duplicates from a word list:

- Drag a word list .txt file to the Word List
- Drag the same word list .txt file to the CheckList
- Click "Delete Unchecked"


## Links
- https://github.com/danbovey/fontname
- https://minify-js.com/
- https://github.com/photopea/Typr.js/

