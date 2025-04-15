# dosa-orders
A repository created to help better keep track of individual orders received from a Dosa restaurant, containing the customers name, phone number, and their orders.
 
Using the code provided in the is601 file, the company will be able to provide a copy of the individual orders that they have received over time in a JSON file, and get out two additional JSON files. 
- The first file contains information about their customers (phone number and first name - assuming there is only one name associated with the provided phone number).
- The second file contains information about what items have been ordered, the price for one of that item, and how many times that item has been ordered over time. 

> **The project is designed as follows:**
<pre>  - Establishing a class called "JSONFile" that takes in 3 parameters - the original file containing the compiled data for individual orders, the name of the file that the user wants created containing the customer information (in this case it is called customers.json), and the name of the file that the user would like to hold the information about their orders (here it is called items.json)
  - The data is declared as an empty list so that it can be loaded from the JSON file.
  - The JSON file is located, and the individual orders are loaded into Python (read from the file)
  - The customer file is then created, taking the phone number and name of the customer as strings from the original JSON file and loading them into a dictionary. The phone numbers are in the format ###-###-####.
  - Next, the item file is created using the order information from the original JSON file which stores each item as a dictionary where the key is the item name and the value is the item price and number of times it has been ordered.
  - Finally, the program is run through the starting point - main - containing the arseparse module components to provide a description of the program to the user, along with help functions to understand what each file does. The main function will print each file name so that the user knows what files they now have access to - specifically if the original file was able to be accessed and that the two new files have been successfully written.
  
</pre> 
> **Instructions on how to use:**
<pre>  - Insert the name of the program into the command line (here it would be is601.py)
  - Insert the name of the original JSON file containing the individual orders using a space after the program name
  - Insert the name of the customer file you want to create (here it is customers.json) using space after original file name
  - Insert the name of the item file you want to create (here it is items.json) using a space after the customer file
  - You should then be able to run the program at the command line and view if the each file has been successfully read or written
</pre>
    
