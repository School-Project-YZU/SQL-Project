# ERD of Operating Income And Collection Cycle

(1) Sales Order : Bill of Lading (1:m): Indicates that an order can be shipped several times.   

(2) Bill of Lading : Invoice (1:1): Indicates that an invoice is issued for a bill of lading.   

(3) Invoice : Remittance Single (1:1): Indicates that if an invoice is issued, a remittance or information will be received.   

(4) Customer : Sales Order (1:m): Indicates that a customer can place multiple orders.   

(5) Invoice : Customer (m:1): Indicates that a customer can receive several invoices. 

(6) Remittance Single : Customer (m:1): Indicates that multiple payments can be received from the same customer.   

(7) Sales Order : Employee (m:1): Indicates that an employee can be responsible for multiple sales.   

(8) Bill of Lading : Employee (m:1): Indicates that an employee can be responsible for multiple shipments.   

(9) Bill of Lading : Shipping Company  (m:1): Indicates that a transport company can be responsible for multiple shipments.   

(10) Remittance Single : Employee (m:1): Indicates that an employee can be responsible for processing multiple collections.   

(11) Remittance Single : Account (m:1): Indicates that multiple payments can be stored in the same account.   

(12) Sales Order : Order Line (1:m): indicates that a sales order can order several kinds of inventory.   

(13) Order Line : Inventory (m:1): Indicates that each type of inventory can be ordered by other different orders.   

(14) Account : Bank (m:1): Indicates that there are multiple accounts in the same bank.   

(15) Employee : Department (m:1): Indicates that a department has multiple employees.    

(16) Inventory: Vendor (m:n): Indicates that one inventory can be provided by multiple vendors, and one vendor can also provide multiple inventories. 

(17) Inventory : Warehouse (m:1): Indicates that the company has only one warehouse, and this warehouse stores a variety of inventory.  

(18) Warehouse : Employee (1:m): Indicates that the warehouse is managed by multiple company employees.  



### Table-Inventory

|    | Attributes           | Abbreviation  | 
| -- | --------             | --------      | 
| 1. | Inventory Number     | INVT_ID       |
| 2. | Inventory Name       | INVT_NAME     |
| 3. | Quantity On Hand     | INVT_QOH      |
| 4. | Reorder Point        | INVT_RP       |
| 5. | Standard Cost        | INVT_SC       |
| 6. | Reorder Quantity     | INVT_RQ       |
| 7. | Manufacturer Number  | MFR_ID        |
| 8. | Warehouse Number     | WHSE_ID       |



### Table-Vendor

|    | Attributes            | Abbreviation  | 
| -- | --------              | --------      | 
| 1. | Vendor Number         | VEN_ID        |
| 2. | Vendor Name           | VEN_NAME      |
| 3. | Telephone             | VEN_PHONE     |
| 4. | Fax                   | VEN_FAX       |
| 5. | E-MAIL                | VEN_MAIL      |
| 6. | Person in Charge Ship | VEN_IC        |



### Table-Warehouse

|    | Attributes            | Abbreviation  | 
| -- | --------              | --------      | 
| 1. | Warehouse number      | WAR_NUM       |
| 2. | Warehouse address     | WAR_ADDRES    |
| 3. | Telephone             | WAR_PHONE     |
| 4. | Employee Number       | EMP_NUM       |



### Table-Sales-Order 
![螢幕擷取畫面 2022-05-15 112650](https://user-images.githubusercontent.com/78516704/168456076-8b3b90de-d35d-49b4-b797-375c87375dba.png)


|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Order Number            | ORD_NUM       |
| 2. | Date                    | ORD_DATE      |
| 3. | Customer Number         | CUS_ID        |
| 4. | Salesperson Number      | EMP_NUM       |
| 5. | Transaction Conditions  | ORD_TC        |


### Table-Sales-Order-Line

|    | Attributes              | Abbreviation      | 
| -- | --------                | --------          | 
| 1. | Order Number            | ORD_NUM           |
| 2. | Inventory Number        | INV_ID            |
| 3. | Quantity                | ORD_LINE_QUANTITY |
| 4. | Amount                  | ORD_LINE_AMOUNT   |


### Table-Bill-of-Lading
![螢幕擷取畫面 2022-05-15 112132](https://user-images.githubusercontent.com/78516704/168456085-62bdd294-d41a-4682-8bb0-4220c57200fa.png)

|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Bill of Lading Number   | LAD_NUM       |
| 2. | Shipping Company Number | SHIP_ID       |
| 3. | Order Number            | ORD_NUM       |
| 4. | Shipping Person Number  | EMP_NUM       |
| 5. | Date                    | LAD_DATE      |


### Table-Invoice

|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Invoice Number          | INV_NUM       |
| 2. | Date                    | INV_DATE      |
| 3. | Invoice Amount          | INV_AMOUNT    |
| 4. | Customer Number         | CUS_ID        |
| 5. | Bill of Lading Number   | LAD_NUM       |

### Table-Remittance-Single 
![螢幕擷取畫面 2022-05-15 112753](https://user-images.githubusercontent.com/78516704/168456100-ee2b21c9-bd79-4e95-9d17-bbcfa2f223fe.png)

|    | Attributes           | Abbreviation  | 
| -- | --------             | --------      | 
| 1. | Money Order Number   | REM_NUM       |
| 2. | Date                 | REM_DATE      |
| 3. | Amount               | REM_AMOUNT    |
| 4. | Customer Number      | CUS_ID        |
| 5. | Invoice Number       | INV_NUM       |
| 6. | Account Number       | ACCT_NUM      |

### Table-Account
|    | Attributes           | Abbreviation  | 
| -- | --------             | --------      | 
| 1. | Account Number       | ACCT_NUM      |
| 2. | Bank Code            | BANK_CODE     |
| 3. | Balance              | ACCT_BALANCE  |

### Table-Customer
![螢幕擷取畫面 2022-05-15 112843](https://user-images.githubusercontent.com/78516704/168456104-7dde091a-48d4-430b-865b-09141635eda3.png)


|    | Attributes            | Abbreviation  | 
| -- | --------              | --------      | 
| 1. | Customer Number       | CUS_ID        |
| 2. | Customer Name         | CUS_NAME      |
| 3. | Billing Address       | CUS_BA        |
| 4. | Shipping Address      | CUS_SA        |
| 5. | Credit Rating         | CUS_CR        |
| 6. | Telephone             | CUS_PHONE     |
| 7. | Fax                   | CUS_FAX       |
| 8. | E-MAIL                | CUS_MAIL      |
| 9. | Person in Charge Ship | CUS_IC        |

### Table-Shipping Company

|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Shipping Company Number | SHIP_ID       |
| 2. |  Name                   | SHIP_NAME     |
| 3. | Address                 | SHIP_ADDRESS  |
| 4. | Telephone               | SHIP_PHONE    |
| 5. | Fax                     | SHIP_FAX      |
| 6. | E-MAIL                  | SHIP_MAIL     |
| 7. | Responsible Person      | SHIP_RP       |

### Table-Employee
![螢幕擷取畫面 2022-05-15 112950](https://user-images.githubusercontent.com/78516704/168456107-57c21261-c412-451d-a205-61a10d64ea9b.png)

|    | Attributes              | Abbreviation   | 
| -- | --------                | --------       | 
| 1. | Employee Number         | EMP_NUM        |
| 2. | Employee Name           | EMP_NAME       |
| 3. | Department Number       | EMP_DEP_NUM    |
| 3. | Date of Employment      | EMP_HIRE_DATE  |
| 4. | Telephone               | EMP_PHONE      |
| 5. | Identity Card Number    | EMP_ID         |
| 6. | E-MAIL                  | EMP_MAIL       |
| 7. | Gender                  | EMP_GENDER     |
| 8. | Birthday                | EMP_BIRTHDAY   |
| 9. | Address                 | EMP_ADDRESS    |


### Table-Bank

|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Bank Code               | BANK_CODE     |
| 2. | Bank Name               | BANK_NAME     |
| 3. | Telephone               | BANK_PHONE    |
| 4. | Address                 | BANK_ADDRESS  |


### Table-Department
![螢幕擷取畫面 2022-05-15 112926](https://user-images.githubusercontent.com/78516704/168456113-c2087dc3-54c1-4dc3-a410-869a4a4bc479.png)

|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Department Number       | DEPT_NUM      |
| 2. | Department Name         | DEPT_NAME     |

# Reference
- https://hackmd.io/xgpPIzO-QH20hdJwDXp-gg
