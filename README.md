#Readme File
1. First tab

The first tab, there are a number of boxes. If you press "add", you will add a box (predefined is black). The color is black, unless you state otherwise in the second tab. You can see a counter at the bottom.

2. Second tab

This view has a preview of the selected color's box. You can change the color here. The selected color has the description under it. If you create a new box, and you selected a color the box created will have the seleted color.

3. Third tab

Third screen is details view for the other screens. 

** It stores the session, so if the tab is refreshed it keeps all the data. Since I am using JSON, it is a pre-step to store it in a local/remote DB.


## Usage
index.html
json3.js
main.css

## Resources
Learning: for learning resources
ResearchAssignment.rtf on the problem: research on the problem

## Functions

###Add a box
addDiv()
 - update()
###Remove a box
removeDiv
- update()


### Called on document ready:
Select Box Callback (listen to click events)
Select Color Button (listen to click events)
getDataStorageSession();

###Select a Box Callback
on document ready
$('body').on('click', '.box', function() {
- update


###Select a Color Button
on document.ready
$('body').on('click', '.button', function()
 -  update();
 
###Update status of the program
update()
- setDataStorageSession()
- getColorName

### Handle StorageSesson
getDatatoStoreSession
- makeStruct()

setDataStorageSession
- makestruct
###Other
setColorToId()
getColorName()


##Future considerations:

1. The global variable (gcolor) can be elimitated, just by using the SelectedColorButton, which should be always initialized.


2. Session is stored, i.d. if the browser/tab is refreshed then results are still kept. The variables are stored in JSON. Same files could be used to store this data in a local/remote database with CouchDB or MongoDB (NoSQL DB).