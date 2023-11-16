# Description
Very simple GUI software for interfacing with Local DB, Irrelevant for non employees since you wont be able to connect without being on the network or having credidentials.

# Log in
When launching the executable, you will encounter a login window that facilitates database connection. If you haven't received login credentials, please reach out to me, and I will provide the necessary information for program access. Kindly note that access to this program requires an existing user account in the database. Passwords are case-sensitive, and usernames are entered in all uppercase by default.

# Input window
On the top left you will see a small black window, this is the entry window.

<img width="199" alt="image" src="https://github.com/UIMlink/DB_GUI/assets/141648522/cfe15037-b2ce-4982-86dd-26829e49c699">

This is where you will put in ID's, Serial numbers, Building codes, Building names, etc.

This window also handles commands:

* '!awol' - this selects our awol report when this is put in and the "Awol Select" button is pressed.
* '!inv' - this selects our Inventory report when this is put in and the "Inventory Select" button is presed.
* '*' - This only works with the "Building code/abbr select" Button. This will just give you a whole list of the Buildings table.

# Buttons
These buttons serve as our "query builders" these will execute the queries for you to mass search serials, id's, etc

<img width="196" alt="image" src="https://github.com/UIMlink/DB_GUI/assets/141648522/0f102bbb-2dfe-4822-b959-8cd4bffcd99d">

-please note that eassets data is pulled every night at 1am, things can change through the day but this is pretty accurate otherwise.

* 'Inventory select' - This will check the serial numbers put into the input window and check them against our entire historics table, you should be able to see everything relating to that serial number that we touched. Once the button is pressed a pop up will will appear to edit the query, select the columns you want, or click the * at the top for everying and click search to get your results.
* 'Awol select' - This works the exact same as the inventory button except that it pulls from the historical awol table so you'll be able to see everything relating to each serial number if it exists within the table.
* 'essets cdsid select' - This will take every cdsid within the input window and search it against eassets data to pull each Id's employee type or employee email
* 'eassets serial select' - this will take every serial number within the input window and search it against the eassets data to pull all their eassets asset data.
* 'Building code/abbr select' - This ones unique, if you put in a building abbreviation it will give you its code, on the flip side of that if you put in a building code it will give you its corresponding building abbreviation.
* 'Export view to CSV' - This one is simple, it will take the current view within the program and put it into a CSV file that will go to your desktop.
* 'Manual SQL' - Possibly the most powerful portion of this program, you can craft your own query and pull any kind of data you would like, this is not limited at all and you can parse information incredibly well with this. once you write your query in the manual sql window press "CTRL-r" to run it. If there are errors the console will reflect it.

# Importing

* 'Import/AWOL Import CSV' - This button will import CSV files to the database of scans or updates, etc. You NEED to use the template that is in the files for this repository and fill in the columns since the information needs to be this way for the program to put it in. Please be sure that the correct information is in the correct fields and if you mess it up it may throw out errors.

# Console

<img width="899" alt="image" src="https://github.com/UIMlink/DB_GUI/assets/141648522/364635b7-2a84-4e1b-b3e3-f1285e1d5c61">

This is just to relfect errors or outcomes. It will tell you how many results were found and will also tell you errors in detail, also where your csv file is exported to which should be desktop by default. 

# view window

<img width="899" alt="image" src="https://github.com/UIMlink/DB_GUI/assets/141648522/fbe1b1af-3553-4cde-b4fd-5068824695a9">

This is the view window, this is where all your results will be shown. The headers at the top will be the database column names and everything under it will be the data in those columns corresponding to what was given in the entry box. This is the view i was refering to when talking about the export button. The export button will export this current view show in the program. The headers can sort some columns but there are bugs with non integer column headers. You cannot copy from this view either, this is another bug.
