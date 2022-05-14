# ERD of Operating Income And Collection Cycle

(1) Sales Order : Bill of Lading (1:m): Indicates that an order can be shipped several times.   

(2) Bill of Lading : Invoice (1:1): Indicates that an invoice is issued for a bill of lading.   

(3) Invoice : Remittance Single (1:1): Indicates that if an invoice is issued, a remittance or information will be received.   

(4) Customer : Sales Order (1:m): Indicates that a customer can place multiple orders.   

(5) Invoice : Customer (m: 1): Indicates that a customer can receive several invoices. 

(6) Remittance Single : Customer (m:1): Indicates that multiple payments can be received from the same customer.   

(7) Sales Order : Personnel (m:1): Indicates that an employee can be responsible for multiple sales.   

(8) Bill of Lading : Personnel (m:1): Indicates that an employee can be responsible for multiple shipments.   

(9) Bill of Lading : Carrier  (m:1): Indicates that a transport company can be responsible for multiple shipments.   

(10) Remittance Single : Personnel (m:1): Indicates that an employee can be responsible for processing multiple collections.   

(11) Remittance Single : Account (m:1): Indicates that multiple payments can be stored in the same account.   

(12) Sales Order : Sales Order Details (1:m): indicates that a sales order can order several kinds of inventory.   

(13) Sales Order Details : Inventory (m:1): Indicates that each type of inventory can be ordered by other different orders.   

(14) Account : Bank (m:1): Indicates that there are multiple accounts in the same bank.   

(15) Personnel : Department (m:1): Indicates that a department has multiple employees.    


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



### Table-Sales Order 

|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Order Number            | ORD_NUM       |
| 2. | Date                    | ORD_DATE      |
| 3. | Customer Number         | CUS_ID        |
| 4. | Salesperson Number      | EMP_NUM       |
| 5. | Transaction Conditions  | ORD_TC        |


### Table-Sales Order Details 

|    | Attributes              | Abbreviation      | 
| -- | --------                | --------          | 
| 1. | Order Number            | ORD_NUM           |
| 2. | Inventory Number        | INV_ID            |
| 3. | Quantity                | ORD_LINE_QUANTITY |
| 4. | Amount                  | ORD_LINE_AMOUNT   |


### Table-Bill of Lading

|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Bill of Lading Number   | LAD_NUM       |
| 2. | Shipping Company Number | SHIP_ID       |
| 3. | Order Number            | ORD_NUM       |
| 4. | Shipping Person Number  | EMP_NUM       |
| 5. | Date                    | LAD_DATE      |


### Table-Sales Invoice

|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Invoice Number          | INV_NUM       |
| 2. | Date                    | INV_DATE      |
| 3. | Customer Number         | CUS_ID        |
| 4. | Bill of Lading Number   | LAD_NUM       |

### Table-Remittance single 

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

### Table-Personnel

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

|    | Attributes              | Abbreviation  | 
| -- | --------                | --------      | 
| 1. | Department Number       | DEPT_NUM      |
| 2. | Department Name         | DEPT_NAME     |

# Reference
- https://hackmd.io/xgpPIzO-QH20hdJwDXp-gg
