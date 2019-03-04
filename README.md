# Inventory_Parser

For this question, I have made the following assumptions:
1. Let us assume that the inventory details of all products for a particular supplier is stored in a directory. Consider a directory supplyHouseInventoryDetails. The structure of this directory will be as follows: there will be sub-directories inside this main directory, each such sub directory will be named as the supplierName. Inside this suplierName sub directory, we will have a file that will contain the inventory details of all the products that it has.


2. Now this file can have  many formats, such as xml, csv, tab seperated or Excel sheets. So we can have a parent fileReader class that will contain all the parsing logic and decisions whether to update the product record for that supplier or create product record for that supplier. Now if we determined the file to be of type csv then we can create and call a new class called fileReaderForCSV that will extend the basic fileReader class.

3. So this are the classes we need: the parent fileReader class, child classes like fileReaderForCSV (which parses the CSV files); fileReaderForXML (which parses the XML files); fileReaderForTabDelimited (which parses the tab delimited files) etc. All these 3 classes will inherit the fileReader Class. We also need a main class which will be the entry point of our app.

