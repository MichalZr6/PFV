# PFV
Invoice Manager with Excel Database

I started this project as some help with my company accounting.
Every received invoice or document is scanned. The invoice information is stored in excel 'database'.
The PFV tasks: 
- loading scanned files from FV folder
- reading UI files' info such as company name, invoice id, date, prices, etc.
- spliting invoice if it relates to more than one investition
- generating prices in terms of given tax
- calculating prices if user types some simple math expression
- generating merged 'database' xls file with PFV records
- renaming all scanned files to a user defined name (when it's not invoice file) or to auto-generated, based on invoice id and company name.

I've tried many different programming platforms before. and this time wanted to test Visual Studio.
It quickly turned out however, that pure c++ coding in VS requires some special efforts.
Despite this, the program's code grew larger in time.


Some important notes:
- BasicExcel.hpp is rather old but works fine with this project
- PFV generates new excel file for merged 1000 (defined in Globals.h) old and new entries
- some features are not yet implemented (i.a. main menu)

Future tasks:
- saving user input as backup every entry read
- adding functionality to edit chosen entry (currently UI only allows user to delete last entry)

- implementing SQL database instead of XLS file
- implementing 'Company Storage'
