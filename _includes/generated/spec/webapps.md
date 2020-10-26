# Apps using Web Flow

## Create App

_Given_ Developer is logged in to Developer Dashboard

_When_ Developer clicks the "Apps" link on the Left Nav

_And_ Developer clicks on "Create" button

_And_ Developer enters Application name, version and description

_Then_ App is created and listed at the top of the list

_And_ the status of the create app is "New".

## Delete App

_Given_ Developer is logged in to Developer Dashboard

_When_ Developer clicks the "Apps" link on the Left Nav

_And_ Developer views the list of "Apps"

_And_ Developer Deletes App from the Actions

_Then_ App is deleted from the backend

_And_ the App is removed from the list.

## Edit App

_Given_ Developer is logged in to Developer Dashboard

_When_ Developer clicks the "Apps" link on the Left Nav

_And_ Developer views the list of "Apps"

_And_ Developer edits App from the Actions

_And_ Developer updates the Apps details

_And_ Developer clicks on Save

_Then_ App details shown in the list is updated.

## List Apps

_Given_ Developer is logged in to Developer Dashboard

_When_ Developer clicks the "Apps" link on the Left Nav

_Then_ List of all the created apps are seen on the webpage

_And_ the Name, version, description, status, created date as data columns.

## Sort Apps List

_Given_ Developer is logged in to Developer Dashboard

_When_ Developer clicks the "Apps" link on the Left Nav

_And_ List of all the created apps are seen on the webpage

_And_ the Name, version, description, status, created date as data columns

_And_ Developer clicks on the sort icon on the "Status" column header

_Then_ The App list is sorted based on the "Status" column.
