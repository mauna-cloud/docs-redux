# CLI Apps	

## Create App

_Given_ I have a valid token for mauna services

_When_ I type the command mauna app:create version:<ver>

_Then_ the new app is created and app uuid, name & version are displayed.

## List Apps

_Given_ the developer has already created the apps

_When_ a user requests to view all apps for chat session using  vailed token

_And_ the user provides <app name> and <app version>

_Then_ the app name, app version, uuid and state of the App will be displayed.

## Delete App

_Given_ the developer has already created the app

_When_ a user requests to delete the apps

_And_ the user provides the <uuid> of the app

_Then_ the app should get deleted from the list.
