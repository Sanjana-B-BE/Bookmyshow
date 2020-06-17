# BookMyShowHackathon
Display all the sports activities for coming weekend in your preferred location with lowest charges on top. Extract all the languages for movies and store it in a list. Display the list.
REFERENCE DOCUMENT

GROUP:  The Heathers
POC:  Sanjana. B (853076)
MODULES TO AUTOMATE:  BookMyShow - Events display
PROJECT NAME SELECTED:  BookMyShow Automation
GROUP MEMBERS:   
	Aafreen. R (853066)
	Aswini. R (853099)
	Pavithra. S (853023)
	Selina Joanna Peter (853119)


WORKFLOW:
For automating the module there will be methods to be automated.
For every stage to be automated, the method “initializeDriver” will be invoked, TestCases class and invalid credential classes will be called. Based on the parameters in each stage, whether the page is displayed or not is checked.
The parameters and the responses will be read from the uploaded requirements document uploaded by the POC and will be compared whether the pages displayed are the same as in the website.
   1.   Invoke the browser
   2.   Launch the website: https://bookmyshow.com/
   3.   Check if the main page title is same as the expected title
   4.   Select city
   5.   Close the popup
   6.   Click “Sign In” button
   7.   Click “Continue via Google”
   8.   Sign in with email ID and password
   9.   Click “Sports” column and select “Weekend” 
  10.   Select the minimum range from the “Price Range” dropdown box
  11.   Check if all the sports events for weekend are displayed with lowest charges on top
  12.   Navigate to “Movies” page
  13.   Click on “Coming Soon” and extract the languages 

PRE-REQUISITE FOR THE SCRIPT TO RUN:
	Include all the jar files of Selenium java, Apache poi, commons.io, ashot, logger
	Add TestNG library

STEPS TO PERFORM AUDIT:
1.	Select the applicable for InitializeDriver
2.	For the first parameter, city is selected
3.	The selected city is displayed
4.	Sign in action is performed
5.	For next parameter ,sports for weekend is selected
6.	Sports are displayed with lowest charges on top
7.	For next parameter, ”Coming Soon” is selected in “Movies” page
8.	The Movie languages are displayed    
      
SCRIPT DETAILS:
	Test Script Name: TestCases.java
	Methods Developed:
1.	Test_Browser_And_URL_Invoked_Correctly( )  
-	Checks if the driver is initiated for the browser
2.	Test_MainPage_Title_Matches_Correctly( )  
-	Checks if the actual and expected page title are the same
3.	Test_City_Is_Selected_Correctly( )  
-	Checks if the preferred city is selected 
4.	Test_Popup_Is_Ignored( )  
-	Ignores the notification pop up
5.	Test_Signin_Button_Is_clicked( )  
-	 To click the “Sign In” button
6.	Test_Continue_Via_Google_Button_Is_Clicked( )  
-	To click “Continue Via Google”
7.	Test_Signing_In_Appears_Correctly( ) 
-	 Checks whether the user is signed in
8.	Test_Sports_Is_Clicked( )  
-	To check if the “Sports” column is clicked
9.	Test_Sports_Available_Are_Displayed( )  
-	To display all the available sports
10.	Test_Weekend_Is_clicked( )    
-	To select the “Weekend” option
11.	Test_Sports_Availabe_Are_Displayed_After_Selecting_Weekend( ) 
-	To display the available sports for the weekend
12.	Test_PriceRange_Is_clicked( )  
-	To click the “Price Range” dropdown box
13.	Test_Minimum_Is_clicked( )  
-	 To select the minimum price range
14.	Test_Sports_Available_Are_Displayed_After_Selecting_MinimumRange( )  
-	 To check the weekend sports with the lowest charges are displayed
15.	Test_Window_Navigates_To_Movie_Page( )  -
-	 To navigate to the “Movies” page
16.	Test_Movies_Are_Displayed( )  
-	To check whether the movies are displayed
17.	Test_Languages_Are_Extracted_And_Stored_In_List( )  
-	 To extract the languages and store in a list
18.	Test_Languages_Are_Displayed( )  
-	 To display the movie languages
19.	exit( )  
-	To close the workbook and the driver


CLASS DETAILS:
	InitializeDriver - package setup
	TestData - package excel 
	ImportFromExcel - package excel 
	ExcelWrite - package excel
	WriteDataToExcelUsingUtilClass - package excel
	HomePage - package pageObjects 
	SportsPage - package pageObjects
	MoviesPage - package  pageObjects
	DateUtils - package extentReport 
	ExtentReporterNG - package extentReport 
	ActualValues - package testcases 
	TestCases - package testcases 
	InvalidUsername - package invalidtests
	Invalidpassword - package invalidtests
	BlankUsername - package invalidtests
	Emptypassword - package invalidtests
	SmokeTesting - package smoketesting

DATA TABLE EXCEL DETAILS:
	Excel file is located in the ‘Excelsheet’ folder in the ‘BookMyShowHackathon’ project.
