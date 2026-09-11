## Working Notes

Group Members:
Atticus Crooks
Antsey Hans
Mohamed Dawoud
Yogi Chopra



Project: HealthTrack: A Real-Time Health Monitoring System Using Wearable Devices -
Using wearable technologies and bioinformatics (? heart rate monitor? Apple watch? I might have an old one I can steal from my dad, should provide loads of info about heart rate, heart rate variability, sleep w/ iPhone or watch)

Do we really have to use a real watch? What about an engine or a simulator?

That could be fine, we could make something that simulates the output of a smart devices data as it gets routed to application.


Other bioinformatic logs – diet, sleep, physical activity, 

Features –
Daily suggestions for health (lacking certain nutrients in diet, poor sleep -> go light on workout vs good sleep -> go hard in workout, spO2 sleep apnea detector)
Connect to a food database to gather info on dietary nutrition(calories, macros, etc.)
SQL based user credential, using a free or lightweight variant (like MySQL, SQLite, DuckDB, or at the extreme level Azure SQL)

Do we want to do a web app? Or a windowed cross-platform app? Mobile app? Apple apps cost liek 100$ per year and are pretty hard to get up. What OS’ is everyone running? I have a windows machine I can use if I need

What frameworks/stacks/languages are you all familiar w/. 
User Stories –

Feature: User Login
User Story
    Scenario: Successful login with valid credentials 
    Given the user is on the login page
    And clicks the login button
    When the user enters a valid username or password
    Then the users home page is displayed

  Scenario: Unsuccessful login with invalid credentials
    Given the user is on the login page
    And clicks the login button
    When the user enters an invalid username or password
    Then an error message should be displayed
    And the users login attempt is tracked 

Feature: Connected Devices Page
User Story
    Scenario: Trying to sync a new device for the first time.
    Given the user opens the application and chooses to use a wearable device.
    And the device is discoverable via Bluetooth. (Or maybe wifi later)
    When the user tries to connect a device that wasn't connected before.
    Then it fails to connect as it can't see the device.
    And takes the user back to the connected devices page.

  Scenario: [Alternate, failure, or boundary scenario name]
    Given [initial state or precondition]
    And [relevant business rule or condition]
    When [user action or event]
    Then [observable and testable result]
    And [additional result, if needed]

Feature: [Feature name]
User Story
    Scenario: [Successful scenario name]
    Given [initial state or precondition]
    And [additional precondition, if needed]
    When [user action or event]
    Then [observable and testable result]
    And [additional result, if needed]

  Scenario: [Alternate, failure, or boundary scenario name]
    Given [initial state or precondition]
    And [relevant business rule or condition]
    When [user action or event]
    Then [observable and testable result]
    And [additional result, if needed]

Review - 
	Does each story identify a specific user, goal, and value?
Is the story small enough to test independently?
Does each scenario describe one primary behavior?
Are the Then outcomes observable and testable?
Does the alternate scenario examine a meaningful condition?
Can you identify which business rule is verified?


