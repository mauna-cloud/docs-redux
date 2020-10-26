# CLI Session	

## Create Session

_Given_ I have a valid token for mauna services

_And_ I have the uuid of the app

_When_ I type the command "mauna session:start" app uuid

_Then_ the new session with "session uuid" is created.

## List Sessions

_Given_ I have a valid token for mauna services

_When_ I enter the command "session:list"

_Then_ the list of all sessions associted with token will be displayed

_And_ the "App Name", "App Version" "session uuid" "status" will be shown for each session.

## Kill Sessions

_Given_ the developer has already has an active session

_When_ a user enters the command "mauna session:stop"

_And_ the user provides the session "uuid"

_Then_ the session should should be stopped

_And_ the status of the session should be "ended".

## View history of a session

_Given_ the developer has created sessions

_And_ the developer has the uuid of a session

_When_ user gives the command "mauna session:history session-uuid"

_Then_ the all the messages exchanged with mauna backend are displayed.

## View Logs for a session

_Given_ the developer has created sessions

_And_ the developer has the uuid of a session

_When_ user gives the command "mauna session:logs session-uuid"

_Then_ the all the logs pertaining to the session are displayed.
