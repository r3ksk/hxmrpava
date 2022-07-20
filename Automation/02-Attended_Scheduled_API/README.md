Before you deploy an automation, it will be good to know about few terminologies

#### What is an Automation Trigger?
A trigger is a rule that defines how and when the agent will execute your project. You can add one or several triggers to your automation project immediately or at a later time. The available triggers are:

1. Attended
2. Scheduled
3. API

Scheduled: A trigger of type scheduled creates jobs that are based on the schedule you define in the trigger. These jobs run fully automatically without any human intervention.
API: A trigger of type API opens a dedicated endpoint that allows an external application to start the execution of an Automation project via an HTTP POST call.

#### What is an Attended Trigger?

With a trigger of type attended, the deployed automation project is distributed to a specific group of agents and the automation can be run manually by the user.

An attended automation runs automated tasks but requires human intervention, using attended triggers. For SAP Process Automation the maximum number of sessions accessing the Cloud Service at any one time is counted. A session refers to the time between logon and logoff (or time out) where a unique user, application, bot or platform accesses the Cloud Service either directly or indirectly via a custom application. Automations triggered in debugging mode will not be counted as a connection.

#### What is an Scheduled Trigger?
A trigger of type scheduled creates jobs that are based on the schedule you define in the trigger. These jobs run fully automatically without any human intervention.

A scheduled or an unattended automation runs automated tasks without human intervention.  For SAP Process Automation the maximum number of sessions accessing the Cloud Service at any one time is counted. A session refers to the time between logon and logoff (or time out) where a unique user, application, bot or platform accesses the Cloud Service either directly or indirectly via a custom application. Automations triggered in debugging mode will not be counted as a connection.

#### What is an API Trigger?

A trigger of type API opens a dedicated endpoint that allows an external application to start the execution of an Automation project via an HTTP POST call.

The automations in this mission are tested with both Attended and Scheduled Triggers. Depending on your automation strategy, you can use any one of them.