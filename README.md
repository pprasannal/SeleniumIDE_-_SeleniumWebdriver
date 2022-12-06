# SeleniumIDE_-_SeleniumWebdriver

I.	instructions to install the chosen web application  :-
1. open xampp in between 7.0 to 7.3.17 version,
2. open http://localhost/80(port number)/ (to check weather it working or not),
3. open http://localhost/project holder name(orangehrm)/ (which use to open the saved project in the xampp/htdocs/(project folder)),
4. during setup id:Admin, passwd:AdminUser@12345,
5. after set up is done

II.	how to open the project :-
1. open xampp run apache and mysql,
2. open browser and use this url to open project http://localhost/orangehrm/orangehrm-4.4/symfony/web/index.php/auth/login 

III.	list of test cases :-

1. Invalid login credentials :- to check does it login page or not and test invalid login credential
•	Steps – check login header page , give the input data , and last check for span message
•	Input data – login, password 
•	Click () – submit button in login page 
•	Assertion – login header , username cannot be empty (span message)

2. Login page (duplicate test class for all test cases) :- to test correct login credential and made this is as default class for all test cases
•	Steps – check login header , give the input data and at last to check the next(home) page header
•	Input data – login, password
•	Click () – submit button in login page 
•	Assertion – home page header(title)  

3. Home page :- to check does login page goes to home page or not 
•	Steps – we give the input data in login page and check does it reach to home page or not  and last from home page go to the user page 
•	Input data – login, password
•	Click () – submit button in login page, admin, user 
•	Assertion – check login header   

4. Go to employee page :- to test employee page after login page reaches to home page , in this we create a duplicate class for continues click action
•	Steps – create duplicate class for click button , then use of login page check the home page header and last if the assertion correct goes to employee page 
•	Input – login, password 
•	Click () – submit button In login page , PIM , add employee go to duplicate class for click action
•	Assertion – check home page header  

5. Go To Add New User Page In User page :- to check does user page reach to new user page or not 
•	Steps – we use login page class and then then later we use implement home page to check does it add user reached to next page or not 
•	Input data – same as login page and home page 
•	Click () – same as login and home page 
•	Assertion – same as login and home page and here we check does user reach to next page or not 

6. Add New User Details :- to test correct details given in correct locators and check the does it giving details in correct page or not 
•	Steps – we use similar to previous one but in this after assertion is done for user page we give set of input data in the present page 
•	Input data – same as previous class , name of employee, user name , password , confirm password
•	Click () – same as previous class , save for the given details
•	Assertion – same as previous class 

7. Add Immigration Details :- to check and search employee is present or not in page
•	Steps – same as login page , go to immigration page in info page, add the immigration details, give input data, and check the details saved message
•	Input data – same as login page , immigration number
•	Click () – same as login page , info, immigration page, add immigration, and save the details 
•	Assertion – assert element present (check the saved message to display) 

8. Go To Recruitment page :- to test recruitment page after login credentials 
•	Steps – same as login page and go to recruitment page
•	Input data – same as login page 
•	Click () – recruitment page  

9. Go To Qualification page :-  to check does it reach qualification page or not through assertions
•	Steps – same as login page , go to info page and qualification page in info page , check the page if its in correct page or not
•	Input data – same as login page 
•	Click () – info page, qualification page in info page 
•	Assertion – assert text , assert element present , wait for element visible, wait for element present , assert element not present (all the elements is present or not )  

10. Go To Info page :- to check does it reach to info page or not after login credentials correct
•	Steps – same as login page and go to info page and check the info page header in info page or not
•	Input data – same as login page
•	Click () – info page 
•	Assertion – check the info page header(title)

11. Go To Immigration page :-  to check does it reach to immigration page or not after login credentials 
•	Steps – After login page, go to immigration in info page and check des it reach to immigration page or not 
•	Input data – login credentials
•	Click () – info , immigration page
•	Assertion – assert element present or not in immigration header(title)

12. Go To Employee time sheets :- to check does it reach to employee time sheets or not 
•	Steps – login credentials, after login is success go to time sheets and check does it in time sheets page or not 
•	Input data – same as login credentials 
•	Click () – time sheets 
•	Assertion – check assert element present or not in time  sheets header(title)

13. Go To Emergency Details :- to check the emergency page does it reached or not 
•	Steps – same as login page , go to info page and go to emergency contacts in person details 
•	Input data – same login incidentals
•	Click () – info, emergency contacts 
•	Assertion – assert element present or not after going to emergency page

14. Go To Directory page :- to check the directory page does it reached  or not 
•	Steps – same as login page , go to directory page and check does it reached or not  
•	Input data – same login incidentals
•	Click () – directory page
•	Assertion – assert element present (check does the reached to directory page or not)

15. Go To Dependency page :- to check dependency page does it reached to that page or not 
•	Steps – same as login page , go to info page and go to dependents in personal details page
•	Input data – same login incidentals
•	Click () – info, dependents
•	Assertion – assert element present (check dependency header element )

16. Go To contact details :- to check the contact details page does it reached or not 
•	Steps – same as login page , go to info page and go to contact details in person details page
•	Input data – same login incidentals
•	Click () – info, contacts details 
•	Assertion – assert element present (check contact details page header title)

17. Edit details in info page :- to test the personal details in info page with correct locator and check personal details page header 
•	Steps – same as login page, go to info page and check person details header and edit the present details with new details using correct locators  
•	Input data – same login incidentals, first name, middle name, last name , personal id , other id , license , expire date , martial status, nationality, dob 
•	Click () – info, edit the data, choose the correct date for dob and save the new details
•	Assertion – assert element present (check the personal details title)

18. Delete immigration details :- to test and check the delete element is not present 
•	Steps – same as login page, go to info page and select the immigration and check the immigration page header, click on one in list and delete it , check does it get deleted message or not 
•	Input data – same as login details
•	Click () – info , immigration , choose one from the list , delete the chosen one
•	Assertion – assert element present (check the immigration page title , check the successfully deleted message)

19. Delete Emergence contacts :- to test the selected element is deleted or not 
•	Steps – same as login page, go to info page and select the emergency and check the emergency page header, click on one in list and delete it  
•	Input data – same as login details
•	Click () – info , emergency , choose one from the list , delete the chosen one
•	Assertion – assert element present (check the emergency page title)

20. Delete dependency details :- to test and check the delete element is not present
•	Steps – same as login page, go to info page and select the dependent and check the dependence page header, click on one in list and delete it , check does it get deleted message or not 
•	Input data – same as login details
•	Click () – info , dependency , choose one from the list , delete the chosen one
•	Assertion – assert element present (check the dependency page title , check the successfully deleted message)

21. Add Work Experience Details :- to test the work experience details in info page with correct locator and check Add work experience title
•	Steps – same as login page, go to qualification page in info, add work experience in work experience header content and check work experience header and give input data in content and save the new details  
•	Input data – same login in credentials, employee name, job title , from date, to date  
•	Click () – info, qualification,  work experience , choose the correct from date, choose the correct to date from calendar and save the new details 
•	Assertion – assert element present (check the add work experience title)

22. Add Post :- to test and check the given post is updated in list or not  
•	Steps – same as login page, go to buzz page , type the text to be uploaded and post it, check the post is uploaded or not   
•	Input data – same login in credentials, type the post  
•	Click () – buzz page , upload the post
•	Assertion – assert element present (check the uploaded post)

23. Add Nationality :- to test the given nationality is in correct locator which we give and check span message if already exits and check the nationality
•	Steps – same as login page, go to nationality page in admin, add nationality and wait for span element present  , layer add new nationality and check that nationality doesn’t give span message   
•	Input data – same login in credentials, nationality name   
•	Click () – admin, nationality , save the nationality 
•	Assertion – assert element present (check nationality name), and wait for element visible (check for span message)

24. Add emergency Details :- to test the emergency contact details is in correct locator and check Add emergency contact header
•	Steps – same as login page, go to emergency contacts page in info, add emergency contacts in emergency contacts page and check emergency contact header and give input data in emergency contacts and save the new details  
•	Input data – same login in credentials,   name, relationship name, phone1, phone 2, phone 3 numbers
•	Click () – info, emergency contacts,  add contacts ,and save the new emergency contact details 
•	Assertion – assert element present (check the Add emergency contacts title)

25. Add Dependency Details :- to test the dependency details in info page with correct locator and check Add dependency title
•	Steps – same as login page, go to dependency page in info, add dependency in dependency page and check dependency header and give input data in content and save the new details  
•	Input data – same login in credentials, dependency name, relationship , type other relationship , dob   
•	Click () – info, dependency , add dependency , choose the correct date for dob, and save the new details 
•	Assertion – assert element present (check the add dependency title)

26. Add Contact Details :- to test the contact details in info page with correct locator and check contact details header name
•	Steps – same as login page, go to contacts page in info, check contacts header and click add contacts and give input data in content and save the new details  
•	Input data – same login in credentials, street1, street2 name , city name , telephone , mobile , telephone2, email id, other email id
•	Click () – info, contacts, add contacts , save the new contact details
•	Assertion – assert element present (check the contacts header title)

27. Add Candidate Details :- to test the candidate details in recruitment page with correct locator and check recruitment title , check successfully saved messaged and give input data
•	Steps – same as login page, go to recruitment page and add candidates, check candidates header , give input data and save the new input data , check the elements saved or not(through message)  
•	Input data – same login in credentials, first name, middle name, last name , mail id , contact no   
•	Click () – recruitment , add candidates , keep the data, save the details  
•	Assertion – assert element present (check the add candidates title, check saved message )
