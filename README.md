# Description
This simple yet efficient GUI software is designed for seamless interaction with our Local Database. It's tailored specifically for our team members, as external access is restricted without proper network connectivity and credentials.

# Log in
Upon initiating the software, users are greeted with a login interface, essential for establishing a connection with the database. If you haven't obtained your login details yet, please contact the system administrator to receive your credentials. Access is contingent upon having an established user account. Keep in mind that while usernames are auto-capitalized, passwords remain sensitive to case.

# Remember me
By clicking the option, your information will be saved for future use. This action creates a directory named 'serial_search_utility' within your Documents folder, containing an encrypted file with your details. If you choose to log out of your current user, a button located at the top left of the program will log you out and delete this file and prompt a new user to log in.

# Input window

<img width="199" alt="image" src="https://github.com/UIMlink/DB_GUI/assets/141648522/cfe15037-b2ce-4982-86dd-26829e49c699">

Positioned at the top left is the entry window, a compact, black interface for data input. This window is versatile, accepting various inputs such as IDs, serial numbers, building codes, and names. It also recognizes specific commands:

* '!awolreport' - this selects our awol report when this is put in and the "Awol Select" button is pressed.
* '!awolpivot' - This will give you the same report but will edit the dates to reflect better in excel pivot tables.
* '!inv' - this selects our Inventory report when this is put in and the "Inventory Select" button is presed.
* '*' - This only works with the "Building code/abbr select" Button. This will just give you a whole list of the Buildings table.

# Buttons

<img width="196" alt="image" src="https://github.com/UIMlink/DB_GUI/assets/141648522/0f102bbb-2dfe-4822-b959-8cd4bffcd99d">

The software features an array of buttons that act as intuitive query builders, facilitating bulk searches:

* Inventory Select - Cross-references serial numbers with our historical data, offering comprehensive details related to each number. A customizable query pop-up allows for specific data retrieval.
* Awol Select - Similar to the Inventory Select but pulls data from the historical AWOL table.
* Eassets CDSID Select - Searches employee types or emails by CDSID from the eassets data which will give manager emails/cdsids.
* Eassets Serial Select - Retrieves eassets asset data for entered serial numbers.
* Building Code/Abbr Select - Provides building codes or abbreviations based on the input.
* Export View to CSV - Exports the current program view to a CSV file on your desktop.
* Manual SQL - Offers advanced data querying capabilities. Write and execute custom SQL queries with CTRL-r. The console reflects errors or successful executions.

# Importing

* Import/AWOL Import CSV - Facilitates the importation of CSV files. It's crucial to adhere to the provided template for compatibility and error avoidance.

# Console

<img width="899" alt="image" src="https://github.com/UIMlink/DB_GUI/assets/141648522/364635b7-2a84-4e1b-b3e3-f1285e1d5c61">

The console serves as a feedback mechanism, displaying error messages, result counts, and CSV export locations.

# view window

<img width="899" alt="image" src="https://github.com/UIMlink/DB_GUI/assets/141648522/fbe1b1af-3553-4cde-b4fd-5068824695a9">

This primary window displays query results, with database column names as headers. Sorting functionality is available for some columns. However, note that there are known limitations with non-integer columns and the inability to copy data directly from this view.
