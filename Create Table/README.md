# Create Table

## Table of Contents
- Conntect SQL Server DB with Visual Studio
- SQL Script 

(之後可以將script的檔案直接上傳上來)

### Conntect SQL Server DB with Visual Studio
1. Open the Visual Studio 2019, choose "Continue without code ->"(不使用程式碼繼續).
![螢幕擷取畫面 2022-05-11 032934](https://user-images.githubusercontent.com/78516704/167707407-ead8e780-2991-4831-ab42-7f2d7652ff50.png)
2. Click "View"(檢視), and choose "Server Explorer"(伺服器總管).
![螢幕擷取畫面 2022-05-11 033156](https://user-images.githubusercontent.com/78516704/167707790-7ed26ed9-4ca7-4c43-987f-68bb128ebfff.png)
3. You can see the screenshot below. (PS you can click "Auto Hide" to pin the server manager)
![螢幕擷取畫面 2022-05-11 033926](https://user-images.githubusercontent.com/78516704/167708899-d1a5aee7-10c9-41f3-97e6-388868efc753.png)
4. Right click on "Data Connections", and choose "Add Connection...".
![螢幕擷取畫面 2022-05-11 034218](https://user-images.githubusercontent.com/78516704/167709712-1d523cee-91ae-41bb-b133-1d0588555cde.png)
5. In "Data Source" select "Microsoft SQL Server", uncheck "Always use this selection", and click "Continue".
![螢幕擷取畫面 2022-05-11 035059](https://user-images.githubusercontent.com/78516704/167710855-4870f737-22c1-48db-9eaa-8510db823e41.png)
6. Open Microsoft SQL Server Management Studio 18 and stay at the following screen.
![螢幕擷取畫面 2022-05-11 034725](https://user-images.githubusercontent.com/78516704/167711429-acbd0586-b54d-4fa6-8816-83746e46f2f2.png)
7. In Visual Studio 2019, you can see the screenshot below.
![螢幕擷取畫面 2022-05-11 035345](https://user-images.githubusercontent.com/78516704/167711130-e6661f9d-e75b-40e0-89bb-7313414b789d.png)
8. Enter the following corresponding to SQL server: "Server Name", "SQL Server Authentication", "User name" and "Password". 
![螢幕擷取畫面 2022-05-11 035918](https://user-images.githubusercontent.com/78516704/167712407-05b27a11-570b-4247-9172-751ab00d078d.png)
9. Connect to Database Server, right click on the "Databases", choose "New Database".
![螢幕擷取畫面 2022-05-11 040530](https://user-images.githubusercontent.com/78516704/167712851-7ad379a7-bf4e-423c-a2ae-b1837cceb40a.png)
10. Enter the "Database Name", and press "OK"
![螢幕擷取畫面 2022-05-11 040706](https://user-images.githubusercontent.com/78516704/167713129-02dc8e9e-c93d-47a5-a744-59698bd0f1ab.png)
11. Go back to Visual Studio 2019, in "Select or enter a database name",  choose the one you created earlier in SQL Server, and click "Test Connection", if it pops up the "Test connection succeeded.", then press "OK".
![螢幕擷取畫面 2022-05-11 041117](https://user-images.githubusercontent.com/78516704/167713840-00158464-0d40-4d06-921c-ed3e544f27b4.png)
12. If your screen like the following, your database connection is successful.
![螢幕擷取畫面 2022-05-11 043151](https://user-images.githubusercontent.com/78516704/167716854-b971e9aa-6af0-4bc4-ad53-fca0fdc4646a.png)
