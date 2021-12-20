## •	Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?

The Personal Weight Monitor application helps the user to achieve one of several weight goals by communicating with the user when a weight target is reached. After logging into the application, the user records their weight readings and date into the application’s database. The application can support several users and keeps the weight measurement history separate for each user.

## •	What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?

The application features a main screen of their weight history. This screen is only active after logging into the application. If the user does not have login for the application, the log-in screen can be used to register the new user. A toolbar is used to navigate to the settings screen and logout function which immediately returns the user the log-in prompt. The main screen shows the weight information in the database along with a button to add a new weight measurement. Each weight entry has a delete button, select checkbox, and can be selected by a long press on the item to edit the data. The data is displayed using a recyclerView object. All weight measurement addition and updates are conducted with an AddWeight Fragment that manages Weight “numberPicker” and “DatePicker” objects to collect or modify new and existing weight measurements.

## •	How did you approach the process of coding your app? What techniques or strategies did you use? How could those be applied in the future?

I identified main purposes of the application and the user base that could be reached. After this, I identified the needed components to meet the user-need, such as a database, login and user registration ability, notification through SMS when a weight target is reached and this ability to set some persistent settings. 

Additionally, I considered how this could be presented to the user in an intuitive and friendly way. I decided just having centrally focused screen accessed only after logging into or registering with the application. This is the weight history view screen. All activities branch out from this screen with minimal complexity. Where possible, actions are one button away like logging out, going to the setting screen, and deleting a weight entry. Other items that require more information are travelled to by one button, this are activities like adding weight and modifying weight entries. 

## •	How did you test to ensure your code was functional? Why is this process important and what did it reveal?

Primary testing was done with sample data creation and sample data entry. 

## •	Considering the full app design and development process, from initial planning to finalization, where did you have to innovate to overcome a challenge?

Some Singleton classes were created to keep track of some managed data to provide access to the logged in status, database, dao, and table references and to some view references to assist in identifying certain view widgets using findByViewId.

## •	In what specific component from your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?

My utilization of classes to keep track of data was very helpful, but I would say the most successful thing in the application was the successful use of the Room database which provided me with a lot of difficulty. Some of this was due to trying to implement a “LiveData” connection with it and use background threads with it. 
