# InventoryManagement
A concise IMS project by Sourav Sen
Functionalities added:
1) Intially a 'records' dictionary has been created where details of 30 items already present in a shop are kept. Next a code to add a new item to the inventory(if needed)
 is also added.
2) Next a code to print all the contents of the 'records' dictionary is written along with a code to check the details of a specific item if the user wants.
3) json module is imported and the entire dictionary is converted into text format and stored inside the record.json file.
4) Next, to do operations on it, the file is again opened and the entire data is  converted back to dictionary format and stored in 'record' variable.
5) Then a separate dictionary to keep track of the no. of items sold is also created and all its values are intialized with 0, since initially, nothing has been sold.
6) Then the main code of the system is written which deals with the order per customer:
7) Firstly, the program asks how many items the customer wants to buy. Upon entering the required data, the loop runs for that many no of times, and inside the loop 
   firstly the customer is asked which item he would like to buy and how many items of that particular product he would like to buy. As per the no. of items the user 
   inputs, the cost of that many items is generated. If the customer wants to buy a larger quantity than what is  currently available in stock, then an error message would
   be thrown.
8) Also depending on the no. of items the user buys, the available stock for that particular product is reduced by that many times in the 'record' dictionary and similarly
   updated by the same amount in the record_sales dictionary.
9) After the user has finished buying all the products, the total bill is generated.
10) The updated record dictionary is then again written back into the record.json file using the json.dumps() function and the updated record_sales dictionary is also
   written into a new sales.json file .
11) Contents of both the files are then printed for more clarity.

(P.S : The code written inside the ipynb file has been run only once since only one customer has been considerd for demonstration and accordingly the sales and records files
   are also similarly updated for the inputs by that one user only. For more customer orders and for the subsequent days, the code shall be run over and over again and the   contents of the files will be similarly updated.)
 
