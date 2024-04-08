# Meet App

## Description
Meet App is a progressive web application (PWA) built with React that allows users to discover and filter events happening in different cities. Users can specify the number of events to display, toggle event details, view charts visualizing event data, and use the app offline. It utilizes the Google Calendar API for event data and implements OAuth2 authentication for user authorization.

## Key Features
Filter Events by City
Show/Hide Event Details
Specify Number of Events
Use the App When Offline
Add an App Shortcut to the Home Screen
Display Charts Visualizing Event Details

## Technical Requirements
React application
Test-Driven Development (TDD) technique
Integration with Google Calendar API and OAuth2 authentication flow
Implementation of serverless functions (AWS Lambda preferred) for authorization server
Hosting on GitHub Pages
Support for latest versions of major browsers including IE11
Responsive design for all screen sizes
Passes Lighthouse's PWA checklist
Offline functionality with service worker
Ability to install on desktop and add to home screen on mobile
Utilizes an OOP approach for alert system
Data visualization features
Test coverage >= 90%
Online performance monitoring tool integration

## Installation
- Clone the repository: git clone https://github.com/yafet4275/meet-app.git
- Install dependencies: npm install
-  Start the development server: npm start
- Open the app in your browser at http://localhost:3000

## Usage
- Filter events by selecting a city from the dropdown menu.
- Toggle event details by clicking on an event card.
- Adjust the number of events displayed using the settings panel.
- Use the app offline or in slow network conditions.
- Add the app to your device's home screen for quick access.

## Contributing
We welcome contributions from the community. Please fork the repository, make your changes, and submit a pull request for review.

### User Stories
1. As a user, I want to be able to filter events by city so that I can view events specific to the city I'm interested in attending.

2. As a user, I want the ability to show or hide event details so that I can customize the level of information displayed and focus on what interests me the most.

3. As a user, I want to specify the number of events displayed so that I can control the amount of information presented to me at once and avoid feeling overwhelmed.

4. As a user, I want to be able to use the app when offline so that I can access event information even without an internet connection, ensuring uninterrupted usability.

5. As a user, I want to add an app shortcut to my device's home screen for quick and easy access, improving convenience and usability.

6. As a user, I want to visualize event details using charts so that I can better understand and analyze event data, aiding in decision-making and planning.

### Scenarios
Feature: Filter Events By City
- Scenario 1: View Events From All Cities
**Given** that I open the events app
**When** I view the list of upcoming events
**Then** I should see events from all cities
  
- Scenario 2: View List of City Suggestions
**Given** that I open the events app
**When** I start typing in the city search bar
**Then** I should see a list of suggested cities

- Scenario 3: Select City From Suggestions
**Given** that I open the events app
**When** I select a city from the suggested list
**Then** the events list should be filtered for the selected city
  
### Feature: Show/Hide Event Details
- Scenario 1: Event Element Collapsed by Default
**Given** that I open the events app
**When** I view the list of events
**Then** each event element should be collapsed

- Scenario 2: Expand Event Details
**Given** that I open the events app
**When** I click on an event element
**Then** the details of that event should be visible

- Scenario 3: Collapse Event Details
**Given** that I open the events app and an event's details are visible
**When** I click on the collapse button
**Then** the details of that event should be hidden
  
### Feature: Specify Number of Events
- Scenario 1: Default Number of Events Displayed
**Given** that I open the events app
**When** I view the list of events
**Then** I should see 32 events displayed

- Scenario 2: Change Number of Events Displayed
**Given** that I open the events app
**When** I specify the number of events as 50
**Then** I should see 50 events displayed

### Feature: Use the App When Offline
- Scenario 1: Show Cached Data
**Given** that I open the events app and there is no internet connection
**When** I view the list of events
**Then** I should see cached event data

- Scenario 2: Show Error When Changing Search Settings
**Given** that I open the events app and there is no internet connection
**When** I try to change search settings
**Then** I should see an error message


### Feature: Add an App Shortcut to the Home Screen
- Scenario 1: Add App Shortcut
**Given** that I open the events app
**When** I choose to add the app to the home screen
**Then** a shortcut to the events app should be added to the device home screen


### Feature: Display Charts Visualizing Event Details
- Scenario 1: View Chart Displaying Number of Upcoming Events
**Given** that I open the events app
**When** I navigate to the charts section
**Then** I should see a chart displaying the number of upcoming events in each city
