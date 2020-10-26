# Playground for interacting with Mauna Services

## Start a playgound session

_Given_ As a developer I am already authenticated

_When_ As a developer I enter the command "mauna playground"

_Then_ I should be in the playground shell

_And_ I can execute commands.

## Exit from the playground session

_Given_ As a developer I am already in the playground

_When_ I enter the command "exit" in playground shell

_Then_ I should exit from the playground shell.

## Load an application

_Given_ As a developer I am already in the playground

_When_ I issue command to load the application script file

_Then_ the application is loaded in the playground

_And_ the message is displayed that the application is loaded.

## Execute the Application

_Given_ As a developer I have already loaded application in the playground

_When_ I issue the commnd "run"

_Then_ the loaded application is executed

_And_ the developer can send the text messages to the Bot app

_And_ the Bot App responds appropriately.

## View the state/context of the App

_Given_ As a developer I have already executed the Application

_When_ I issues the command "status"

_Then_ All the context and status information should be display.

## Show logs during playground session

_Given_ As a developer I have already executed the Application

_When_ I issues the command "logs"

_Then_ All the logs collected should be displayed on the playground shell.

## Reset Application

_Given_ As a developer I have already executed application in the playground

_And_ I have sent few messages

_When_ I issue the commnd "reset"

_Then_ the application should be re-initialised

_And_ the context/state is reset

_And_ the history is cleaned.

## Display help

_Given_ As a developer I am already in the playground

_When_ I give the command "help"

_Then_ the list of commands and their description is displayed.
