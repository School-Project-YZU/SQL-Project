# ERD Of operating income and collection cycle
(後面可以再放圖)

(1) Sales order file: Bill of lading file (1:m): Indicates that an order can be shipped several times.   
(2) Bill of Lading File: Invoice file (1:1): Indicates that an invoice is issued for a bill of lading.   
(3) Invoice file: Remittance single file (1:1): Indicates that if an invoice is issued, a remittance or information will be received.   
(4) Customer file: sales order file (1:m): Indicates that a customer can place multiple orders.   
(5) Invoice document: customer document (m; 1): Indicates that a customer can receive several invoices. 
(6) Remittance single file: customer file (m:1): Indicates that multiple payments can be received from the same customer.   
(7) Sales order file: Personnel file (m:1): Indicates that an employee can be responsible for multiple sales.   
(8) Bill of Lading File: Personnel document (m:1): Indicates that an employee can be responsible for multiple shipments.   
(9) Bill of Lading File: Carrier Document (m1): Indicates that a transport company can be responsible for multiple shipments.   
(10) Remittance single file personnel file (m:1): Indicates that an employee can be responsible for processing multiple collections.   
(11) Remittance file: Account file (m:1): Indicates that multiple payments can be stored in the same account.   
(12) Sales order file: sales order detail file (1:m): indicates that a sales order can order several kinds of inventory.   
(13) Sales Order Details: Inventory File (m:1): Indicates that each type of inventory can be ordered by other different orders.   
(14) Account file: Bank file (m:1): Indicates that there are multiple accounts in the same bank.   
(15) Personnel file: Department file (m:1): Indicates that a department has multiple employees.    


![image](https://github.com/Annie0727/Pictures/blob/main/SQL01.jpg)
![image](https://github.com/Annie0727/Pictures/blob/main/SQL02.jpg)
![image](https://github.com/Annie0727/Pictures/blob/main/SQL03.jpg)
![image](https://github.com/Annie0727/Pictures/blob/main/SQL04.jpg)
![image](https://github.com/Annie0727/Pictures/blob/main/SQL05.jpg)
![image](https://github.com/Annie0727/Pictures/blob/main/SQL06.jpg)
![image](https://github.com/Annie0727/Pictures/blob/main/SQL07.jpg)

