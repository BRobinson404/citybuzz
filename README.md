# City Buzz Event Finder

<h1>What is it?</h1> <br>
a serverless, progressive web application (PWA) with React using a
test-driven development (TDD) technique. The application uses the Google
Calendar API to fetch upcoming events
<h2>Serverless Functionality</h2>
<br>
City Buzz will utilizes serverless functions through Amazon Web Services (AWS) and the Google Calendar API.<br>
The app shows information about upcoming events by city

<h1>User Stories</h1>
<br>
As a user, <br>
I should be able to filter events by city <br>
So that I can see the list of events that take place in that city.<br>
<br>
As a user, <br>
I should be able to show/hide event details <br>
So that I can see more/less information about an event.<br>
<br>

As a user, <br>
I should be able to specify the number of events I want to view in the app <br>
So that I can see more or fewer events in the events list at once.<br>
<br>
As a user, <br>
I should be able to use the app when offline <br>
So that I can see the events I viewed the last time I was online.<br>
<br>
As a user, <br>
I should be able to add the app shortcut to my home screen <br>
So that I can open the app faster.<br>
<br>
As a user, <br>
I should be able to see a chart showing the upcoming events in each city <br>
So that I know what events are organized in which city.<br>
<br>
<h1>Key Features</h1>

<h2>FILTER EVENTS BY CITY</h2>

![FilterByCity](https://github.com/BRobinson404/citybuzz/assets/122922678/547028e4-0728-466b-9878-c9bef71ac6b8)

Scenario 1:
•	Given a list of events
•	When the user selects a specific city from the filter options
•	Then only events from that city should be displayed

Scenario 2:
•	Given a list of events
•	When the user selects multiple cities from the filter options
•	Then only events from the selected cities should be displayed

Scenario 3:
•	Given a list of events
•	When the user clears the city filter
•	Then all events should be displayed regardless of the city

<h2>SHOW/HIDE AN EVENT'S DETAILS</h2>

![HideEventDetails](https://github.com/BRobinson404/citybuzz/assets/122922678/8cdb8cb0-5392-4163-9d88-9b0ef7b716e5)

Scenario 1:
•	Given an event element
•	When the page loads
•	Then the event element should be collapsed by default

Scenario 2:
•	Given an event element
•	When the user clicks on the event
•	Then the event details should be displayed

Scenario 3:
•	Given an event element with details displayed
•	When the user clicks on the event
•	Then the event details should be collapsed

<h2>SPECIFY NUMBER OF EVENTS</h2>

![FilterNumberofEvents](https://github.com/BRobinson404/citybuzz/assets/122922678/17e57fe7-0145-4268-b50b-cbf2605e3001)

Scenario 1:
•	Given the user hasn't specified a number of events
•	When the page loads
•	Then the default number of events displayed should be 32

Scenario 2:
•	Given the user is viewing events
•	When the user changes the number of events they want to see
•	Then the number of events displayed should be updated accordingly



<h2>USE THE APP WHEN OFFLINE</h2>

![OfflineView](https://github.com/BRobinson404/citybuzz/assets/122922678/79c2a7d8-fb4c-40b5-8a99-ce81b00093a1)

Scenario 1:
•	Given the app has cached data
•	When there is no internet connection
•	Then the app should display the cached data

Scenario 2:
•	Given the user is using the app with no internet connection
•	When the user changes the settings (city, time range)
•	Then the app should show an error message indicating the inability to fetch updated data

<h2> DATA VISUALIZATION</h2>

![DataView](https://github.com/BRobinson404/citybuzz/assets/122922678/ad16847a-6a5d-4e8c-a241-188d4dcc8558)

Scenario 1:
•	Given upcoming events in different cities
•	When the user requests to see a chart
•	Then a chart should be displayed showing the number of upcoming events in each city
