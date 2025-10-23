Hi there 👋
I’m passionate about ensuring product quality and delivering smooth user experiences. Recently completed QA courses at EPAM and Beetroot Academy, where I gained hands-on experience with:

🧩 Functional, UI/UX & Exploratory Testing, manual testing of Web and Mobile applications.
🔍 Working with SQL, Jira, and DevTools. 🔍 API Testing (Postman, Swagger)
🐞 Bug tracking (Jira, TestRail) 🌱 Currently exploring new tools and QA practices to grow as a professional.

# Testing of the Citrus website

```
Checklist
```

**Main page**

1.Check that the main menu has sections: smartphones, Apple, kitchen appliances, home appliances, personal transport, TVs and multimedia, laptops, tablets - pass

2.Check that the "smartphones" button takes you to the smartphones section - pass

3.Verify that the "Apple" button takes you to the Apple products section - pass

4.Check that the "kitchen appliances" button takes you to the kitchen appliances section - pass

5.Check that the "home appliances" button takes you to the home appliances section - pass

6.Check that the "personal transport" button opens the category with personal transport - pass

7.Check that the "TVs and Multimedia" button opens the TVs and Multimedia category - pass

8.Check that the "laptops, tablets, MFPs" button opens a page with laptops, tablets - pass

9.Check that there is a directory on the main page in the upper right corner - pass

10.Check that the "Catalog" button opens all product categories accordingly - pass

**Search field**

1.Make sure the search box is placed at the top center of the main page - pass

2.Check that you can enter numbers in the search field - pass

3.Check that Cyrillic is available for entry in the search field - pass

4.Check that Latin is available for input in the search field - pass

5.Check that if you type the word "phone" in the search field, a drop-down window will appear with the corresponding sections - categories, popular products, all search results - pass

6.Verify that the drop-down menu close button is active and closes the corresponding window - pass

7.Verify that the voice dial button in the right corner of the search field triggers voice dialing - pass

8.Verify that the "Magnifying Glass" button illustrated at the right end of the search field results in a search for the written product in the product search field - pass

9.Verify that the "Magnifying Glass" illustrated at the left end of the search field leads to the search for the selected product - failed

10.Check that after searching for a product, a drop-down window appears, and the "Cross" button closes this drop-down window - pass 

11.Check that products that were previously entered into the search field are displayed in the "Search History" drop-down box - pass

12.Check that after entering a product in the search field one or more times, the "Clear history" button appears in the drop-down box below "Search history" - pass

13.Verify that after clicking the "Clear History" button, the search history does not display any products - pass

14.Check that when entering the beginning of the name of the selected product, all matches are displayed in the drop-down window - pass

15.Check that when entering the full name of the selected product, all matches are displayed in the drop-down window - pass

16.Check that when entering a number, all matches are displayed in the drop-down window - pass

17.Check that when entering the product name in the drop-down box in the "Categories" section, when clicking on the corresponding product, the website redirects to the page with the selected product - pass


**"Login" button**

1.Check that there is a "Login" button on the main page in the upper right corner - pass

2.Check that when you click the "Login" button, the profile for logging into your personal account appears - pass

3.Check that the profile has the "Enter phone number" field - pass

4.Check that the profile has the "Login by Email" field - pass

5.Verify that after entering the correct phone number, the user is sent an SMS with a code to the corresponding number - pass

6.Check that after entering a valid code, the user is logged into their personal account - pass

7.Check that a user registered via Email, after entering a valid Email, receives an email with a code to the corresponding email address - pass

**Registration**

1.Check that there is a "Register" button in the upper right corner - failed

2.Check that Cyrillic characters are valid for input in the "name" field - pass

3.Check that entering Latin characters in the "name" field is valid - pass

4.Check that only after entering the correct format of the email address, which has not been registered with an account on this website, and the number, which has not been registered with an account on this website, and when entering the name, the user will receive a code to the corresponding number - pass

5.Verify that after entering the correct code from SMS, the user will be registered - pass

6.Check that after entering an incorrect code from SMS, the user will not be registered - pass

7.Check that the system does not skip the user when entering the wrong email format and when entering a phone number in the correct format for which an account has not yet been registered, the registration will not be successful. The system will display a message about the corresponding error - pass

8.Check that if you enter the correct email format and if you enter the wrong phone number, the registration will not be successful. The system will display a message about unsuccessful registration - pass

**"Comparison" section**

1.Check that there is a "Compare" button in the upper right corner - pass

2.Check that if the products have not been added to the "Comparisons" section, when you go to this section, the message "Comparison is not filled in. For comparison, add several products. To do this, find the desired product and click the compare products button" will appear - pass

3.Check that when adding a product to the "Comparison" section, the corresponding product will appear in the "Comparison" section - pass

4.Check if when adding two or more products of the same category to the "Comparison" section, they are displayed in the "Comparison" section - pass

5.Check that when adding two products from different categories to the "Comparison" section, they will not be compared - pass




```
Test cases for testing the functionality of the Citrus website
```


**Test Case ID1.Registration verification**
									
											 
|Tester's Name| 		Manetska Daria	|  
|-----------|--------------|
|Date Tested |	06.08.2025	|
|Test Case   | 		Pass		|
											
|	Prerequisites:                                          |				Test Data					      |
|---------------------------------------------------------|---------------------------------|
|1	Chrome version 138.0.7204.1011                        |	1 Email: tatianarotaru@gmail.com	|
|2	macOS Sequoia 15.5 (24F74)	                         	|	2 Number: 0679585985					|
|3	Go to the profile ""Login"" in the upper right corner| 3 Name: Tatiana	                  |
                                            

											
**Step to reproduce**					

|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|
|"Enter the email in the "Mail field"|	The email is displayed in the "Mail" field	|Pass|
|2	Enter your phone number            |The email is displayed in the "Number" field |		Pass	|	
|3	Enter name in the "Name" field	|	The entered name is displayed in the  "Name" field |		Pass	|					
|4	Write the "Sign up" button	|	The code is sent  to the specified phone number. The field for entering the code is shown to the user |		Pass		|				
|5	Enter the correct code| The user is registered successfully on the web side. The user's personal account is created |		Pass	|		

---

											
**Test Case ID2.Сheck registration  without entering a code**
									
											
|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Fail		|
											
|Prerequisites		|Test Data		|
|----------|-------------|
|1	Chrome version 138.0.7204.101	|			1	Email: tatianarotaru@gmail.com	|				
|2	macOS Sequoia 15.5 (24F74)		|		2	Number: 0678394674				|	
|3	Go to the profile "Login" in the upper right corner	|			3	Name: Tatiana			|		
		
**Step to reproduce**																				
|Step Details          |      Expected Results|    Pass/Failed |
|--------------------|----------------------|---------|										
|1	Enter email on the "Mail" field	|	The email is displayed on the "Mail" field	|	  Pass	|					
|2	Enter number on the "Number" field |		The number is displayed on the "Number" field|		Pass |						
|3	Enter name in the "Name" field		|The name is displayed on the "Name" field	|	Pass			|			
|4	Press "Enter" at the bottom	|	The code is sent to the specified phone number. The field  for entering the code is shown to the user	|	Pass				|		
|5	Don't enter the code and reload the page 	|	The user  isn`t registered on the website. The following message is shown.	 Тестувала з реальним номером,який ще не був зареєстраний. Код надійшов, проте я  його не ввела, думаючи, що  тест пройшов.Проте коли нижче використала цей номер для повторної перевірки реєстрації - сайт написав, що користувач з таким номером телефону існує. Також можна зайти в особистий кабінет за цим номером телефону.	|		Fail|

---

**Test Case ID3.Checking registration with an incorrect code**
						
										
|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass|		

 **Step to reproduce**	
|Prerequisites		|Test Data		|
|----------|-------------|		
1	Chrome version 138.0.7204.101		|		1	Email: tatianarotaru@gmail.com				
2	macOS Sequoia 15.5 (24F74)		|		2	Number: 0674895947				
3	Co to the profile "Login" in the upper right corner		|		3	Name: Tatiana							

										
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|				
1	Enter email in the "Mail" field	|	The email is displayed in the "Mail" field	|	Pass					
2	Enter a number in the "Number" field	|	The number is displayed in the "Number" field	|	Pass					
3	Enter name in the "Name" field	|	The name is displayed on the "Name" field	|	Pass					
4	Press "Enter" bottom	|	The code is sent to the specified phone number. The field  for entering the code is shown to the user	|	Pass					
5	Enter the correct code |		The user isn`t registered on the web side|		Pass			

---

**Test Case ID4.Checking registration when entering an incorrect email format**


										
|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		
										

|Prerequisites		|Test Data		|
|----------|-------------|		
1	Chrome version 138.0.7204.101			|	1	Email: @tatianarotaru@gmail.com				
2	macOS Sequoia 15.5 (24F74)		|		2	Number: 0664795083				
3	Co to the profile "Login" in the upper right corner			|	3	Name: Tatiana				

										
**Step to reproduce**					
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|				
1	Enter an incorrect email format in the Mail field |		The email is displayed on the "Mail" field	|	Pass					
2	Enter a number in the "Number" field	|	The number is displayed in the "Number" field	|	Pass					
3	Enter name in the "Name" field	|	The name is displayed on the "Name" field	|	Pass					
4	Press "Enter" bottom	|	The "Mail" field is highlighted in red. A message about the incorrect mail format is displayed |	Pass		

---

**Test Case ID5.Checking registration when entering an already used phone number**			

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|


|Prerequisites		|Test Data		|
|----------|-------------|		
1	Chrome version 138.0.7204.101			|	1	Email: tatianarotaru@gmail.com				
2	macOS Sequoia 15.5 (24F74)				|2	Number: 0678394674				
3	The phone number has already been used for registration		|		3	Name: Tatiana				
				
										
**Step to reproduce**						
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|							
|1	Enter the correct email format in the Mail field |	The email is displayed on the "Mail" fiedl	|	Pass			|		
|2	Enter the phone number you have used to register before | The number is displayed on the "Number" field	|	Pass|					
|3	Enter name on the "Name" field	|	The name is displayed on the "Name" field |	Pass	|				
|4	Click the "Login" button | The message "A user with this phone number already exists" is displayed	|	Pass	|			

---

**Test Case ID6.Checking registration with an incorrect phone number**

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|
										
|Prerequisites		|Test Data		|
|----------|-------------|				
1	Chrome version 138.0.7204.101			|	1	Email: tatianarotaru@gmail.com				
2	macOS Sequoia 15.5 (24F74)		|		2	Number: 0758394674				
3	Go to the profile "Login" in the upper right corner	|			3	Name: Tatiana				

**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|																						
1	Enter the correct email format in the Mail field |	The email is displayed on the "Mail" field |		Pass|					
2	Enter an incorrect phone number in the "Number"	|	The number is displayed in the "Number" field|		Pass|					
3	Enter name in the "Name" field	|	The name is displayed on the "Name" field|Pass	|				
4	Click the "Login" button |The field with the number will be underlined in red| Pass		|

---

**Test Case ID7.Login verifycation wirh correct data**

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|


             
|Prerequisites		|Test Data		|
|----------|-------------|
1	Chrome version 138.0.7204.101			|1	Number: 0679585985				
2	macOS Sequoia 15.5 (24F74)				|2	Email: tatianarotaru@gmail.com				
3	User successfully registered	|							
							
										
**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|	
1	Co to the "Login" section	|	The profile is opened with a field for entering a number|		Pass					
2	Enter the correct number in the "Number" field	|	The number is displayed in the "Number" field|	Pass					
3	Enter "Next"	|	The field for entering the code is displayed. The message "Code from SMS sent to +380679585985" is displayed in the profile"	|	Pass	

---

**Test Case ID8.Verification of the correct mail login**

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|


|Prerequisites		|Test Data		|
|----------|-------------|
1	Chrome version 138.0.7204.101		|		1	Email: tatianarotaru@gmail.com				
2	macOS Sequoia 15.5 (24F74)			|				
3	User is successfully registered on the website|
		
**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|	
1	Go to the "Login" section	|	A profile is opened with a field for entering a phone number|	Pass					
2	Click "Sign in by Email"|	The "Number" field is changed to the "Email" field |Pass					
3	Enter mail | The entered is displayed in the "Mail" field| Pass					
4	Click "Next" |	A code is sent to the appropriate email	|Pass					
5	Enter the correct code | The user is able to log in to your account	|	Pass				

---

**Test Case ID9.Checking the comparison**		

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|


|Prerequisites		|Test Data		|
|----------|-------------|
1	Chrome version 138.0.7204.101		|					
2	macOS Sequoia 15.5 (24F74)		|		
		
				
**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|										
1	Add two different products from the same category to the Comparison section		|Products are added to the "Comparison" section|	Pass					
2	Check if they are comparable |A comparison chart of the characteristics of the corresponding products is created and displayed on the web page |Pass		

---

**Test Case ID10.Check that the "Electric vehicles" button takes you to the appropriate category**

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|


|Prerequisites		|Test Data		|
|----------|-------------|
1	Chrome version 138.0.7204.101	|					
2	macOS Sequoia 15.5 (24F74)		|				
3	Go to the main page				|		
		
										
**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|		
1	Click on the "Personal transportation" button |The user will be redirected to the page with the electric vehicle |	Pass		


---

# Testing of the Kittigram 

**Test Case ID1.Verifying functionality of the "Like" button**
										
|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|


|Prerequisites		|Test Data		|
|----------|-------------|			
1	Chrome version 138.0.7204.101	|				
2	macOS Sequoia 15.5 (24F74)		|					
3	User is logged in app|			

										
**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|							
1	Enter the "Like" button 1 time		|The "Like" button is changed to violet color. The number near the"Like" button is  increased by 1	|	Pass

---
										
**Test Case ID2. Verifying the functionality of the "Like" counter**

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|


|Prerequisites		|Test Data		|
|----------|-------------|	
1	Chrome version 138.0.7204.101|
2	macOS Sequoia 15.5 (24F74)|
3	User is logged into the application|
4	The post already has 5 likes displayed|

**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|							
1	Enter the "Like" button 1 time		|The "Like" button is changed to violet color. The number near the"Like" button is  increased by 1	|	Pass
2 	Enter the "Like" button 1 time		|The "Like" button is changed to white color. The number near the "Like" button decreases by 1	|	Pass	

-----

**Test Case ID3.Checking the writing of comments**

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|


|Prerequisites		|Test Data		|
|----------|-------------|				
1	Chrome version 138.0.7204.101			|				
2	macOS Sequoia 15.5 (24F74)				|				
3	User is logged in app				|				
4	Go to comments to another correspondent				|				
																			
										
**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|		
1	Enter the field for comment		|The flashing cursor is shown in the field |Pass	|				
2	Fill the letters of a valid language in the "Comment" field 	|	The letters are displayed in the field	|	Pass	|				
3	Fill the special symbols on the "Comment" field |		The special symbols are displayed in the field	|	Pass	|				
4	Fill the numbers in the "Comment" field 	|	The numbers are displayed in the field	|	Pass		|			
5	Fill the smiles on the "Comment" field 	|	The smiles are displayed in the field	|	Pass	|	

---

**Test Case ID4.Checking photo upload without cat**

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|

|Prerequisites		|Test Data		|
|----------|-------------|		
1	Chrome version 138.0.7204.101	|Photo without a cat							
2	macOS Sequoia 15.5 (24F74)								
3	User is logged in app							
				
		
**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|											
1	Enter the "+" buttom 	|	The window with drop down list with categories "Select photo from gallery", "Take a photo"	|	Pass|					
2	Enter categories "Select photo from gallery"	|	  The gallery is opened		|Pass|					
3	Enter categories "Take a photo"	|	The camera is activated|		Pass	|				
4	Select the photo without a cat from the gallery of the phone	|	The message is displayed " There is no cat in this photo|	Pass	|				
5	Take a photo without a cat using a phone camera	|	The message is displayed " There is no cat in this photo|		Pass	|		

---

**Test Case ID5. Сheck video addition**

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|

|Prerequisites		|Test Data		|
|----------|-------------|				
1	Chrome version 138.0.7204.101	|	Video with cat					
2	macOS Sequoia 15.5 (24F74)							
3	User is logged in app							
4					4					
										
				
**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|								
1	Enter the "+" buttom 	|	The window with drop down list with categories "Select photo from gallery", "Take a photo"		|Pass	|				
2	Enter categories "Select photo from gallery"	|	The gallery is opened	|	Pass		|			
3	Enter categories "Take a photo"	|	The name is displayed on the "Name" field	|	Pass					
4	Select the video with a cat from the gallery of the phone	|	The message is displayed " Unsupported format type"	|	Pass					
5	Take a photo with a cat using a phone camera	|	The message is displayed " Unsupported format type"	|	Pass	

---

**Test Case ID6.Checking subscriptions to other users**

|Tester's Name |		Manetska Daria|
|------------|-------------|
|Date Tested|		06.08.2025|	
|Test Case |		Pass		|


|Prerequisites		|Test Data|
|----------|-------------|					
1	Chrome version 138.0.7204.101	|						
2	macOS Sequoia 15.5 (24F74)		|				
3	User is logged in app			|					
													
								
**Step to reproduce**	                
|Step Details|Expected Results| Pass/Failed |
|-------------|------------|---------|																		
|1	Enter the "Subscribe" bottom	| A window with the information "(Username) is your friend" is displayed. Your friends count will increase by 1. New photos added by a "friend" is displayed on the user's feed|Pass	|				
									
