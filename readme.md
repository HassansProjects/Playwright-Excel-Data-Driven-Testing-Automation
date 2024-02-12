********* Playwright Excel Data-Driven Testing Automation ********

 This is a basic example of how to use the playwright library for data driven testing in excel. 

This is a test script written in JavaScript using the Playwright library for end-to-end testing. The test is designed to read data from an Excel file named "Computer_List.xlsx" and use that data to perform automated tests on a web page.

The script begins by loading the Excel file using the exceljs library and getting a reference to the first worksheet in the file. It then iterates over each row in the worksheet, starting from the second row (assuming the first row contains headers).

For each row, the script extracts the values of four columns: Computer_name, Introduced, Discontinued, and Company. It then uses Playwright to automate a web browser and perform the following steps:

Navigate to the URL "https://computer-database.gatling.io/computers".
Click on the "Add" button to open the computer creation form.
Fill in the form fields with the data extracted from the Excel sheet.
Submit the form.
Verify that a success message is displayed, indicating that the computer was added successfully.
The script uses the expect function from Playwright to check that the success message contains the name of the computer that was just added.

Overall, this script demonstrates how to use data-driven testing to automate repetitive tasks and ensure that the web application behaves correctly with a variety of input data.

***********************************************
URL:  https://computer-database.gatling.io/computers

        A               B           C               D
1-  Computer_name	Introduced	Discontinued	 Company
2-  Comouter001	    2024-02-11	2025-03-12	     Sony
3-  Comouter002	    2024-02-12	2025-03-13	     Nokia
4-  Comouter003	    2024-02-13	2025-03-14	     Canon
5-  Comouter004	    2024-02-14	2025-03-15	     Sony
6-  Comouter005	    2024-02-15	2025-03-16	     Nokia
7-  Comouter006	    2024-02-16	2025-03-17	     Canon
8-  Comouter007	    2024-02-17	2025-03-18	     Sony
9-  Comouter008	    2024-02-18	2025-03-19	     Nokia
10- Comouter009	    2024-02-19	2025-03-20	     Canon
11- Comouter010	    2024-02-20	2025-03-21	     Sony

